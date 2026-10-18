FROM node:18-alpine

WORKDIR /app

RUN npm install -g serve

# Copy thư mục đã build sẵn từ máy local vào container (kiểm tra xem dự án của bạn là thư mục 'dist' hay 'build')
COPY dist ./dist

EXPOSE 3000

CMD ["serve", "-s", "dist", "-l", "3000"]