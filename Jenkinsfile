node {
    def slackResponse = slackSend(channel: "builds", message: "Started build")
    slackSend(channel: slackResponse.threadId, message: "Build still in progress")
    slackSend(
        channel: slackResponse.threadId,
        replyBroadcast: true,
        message: "Build failed. Broadcast to channel for better visibility."
    )
}