# DevelopProject


 @Override
    public void onMediaPeriodCreated(int windowIndex, MediaSource.MediaPeriodId mediaPeriodId) {
        log("Media period created", null, -1, -1, null, -1, null, -1, -1, -1);
    }

    @Override
    public void onMediaPeriodReleased(int windowIndex, MediaSource.MediaPeriodId mediaPeriodId) {
        log("Media period released", null, -1, -1, null, -1, null, -1, -1, -1);
    }

    @Override
    public void onLoadStarted(int windowIndex, @Nullable MediaSource.MediaPeriodId mediaPeriodId, LoadEventInfo loadEventInfo, MediaLoadData mediaLoadData) {
        log("load started", loadEventInfo.dataSpec, mediaLoadData.dataType, mediaLoadData.trackType, mediaLoadData.trackFormat,
                mediaLoadData.trackSelectionReason, mediaLoadData.trackSelectionData, mediaLoadData.mediaStartTimeMs, mediaLoadData.mediaEndTimeMs,
                loadEventInfo.elapsedRealtimeMs);
    }

    @Override
    public void onLoadCompleted(int windowIndex, @Nullable MediaSource.MediaPeriodId mediaPeriodId, LoadEventInfo loadEventInfo, MediaLoadData mediaLoadData) {
        log("load completed", loadEventInfo.dataSpec, mediaLoadData.dataType, mediaLoadData.trackType, mediaLoadData.trackFormat,
                mediaLoadData.trackSelectionReason, mediaLoadData.trackSelectionData, mediaLoadData.mediaStartTimeMs, mediaLoadData.mediaEndTimeMs,
                loadEventInfo.elapsedRealtimeMs);
    }

    @Override
    public void onLoadCanceled(int windowIndex, @Nullable MediaSource.MediaPeriodId mediaPeriodId, LoadEventInfo loadEventInfo, MediaLoadData mediaLoadData) {
        log("load canceled", loadEventInfo.dataSpec, mediaLoadData.dataType, mediaLoadData.trackType, mediaLoadData.trackFormat,
                mediaLoadData.trackSelectionReason, mediaLoadData.trackSelectionData, mediaLoadData.mediaStartTimeMs, mediaLoadData.mediaEndTimeMs,
                loadEventInfo.elapsedRealtimeMs);
    }
