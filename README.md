# TAC reviews

- ~~The font size for the figures is very small.~~
- ~~The authors could explain their choice of c2 for the examples more detailed. In~~ ~~particular, does c2(x) have its minimum at xtg?~~
- ~~On Page 5 I was wondering how the policy is parameterized. Maybe the authors could add
there a hint that this will be explained later.~~
- Why is not p(xtn,m|πψ) used to denote the probability distribution conditioned on πψ?

  **no need, I think this will complexify equations**
- ~~The symbol p() for probability distributions should be defined.~~
- ~~The statement in the abstract that a self-triggered controller is learned by minimizing a cost function might be a little bit confusing. Maybe it would be more clear to write that a self-triggered controller is derived by minimizing a cost function for the lifted model that is learned.~~
- The introduction could be better structured. In the short discussion
of "standard" event-/self-triggered control techniques, it is unclear
why exactly those works are presented. After the short mentioning of
deep reinforcement learning based approaches, it should be stated which
advantages a model-based approach as presented in this note can offer.
 **I have no idea with this**
- ~~When discussing [15], it should be made clearer that [15] considers
periodic control.~~
- ~~The network setting considered in this note should be made explicit.
Where exactly is the network, which information has to be transmitted?
This might also be helpful to better motivate why we not simply
accumulate the cost at the sensor and then send the accumulated cost to
the controller.~~
- ~~It was not obvious in the beginning (at least for me), that the time
for state measurements and the application of the control input is the
same. Maybe it can be added in the second sentence in the intro.~~
- ~~After (1): u_t\in\R^n_u but in (1) u_t\in\U (and clearly U\neq\R).
Same with :\R^n_x??~~
- ~~Footnote 1 is unnecessary.~~
- ~~II B: Then, given D_j, an arbitrary state ... Very long sentence~~
- III G could be written in Theorem-proof form to increase the clarity
- There are some design parameters in the simulation, e.g. \tau min and
max. It would be nice to see how sensitive the results are with respect
to these parameters.
  **no need I think**

- I miss a clear motivation why the proposed approach is important and
extends the state of the art. The authors mention how it differs from
other approaches but it is rarely mentioned why it is necessary. For
instance: 

our approach differs from these works, in the sense that we here
provide a model-based solution, in which the (lifted) dynamics is
learned by the GP regression and the optimal self-triggered controller
is designed accordingly.?

moreover, in constrast [sic] to [14] in which an event-triggered
controller is designed based on a Lyapunov function candidate, our
approach investigates a way to design a self-triggered controller based
on an optimal control problem with a policy gradient technique.?

So what are the benefits of these different approaches? Maybe there are
benefits but I would recommend to point it out in a crystal clear way.

- I am surprised that there are not a single assumption on f.
Obviously, there should be at least some minor assumptions such that a
solution for the DGL (1) exists (which are simple to add). More
important, I would assume that there is a need of Lipschitz like
assumptions to guarantee the feasibility of the proposed algorithm.
Maybe I missed this part but at least some discussion about that would
be of interest to me.
# Other reviews

- While the given tool is the tractable lifting approach?  Please explain it and add some comments in the revised paper.

- In addition, the conclusion should be condensed a little.

- ~~The detail descriptions on the design of self-trigger mechanism are missing.~~

- Generally, the research background is not sufficiently presented in the introduction section (only two paragraphs), which is not friendly to readers.
