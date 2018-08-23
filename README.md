# Preserve history sample for Bot Framework

[![Build Status](https://travis-ci.org/compulim/BotFramework-Samples-PreserveHistory.svg?branch=master)](https://travis-ci.org/compulim/BotFramework-Samples-PreserveHistory)

The Bot.js and Web Chat UI is hosted at [webchat-samples-preservehistory.azurewebsites.net](https://webchat-samples-preservehistory.azurewebsites.net/).

# Scenarios

Few different dimensions to test:

- Time
   - Within 24 hours (same conversation ID, same watermark)
   - 24 hours to 2 weeks (same conversation ID, watermark lost, temporary history is lost)
   - After 2 weeks (different conversation ID)
- Activity types
   - `"message"`
   - `"event"`, including page commands

We need to build sign-in flow, so we can give the dev a better sense of how to relate user ID and conversation ID.
