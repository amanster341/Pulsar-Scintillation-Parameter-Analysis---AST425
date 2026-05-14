# Results Summary

This file summarizes the main results from my AST425 pulsar scintillation parameter analysis project. The goal of this project was to test whether phase parameters could be recovered from scintillation data using a power-maximization method over a grid of possible parameter values.

The project was first tested using simulated dynamic spectra, where the true parameters were already known. After validating the method on simulated data, I applied the same general procedure to real observational data.

## Simulated Data Results

For the simulated data, I generated dynamic spectra using known input parameters and then attempted to recover those parameters using the analysis pipeline. This was useful because it allowed me to check whether the method was working under controlled conditions.

The simulated dynamic spectrum showed clear scintillation structure, and the secondary spectrum showed a visible parabolic arc. A delay slice was selected along a bright region of the secondary spectrum, and the power was calculated over a grid of possible values for the parameters `A` and `δ`.

The recovered values were:

| Parameter | Recovered Value |
|---|---|
| `A` | `-0.1907 ± 0.0132` |
| `δ` | `3.1372 ± 0.036 rad` |

These results were close to the expected input values, which showed that the pipeline was able to recover the correct parameters from simulated data. The simulated case was cleaner than the real data because the signal was more controlled and there was less ambiguity in the secondary spectrum.

Overall, the simulated results showed that the method works well when the signal is clear and the chosen delay slice contains useful scintillation structure.

## Real Data Results

After testing the method on simulated data, I applied it to real observational data. The real data was more difficult to analyze because the secondary spectrum had more noise, multiple bright regions, and less clean structure compared to the simulation.

For the real data, I focused on a selected region of the dynamic spectrum where the scintillation signal appeared stronger. I then used the secondary spectrum to choose a useful delay slice for the parameter search.

The best real-data result came from using:

| Quantity | Value |
|---|---|
| Selected delay index | `τ_sel = 52` |
| `A` | `-0.31734384615384614` |
| `δ` | `3.145084379310345 rad` |

The real-data heatmap showed a preferred region in parameter space, but it was not as clean as the simulated case. This makes sense because the real data contains more noise and complicated structure. There were also multiple bright regions in the heatmap, meaning the result was not as uniquely constrained as the simulated data.

Still, the real-data result was useful because it showed that the method could be applied beyond ideal simulations. The result gave a reasonable estimate for the phase parameters, even though the uncertainty is harder to interpret than in the simulated case.

## Interpretation

The simulated results acted as a validation test. Since the recovered parameters were close to the known input values, this showed that the pipeline was working properly in a controlled case.

The real-data results were more complicated. The selected region of the secondary spectrum still produced a clear preferred result, but the heatmap was broader and noisier. This suggests that the real-data estimate is useful, but should be treated more carefully than the simulated result.

In particular, the uncertainty from the simulated Monte Carlo runs should not be treated as a full uncertainty estimate for the real data. The simulated uncertainty mostly shows the precision of the method under cleaner conditions. The real data likely has additional uncertainty because of noise, delay-slice selection, and the more complicated structure of the secondary spectrum.
