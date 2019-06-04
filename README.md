# diffGrad
diffGrad: An Optimization Method forConvolutional Neural Networks

<b>Abstract—</b>Stochastic Gradient Decent (SGD) is one of the coretechniques  behind  the  success  of  deep  neural  networks.  Thegradient  provides  information  on  the  direction  in  which  thefunction  has  the  steepest  rate  of  change.  The  main  problemwith   SGD   is   to   increase   by   equal   steps   for   all   parametersirrespective  of  gradient  behavior.  Thus,  one  of  the  importantaspects of high-dimensional optimization problem is to have theadaptive step size for each parameter. Recently, several attemptshave  been  made  to  improve  the  gradient  descent  methods  suchas  AdaGrad,  AdaDelta,  RMSProp  and  Adam.  These  methodsrely  on  the  square  roots  of  exponential  moving  averages  ofsquared  past  gradients.  Thus,  these  methods  can  not  take  theadvantage  of  local  change  in  gradients.  In  this  paper,  a  noveloptimizer   is   proposed   based   on   the   difference   between   thepresent  and  the  immediate  past  gradient  (i.e.,  diffGrad).  Inthe  proposed  diffGrad  optimization  technique,  the  step  size  isadjusted   for   each   parameter   in   such   a   way   that   it   shouldhave  a  larger  step  size  for  faster  gradient  changing  parametersand  lower  step  size  for  lower  gradient  changing  parameters.The  convergence  analysis  is  done  using  regret  bound  approachof  online  learning  framework.  Rigorous  analysis  is  made  inthis  paper  over  three  synthetic  complex  non-convex  functions.The  image  categorization  experiments  are  also  conducted  overCIFAR10 and CIFAR100 datasets to observe the performance ofdiffGrad  with  respect  to  the  state-of-the-art  optimizers  such  asSGDM,  AdaGrad,  AdaDelta,  RMSProp,  AMSGrad,  and  Adam.The residual unit (ResNet) based convolutional neural networks(CNN) architecture is used in the experiments. Our experimentsshow that diffGrad outperforms the other optimizers. The effectof  different  activation  function  is  also  analyzed  with  ResNet50for  the  proposed  optimizer.
