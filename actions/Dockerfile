FROM rasa/rasa-sdk:2.8.1

 # The Rasa SDK image runs as non-root user by default. Hence, you have to switch
 # back to the `root` user if you want to install additional dependencies
USER root

RUN pip3 install recognizers-text-suite
RUN pip3 install pandas
# RUN pip install gunicorn==20.1.0

# Switch back to a non-root user
USER 1001
