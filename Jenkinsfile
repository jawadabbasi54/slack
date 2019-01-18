node {
    def slackResponse = slackSend(channel: "builds", message: "Started build", thread_ts: "1547797142.004700")
    slackSend(channel: slackResponse.threadId, message: "Build still in progress")
    slackSend(
        channel: slackResponse.threadId,
        replyBroadcast: true,
        message: "Build failed. Broadcast to channel for better visibility."
    )
}