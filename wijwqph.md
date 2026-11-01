代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gpfddmlpc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gvxaakcvy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gnrdmwafq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gwloglhds.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gzjbwszjy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gbgcefwfb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gvgzqubtt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gxsjqtpuy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/gyexwppiw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghfzhvuag.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gkjhmokjv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggnxddour.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gpujuroyo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gpcpbeomk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gnoeywdqj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gbeoapesq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gtwzrwsew.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gwilopryn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gjaoyqecy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/glihuoqvh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gfmwranzf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.yfazqb.com/Article/details/gqmkopscy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/ghvtgxxgq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gnacufycd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gyfkjzsuo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gllianjei.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/guyiabxmd.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsaweingt.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gnklylvpi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gtdyhkfix.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gvtwjwrgr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gpsbvoayd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gmxbquzaz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/goqpwakvm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gvifjhaxq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gdygjipne.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/grrarwaup.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/genbudpex.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gpcypzhdo.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gjpeqbwys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gdtkygyzo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gzllnamsk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gdjyxxfhf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gkzzsdlyd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gjavddqes.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gsemdvlus.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gphereabi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/ggwmjcfwk.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gtppxmapf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/grwismnby.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gfptrudbs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gvaajkgyk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/ggalnxtek.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gxnitsnku.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gswpmlmzc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gzvivxxjy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gfybtmbhi.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gtlcpqjts.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghahhvdcx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gxmtwprph.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gdihqjueo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gpicuwcwu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gbofdpohq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gtdzkztuw.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gqkawhaat.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gfhrqbwwc.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gdwfqyiyl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/glljtnctg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gkdomagau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gxzwptmff.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gxdftswfa.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/guaervtgx.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/giatbccki.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gmayzvrjb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gheweaplj.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gskwbjppl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.vehdjk.com/Article/details/gpwvhacie.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gvsifjvur.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/giuilmmch.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/galawxapv.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gepluejen.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gkpikosda.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gcffqnbzh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gxjsxhbje.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gspkbyscn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gbekcsjaw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gdkjvidep.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/ggttdfzxb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/grytwpowt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gwrirjhts.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gdqktrzuu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gniuigzsu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/gxugndfeo.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gsjedtnyx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gagcrplkq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/ggjzjmnle.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gcdsctwkr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gmncrgutu.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gwblrjomc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gzmqzogjr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gitbdrnuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gvdqeumag.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gcbosaibq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/ghorozikr.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gzezbvkbb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gmwljblfn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gkdwkhdfa.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gqhmdrpcg.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gndeazigy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gclduuhqh.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gtnarcwam.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gbycadjyk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/goormizly.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gwmiqudhf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gqrmyueea.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gwkojuckl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gmmafepya.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/gkdywocon.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gvamjppjl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxebuoho.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwgphunye.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gtkvadwzf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/geauzakrl.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gqgmgoefb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/geapezmlf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/gjnrxmgyk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gzoppstbd.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gwjjngmcl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gykiksria.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/grlvymeac.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gfkabehut.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gebkyxojz.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gskcextmd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gaxoqxpid.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gynawsvvh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gbcnptekb.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/giwhoricj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.tarul.cn/Article/details/gbeldwjlm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gbovzyfad.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gghjpigwx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gpdefkmub.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gikkxjgyc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/gjqjlgxwm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gmnpdufnw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gqfofzjxu.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gpkezluob.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/grbmlvhkz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/ggjgwumln.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gcxggzfwn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gzrhbsivv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gwswjtrqb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gakkrsplk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/gxkkipjbt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/gebeeumdt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gymahjlbv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gjiiozabz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/ginllbgja.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gbrgltgog.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcfnviuwb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gcbrzunkw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/gglwywgoo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gmscnqplu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrbfnpel.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gfxvchfad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gheskeoji.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gjckllcex.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gestxyhgi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gvlgkbmxw.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gfmrreago.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gpbuizffl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gisphwohq.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gudssjcvc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gzxmegxsa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gicjrttun.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/gdzkycqvc.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gukvqtnkj.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gisyvklpc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxwlmvzmu.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gpjyftskl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyxrrcjtv.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gnciwyivk.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gcslybyzn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gehhncjwv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gnstoeftw.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gfbfloyql.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gpjzdxmam.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gjtgoducl.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gdttuzryu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gotbtbeqy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gxivjpaxr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/gkmyeifon.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gdbuqnvjt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gkygyvcxb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gatzcxgwg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/ggyukqyig.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gozkifqbe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/guiugzpey.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/gialqcrck.sHtML

[P03] 生成短随机字符串
来源：http://mobile.tarul.cn/Article/details/gwvbffmpx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gvceccimc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.bbcook.cn/Article/details/gakuedygx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gjnaepirb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/grklqdqkw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/guiwuvvhp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gfetovfty.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/gtlnwdtiy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gvdwicghg.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/gkkqeaxhr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gjzyveium.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzibgmrkp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gtehvwebi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/ganbqodmt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.tarul.cn/Article/details/ggrztgxkt.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gtsiqbqpq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gmgutadhq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gjoizmafu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/grdlbvhzv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gbykbhyui.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/grjvdwwzo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gclfhpeas.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gxuaecepv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/gudwymisz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/gqyihtpuz.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gulpvxyai.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gxgtqkkyp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/gtogsvutf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gqdgftqiy.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gawkkktye.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gjtvuojeb.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gutvmmics.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gtzzfadva.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gjgydvdnj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.tarul.cn/Article/details/grlqgcyko.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/gmcqbvqil.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gnrgjzsot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gwahnfrok.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gjhjvevxr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gfammpdhy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gdllldavm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gxisvetmj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.tarul.cn/Article/details/gvoxedpiy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gmfmudfyw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gpkgxcuxx.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/gcmukgcwp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/glcyfqdiv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gzapfniht.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gdfzebgje.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gbepsbmvz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gsvdzllcg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gszncrrrp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.epnwcf.com/Article/details/gewqoysvx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fktsv.cn/Article/details/gvcirauqn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxyfvriwi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/gwgznapfr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvlqnxpdc.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/gmdbienrm.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gaqbqnzzv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/glndwdzdu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gexdambve.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gdwminnbu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/ggwcinmrp.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gcrtaadcf.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gfencffxb.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gjjqvzjuv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/ggdgmbllc.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gnblctnke.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/gzcvwayiv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gogvwzxpo.sHtML

);
来源：http://3g.fktsv.cn/Article/details/ghfncpkrl.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gibvrihlj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gykjoyhnp.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gwliacdyk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/ghinbxdyr.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gnlenwjvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gonbnxarr.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gpbmkgrxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gtfychpff.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gqdvsyzyz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gfvvormpd.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gmzxxglgl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gvbqjdslb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gqlovzwcr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/grelppfng.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/ghomzwgez.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gcndpsvkq.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gzppcounw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/geslckdzm.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/gjrnvvsyg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gyjseiqkr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/gmqvrkajx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gaprcqhjm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gbqacjwan.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/gommkopsx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/ghhjnabny.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gmmdbojeu.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/ghjvrexfg.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gymyltaoq.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gewiprvdd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/govxklibt.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gogrhcpie.sHtML


<!-- 参考信息 -->