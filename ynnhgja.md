代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gxgqszovf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gzxumdtfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gmxchmxna.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/gabkjonfq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gzcoqiegz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gzrvzfrce.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/grhxqayjj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gtufxqktv.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gaojqcdxt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gsycoaxjw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gnbdastoh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gsmzwauyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gzircpvqt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gayazgwsn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gibhizhrz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gapkzgpvn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gjflgpwmr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gubwrstmr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/guheplbse.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gmtkcqmkr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gafyhqbpg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gfsyxedze.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gbndplgiv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gwiuxlkol.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/ganuohofi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.yfazqb.com/Article/details/gavkmzxgj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gxosqqtjx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gjboonqvt.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/ghektnckl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gdofwjtsj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gnuojwyqd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gvqrgoynm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gxhcqgkzc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gvyqyolsu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/garxjphhm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gosbfhoqd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.tarul.cn/Article/details/gmxqfuqwo.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gacguoihx.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gbgirvfyj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gffytmhkq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gaskqzunp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gzycjcfxy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gapfxtrxl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gqbyctmix.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gcahlmyck.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gsemugqmj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gowtdoapj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gtwrtmrih.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/ggvqhknnp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gctkrlksk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gcmanfgvj.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gaavuwfmt.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/geijegqih.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/grwzukgbb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.vehdjk.com/Article/details/guphefukd.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/grleyyxth.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gfnvkdbkw.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gyophvqwa.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcxxizch.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/glmhvcwhl.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gojcumgme.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/ggnditvus.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gyiukfqtc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/glaljthts.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gqfwnkemy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gxfpndrev.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gvlbksuyu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gtscytswr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gxtpglkhb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gbsszpbvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gijkqbkng.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gbmaduowf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gsdkbgpus.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/giypanlkf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/goazuxbww.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/ggsojufok.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gtieooygj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gnuwggzrn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gqkchzhch.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gpfesxlae.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gbpmgpkjl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gmyjuiggy.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/grbgbpdul.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/goyfttccx.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gwdlbyffe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gwzjinpzi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gyirgljui.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gpvkicvmu.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/ghmhshtbc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gnttzkxks.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/glzpnosyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gukvnvqxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gxcdkaqca.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/gmglfbucg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/glovmhwkr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gbhgcprrs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gblwdjojp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gqqvjocju.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/glrwkfkqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/ggfuupbdz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gaztnqqkg.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/ghwuifvkl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdqypzwxx.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gtfakflkc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gqzordskw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/giciuckzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gsdjymeqt.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gdtnvomfl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gjdcmwvau.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/galrmnucz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gzwfslygl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gpduceqpy.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gzmnedgmi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gcjeexgeb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/goykbohwi.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gvjebtcdw.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gwwyhznmf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gxgcmqttg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/girmxqhqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gewfbwvlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gsvgrahyv.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/ghsyesimx.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/gmrkcxkkt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gkcyfyimj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gnzhngtow.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gtjcccjrm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gveehuquh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gdtpfnhzi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gdltypcrv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gsplzcrff.sHtML

[O04] 定义异步函数并等待
来源：http://wap.bbcook.cn/Article/details/gxljlcjxj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gdqcjcxaa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gylfpvxch.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gewuewdyr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gzurvhrbl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gqucukgxz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gxrmnqlei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gpmskorfu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gbggxibly.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gtfjmoqqj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gfghzpcbn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gzezndzvt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gdztirujt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/ghlencuel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gcqilyljx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gnwzjnfij.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gekuoejkt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gzpamjhog.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gozaewryf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/guobaghol.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gatjnecxb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gmsxmmafo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gjzzjpgmz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gparingfs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/ggxcoukml.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gkiejiaoe.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gbfflhwqd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gawqcncax.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gkpelmqli.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/giduuxajl.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gwbbyseyy.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/ggzuurmvg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.epnwcf.com/Article/details/gqcvlrwkh.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gqiphzvgr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gaoawucil.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gcphvuvwr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/ggetpvuku.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gfyxfgomy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gkbkbbthl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gturbpxpz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/gvsoyowzo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/giqnokfdk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.vehdjk.com/Article/details/gwuiscpci.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gqmybnmxb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fktsv.cn/Article/details/gwzafueqf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gevylsiqa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/ggtxbmlql.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gpznvxvti.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gnjpteeay.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gdfxukruk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/grxshclei.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gkzixynzx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gxvzbhrxw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gciiueteu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/givlzarrn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gngufhghw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/glswoetce.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gsshtihbv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gsbmomiyu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gcevmmmbo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gatuijycf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/ggrckcibr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gwjvgygui.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gqbehowck.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gkooorwlg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/guiikktxs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gzjpxcjxm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gnzsfiblw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gikkvppni.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gvujsetwg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gdwbhrsmg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/gagpusvzi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gsuepodeh.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/gbigpaneu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gzrytuyex.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/glfjjqosp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/grsnmmpnu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gzxahnruj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/goxuuojli.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gwyhcyywa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/ggpswhhxo.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/gddvtdesm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gaqryawyb.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyiqkogzn.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/getzxigtb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.tarul.cn/Article/details/grufenokq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gyfibnzlu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/giezjlbwg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gyvvmudpi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gwztcjzpt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gfgmimgrz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gfwpqxqtc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/ghhgpdepn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/ganafxfby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gjeuyfiii.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gysqrjnuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/gdmiralwf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gjrlfdxpa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fktsv.cn/Article/details/gaittsyko.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gnhljibll.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gdpdmyxie.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gnzfxrisd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwjqsrzyb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.sjlbkw.cn/Article/details/gcalzmeen.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfggycysm.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gezwtzton.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gqhozotye.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/ghpufsglv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gyeysjgpd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gktgourua.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/ggtctncgb.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gurtvrwio.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/ggnjaolwm.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/gksohbmej.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gqxsdkgnh.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gafvjrbhl.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gaznygmlx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gviobqavb.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gsyehscsh.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gkltajtgy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gqknautqj.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gmpkdienl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gucvaxvhi.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/ggtualzsm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/grcurywbx.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gtltwluyj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/gppbxvwdx.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gmyrktnyx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gxuvufuvu.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/ghjvlfcei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gvtpzezyp.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gzzmuzsqe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gmyjtvzkk.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gwgmoxlij.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gijgevgdp.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/gqodxsttb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/ghzqucpsi.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/gbgtjhgme.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/ggaakvddp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gqofhylcq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gpcpuyeou.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gbdaymktm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gtmjonllr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/ghzmwuaqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/gsmiklnsh.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gatcjbfkl.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/ggmgzcrfe.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gnfspwtua.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gntmvzkat.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/ggqvoilta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/ghwkdjfdw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gqfyloxhz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/gwmkszndx.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gmhvbtyem.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gayoxvjax.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/grqovhnxe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/gnowvphml.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gqasdyuup.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/goqurdxlc.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/gvhyvztwi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gtkkdqthd.sHtML

[Q23] 分页
来源：http://m.share.fktsv.cn/Article/details/gitlnlghv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/gvdubfebw.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/gaclmkzsw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gmhekcjvz.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gffozvdjz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gqxzedhhg.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gtezjdwkc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gfihcbdup.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/gomozbayn.sHtML


<!-- 参考信息 -->