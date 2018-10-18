### statsample
---
https://github.com/clbustos/statsample

```
sudo gem install statsample
sudo gem install statsample-optimization
sudo gem install statsample-optimization --platform ruby
sudo gem install statsample-sem
sudo gem ruby setup.rb

```

```ruby
require 'statsample'
ss_analysis(Statsample::Graph::Boxplot) do
  n=30
  a=rnnorm(n-1,50,10)
  b-rnorm(n, 30,5)
  c=rnorm(n,5,1)
  a.push(2)
  boxplot(:vectors=>[a,b,c], :with=>300, :height=>300, :groups=>%w{first first second}, :minimum=>0)
end
Statsample::Analysis.run

require 'statsample'
ss_analysis("Statsample::Bivariate.correlation_matrix") do
  samples=1000
  ds=data_frame(
    'a'=>rnorm(samples),
    'b'=>rnorm(samples),
    'c'=>rnorm(samples),
    'd'=>rnorm(samples))
  cm=cor(ds)
  summary(cm)
end
Statsample::Analysis.run_batch

```

```

```


