# Learning to Transfer with Triply Adversarial Nets

Work in progress, for a tentative paper submission to NIPS'16. Deadline: May 20. 

## Abstract (tentative)

In classification, transfer learning (or its variants known as co-variate shift
or domain adaptation) arises whenever target instances are governed by a
distribution that may be arbitrarily different from the distribution of the
source instances used at training. This problem has traditionally been solved by re-weighting
approaches or by learning robust representations over domains. In this work, we
propose a new paradigm based on the assumption that the co-variate shift is only
due to a different representation of the same underlying objects.
Accordingly, we propose to learn how to transform source instances into target
instances, possibly across input spaces of distinct dimensions, structures or
supports. For this purpose, we extend the generative adversarial networks
framework of \cite{goodfellow2014generative} to a triply adversarial process: a
transformer network $G$ for generating target instances from source instances, a
discriminative network $D$ for separating transformed source instances from
actual target instances, and a classifier network $C \circ G$ for classifying source
instances in the projected space. This 3-player game results in a network $G$
capable of transforming source into target instances, while preserving
separation between classes as enabled by $C$ in the adversarial setup.
Preliminary experiments demonstrate the potential of this novel approach, with promising
results when the construction of $C$ can be bootstrapped in a semi-supervised
way  from a few labeled instances from the target space.

## Help is welcome! #openscience

The writing of this paper is open source and welcome contributions! 

* Why? Despite being myself a machine learning researcher, this paper is my first serious
  attempt at a contribution in deep learning. While I am convinced the proposed idea to be
  worth it, I also firmly believe that it could be strengthened, matured and 
  improved with the help of experienced fellow researchers from the field. 

  I would also rather
  see this idea materialize than die in some random page of my notebook :-)

* Don't you fear being scooped? This is indeed a risk I am willing to take. Yet, 
  given the general openness of the ML and AI community, I bet that the overall 
  outcome will be more positive than the opposite. 

* How? Anybody willing to actively take part, in terms of writings, code or suggestions 
  is welcome to do so. Everything should happen publicly through Github. 
  Contributors become co-authors. 

* La question qui fâche, what about author order? Co-authors will be listed on the paper
  in chronological order of first contribution. Period. 
