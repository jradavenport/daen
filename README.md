# daen

My workflow goal here:

- Given a list of signal events (ra, dec, dist, time), including SN 1987A
    - maybe include historic supernovae?
    - galactic nova
    - other good signal events?
- Include uncertainties on coordinates (event duration for time?)
- For each event, compute today's 3D SETI Ellipsoid, in Galactic XYZ coordinates
    - do N~100 samples of uncertainties to get range of ellipsoids
    - determine 5-95% (or 1-sigma?) ellipsoids that encompass the error range
    - really just want coefficients that define these inner & outer ellipsoids
- Determine if star or event is contained within any of these ellipsoidal regions
    - compute for ZTF real-time alerts for stars w/ distance estimates
    - also good to compute each day against stars out to few kpc (from Gaia)
