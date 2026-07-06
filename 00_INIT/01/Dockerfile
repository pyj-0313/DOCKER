# Node.js 18 공식 이미지를 베이스로 사용 (Debian 기반, 풀 사이즈)
FROM node:18
# 컨테이너 내부 작업 디렉토리 설정 (이후 명령은 모두 /app 기준)
WORKDIR /app
# package.json과 package-lock.json만 먼저 복사
COPY package*.json ./
# 의존성 설치
RUN npm install
# 나머지 소스 코드 전체 복사
COPY . .
# 컨테이너 시작 시 실행할 명령
CMD ["node", "index.js"]