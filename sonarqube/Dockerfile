From sonarqube
## ENV SONARQUBE_JDBC_USERNAME=root
## ENV SONARQUBE_JDBC_PASSWORD =root
## ENV SONARQUBE_JDBC_URL=jdbc:mysql://localhost:3306/sonar?useUnicode=true&characterEncoding=utf8&rewriteBatchedStatements=true&useConfigs=maxPerformance
ENV PLUGIN_HOME=/opt/sonarqube/extensions/plugins
ADD sonar-github-plugin-1.4.2.1027.jar ${PLUGIN_HOME}
ADD sonar-gitlab-plugin-3.0.1.jar ${PLUGIN_HOME}
ADD sonar-l10n-zh-plugin-1.20.jar ${PLUGIN_HOME}
ADD sonar-scm-git-plugin-1.4.0.1037.jar ${PLUGIN_HOME}

EXPOSE 9000
ENTRYPOINT ["/opt/sonarqube/bin/run.sh"]