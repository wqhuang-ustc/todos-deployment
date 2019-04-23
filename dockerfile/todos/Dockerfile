FROM kylinhuang/todos_base:latest
LABEL MAINTAINER="Weiqing Huang <wqhuang.ustc@gmail.com>"
RUN git clone https://github.com/wqhuang-ustc/react-todos.git
WORKDIR /react-todos
# install necessary dependencies and Builds the app for production to the build folder.
RUN npm install && npm install -g serve && npm run build
EXPOSE 5000
# use serve to serve the static site on port 5000(most easiest way), alternatively,you can use express/nginx/apache to serve the content.
CMD serve -s build