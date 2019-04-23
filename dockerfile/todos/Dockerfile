FROM kylinhuang/todos_base:latest
LABEL MAINTAINER="Weiqing Huang <wqhuang.ustc@gmail.com>"
RUN git clone https://github.com/wqhuang-ustc/react-todos.git
WORKDIR /react-todos
RUN npm install && npm install -g serve && npm run build
EXPOSE 5000
CMD serve -s build