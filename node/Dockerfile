FROM node:18-alpine

# 앱 디렉터리 생성
WORKDIR /usr/src/app

# 앱 의존성 설치
# package.json과 package-lock.json을 모두 복사
COPY package*.json ./

RUN npm install

# 앱 소스 추가
COPY . .

EXPOSE 3000
CMD [ "npm", "start" ]
