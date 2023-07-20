
# Sections Q: Quantities

## <a name="MR signal quantities"></a> MR signal quantities
The items in this group are related to the MR signal and quantities of the MR sequence used to acquire the signal.

| Code | Standardised name| Alternative names|Notation|Description|Standardised units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| CAPLEX:Q.MS1.001.[j] | <a name="S"></a> Signal | -- | *S<sub>j</sub>* | The MR signal (magnitude, phase or complex depending on context) in compartment *j*. | a.u. | -- |
| CAPLEX:Q.MS1.005 | <a name="TE"></a> Echo time | -- | TE | The time between the application of the radiofrequency excitation pulse and the center of the echo. | ms |-- |
| CAPLEX:Q.MS1.006 | <a name="TR"></a> Repetition time | -- | TR | The time between the beginning of a pulse sequence and the beginning of a succeeding (essentially identical) pulse sequence. | ms | -- |
| CAPLEX:Q.MS1.007 | <a name="Flip angle"></a> Prescribed excitatory flip angle | -- | <img src="https://latex.codecogs.com/svg.image?\alpha&space;" title="https://latex.codecogs.com/svg.image?\alpha " />| The prescribed nutation angle of the net magnetization immediately following an excitation RF pulse. | deg | -- 
| CAPLEX:Q.MS1.008 | <a name="PD"></a> Prepulse delay time | Inversion time TI (in case of an inversion recovery sequence) | PD | The time between the middle of a prepulse (e.g. inversion pulse) and the middle of the pulse that reads out the center of k-space. | ms | -- |
| CAPLEX:Q.MS1.009 | <a name="PF Flip angle"></a> Prepulse flip angle | -- |<img src="https://latex.codecogs.com/svg.image?\alpha_{p}" title="https://latex.codecogs.com/svg.image?\alpha_{p}" /> | The nutation angle of the net magnetization immediately following a prepulse. | deg | -- |
| CAPLEX:Q.MS1.010 | <a name="S_0"></a> Signal scaling factor | -- | *S<sub>0</sub>*  | A constant scaling factor in a signal model. <img src="https://latex.codecogs.com/svg.image?S_0" title="https://latex.codecogs.com/svg.image?S_0" /> typically includes contributions from the receiver gain, the proton density and the coil sensitivities. | -- | -- |
| CAPLEX:Q.MS1.011 | <a name="n k-space"></a> Number of lines to k-space center | --| *n* | The number of lines to *k*-space center in the phase encoding direction. | -- | -- |
| CAPLEX:Q.MS1.012 | <a name="N k-space"></a> Total number of k-space lines | -- | *N* | The total number of phase encoding lines for acquiring an image. | -- | -- |
| DIFFUSIONLEX:Q.MS1.001 | <a name="Big Delta"></a>  Diffusion time | -- |  $\Delta$ | The time interval between bi-polar diffusion encoding gradient | ms | -- |
| DIFFUSIONLEX:Q.MS1.002 | <a name="Little Delta"></a>  Diffusion gradient duration | -- | $\delta$ | The duration of the diffusion encoding gradient | ms | -- |
| DIFFUSIONLEX:Q.MS1.003 | <a name="Diffusion gradient strength"></a>  Diffusion gradient strength | -- | *G* | The strength of the diffusion encoding gradient | mT/m | -- |
| DIFFUSIONLEX:Q.MS1.004 | <a name="b"></a>  b-value | -- | *b-value* | A factor that reflects the strength and timing of the gradients used to generate diffusion-weighted images |  s/mm² | -- |
| Q.MS1.999 | <a name="not listed MS1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Electromagnetic quantities"></a> Electromagnetic quantities
The items in this group are related to electromagnetic tissue properties. The abbreviations SE and GE denote spin and gradient echo.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| CAPLEX:Q.EL1.001.[j]| <a name="R1"></a> Longitudinal relaxation rate | *R<sub>1</sub>* -relaxation rate | *R<sub>1,j</sub>* | Longitudinal relaxation rate in compartment *j*. | 1/s | -- |
| CAPLEX:Q.EL1.004.[j] | <a name="R2"></a>  Transverse relaxation rate (SE) | *R<sub>2</sub>*-relaxation rate | *R<sub>2,j</sub>* | Natural transverse relaxation rate (observed using a SE) in compartment *j*. | 1/s | -- |
| CAPLEX:Q.EL1.007.[j] | <a name="R2Star"></a> Transverse relaxation rate (GE) | *R<sub>2</sub><sup>*</sup>*-relaxation rate | *R<sub>2,j</sub><sup>*</sup>* | Effective transverse relaxation rate (observed using a GE) in compartment *j*. | 1/s | -- |
| CAPLEX:Q.EL1.011.[j] | <a name="Chi"></a> Molar magnetic susceptibility | -- | $\chi_{j}$ | Molar magnetic susceptibility in compartment *j*. | mL/mol | -- |
| Q.EL1.999 | <a name="not listed EL1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Diffusion quantities"></a>  Diffusion tensor imaging model quantities
The items of this group of quantities are either measured or modeled quantities used when pharmacokinetic modeling is applied.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| DIFFUSIONLEX:Q.DTI1.001 | <a name="D"></a> Apparent diffusion coefficient | Trace | *ADC* | The diffusion coefficient of water as observed in a diffusion-weighted MRI averaged over the three principal directions (i.e. the mean of the 3 tensor eignevalues). The "Apparent" describes the fact that water in biological tissues is hindered/restricted and hence appears lower than it would in a freely diffusing environment  | mm²/s | -- |
| DIFFUSIONLEX:Q.DTI1.002 | <a name="D"></a> Diffusion Tensor | -- | **D** | A 3 x 3 symmetric tensor matrix containing elements (Dxx, Dxy, Dxz, etc) representing observed diffusion coefficients along different directions in anisotropic media. | mm²/s | -- |
| DIFFUSIONLEX:Q.DTI1.003 | <a name="RD"></a> Radial Diffusivity | -- | $D_{r}$ | The diffusion coefficient of water as observed in a diffusion-weighted MRI in a direction perpendicular to of an axonal fibre. Often used as a marker of axonal integrity. | mm²/s | -- |
| DIFFUSIONLEX:Q.DTI1.004 | <a name="AD"></a> Axial Diffusivity | -- | $D_{a}$ | The diffusion coefficient of water as observed in a diffusion-weighted MRI along parralel to the axis of an axonal fibre. | mm²/s | -- |
| DIFFUSIONLEX:Q.DTI1.003 | <a name="FA"></a> Fractional Anistropy | -- | *FA* | A scalar value between 0 and 1 that describes the degree of anisotropy of a diffusion process. $$FA = \frac{\sqrt{(\lambda_{1} - \lambda_{2}) + (\lambda_{2} - \lambda_{3}) + (\lambda_{1} - \lambda_{3})}}{\sqrt{2}\lambda_{1} + \lambda_{2} + \lambda_{3}}$$ | n.a. | -- |
| Q.DTI1.999 | <a name="not listed IC1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Microstructure quantities"></a> Microstructure quantities
In this group commonly used quantities with a physiological meaning are listed.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.PH1.001.[j] | <a name="v"></a> Relative volume fraction | -- | *v<sub>j</sub>* | The relative volume fraction of compartment *j*. Only capillary vasculature is considered, thus the *c* subscript is dropped. | mL/100mL | -- |
| Q.PH1.007 | <a name="Ta"></a> Arterial delay time | -- | *T<sub>a</sub>*  | Delay between indicator arrival at the arterial input function location and the voxel or tissue region of interest. | s | -- |
| Q.PH1.009.[j] | <a name="k"></a> Indicator exchange rate | -- | *k<sub>j</sub>*  | Indicator exchange  rate constant between two compartments (e.g. *k<sub>e &#8594 b</sub>*) | 1/s | -- |
| Q.PH1.010.[j] | <a name="kw"></a> Water exchange rate  | *k<sub>in</sub>*, *k<sub>out</sub>* | *k<sub>w,j</sub>* | Equilibrium water exchange rate between two compartments  (e.g. *k<sub>w, e &#8594 b</sub>*)  | 1/s | -- |
| Q.PH1.011 | <a name="rho"></a> Density | -- | *&#961* | The density of the tissue of interest. | g/mL | -- |
| Q.PH1.012.[j] | <a name="Hct"></a> Hematocrit | -- | *Hct<sub>j</sub>*  | The volume percentage of red blood cells in the blood compartment *j*. | -- | -- |
| Q.PH1.013 | <a name="Hctf"></a> Hematocrit factor|-- | *Hct<sub>f</sub>* | Blood flow correction factor accounting for the difference in arterial hematocrit *Hct<sub>a</sub>* and capillary hematocrit *Hct<sub>c</sub>*.| -- | -- |
| Q.PH1.014 | <a name="CTTH"></a> Capillary transit time heterogeneity | -- | *CTTH* | Standard deviation of the capillary transit time distribution.| s | -- |
| Q.PH1.015 | <a name="OEFmax"></a> Maximum oxygen extraction fraction| -- | OEF<sup>max</max> | Upper biophysical limit of the proportion of oxygen that can be extracted by tissue. | -- | --|
| Q.PH1.999 | <a name="not listed PH1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Exchange quantities"></a> Exchange quantities
In this group commonly used quantities relating to exchange of water across cell membranes are described.
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.PH1.010.[j] | <a name="kw"></a> Water exchange rate  | *k<sub>in</sub>*, *k<sub>out</sub>* | *k<sub>w,j</sub>* | Equilibrium water exchange rate between two compartments  (e.g. *k<sub>w, e &#8594 b</sub>*)  | 1/s | -- |
| Q.EX1.001 | <a name="AXR"></a> Apparent exchange rate | -- | AXR  | The apparent exchange rate of water across a membrane observed using filtered exchange imaging. $$AXR = k_in + k_out$$. | 1/min | -- |
| Q.EX1.001 | <a name="filter_eff"></a> Filter efficiency | -- | $\sigma$ | The ratio of diffusivity at very short mixing time with and without the diffusion filter in FEXI experiment | a.u. | -- |
| Q.PH1.004 | <a name="PS"></a> Permeability surface area product | Extraction flow (FE) | *PS* | The volume of tissue plasma that is fully cleared of indicator in a unit of time by a unit tissue volume. | mL/min/100mL | -- |
| Q.PH1.005 | <a name="E"></a> Extraction fraction | -- | *E*  | The fraction of indicator particles that is extracted from plasma in one pass through the vasculature. | -- | -- |
| Q.PH1.008 | <a name="Ktrans"></a> Volume transfer constant | Transfer constant | *K<sup>trans</sup>* | The rate of indicator particle delivery from the blood plasma to the extravascular, extracellular volume per unit of tissue volume, per unit arterial plasma concentration. | 1/min | -- |
| Q.PH1.015 | <a name="OEFmax"></a> Maximum oxygen extraction fraction| -- | OEF<sup>max</max> | Upper biophysical limit of the proportion of oxygen that can be extracted by tissue. | -- | --|
| Q.PH1.999 | <a name="not listed PH1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Flow quantities"></a> Flow quantities
In this group commonly used quantities related to vascular, interstitial, or CSF flow are described.
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.PH1.006.[j] | <a name="MTT"></a> Mean transit time| -- | *MTT<sub>j</sub>* | The average time the indicator spends in compartment *j* before exchanging into another compartment. | s | -- |
Q.PH1.003 | <a name="Fb"></a> Blood flow | Cerebral blood flow (CBF) | *F<sub>b</sub>* | The volume of blood flowing into a unit tissue volume per unit time. The flow inputs and exits the capillary vasculature. | mL/min/100mL | -- |
| Q.PH1.006.[j] | <a name="MTT"></a> Mean transit time| -- | *MTT<sub>j</sub>* | The average time the indicator spends in compartment *j* before exchanging into another compartment. | s | -- |
| Q.PH1.014 | <a name="CTTH"></a> Capillary transit time heterogeneity | -- | *CTTH* | Standard deviation of the capillary transit time distribution.| s | -- |
| DIFFUSIONLEX:Q.Ex1.001.[j] | <a name="v"></a> Relative volume fraction | -- | *v<sub>j</sub>* | The relative volume fraction of compartment *j*. Only capillary vasculature is considered, thus the *c* subscript is dropped. | mL/100mL | -- |
| DIFFUSIONLEX:Q.Ex1.003 | <a name="Fb"></a> Blood flow | Cerebral blood flow (CBF) | *F<sub>b</sub>* | The volume of blood flowing into a unit tissue volume per unit time. The flow inputs and exits the capillary vasculature. | mL/min/100mL | -- |
| Q.PH1.007 | <a name="Ta"></a> Arterial delay time | -- | *T<sub>a</sub>*  | Delay between indicator arrival at the arterial input function location and the voxel or tissue region of interest. | s | -- |
| Q.PH1.012.[j] | <a name="Hct"></a> Hematocrit | -- | *Hct<sub>j</sub>*  | The volume percentage of red blood cells in the blood compartment *j*. | -- | -- |
| Q.PH1.013 | <a name="Hctf"></a> Hematocrit factor|-- | *Hct<sub>f</sub>* | Blood flow correction factor accounting for the difference in arterial hematocrit *Hct<sub>a</sub>* and capillary hematocrit *Hct<sub>c</sub>*.| -- | -- |
| Q.PH1.999 | <a name="not listed PH1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="General physical and mathematical quantities"></a> General physical and mathematical quantities
This section contains general physical and mathematical quantities which are used in the context of perfusion image analysis.

| Code | OSIPI name | Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.GE1.001 | <a name="DataGrid"></a> Data grid | -- | *[x<sub>1</sub>,...,x<sub>n</sub>]* | Sampling points of a data set (typically time or frequency). | variable | -- |
| Q.GE1.002 | <a name="Data"></a> Data | -- | *[f<sub>1</sub>,...,f<sub>n</sub>]* | Values of a data set with respect to a data grid. The data set has the value *f<sub>i</sub>* at data grid point *x<sub>i</sub>*. | variable | -- |
| Q.GE1.003 | <a name="index"></a> Index | -- | *i* | The number of the index of a data or data grid point. | -- | -- |
| Q.GE1.004 | <a name="time"></a> Time | -- | *t* | Time | s | -- |
| Q.GE1.005 | <a name="timeStep"></a> Time step | -- | *&#916t*  | Time between two successive data points, e.g. two images (for fixed temporal resolution). | s | -- |
| Q.GE1.006 | <a name="freq"></a> Frequency | -- | *&#957* |Frequency | 1/s | -- |
| Q.GE1.007 | <a name="Lax"></a> Axial length | -- | *L<sub>ax</sub>* | The axial length of a cylindrical object, e.g. a capillary. | &#956m | -- |
| Q.GE1.008 |<a name="xax"></a>  Axial position | -- | *x<sub>ax</sub>* | The spatial position within a cylindrical object, e.g. a capillary. In the case of a capillary x=0 denotes the arterial inlet position and x=L<sub>ax</sub> the venous outlet position. | &#956m | -- |
| Q.GE1.009 | <a name="const"></a> Constant value | -- | *k* | A constant value which can be used e.g. for scaling. | variable | -- |
| Q.GE1.010 | <a name="L"></a> Lower threshold | -- | *L* | The lower value at which the behavior of a function or algorithm changes. | variable | -- |
| Q.GE1.011 | <a name="U"></a> Upper threshold | -- | *U* | The upper value at which the behavior of a function or algorithm changes.   | variable | -- |
| Q.GE1.012 | <a name="f(x)"></a> Dynamic function | -- | *f(x)* | A function of an independent variable *x* (typically time or frequency) with value *f(x<sub>i</sub>)* at data grid point *x<sub>i</sub>*. | variable | -- |
| Q.GE1.013 | <a name="x_start"></a> Start of range | -- | *x<sub>start</sub>* | The start point of the range [*x<sub>start</sub>*, *x<sub>end</sub>*].  | variable | -- |
| Q.GE1.014 | <a name="x_end"></a> End of range | -- | *x<sub>end</sub>*  | The end point of the range [*x<sub>start</sub>*, *x<sub>end</sub>*]. | variable | -- |
| Q.GE1.015 | <a name="sampleSize"></a> Sample size | -- | *n* | The number samples within a data set.| variable | -- |
| Q.GE1.999 | <a name="not listed GE1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Curve descriptive quantities"></a> Curve descriptive quantities
Descriptive parameters describe the shape of a data set sampled at a data grid, but do not offer a direct physiological interpretation. <br/>
The data set is often the measured MR signal sampled at specified time points, but it can also be some normalized version of it, or a derived signal such as dynamic concentration time curve or dynamic relaxation rate curve derived from an MR signal.
To keep the inputs of these processes flexible, they are all defined for general data *f(x<sub>i</sub>)* on a data grid of points *f(x<sub>i</sub>)* and it is left to the user to specify the data and data grid these processes are applied to (e.g. [Tissue indicator concentration (Q.I.002) , Time (Q.G.004)]).

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.CD1.001| <a name="f(x_i)"></a> Data value at data grid point | -- | *f(x<sub>i</sub>)* | The data value at the data grid point x<sub>i</sub>. | variable | -- |
| Q.CD1.002 | <a name="f_max"></a> Maximum value | -- | *f<sub>max</sub>* | The maximum value of given data. | variable | -- |
| Q.CD1.003 | <a name="x_max"></a> Data grid point of maximum value| -- | *x<sub>max</sub>* | The data grid point at which the maximum value of a given data set occurs. | variable | -- |
| Q.CD1.004 | <a name="f_min"></a> Minimum value | -- | *f<sub>min</sub>* | The minimum value of given data. | variable | -- |
| Q.CD1.005 | <a name="x_min"></a> Data grid point of minimum value | -- | *x<sub>min</sub>* |The data grid point at which the minimum value of a given data set occurs. | variable | -- |
| Q.CD1.006 | <a name="f_fin"></a> Final data value | -- | f<sub>fin</sub> | The value of the data at the last data grid point. | variable | --|
| Q.CD1.007 | <a name="x_fin"></a> Final data grid point | -- | x<sub>fin</sub> | The last point of a given data grid. | variable | -- |
| Q.CD1.008 | <a name="maxDev"></a> Maximum deviation from baseline | -- | *&#916 f<sub>BL,max</sub>* | The maximum absolute deviation of a given data set from the baseline. | variable | -- |
| Q.CD1.009 | <a name="Deriv"></a> Derivative at data grid point <img src="https://latex.codecogs.com/svg.image?x_i" title="https://latex.codecogs.com/svg.image?x_i" /> | -- | <img src="https://latex.codecogs.com/svg.image?\frac{df(x_i)}{dx}" title="https://latex.codecogs.com/svg.image?\frac{df(x_i)}{dx}" /> | Derivative of a function f with respect to the independent variable x at the data grid point <img src="https://latex.codecogs.com/svg.image?x_i" title="https://latex.codecogs.com/svg.image?x_i" />. | variable | -- |
| Q.CD1.010 | <a name="TTP"></a> Time to peak | -- | *TTP* | The time between the bolus arrival time (BAT) and the maximum time point *x<sub>max</sub>*. *TTP=x<sub>max</sub>-BAT* <br/>(Remark: this is expressed for time rather than a general data grid, because TTP is an often used parameter in perfusion analysis). | variable | -- |
| Q.CD1.011 | <a name="WIS"></a> Wash-in-slope | -- | *WIS* | The ratio of the difference of the maximum data value *f<sub>max</sub>* and the baseline value *f<sub>BL</sub>* and the time to peak: <img src="https://latex.codecogs.com/svg.image?\frac{f_{max}-f_{BL}}{TTP}" title="https://latex.codecogs.com/svg.image?\frac{f_{max}-f_{BL}}{TTP}" />  | variable_1/variable_2 | -- |
| Q.CD1.012 | <a name="WOS"></a> Wash-out-slope | -- | *WOS* | The ratio of the difference of the maximum data value f<sub>max</sub> and the data value at the last data grid point f<sub>fin</sub> and difference between the last time point and the time at which the maximum occurs: <img src="https://latex.codecogs.com/svg.image?\frac{f_{max}-f_{fin}}{x_{max}-x_{fin}}" title="https://latex.codecogs.com/svg.image?\frac{f_{max}-f_{fin}}{x_{max}-x_{fin}}" /> | variable_1/variable_2 | -- |
| Q.CD1.013 | <a name="AUC"></a> Area under curve | --| *AUC<sub>x<sub>start</sub>,x<sub>end</sub></sub>* | The integral value of a given dynamic function f (or the numeric approximation for discrete data <img src="https://latex.codecogs.com/svg.image?[f_1,...f_n]" title="https://latex.codecogs.com/svg.image?[f_1,...f_n]" /> ) between the data grid points <img src="https://latex.codecogs.com/svg.image?x_1" title="https://latex.codecogs.com/svg.image?x_1" /> and <img src="https://latex.codecogs.com/svg.image?x_2" title="https://latex.codecogs.com/svg.image?x_2" />.  | <img src="https://latex.codecogs.com/svg.image?variable_1&space;\cdot&space;variable_2" title="https://latex.codecogs.com/svg.image?variable_1 \cdot variable_2" /> | --|
| Q.DC1.999 | <a name="not listed DC1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Bolus arrival time estimation quantities"></a> Bolus arrival time estimation quantities
This section lists all quantities related to the estimation process of the bolus arrival time of a data curve.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.BA1.001 | <a name="BAT"></a> Bolus arrival time | Onset Time, Lag Time| *BAT* | The time between the first data grid point and the onset obtained by applying a specified BAT estimation method. | variable| -- |
| Q.BA1.002 | <a name="IntersectionBATParms"></a> Intersection- based BAT estimation parameters| --| *[N]* | Vector of ordered inputs to the intersection-based BAT estimation process. | -- | --|
| Q.BA1.999 | <a name="not listed BA1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Baseline estimation quantities"></a> Baseline estimation quantities
This section lists all quantities related to the estimation process of the baseline of a data curve.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.BL1.001 | <a name="f_BL"></a> Baseline value  | -- | f<sub>BL</sub> | The value of a series of data of constant values in the beginning of a data set before the behavior of the data set changes. The baseline value is obtained by applying the baseline estimation process. | variable | -- |
| Q.BL.999 | <a name="not listed BL1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Descriptive model quantities"></a> Descriptive model quantities
This section lists all quantities related to the estimation process of the baseline of a data curve.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.DM1.001 | <a name="UnitStepParams"></a> Unit step model parameters  | -- | *[T]* | Vector of ordered inputs to the unit step model (M.DM1.001).| [variable units] | -- |
| Q.DM1.002 | <a name="LinQuandraticParams"></a> Linear-quadratic model parameters | -- | *[BAT,f<sub>BL</sub>,&#946<sub>1</sub>,&#946<sub>2</sub>]* | Vector of ordered inputs to the linear quadratic model (M.DM1.002). | [variable units]  | -- |
| Q.DM1.003 | <a name="2SLParams"></a> Two step linear model parameters | -- | *[BAT,f<sub>BL</sub>,b<sub>1</sub>]* | Vector of ordered inputs to the two step linear model (M.DM1.003). | [variable units] | -- |
| Q.DM1.004 | <a name="3SLPamars"></a> Three step linear model parameters | -- | *[BAT,f<sub>BL</sub>,&#946, b<sub>1</sub>,b<sub>2</sub>]* | Vector of ordered inputs to the three step linear model (M.DM1.004). | [variable units] | -- |
| Q.DM1.005 | <a name="MultiExpParams"></a> Multi-exponential model parameters | -- | *[A<sub>1</sub>,...A<sub>n</sub>,a<sub>1</sub>,...a<sub>n</sub>]* | Vector of ordered inputs to the multi-exponential model (M.DM1.005). |[variable units]  | -- |
| Q.DM1.006 | <a name="GammaVarParams"></a> Gamma-variate model parameters | -- | *[BAT,&#945,&#946]* | Vector of ordered inputs to the gamma-variate model (M.DM1.006). | [variable units] | -- |
| Q.DM1.007 | <a name="FermiParams"></a> Fermi model parameters | -- | *[F,a,b]* | Vector of ordered inputs to the Fermi model (M.DM1.007). | [variable units] | -- |
| Q.DM1.008 | <a name="NormalParams"></a> Normal distribution model parameters | -- | *[&#956,&#963]* | Vector of ordered inputs to normal distribution model (M.DM1.008). | [variable units] | -- |
| Q.DM1.999 | <a name="not listed DM1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |



## <a name="Leakage correction model quantities"></a> Leakage correction model quantities
Leakage correction model parameters are typically ad-hoc correction factors for physical models that are not purely descriptive but are not derived from rigorous physical models, therefore they are not listed in the physiological quantities group. 

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.LC1.001 | <a name="K1"></a> Uncontaminated R<sub>2</sub><sup>*</sup> scaling term  |--| K<sub>1</sub> | Scaling constant for the uncontaminated effective transverse relaxation rate in the BSW leakage correction model and Bidirectional leakage correction model. | -- | -- |
| Q.LC1.002 | <a name="K2"></a> Leakage scaling term | -- | K<sub>2</sub> | Scaling constant which reflects the effects of leakage in the BSW leakage correction model and Bidirectional leakage correction model. | 1/s | -- |
| Q.LC1.999 | <a name="not listed LC1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Uncertainty and statistical quantities"></a> Uncertainty and statistical quantities
<b><font color=#FF0000>This section is currently work in progress</font></b> </br></br>
In this group commonly used quantities to describe uncertainties of the extracted parameters and other statistical properties in the context of perfusion image analysis.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.US1.001 | <a name="Mean_sample"></a> Arithmetic mean (sample) | Average | <img src="https://latex.codecogs.com/svg.image?\bar{x}" title="https://latex.codecogs.com/svg.image?\bar{x}" /> | The mean value of a given data sample *[x<sub>1</sub>,...,x<sub>n</sub>]*, with sample size n, calculated as <img src="https://latex.codecogs.com/svg.image?\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_i" title="https://latex.codecogs.com/svg.image?\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_i" />.| variable | -- |
| Q.US1.002 | <a name="GeomMean_sample"></a> Geometric mean (sample) | -- | <img src="https://latex.codecogs.com/svg.image?\bar{x}_{geom}" title="https://latex.codecogs.com/svg.image?\bar{x}_{geom}" />| The mean value of a given data sample *[x<sub>1</sub>,...,x<sub>n</sub>]*, with sample size n, calculated as <img src="https://latex.codecogs.com/svg.image?\bar{x}_{geom}=\sqrt[n]{\prod_{i=1}^{n}x_i}" title="https://latex.codecogs.com/svg.image?\bar{x}_{geom}=\sqrt[n]{\prod_{i=1}^{n}x_i}" />| variable| -- |
| Q.US1.003 | <a name="Var"></a> Variance (sample) | -- | *s<sup>2</sup>* | Mean squared deviation of the mean of a given data set *[x<sub>1</sub>,...,x<sub>n</sub>]* with sample size *n* and mean value <img src="https://latex.codecogs.com/svg.image?\bar{x}" title="https://latex.codecogs.com/svg.image?\bar{x}" />, calculated as <img src="https://latex.codecogs.com/svg.image?s^2=\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}" title="https://latex.codecogs.com/svg.image?s^2=\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}" />.| variable<sup>2</sup> | -- |
| Q.US1.004 | <a name="StdDev"></a> Standard deviation (sample)| -- | *s* | The standard deviation of the mean value of a given data set *[x<sub>1</sub>,...,x<sub>n</sub>]* with sample size *n* and mean value <img src="https://latex.codecogs.com/svg.image?\bar{x}" title="https://latex.codecogs.com/svg.image?\bar{x}" /> , calculated as <img src="https://latex.codecogs.com/svg.image?s^2=\sqrt{\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}}" title="https://latex.codecogs.com/svg.image?s^2=\sqrt{\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}}" />. | variable | -- |
| Q.US1.005 | <a name="Median"></a> Median value (sample) | -- | *x<sub>median</sub>* | Centermost point  of ordered data points   for an odd number of samples or the average of the two centermost points xn/2+xn/2+12 for an even number of samples. | variable | -- |
| Q.US1.006 | -- | -- | -- | -- | -- | -- |
| Q.US1.007 | -- | -- | -- | -- | -- | -- |
| Q.US1.008 | -- | -- | -- | -- | -- | -- |
| Q.US1.009 | -- | -- | -- | -- | -- | -- |
| Q.US1.010 | -- | -- | -- | -- | -- | -- |
| Q.US1.011 | -- | -- | -- | -- | -- | -- |
| Q.US1.012 | -- | -- | -- | -- | -- | -- |
| Q.US1.013 | -- | -- | -- | -- | -- | -- |
| Q.US1.014 | -- | -- | -- | -- | -- | -- |
| Q.US1.015 | -- | -- | -- | -- | -- | -- |
| Q.US1.016 | -- | -- | -- | -- | -- | -- |
| Q.US1.017 | -- | -- | -- | -- | -- | -- |
| Q.US1.018 | -- | -- | -- | -- | -- | -- |
| Q.US1.019 | -- | -- | -- | -- | -- | -- |
| Q.US1.020 | -- | -- | -- | -- | -- | -- |
| Q.US1.021 | -- | -- | -- | -- | -- | -- |
| Q.US1.022 | -- | -- | -- | -- | -- | -- |
| Q.US1.023 | -- | -- | -- | -- | -- | -- |
| Q.US1.024 | -- | -- | -- | -- | -- | -- |
| Q.US1.025 | -- | -- | -- | -- | -- | -- |
| Q.US1.026 | -- | -- | -- | -- | -- | -- |
| Q.US1.027 | -- | -- | -- | -- | -- | -- |
| Q.US1.028 | -- | -- | -- | -- | -- | -- |
| Q.US1.999 |  Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |



## <a name="Analytical inversion quantities"></a> Analytical inversion quantities

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.AI1.001 | <a name="AI_SMP"></a> Static model parameters | -- |SMP | A vector of the known quantities of a forward model. Select from section Q. | [variable units] | -- |
| Q.AI1.002 | <a name="AI_MP"></a> Model parameters | -- | MP | A vector of the quantities to be determined by the analytical inversion of a forward model. Select from section Q. | [variable units] |-- |
| Q.AI1.999 | <a name=""></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Optimization quantities"></a> Optimization quantities
In this group, quantities related to optimization methods are listed. In this version, only least squares optimization methods are considered. Approaches that use e.g. maximum likelihood estimation, bayesian inference, machine learning will be taken into account in future versions of the lexicon.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.OP1.001 | <a name="MP"></a> Model parameters | -- |*&#934*, MP | A vector of quantities which are the variable of the model fitting process. Select from section Q. | [variable units] | -- |
| Q.OP1.002 | <a name="SMP"></a> Static model parameters | --| &#952, SMP | A vector of the quantities of the forward model to be fitted which are not in the scope of the optimization. Select from section Q. | [variable units] | -- |
| Q.OP1.003 | <a name="EMP"></a> Estimated model parameter | -- | <img src="https://latex.codecogs.com/svg.image?\hat{\phi}" title="https://latex.codecogs.com/svg.image?\hat{\phi}" />, EMP | A vector (in the same order as model parameters, indicated with “^”) of the estimated model parameters resulting from the optimization process. | [variable units] | -- |
| Q.OP1.004 | <a name="CostValue"></a> Cost value | -- | *C* | The scalar or vectorial value of a specified cost function. | [variable units] | -- |
| Q.OP1.005 | <a name="CostValue_min"></a> Cost value minimum | -- | *C<sub>min</sub>*| The minimum cost value as returned by an optimizer. This can be a local or global minimum. | [variable units] | -- |
| Q.OP1.006 | <a name="MP_init"></a> Initial model parameters | -- | *&#934<sub>init</sub>* | Vector of the starting values of the search for the model parameters. | [variable units] | -- |
| Q.OP1.007 | <a name="MP_L"></a> Model parameter lower bounds | -- | *&#934<sub>LB</sub>* | Vector of the lower bounds for the search for the model parameters. | [variable units] | -- |
| Q.OP1.008 | <a name="MP_U"></a> Model parameter upper bounds | -- | *&#934<sub>UB</sub>* | Vector of the upper bounds for the search for the model parameters. | [variable units]  | -- |
| Q.OP1.009 | <a name="Weights"></a> Data weights | -- | *&#969* | Vector of weights on the measured values during the optimization process. | -- | -- |
| Q.OP1.010 | <a name="N_iter_max"></a> Maximum number of iterations | -- | *N<sub>it,max</sub>*| Largest number of steps taken in an iterative optimization. | - | -- |
| Q.OP1.011 | <a name="ConvThresh"></a> Convergence threshold | -- | *e* | Convergence threshold on the optimizer. | -- | -- |
| Q.OP1.012 | <a name="A"></a> Linear coefficients matrix | -- |*A* | A matrix with elements A<sub>ij</sub> with which a function linear in the model parameters  can be  expressed as <img src="https://latex.codecogs.com/svg.image?f(\phi;x_i)=&space;\sum_{j=1}^{m}A_{ij}\phi_j" title="https://latex.codecogs.com/svg.image?f(\phi;x_i)= \sum_{j=1}^{m}A_{ij}\phi_j" />. The A<sub>ij</sub> contain the data grid and the static model parameters.| -- | -- |
| Q.OP1.013 | <a name="Lambda"></a> Regularization parameter | -- |*&#955* | A parameter which determines the weight of the regularization in an optimization.  | -- | -- |
| Q.OP1.014 | <a name="Lambda_norm"></a> Normalized regularization parameter | -- | <img src="https://latex.codecogs.com/svg.image?\hat{\lambda}" title="https://latex.codecogs.com/svg.image?\hat{\lambda}" /> | The regularization parameter is expressed relative to the largest singular value &#963<sub>1</sub> of a SVD: <img src="https://latex.codecogs.com/svg.image?\hat{\lambda}=\frac{\lambda}{\sigma_1}" title="https://latex.codecogs.com/svg.image?\hat{\lambda}=\frac{\lambda}{\sigma_1}" /> .| -- | -- |
| Q.OP1.015 | <a name="Lambda_fixed"></a> Fixed *&#955* value | -- | *&#955<sub>fixed</sub>* | A fixed value, e.g. a literature value, assumed as regularization parameter. | -- | -- |
| Q.OP1.999 | <a name="not listed OP1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |



## <a name="Native R1 estimation quantities"></a> Native R1 estimation quantities
This group lists quantities required in the context of native R1 estimation.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.NR1.001 | <a name="R10_fixed"></a> Fixed R10 value | -- | *R<sub>10,fixed</sub>* | A fixed value, e.g. a literature value, assumed as native *R<sub>1</sub>* relaxation rate value.| 1/ms | -- |
| Q.NR1.999 | <a name="not listed NR1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Arterial input function estimation quantities"></a> Arterial input function estimation quantities
The items of this group are quantities which are required to describe arterial input function estimation methods.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.AE1.001 | <a name="kMeansParams"></a> *k*-means-cluster-algorithm-parameters | -- | *[k]* | Vector of ordered inputs to the *k*-means AIF detection algorithm. | [variable units] | -- |
| Q.AE1.002 | <a name="fuzzycMeansParams"></a> Fuzzy-c-means-cluster-algorithm-parameters | -- | *[m,&#917,c,P<sub>c</sub>,c<sub>i</sub>]* | Vector of ordered inputs to the fuzzy-c-means AIF detection algorithm. | [variable units] | -- |
| Q.AE1.003 | <a name="PVC"></a> Partial-volume corrected | -- | PVE | If the value of this flag is 1, partial volume effects are accounted for. Otherwise, or if not specified, no partial volume effect correction was done. | -- | -- |
| Q.AE1.004 | <a name="DB"></a> Dual Bolus | -- | DB | The full-dose AIF is reconstructed from pre-bolus injection with a smaller dose. If the value of this flag is 1, a dual bolus approach is used. Otherwise, or if not specified, no dual bolus approach is used. | -- | --|
| Q.AE1.005 | <a name="PA"></a> Arterial partial volume correction factor| -- | *P<sub>A</sub>* | A factor that scales signal or indicator concentrations measured in a partial volume affected artery such that partial volume effects are removed. Usually this is estimated by deconvolving arterial and venous signals or indicator concentrations. | -- | -- |
| Q.AE1.999 | <a name="not listed AE1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |


## <a name="Segmentation quantities"></a> Segmentation quantities
This group contains quantities related to the process of image segmentation.

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.SE1.001 | <a name="BinMask"></a> Binary mask | -- | Mask | Binary mask of segmented region of interest. | -- | -- |
| Q.SE1.002 | <a name="BinAIFMask"></a> Binary AIF mask | -- | AIF mask | Binary mask of a vessel in which the arterial input function is estimated. | -- | -- |
| Q.SE1.003 | <a name="BinROIMask"></a> Binary ROI mask | -- | ROI mask | Binary mask of a tissue region of interest. | -- | -- |
| Q.SE1.004 | <a name="Seeds"></a> Seeds | -- | [seeds] | Vector of ordered voxel coordinates of seed points for seed based segmentation (e.g. region growing segmentation). | -- | -- |
| Q.SE1.005 | <a name="N_kMeans"></a> Number of k–means clusters | -- | *N<sub>k-means</sub>* | Number of clusters in the k-means clustering algorithm. | -- | -- |
| Q.SE1.999 | <a name="not listed SE1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

