# OptimizingEarthquakeNowcasts
Python code for the paper Optimizing Earthquake Nowcasts with Machine Learning published in Earth and Space Science
    #   PARAMETERS
    
    #   Three Primary Adjustable Parameters Are:
    #
    #       NSteps:             Used for the Exponential Moving Average
    
    #       min_rate (Rmin)):   Minimum monthly rate of small earthquakes,
    #                           used to represent the "true" rate of small
    #                           earthquakes, unstable stick slip plus stable
    
    #       max_rate (Rmax):    Adjustable parameter used to improve the 
    #                           skill of the nowcast.  Used when there is 
    #                           a large earthquake that dominates the data.
    #                           Max. number of small earthquakes in a month
    #
    #   Other Main Parameters:
    #
    #       TW, or forecast_interval:   In years.
    #
    #       
        #   Begin by downloading the catalog by setting Download_Catalog = True
    #   Select other functions by setting the appropriate False flag to True
    #   Note that some of these functions can take seconds, others hours
    
    Download_Catalog                                    = False
    
    #   Basic Timeseries
    Plot_SEISR_Timeseries                               = False     #   Plots the basic state variable time series
    Plot_Precision_Timeseries                           = False     #   Plots the Positive Predictive Value (PPV) time series
    Plot_Timeseries_PPV_Precision_Information           = False     #   Plots a combination of the above
    
    #   Receiver Operating Characteristic + Precision
    Plot_Temporal_ROC                                   = False     #   Computes and plots the temporal ROC diagram
    Plot_Temporal_Shaded_ROC                            = False     #   Same as above, but shading indicates skill
    Plot_Temporal_TPR_FPR_Threshold                     = False     #   Plots the True Positive Rate and the False Positive Rate
    Plot_Spatial_ROC                                    = False     #   Plots the spatial ROC at 1-year intervals
    Plot_Precision_vs_Threshold                         = False     #   Plots the PPV vs. the threshold value
    Plot_Temporal_Skill_Info_vs_TW                      = False     #   Plots the temporal skill as function of the Time Window TW

    #   Miscellaneous
    Optimize_Params                                     = False     #   Set param ranges above
    Plot_Seismicity_Map                                 = False     #   Plots a geographic map of the seismicity
    Plot_Event_Timeseries                               = False     #   Plots time series of earthquake events with EMA
    Plot_Mean_EQs_Time                                  = False     #   Plots the mean number of earthquakes as time series     
    Plot_Event_Timeseries_Mean_EQs_Time                 = False     #   Plots a combination of the above two time series
    
