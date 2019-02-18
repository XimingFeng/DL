11 Practical Methodoloogy
===========================

One can usually do much better with a correct application of a commonplace algorithm than by sloppily applying an obscure algorithm. Below is the recommended design process.

* Determine your goals. Error metric, target value for the error metric.
* End to end pipline estimation of the approppriate performace metrics.
* Instrument the system well the determine bottlenecks in performance. Diagnose which components are performing worse than expected and whether prro performacen is due to overfitting, underfitting, or a defect in the data or software.
* Repeatedly make incremental changes such as gathering new data, adjusting hyperparameters, or changing algorithms, based on specific finds from your instrumentation.


.. toctree::
   :maxdepth: 1
   
   11.1 Performance Metrics

