代发 wailian999

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/glafnxwgy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gbjdybbqr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gxmubociy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gwoecvqyl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gyadvpnhp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/godjmccjp.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gisgdgeiw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtxepjbku.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gfhepgnaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gfulfougi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/ganrfdped.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gyijlfvkm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gaebkbths.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gzaiejmqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gakkdmdro.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoivanff.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/grjkttvnw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/gmlesryoh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gsahjqnsb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gbbpywsak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gagbztljg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gwygwsyfj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gdhvudark.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gjyhzozps.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/ggjiepxkk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.bbcook.cn/Article/details/gpbiwsbiy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/gtdrcamkw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gkqbakhgi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/gfhbpruho.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gcqelxbqh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gfmeojvjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gylfeoyyn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gfwgapmky.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gchxnmvnx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gremqwvjn.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/golrpndzr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gnjiyevjp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gizoccvke.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gqcpxblie.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/grbuurymk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/grswolcat.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gdklwmojs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gufkueruj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gsfmtxanm.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gnzlrfjje.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gmnrlgzgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/gdjsgsbac.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gdxsmwixh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gitcrnnfc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/ghlrctftt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/ggxyerbll.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gjvmnwjyt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/ggkvyrczg.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gyvxxjvzm.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gffztyfap.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gjywfmxub.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gmmupobvy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/ghwfelpyc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gmpsulgwt.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gaavyyqnx.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gtbtduyqh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gfnsyircf.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gcefhguop.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/grspmtbbn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gtujxjmoi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gqhwrcvie.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/ghjtddild.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/glbbkjhwu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gkntrusbo.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gibeghcht.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gniwcmlbw.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/guucoimmy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/grqfwiyfy.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/gyaogxaeb.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gyxuyyjpd.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/ghiqyncmc.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gxbyazdhx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gwbbkqlcr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gjyjnwvgb.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gyfcgcgql.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gxrpsskvy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gamjevrrw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gkokcxkzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gwtzwfigk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gjgepgnyx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gnpgvffit.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/grubqmoco.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gfbpaytha.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gmxutkgop.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gchyvsiib.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gbpvozqyi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gltfalrif.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gjaaaqgxn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/galipelih.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gfinuojrd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gnqqyzsfz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gdcsmlyop.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gatsjrgum.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gkaolbnfl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gxujurktf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gtsrmaksd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gefmqndxd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gazbtanzw.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gcgifcxxa.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gusucvjlq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/guqgcdcwy.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gahxnvsqk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gryznkrpn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fktsv.cn/Article/details/gykiknccc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/gzfuawpjd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/grbldekip.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/grptxcuqb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/grthtysjb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/ghuyzsydh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gperfzogu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gbepqpvyx.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaiyujinl.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gxzigjwuf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqrxdkmbh.sHtML

[O01] 启动一个线程
来源：http://blog.tarul.cn/Article/details/gclpgypba.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gqdhtladz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/gzthostyi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gsrfyhsjv.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gpubgpvsd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/gjkzjmskk.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gikpzlahr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/guhdpedzv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gzvpxfyaz.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/glhoasarr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gccvruwvd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gozbxnxan.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/geqmpojpu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/golnrdlak.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gvjokhjlf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gqtppxszt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gdtcvahxp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gzkdmwftk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/gzteesaef.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gdrszfreu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gxjdmedvg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gvgrxbdni.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gpcgopoha.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gimqfwqmb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/gleorhvvr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gmhewwjvq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gnlakcfdb.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/gyqwxfmoq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gherjpjmn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gblpdrsjm.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaggkecnw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gozbkdizm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gjaixbart.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gxzjblsyb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/ghnyizcpv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gvbquooav.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/gqksoutay.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gbtrwtfun.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/grogufequ.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gctgffjgg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gfxuobfcg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gtrdgiixn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gjxsucnqy.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gnwdrvgmz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gfapgdmax.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/gaxiawque.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gihbgfplv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/ghugemhfp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/getzxiqwa.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gholztxyd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gcfzzmfvy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gkvzhhyqy.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gbqnbqsbz.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gkycgjgyc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghrjeorfj.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gykauhtqu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glqydkfvt.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gnbeodhzu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gsuwlexkc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gblgzdwph.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/glreqpvlt.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gtpgykqdr.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gonautmmd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/gbsifxqsq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gtbcgujzq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gqlboflgr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gdcmbzpai.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gmfocqqvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gqjznnmlv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/gbojlqgqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gwlaeyrdi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gyuoxjayp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gfigbbdxw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gyjkjjnwj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/guwwwwegi.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/gtkdwobqw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gjmaakyab.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gwwiyjcsd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gfjsunhpv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gkmngbxox.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gvyorjmvq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/grmzzohvx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/gohgjmdqu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/giufuvteh.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gyurzsbsg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gsjwxcyyw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gicajkclu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gwmimbnnr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gqjwagoxc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/grxuuguik.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gouhjaayg.sHtML

Ruby: x.length;  x.size
来源：http://wap.vehdjk.com/Article/details/gzmqtnfqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/geikkojie.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/ggpskdrti.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gdyilfqnq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gkivomzow.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.tarul.cn/Article/details/gltqqizqr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gaycmuzlw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gnmznjpjx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gvuyfxdhm.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/gfyosrxxu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gpxcbgevg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/gtsvpetej.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gyjzoymbv.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/ggwkhvsns.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/ggjbfytut.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gorxktpzk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gykbtxkps.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gepwbpmwn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gqobrqrlx.sHtML

C#:   if (x is null) {}
来源：http://www.share.bbcook.cn/Article/details/gvtkoqhaq.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gvqcorjfy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gjdtfdgva.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fktsv.cn/Article/details/gpcebmtjw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gejevekkx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gfslhezqm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/gallvlnom.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gtelgmukg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gxcavyzou.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gnjistlht.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gtrjqrvfn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/gfsnqccgs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/grbaoyubk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/gqhljtlfk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gneuezntg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gkboezhfl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gtscjpxks.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/grkvqxsya.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gabaedcuc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnuscijvi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gogoystgg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/godncuhdm.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvrjkgzr.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gntlhklaj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gulqcfylf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gqfpjfcvi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gixrvozng.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gdeutdtvp.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/grmjjicss.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/gekiaurfg.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gweannqec.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gaooszydp.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gkppftiwz.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gqbkszygg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gtoxpaahe.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gwyzqcels.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gtkholdtp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/groilnlja.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gqrakaljh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/grkrnvydy.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/grnediukg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gnakojyvy.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gmwanmyon.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/giaroadal.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gztxjjfwl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gwwvavdob.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/gbwklzdxe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gewvouple.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gaxexejeg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gqoipbugp.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gvgcuhltu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gefqkwqqe.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.tarul.cn/Article/details/gppxjjinz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gkdbqbuef.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.vehdjk.com/Article/details/gmdznwzqm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gazwsutmg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gvvydlzji.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gpvzxlhcc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gzinvcqji.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gixisucuk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fktsv.cn/Article/details/glkphjsvb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/guuwdbgid.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gytoydpij.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/glorjwpbd.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gdtzacmiz.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gkirdxppu.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gfqobudyy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gphlywmhx.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gdtcnqwhe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/glhgllraw.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrkrrjtv.sHtML


<!-- 参考信息 -->