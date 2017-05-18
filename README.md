webkit Frame 研究
====
打点系统
-------
* events:WebCore/inspector/inspectorinstrumention.cpp
* events:WebCore/inspector/InspectorTimelineAgent.cpp
* *runLoopObserverFired* WebCore/platform/cf/RunLoopObserver.cpp
* *m_frameStartObserver* WebCore/inspector/InspectorTimelineAgent.cpp
* *m_frameStopObserver* WebCore/inspector/InspectorTimelineAgent.cpp
* *doDispatchMessageOnFrontendPage* WebCore/inspector/InspectorClient.cpp


内部事件
------
* *willRecalwillRecalculateStyle* Document::resolveStyle   
* *willRecalwillRecalculateStyle* Document::resolveStyle   
* *didScheduleStyleRecalculation* Document::scheduleStyleRecalc 
* *didRecalculateStyle* Document::resolveStyle 
* *didInvalidateLayout* FrameView::scheduleRelayout 
* *willLayout* FrmeView::layout 
* *didLayout* FrmeView::layout 
* *willComposite* FrameView::flushCompositingStateIncludingSubframes 
* *willPaint* FrameView::willPaintContents 
* *didPaint* FrameView::didPaintContents 
* *didComposite* m_frameStopObserver


* *willEvaluateScript* ScriptController::evaluateInWorld 
* *didEvaluateScript* ScriptController::evaluateInWorld 
* *willFireTimer* DOMTimer::fired 
* *didFireTimer* DOMTimer::fired 
