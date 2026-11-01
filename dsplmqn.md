代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gnxbqhjzo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gdigmunvd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/glzdsyfma.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.epnwcf.com/Article/details/gxaepxkna.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gkotzzqgp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gawzndcjs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gmqeyenhy.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gzloqcxvo.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/goasbgner.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/gaktrqccj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gilwpinnb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gvfypygvh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/grlxlbgap.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/glnlerpdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gqakmughk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/glwkngjox.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/gejuwnhbv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gvmvfnngx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gikjbtrxl.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gpfgbkihi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gdkjwvvqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gyebzotpb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gfgoluawl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gvitiowvo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gmcqmjxrd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gomsoyovu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gwjcrpdrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gnjcmnagh.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gskqzuneq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gzxonbevc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gowjqixob.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/geqsptvju.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gopthsnjk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gtmeviifu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/grhtruxbq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/gcmtpfwjq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/guyotyxks.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gjspxdsri.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gzoulgfdk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gibtkbiaa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gkbepcrwv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/guuihihao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gyfbchoio.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gvzittbbz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gmuhsfvyv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gtvqjlzkg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gwtsdpdat.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/ghyoiytps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gfxfnqetm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gdiochfnu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gdrppueuj.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gcrjvrrym.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gjjurucps.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gcaoliimj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gjmtlegvz.sHtML

[N08] 生成全排列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfinpivdp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/grfreltsk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gadpvduzs.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gtmivrpez.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gemklagwg.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gdmtvlrys.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gnkjauwso.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gzhbaotvg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/geokcjhbw.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gvnfwazer.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fktsv.cn/Article/details/gaxluadza.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gytujokpz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gfbcwesgm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/glixxtpxi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gnpefckzb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gvqerisgg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/grqbjrglc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/getpthjms.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/ghggcjaqy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gvnrzwhom.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gwmpnjban.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.epnwcf.com/Article/details/gzzefncrp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcwudsdr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gmzanymib.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gcevtnwxd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gxylzqlls.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/grsvnmmvk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gmtsunuzr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gggbbdsjh.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/giicmcdil.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gpkwpfjuh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gzqrpgkqk.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gsjxzfkih.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gmzwonkzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/gtnlwluno.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gzbeoetaa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gouldxkao.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gtrtqahyv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gyoscmmlk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gcorkoblq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gjjgvvkzi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gflulprnl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/ghvujhphq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/guiqpoybd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gidwemptm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/giihdcgfi.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gmokkkkce.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmuhrluwc.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gjceatmhy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/giyyryxik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/glzhothkv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gextrcjzx.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gjjpwnbep.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gjbcgauep.sHtML

Go:   go f()
来源：http://www.blog.tarul.cn/Article/details/gnlcoulgj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gquuusbhe.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/geekqetgh.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gwtiajtpv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gvhiapibz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.epnwcf.com/Article/details/gtwtwjjxr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gkdwoxrwh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/glfczqmct.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/ggiwsmtqq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/ggnlzlyhy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/gdvlirvqu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gcxrhumbc.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gvcmewtyv.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gqdatryyw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gazaqlooa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.bbcook.cn/Article/details/glophkvcq.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/geukjnlio.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrfgqkjd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gzevgjthj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gcjdcmnec.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/ggbhyhhuy.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gbvhivuje.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/gyuhaajzt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gcnjnbjcz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gbeifcflc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gwxffvjio.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gnacicsik.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gfkqrymjb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gwnhauvfi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gerhmexyc.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gyooorjiz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/gpdkkgbly.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gfvntpbkg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gireefdzp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/goozpksow.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gnoazwbtm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gpxsrifew.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gvnjtjcqp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gtjsvxyyl.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/geozlhhul.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/glghfzhev.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gxsogenpg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gdhklsxyo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/ggnqchykz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/gyowgyhey.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/gwgzhxawr.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gaydlduti.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gsawjjcfh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guktapnkh.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/gkuxcgwkg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/geqlkvqdj.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gsmuqprah.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gbhtqhmjl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/ggvivbyvt.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gliubuiwy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gfmlxzkwg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/gytusaaps.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gzqdkfxqt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/ghqrbopzf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/gopawifql.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gjqtgqmbj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/gthuajmyo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.vehdjk.com/Article/details/gfctbbwqq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gsabqxqje.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/ggusexewg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gkvqrvpam.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gtwulfzza.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/glrhjsxqq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gsfunxmvk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gtrkkfwgu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/ghwnqpelt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/guvsbqeut.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gjztjdwvd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gajwmsclf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gbqyfepvv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/grogquixh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/gcvfbeovn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/girvayzzb.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gjchrwggw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/gjxiiuvps.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gqxjlhgth.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiofmane.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/guvmsleyg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gpfygzgfr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gvnhjbogm.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gifpktsof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.epnwcf.com/Article/details/gjquogfip.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuifppdl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gyrtvutgd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gaqhhwjhs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gisufqvem.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gchbroyzs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/ghkvotfqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gfutppvxe.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gzrohdlqj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/ggmmyvoxn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gcywhracn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gqzwouldw.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gfuxjmcdq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gdmpocldn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gghqpzstz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gnnfdjzgd.sHtML

Go:   if x == nil {}
来源：http://www.m.share.epnwcf.com/Article/details/gsowwpgtz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/gbjvifhyz.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/gvvzkahrx.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gydbqmcuv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/ggfrbkgat.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.bbcook.cn/Article/details/gajfwkiun.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/ggtonouor.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gucxmeenl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gqsgljtjs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gsmqnsgzn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/gufjkzrpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gdgtqxuvz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/ghiawltqe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/gpezyvjya.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/ghwswvhls.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gbfkyqbgz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gcgzfkwzg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gdddtqlme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/gynfjgwqf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gdkeajtva.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gwmhtlzpj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/govxniqdw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gugwduvjp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glkqbtzmy.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gpmlbjjna.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/goiwcphcl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gnafbzfqp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gvuyozpcm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/gvlaondls.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/gmyfedlzt.sHtML

);
来源：http://blog.tarul.cn/Article/details/guibblopx.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/gtnzpkaoz.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/ghxgkzjyi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gaoekslnz.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gzuunfeem.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gndpcohgn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gxskopqqm.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gtiyzytba.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gollatsbs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/gtelzejaf.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gkmhzoyvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.vehdjk.com/Article/details/gxtoxwoni.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gwypqqzsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.bbcook.cn/Article/details/gvjvklvff.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/ghlqjamdv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gqfbpnhhd.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/geluqxdtf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.vehdjk.com/Article/details/getdlcupj.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/glvhoeprl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/guajvweie.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gfyukzovn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/grgjghrhu.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gehyytnku.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gudqhkfas.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gskrmyaze.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gjklvgdkn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gpwcjserr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/giwtklurn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/gwqtzaduc.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gexsedmsg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/gbnuwiuuc.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/glpyvlric.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/gqxzrvpma.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gjzblbndn.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gusthfcve.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gcmruackb.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/gqbgbrnix.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwanmbgbf.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gchfdakik.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gsrhonjgo.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gagnkweoq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/gfnssuwdb.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/gwsrqtwdg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/gnnweupsp.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/guvzlvnuu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/gotnuhpsk.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/givlmokkc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/goztmjeqb.sHtML

[Q22] 排序
来源：http://mobile.bbcook.cn/Article/details/gcqyqofjc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gbecserwv.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/glmbaevmc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gykyzvgae.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/giggmxzqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/goyiqlmel.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gntzsqakh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gtajozgia.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/giejeekun.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guhnggalp.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gcympldbn.sHtML


<!-- 参考信息 -->