FROM node:22-alpine AS build

WORKDIR /app

# Nhận biến từ docker-compose
ARG VITE_BASE_API_URL
ENV VITE_BASE_API_URL=$VITE_BASE_API_URL

COPY package*.json ./
RUN npm ci

COPY . .
RUN npm run build

# =========================
# Runtime stage
# =========================
FROM nginx:alpine

COPY --from=build /app/dist /usr/share/nginx/html
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]