FROM leapci/robot:core as robot
FROM leapci/protractor-chrome
WORKDIR /robot
COPY --from=robot /robot /robot
RUN chmod +x entrypoint.sh
ENTRYPOINT exec ./entrypoint.sh