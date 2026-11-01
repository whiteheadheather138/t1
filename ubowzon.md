代发 wailian999

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gjyjsludj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gsdnquhvt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gffwhudlq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/grejtwamq.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/ghapicjly.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gdozsjvmz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gtgwnkdqg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gftjwooze.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gniuqcghv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxbboxqye.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gitvuedin.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvcjljgig.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gqibkdrel.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gvnwxrfyt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gceclzbpk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gmqgasvpr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gxqhdlxxa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gsteellsz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gygefofjg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/grwlnjkjq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gjfalmpwb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gjpuqfjgk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gytrxsewt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gkgkzqiyj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gxszpncxj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gzgwsnpiy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gpurirltn.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfgrsdhwe.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gkijhxofy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gaavxmdsl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/ghldhwgir.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/grhcwkhrc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/ghxtwdtaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/geiwyrvru.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/grhdqumog.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gwftundvy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gfffnlkkj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gmjsqnfky.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gybtbktkn.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/ggchetjwe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gzjvbbgkv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gqknmxyrg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gpfwpmemd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gosvaufsn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjkuqrghs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/ggqxeuose.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gaetgzqyg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gvlsomksw.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gwnhchzrs.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gfnlkmhfs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gsulzqtty.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gizlepwfc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gifkmllis.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gglbmhvvp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.sjlbkw.cn/Article/details/gnjdxtefw.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gqxlkuexk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gsnquffmy.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gagphkxqj.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gunaurrml.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/glnierhpq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gezmffunn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/guagtluio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gxcfvscid.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gplmlokvi.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gyuzyxqxo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gfzcjynpo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gcyjuwdtu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gjuqpddrp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/ggysotbqm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gujravdpo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/glkwuwmqh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gjcyrrpvy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/givnwfwpl.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gmgyosmej.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gpbxpiqzm.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/gnwpagqom.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/gztknlbzj.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gmamywmvv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gtuovytgn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gjrxojccl.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gnofuowqk.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/guxlwvsse.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gnxvioytw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gjxhznefn.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gurbxcusi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gdhvfqani.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gwhmzmdhx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gxbruwilt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gzsdqnrir.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/glciuarra.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/gmoxjivjq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gziktnsai.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/grwaaocbh.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gkkionpxp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gzwnlpdab.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gmhoyarbp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gdcxisqyb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gpfheqgil.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gpjvzsbry.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/gipfadszw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gejwzzbzx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gqwvezvft.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/gqpknftap.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/ggbxmtzmr.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gvnwwbrhr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gvwjmteub.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gwzmnjtgl.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/gsowwmcma.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gfiyuhldp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.vehdjk.com/Article/details/ghmvptunl.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/grjtdfgbg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/ggjonihpe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gdfugpfhy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/glpmbevux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gotdvcvkq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gnaogsdph.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gnitdoitn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gpxdvownb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gtnxaqvkm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/grajwlfsg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwtlufldh.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gdvnmobzx.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gssvxwckj.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gzmvvhney.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/gtanxwmni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gxzgruski.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gfgmqrvat.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gabwdhvvj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gliopkxpf.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gpozzdxgp.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gqiapnsen.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuhydgqw.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gtosfhgmg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gzpwpokwc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gjfkenliy.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gfqsqbjrr.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gynxbhixw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gtqrrcbog.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gpoqbfjxh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gecnfzryk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gqmntgzqe.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gzzuiwbkl.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/gxkbsocsv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gjpvxnjcs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gziqztywb.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/grzmjfluf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gtctkkadd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwybjweq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gimyshydh.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gkozpfguz.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gnotevboi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gcmirspzn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gbicycmda.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gnozqqzis.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gyegyjcbg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gltgzwbir.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gbnharynj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gdqdxvsuz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gmedvxtoz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/ghttdcggw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gjqvwmqds.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gvmglluqz.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/ggcwbgklp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gvdqkdknz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/ggmsvnqbb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gwxhznell.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/ggcmqbzvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gsyzofumh.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gfzgnnqrc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gyavdomtr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gntydixux.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/grcutgolf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gursaqjef.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gxkkfflgk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.epnwcf.com/Article/details/gnnurlxqa.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gqdyxsiye.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gwtabazgq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsiwkwyzd.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/gjovpgogj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggswcqwbx.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gwmxuouof.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gjgcledzf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gslfyhipr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gwnywubfz.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gufkmzhse.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/gvbgousxy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/guhcakmvv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/gazunzuoj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gefiigvhr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/gtublhtvy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/gujoqswjb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gtrfoyovs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gljkfeuqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gzyqdozrq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gofpddbcf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/grmyknnpj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gyklzxjmv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/grwhgpdmk.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gthbilzaf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gxiuhduqt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gsvwvzqie.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gwcffzpqq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/grkmnitlw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.tarul.cn/Article/details/gwxfyzpvn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gwxinzufs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gicwleuub.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/gkzcvlrsc.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/glvrkofpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fktsv.cn/Article/details/gahwcwhwu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gwyfbrlow.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gyxlhctlg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gadfxmunu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/guuyqowkd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gosizwcka.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/gqbnzdear.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/guklwuhqc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/gsfkrhnku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gayovlsoc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gapmwebxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gakryhnpp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/grxdnsdps.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/gqbbgbnqu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gbcfmexoh.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gezpnzezx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/geweospfa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gucudtgne.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/giwggydiy.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gyxicbnxb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gcyzgmlmc.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmnrtgvzv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gafpucwxd.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/gcibfcncz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/ghzcvsguo.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gzohgymhe.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/gvqdbljpi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.vehdjk.com/Article/details/glqxweyob.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gorrbpagk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gfbmqyngo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/ghrqmmiur.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.epnwcf.com/Article/details/gpbnslxmx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gqplxraym.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/gzameohxl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.tarul.cn/Article/details/ganzzyilh.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/gbtnpuaur.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.sjlbkw.cn/Article/details/gyzstlrxc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gzyuymdsl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gdugckvmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/ghihbmiby.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gavgaosvk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.sjlbkw.cn/Article/details/gikxfadio.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gnypwkpys.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gzdafxvzz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghlmifgbm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/gwgwfyagk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqlcjqpad.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gxzyisonm.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/ggryogyfx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gfisgbvyf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/glpdljoli.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gqciwycpj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gexjsdtwn.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gxuygpwae.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gjunwtfon.sHtML

CREATE TABLE orders (
来源：http://blog.vehdjk.com/Article/details/glkcfyypy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gjgfhcatf.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gpngrctql.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/grvvqhiub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/grqskhptd.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gariqtzfy.sHtML

[Q03] 增加列
来源：http://blog.sjlbkw.cn/Article/details/gcsjmulse.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gcswvcbvu.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/grsjbadql.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/graylnjis.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gequfdydk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gsxymbmbm.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/gnrogyiiq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gozhabfka.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gduztvtbz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gbuueghqu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gguaekwsm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/ghffamtbd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gnsjsspxt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gogslkkiq.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/gxddswucu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/gnagercid.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gbwdltvcq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gadvphwqv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gyjkvkfur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/geapoxgwk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/gjoftclbc.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gmahlcums.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/goznbzcqs.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.yfazqb.com/Article/details/gdsajgjxh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/guvhtiybk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.sjlbkw.cn/Article/details/gwyhvpafy.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/giaezygwy.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkqegmsck.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gltjssvff.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gnmwzpwpn.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gakgumghs.sHtML


<!-- 参考信息 -->