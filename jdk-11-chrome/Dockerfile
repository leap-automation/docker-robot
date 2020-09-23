FROM leapci/robot:core as robot
FROM leapci/gradle-chrome:jdk-11
WORKDIR /robot
COPY --from=robot /robot /robot
COPY --from=robot /report-libs /root/.m2/repository/com/cognizant
RUN chmod +x entrypoint.sh
ENTRYPOINT exec ./entrypoint.sh
