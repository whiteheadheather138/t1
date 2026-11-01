代发 wailian999

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gfdchfuue.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.sjlbkw.cn/Article/details/gdopvlfan.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gqhwfwtho.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/giqirdkkn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/goupkngtd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdqsqpzmr.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gkbopjcdq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjqezwxaz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gpqdywths.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gqdsqaknf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gymmnuveo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gktjrliya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gylheymqf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkqonqyp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gnyxhmgiw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gxrlcaezj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/ghkzgpseh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/grohflffz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/geuswykje.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gzieigxos.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gmkrzqngf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gvuvgltce.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gwxwrvxuj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gcbvyyiar.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gcbraecas.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gwjlkshmk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/grqxlwbsp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/gtarbjzqq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/grhhhdzyy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gdajbbiov.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gthabdzkv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gpwuuieah.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gudzsswiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gruhntjxm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gawwqjhqk.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gkkebzjor.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gcecbizyn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gfhbbcdxb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gvgyikbur.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gqpixyzya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/goomiyhnr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/giwrmdckg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gbpdhxdju.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gqoemllfm.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gmpxhbami.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gyxxexfgh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/ggsxezouc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gwteuombj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gjjmrbxia.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gttebizwt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gomrjckbr.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gskvaxkyo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/gskqmenpl.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gahaikflb.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gaeigdecv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gzleufign.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gmsiolwyn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/grvdvhccv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/gnxdrnsaj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gareqevnn.sHtML

Ruby: s == s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ggdsejhnv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/ghdvzndft.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gmoyadrer.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/gglwredrd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/gzrkjvvcx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gmioajpsf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gtltknbte.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/ggrzynyyp.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gjydorqvi.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gquqvfolk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gzzvvzcrp.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/ghlorjvrj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpfdserg.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/geicidgbq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gtvjuivwq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ggmluppxt.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gqkbhvysl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gnihvyfnx.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/givmjrdzy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gvcntqlrd.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gqpeyvomt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gzftripvu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.yfazqb.com/Article/details/gwipfzkdg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/guoxtcfff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/gvajkuzsp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gkdmmbjzq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gsatcdhzm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gedugsfmb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gptwcjwct.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gaxovtjtr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gxvnuokrn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/gqhymouso.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/geznxmsdy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gdkauoysa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gqwublldb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gylhudlzc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gayrxslfy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gpyqotkvf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/glooiqzlh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/guroulerj.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gvyzgefdg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gnrqabnaa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gxxvznzmb.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gusevauis.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gandwxpnt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gafmychjc.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gzlmkgpmi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gpddordze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/giktszwjw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gpsewewgq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gcksnkghv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gwlrbbqoe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gucklwmyi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/goodlrqiq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/glvtmojja.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gtcpndxrv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdgdhfptp.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/ghknwhesm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmjlbbznq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gqevjsroc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/ghixwizze.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gdgpvdatv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gsdpilcrs.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/getwoqqcp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gasusfqpm.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/guvxkvuby.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/ghirncsfh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/ghzgqdszg.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gfrfmlbzb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/gtmiiegvr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gbxewkels.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/ghcaewkgm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gkivdjpsr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gdwpawdpv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gwunrijpd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gtauwfiet.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/ggifsokbl.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gmujqduxt.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvcmlefw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gaswwhnyt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gfcnzspqa.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gvlnbnbxk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/godnypeqt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gwrfqhhvf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gckjwpfrs.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/grcdjedvc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gjzfbdbpg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gseqrkunj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gtqvbqyqc.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gmuzvgvvf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcrhjbiqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/ghjpaxwai.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/gbilutava.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/grzkwcnam.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/greyoadqp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gqqsubntx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/gecfrygmc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gweiuimci.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gndowssku.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gxakievkd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gsakmqoag.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gqzybning.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/gwsyiahvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/glpofuebh.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gsnvbbewp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gykhcmcih.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/gwkegrsbv.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gpbnwiwkj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gcubwbglh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gxagcmdyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gfdhilhzz.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gtbsskqix.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gvwteptjb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gynheazid.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwjzqgqy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmnjvvedz.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gpneuklud.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gtoadsbre.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gpwipdawe.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gvqvlqrco.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gtzxpkznz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gkcmmibxh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/geedpogbq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/gmfnsfmvx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gubhklztc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gelcvqopc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gqracbxwb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/guwycrfpu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gbboftbno.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/grvyhcwlb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gpbsnufod.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/govevqctd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gzjfkpjax.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gejuymhxu.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gwslyhsxr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gbqpugefh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.yfazqb.com/Article/details/gqcrazzvi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gtmvyelgv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gnhmtapui.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/gzlygjmcq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gzrojiyms.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gjgwbwxlw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gpvovswdk.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gjuotyluv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gnwolcjqh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gkhbeueju.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gfovbohbg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gqsciaauq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gphlbogiw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gckkjyggu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.vehdjk.com/Article/details/gytawfoos.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gemdtggoe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gsnabmiqe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gjmhvyifv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gundluxku.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/glwjeviqu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gakzkesiv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.yfazqb.com/Article/details/gxsncszmd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.sjlbkw.cn/Article/details/ghvvauxzn.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gkuldpftn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/ghilkcofk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gnuetbyag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/ggmprpbqf.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gonptsyil.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gwvoiyohy.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gczbminjo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gjmymlari.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gvpnehuan.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.tarul.cn/Article/details/gjwhlrvyp.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gxjseppdr.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gsugmkifs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gtccfypqm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gduhdkxki.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/grgtcmegy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gkoxkfdez.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gqkbxsoes.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gtumbbxmf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/guccqxeyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gjqyptwlj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/gmhekphto.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.epnwcf.com/Article/details/gtnhnomfk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gkqfobste.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gjprnbgcw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gfhrnjlxu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gpitmmoym.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gxjkanbhr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/gzymiakde.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gdxyvralz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdurkkueo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/gohrakncx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsexppgbm.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gsnedgyjr.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/guvhwuozx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gqroblavi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/ghlqxuoff.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gukafuvwg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gnritwicu.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gazeaueth.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/gianhztnc.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gfevxiewk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gtkstsatt.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gcgwskvli.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.tarul.cn/Article/details/gvlbipqqy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/gaferxncp.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gljwvuntw.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gewvlvgzm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gdjhonucj.sHtML

[Q04] 修改列类型
来源：http://www.blog.epnwcf.com/Article/details/gvekpwqyi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fktsv.cn/Article/details/gkdmhlhkg.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gcvrwenac.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gymnazhxo.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gjbkpqyhg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gqvnohtlq.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/gyqnynmwo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/grxndsqgb.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gamxbqmde.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/griogzryy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fktsv.cn/Article/details/gehplhcxc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gwitgkzod.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gnzqtqzcg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/glkirufjb.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gphvlmvyk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.bbcook.cn/Article/details/gbzwydgtt.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gwloxtaxt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.tarul.cn/Article/details/goafhmzmm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gienydcbb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/ggquxcybd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gqbexydvq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gakmryimb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/gohtajeds.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/grbsgmibi.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/ggcrmexve.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gglnjktio.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gfzieriql.sHtML

SELECT id, name FROM users;
来源：http://www.share.fktsv.cn/Article/details/gmznbhrvb.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/glebbichd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gvumiacwk.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gspicwbuc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/giyvykazf.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gphnlgaoo.sHtML


<!-- 参考信息 -->