# Sections Q: Quantities

## <a name="MRI sequence quantities"></a> MRI sequence quantities
The items in this group are related to the MR sequence used to acquire the signal.

| Code | Standardised name| Alternative names|Notation|Description|Standardised units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| DIFFUSIONLEX:XXX | <a name="Big Delta"></a>  Diffusion time | -- |  $\Delta$ | The time interval between bi-polar diffusion encoding gradient | ms | -- |
| DIFFUSIONLEX:XXX | <a name="Little Delta"></a>  Diffusion gradient duration | -- | $\delta$ | The duration of the diffusion encoding gradient | ms | -- |
| DIFFUSIONLEX:XXX | <a name="Diffusion gradient strength"></a>  Diffusion gradient strength | -- | *G* | The strength of the diffusion encoding gradient | mT/m | -- |
| DIFFUSIONLEX:XXX | <a name="b"></a>  b-value | -- | *b-value* | A factor that reflects the strength and timing of the gradients used to generate diffusion-weighted images |  s/mm² | -- |
| DIFFUSIONLEX:XXX | <a name="not listed MS1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Diffusion tensor quantities"></a>  Diffusion tensor quantities
The items of this group are quantities related to diffusion of water (rate, directionality, orientation)

| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| DIFFUSIONLEX:XXX | <a name="D"></a> Apparent diffusion coefficient | (Trace)/3 | *ADC* | The diffusion coefficient of water as observed in a diffusion-weighted MRI averaged over the three principal directions (i.e. the mean of the 3 tensor eignevalues). The "Apparent" describes the fact that water in biological tissues is hindered/restricted and hence appears lower than it would in a freely diffusing environment  | mm²/s | -- |
| DIFFUSIONLEX:XXX | <a name="D"></a> Diffusion Tensor | -- | **D** | A 3 x 3 symmetric tensor matrix containing elements (Dxx, Dxy, Dxz, etc) representing observed diffusion coefficients along different directions in anisotropic media. | mm²/s | -- |
| DIFFUSIONLEX:XXX | <a name="RD"></a> Radial Diffusivity | -- | $D_{r}$ | The diffusion coefficient of water as observed in a diffusion-weighted MRI in a direction perpendicular to of an axonal fibre. Often used as a marker of axonal integrity. | mm²/s | -- |
| DIFFUSIONLEX:XXX | <a name="AD"></a> Axial Diffusivity | -- | $D_{a}$ | The diffusion coefficient of water as observed in a diffusion-weighted MRI along parralel to the axis of an axonal fibre. | mm²/s | -- |
| DIFFUSIONLEX:XXX | <a name="FA"></a> Fractional Anistropy | -- | *FA* | A scalar value between 0 and 1 that describes the degree of anisotropy of a diffusion process. $$FA = \frac{\sqrt{(\lambda_{1} - \lambda_{2}) + (\lambda_{2} - \lambda_{3}) + (\lambda_{1} - \lambda_{3})}}{\sqrt{2}\lambda_{1} + \lambda_{2} + \lambda_{3}}$$ | n.a. | -- |

 CL, CP, and CS: the linear, planar, and spherical shape measures.
 Mode of anisotropy (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3163395/#:~:text=In%20diffusion%20MRI%2C%20magnetic%20field,areas)%20due%20to%20anisotropic%20diffusion.)
| Q.DTI1.999 | <a name="not listed IC1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Tractography quantities"></a> Tractography quantities
In this group quantities used to describe tractography are listed 
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
Euler’s method (following the eigenvector or tangent for a fixed step size) -(https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3163395/#:~:text=In%20diffusion%20MRI%2C%20magnetic%20field,areas)%20due%20to%20anisotropic%20diffusion.))
second order Runge-Kutta (also known as the midpoint method, where the tangent is followed for half a step, then a new tangent is calculated at the midpoint of the interval and used to take the full step), 
fourth order Runge-Kutta (where the weighted average of four estimated tangents to the curve is used when taking each step) 
FACT 
Some related methods attempt to introduce “inertia” when tracking through regions of planar anisotropy (likely fiber crossings). 
## <a name="Structural connectivity quantities"></a> Structural connectivity quantities
In this group quantities used to describe structural connectivity are listed 
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |

## <a name="Microstructure quantities"></a> Microstructure quantities
In this group quantities used to describe tissue microstructure are listed 
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
(https://www.frontiersin.org/articles/10.3389/fninf.2019.00064/full)
IVIM, 
AxCaliber, 
NODDI
Bingham-NODDI,
the spherical mean-based SMT and MC-MDI, 
and spherical convolution-based single- and multi-tissue CSD
SANDI 
NEXI 
DOC 


## <a name="Exchange quantities"></a> Exchange quantities
In this group commonly used quantities relating to exchange of water across cell membranes are described.
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
| Q.PH1.010.[j] | <a name="kw"></a> Water exchange rate  | *k<sub>in</sub>*, *k<sub>out</sub>* | *k<sub>w,j</sub>* | Equilibrium water exchange rate between two compartments  (e.g. *k<sub>w, e &#8594 b</sub>*)  | 1/s | -- |
| Q.EX1.001 | <a name="AXR"></a> Apparent exchange rate | -- | AXR  | The apparent exchange rate of water across a membrane observed using filtered exchange imaging. $$AXR = k_in + k_out$$. | 1/min | -- |
| Q.EX1.001 | <a name="filter_eff"></a> Filter efficiency | -- | $\sigma$ | The efficient of a diffusion filter. The ratio of diffusivity at very short mixing time with and without the diffusion filter in FEXI experiment | a.u. | -- |
| Q.PH1.004 | <a name="PS"></a> Permeability surface area product of membrane | Extraction flow (FE) | *PS* | The volume of tissue plasma that is fully cleared of indicator in a unit of time by a unit tissue volume. | mL/min/100mL | -- |
| Q.PH1.005 | <a name="E"></a> Extraction fraction | -- | *E*  | The fraction of indicator particles that is extracted from plasma in one pass through the vasculature. | -- | -- |
| Q.PH1.008 | <a name="Ktrans"></a> Volume transfer constant | Transfer constant | *K<sup>trans</sup>* | The rate of indicator particle delivery from the blood plasma to the extravascular, extracellular volume per unit of tissue volume, per unit arterial plasma concentration. | 1/min | -- |
| Q.PH1.015 | <a name="OEFmax"></a> Maximum oxygen extraction fraction| -- | OEF<sup>max</max> | Upper biophysical limit of the proportion of oxygen that can be extracted by tissue. | -- | --|
| Q.PH1.999 | <a name="not listed PH1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |

## <a name="Biophysical quantities"></a> Biophysical quantities
In this group commonly used quantities relating to the bioiphysical properties of tissue are described.
| Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
| -- | -- | -- | -- | -- | -- | -- |
fibre density
neurite density
myelin density
microglial density
neuronal density
fibre orientation
orientation complexity
axon diameter
cell size
