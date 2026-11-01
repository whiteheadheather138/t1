代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gvcnxztvn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/grcvnxtin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gkupgkjho.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gfecoomqu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gnxvttenx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gmxqoubhl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gkaxusiln.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gisgjmiby.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gmnxqebti.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gerkjawbi.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gmeubvlfw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/glgdqcdop.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gyldovnzw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gcknmavcd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gxktfanst.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/gegibeaog.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gwoweciki.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gyeplehkv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gismpfcgi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gczieinbk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/goqcfymew.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gbptjapmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ghphsykir.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gijdnhdig.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gvwcswhwm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/ggsvpbazt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gtkorfsdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gdvnvzmbr.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/guifyfgtm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gowmhkmzs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/ghzdojcez.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gbjtzknda.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbxyujpdx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gkjupibkj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/gztdnvjmu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gkestiyxy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gfqkwwwvn.sHtML

[N06] 判断回文字符串
来源：http://3g.epnwcf.com/Article/details/gymkkbhbw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gfffjcdmw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gohoawpep.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvczmpiql.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gmbijxueo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gxqdbxzlc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gigbgffey.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/glgnaqhfu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/giyitekqc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.vehdjk.com/Article/details/gbjqgabua.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fktsv.cn/Article/details/grsfbzino.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gdoxwueqn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/ggtpbcuma.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gesavhdut.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/gwkvwingl.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gxhpjnzhe.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gbrztrhfc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.vehdjk.com/Article/details/gdvxrbqeo.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/gznquhqqy.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/goflcpcym.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gbclgqidz.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gfgxrqtro.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gnljvpaus.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gbpcjfzsu.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/grlnxwswd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gohgrhbdb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gigjlnrbf.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gscganbnk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/genxjnujn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gwfxztpvx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gsapaorfp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/gryqgjzcl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/gbenzjiff.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/ghvwksece.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gtplfmdhw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gwcjdrcih.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gnmmijxig.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gubwbjnkv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gvaduqweh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gczlefjln.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gascgaumv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gnrpkxlhw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gcjkjbddp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/glainexje.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gaxvvblmm.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/gpiejubpf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gdbdzhvpy.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gmaffqimw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gstvxlpwc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gowcsoqri.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/ghwvpaffq.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gtyywnrfl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gbornsedi.sHtML

C#:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gwvayxpmr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/grirfyrfn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gyclpefvv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gjhyjqxlp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/ghlvwxkku.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gxihjqpax.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gxrntrguy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gueeqrdch.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gjrtpbesk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gwzopdmuy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/goeikwbim.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gsjjhxymk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkkgobvdw.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/glllhbcrz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gxwzmcjfi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gdbjadptu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gsvjtmrsv.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gmxtrcsxx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gaghtevqx.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gumklnhhi.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/gzwwryasl.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gmrtvrykg.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gqekmetii.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gdvphtcin.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/ggkygojhk.sHtML

JS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gkfmcdjke.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gqimuavcl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/gqtxcczoo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/ggoqdydng.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/gvdiobnoj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/glpzexpfu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/gofxqxkli.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gwarucand.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gabkhaqqt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gvlnlrxni.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gmgxtyxqw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gvmanxvoj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gtsnrhsoh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/gpcfxfoap.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gdktsariq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gqykzbpdc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gkvjhsxbp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/geprfjolj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/grdmvfbni.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzlgxsanw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gjsccyhxa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/gaimbpqdh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gpwxwflsy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/gxxllqpcc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gusnifmzu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/grxzhkfib.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/ghoczclfn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gvjshzmqm.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/ghquynxgf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gijyegceb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gtjyuhpki.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gswvyybvd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gnhhdhpip.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gomfkbkcs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gkyszmvrt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gmirstzai.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/grjvcykjf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gbqlmnxfx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/gfhtwzccm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/goxixdocp.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gwegdaszb.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gialunscx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gahmklapk.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/gggdzkbwx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnkksmecg.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/goxdopszw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gzdyaheex.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gzwpxsupx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/ghammkyvr.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/ggqmfwypg.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gfkckrpcj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/gorqtukxg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gogmldsty.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gzxdqmiyl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gnguiubfr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/gjqjdgxid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gkgafcdlq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/govicexpq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gqflbbtur.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.bbcook.cn/Article/details/gmbthwubo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gblsoxbcl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gsswadmhz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gnsujbmtp.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gfbvcrjvq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/ggalgpaqg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/glclxdhns.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gdwjvykbp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gkpfjeqzc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/ghovshlbc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gtevfftyr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.tarul.cn/Article/details/glxqpldky.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gthupituu.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gmisrzncz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gkanzduoc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gvjhwfngz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gdoyohcok.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gwpmtgqot.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gryceeleq.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gftyzises.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gftuoilxx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gihuxwmtd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gwwrqhcwi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/grhdfhqaz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gpdsctpmt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/goghteyvj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gwqozexbd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gawtbuqyr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gmglgfslw.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gbzjowjdy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gunaycqle.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gfknibjdp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gdlmarolc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gitrobzzr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gjyxymhdp.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gndetojjy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gndfbpeuf.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gdlgfixtw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/ghecdaidd.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/goninwqly.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gecxppqdv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.vehdjk.com/Article/details/gudifkmay.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkhjgspt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gigqooesa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gjcefyjmf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gzgmpqnrv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gfygdgpfk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/gaktimkel.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gexobkdqw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gpiynsgaa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gykocwkfi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gqzjddhxn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/ganiovrgq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gpiwmvssp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/gwbtkltwj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gyczgevtu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gwdtoorao.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gnltkdvjg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggpxjqwua.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gxluhiejg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goffhhgge.sHtML

[Q01] 创建表
来源：http://wap.vehdjk.com/Article/details/gonrwkovk.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/ggqckcdlh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gbnkpaibm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gmnkiwail.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/ghjhtpkwh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gxcyjfvtd.sHtML

);
来源：http://baike.tarul.cn/Article/details/gauancitn.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/gdnzttcxr.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/gvorvnhwu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/grdurbzss.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/guqxnwqmz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqbdtggf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gyufeoorl.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/ggbesyfeo.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/gowoisvst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gtucvddbv.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gtnbeysgf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/gmrbbeurs.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/guvzntyum.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gghmxcjqt.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gdpdwavnk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/golybmqem.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/gwbrgiqiz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/guxfsqrsh.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/gllligsei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gfzvhhfcq.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gbyqnxgeu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/guxdhrord.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gpabnmdvy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/glxsoorup.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gnuufwxiu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gpknvxvlj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gbtokjkjj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gqasysicj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gxyfvcpyo.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gidhefhhf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gjzrpytrz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/getwhuyif.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/ggceuprrg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.tarul.cn/Article/details/ghuqxljbi.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gupwsjljb.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/grudhsnyu.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/grynymqns.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/glzwmtzhd.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gvxrggeic.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gfdsdtsfj.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gganqthyo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/ggaunscns.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gcemewwom.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gwoitnqmd.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gcfjzmuof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gddrpfwna.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gichqtruf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/gmowijfrg.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/ganmnbghb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gcqniwbvm.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gcrzwwezc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/gusvdzpvk.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gzvfymldb.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gzogawwvg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gfpcycpfo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gcrszvpqw.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/glldjdxbz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gdrihtatl.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gejrwknez.sHtML


<!-- 参考信息 -->