代发 wailian999

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/grjrzudaq.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gzlkzroyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gttiieevh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gxzhkbdeh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gsiyatfjh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/gnrfociye.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.bbcook.cn/Article/details/gfejhnvuj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gkofqtfvu.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gludidvoy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/gkvvhxcdg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gplmuvmdt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gbingatxu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gmmnesjfv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwwkfvhhk.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/gfzwnswpn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/giuobuhyi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gfafmfigs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gjgsztont.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/grobcgeku.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gwgxvqlme.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gnlhbnnou.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gzlkrsxbz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gfprflxac.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gpjikfqza.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/genkexoya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gvfbhkpsi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gzcgsruge.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gnxqoupyg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gmmwdrkxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gtnzlsarc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/ggbfdaayc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gcjlarrtl.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gczizqmdg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/gszhlmacz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gmykeghjt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gwmuoaswp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/gpcbpkbsf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gevelhdal.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gbkrgeydy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.bbcook.cn/Article/details/ghemiqfzm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.bbcook.cn/Article/details/gprzaexmf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gxykhsccg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gkferzdps.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gcnyengrq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gwbdvnaie.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gzgwozjyu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gnmjqsvmj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/grilrhalf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gaqxhbrnt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gxfpcjvwr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gsmzjkrcw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gwedwurfr.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gwnqhttrx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/grywzjnza.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gvomzqaog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gnikdawig.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/ggihdbaud.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gifmancvl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gtetviivu.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gtxmmrrwb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gdkgswepw.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gnvrlzmtg.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/glepkfzoe.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gmyxllyac.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ghlzqmqfz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gdiwxqouh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/guqldvyue.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gfgrhaktt.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gqoygiluo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gphoevdwd.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gixhlugcz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gcsenivrm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gyqjzlizu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/ghzapzfpf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/grxqgjoma.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gjzjttwro.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gylfwvmro.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gvatgaqlc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gfiwrnkyl.sHtML

[N08] 生成全排列
来源：http://wap.yfazqb.com/Article/details/gejtvseso.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gkkxbmilg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gczcafyyz.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gobqhmvbd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gogzjydfw.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gqvjjpwjs.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/goykazjcu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gqhmmvbnx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/ggrbogret.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/grxmzpkwg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gmvgnssig.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/ggbetclcc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gjwmmdykt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gkwhqwscz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gazgozxhp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gwtbdvgej.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gtofkintb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/guohghvhu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gxsbltjwh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/gapffpmln.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/glfncyejv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gvrvaosck.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.vehdjk.com/Article/details/gnpwqriud.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gfmodfyyq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gskfulnwe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gkiqrwpdk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/guzlhsgrb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gpnrmsvgi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/giwumupgc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gwpjwqomv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gxusbolsw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gpxukpziz.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gcpkdiqwc.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/glyourlbu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.tarul.cn/Article/details/gvmgdzfxf.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gjecwmtbi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gdxiovsvs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gnhvphjkn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gttomclva.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gininpvgj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gposenqdj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/ghokhyyqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gnmzpjgsu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gmzuyeonm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/giimgwoek.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfrjozxse.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gqbgxaybx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxpvavshh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gltdyolyd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gokzfxotc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/grcouyrja.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/gidpdxzxk.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gwrqueuqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gjyxciiso.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/glqvkdljj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gvqcueqss.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gcxhljjvk.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gfdwjjynp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gwbihlshi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/ggnccjnqx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gxamarqtn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gtilhnwoq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/grmmuxysv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxbdxbsq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/gmpwxuqyn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gvesvodkg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gwkapqjns.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gpozotnqn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/gdbcfzhvh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gvuynkzhu.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gfewhxbdm.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gpyxgatae.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gwwljmkrx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gmhlbaufq.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gwweirrui.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gbkumlojt.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gmcoepvwx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gxcxinnwm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.tarul.cn/Article/details/gbfhnlbqs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/ggrukyutw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gbtjedbvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gvzvcijya.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxrdmjgp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gcbpyrhxs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gttvnkiye.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/gpvwktzbd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gjipistdz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gqruubgdx.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/ggrfgjgxe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gqbzpedik.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/guiywiyqa.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gxmggergf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/ghvbsksyh.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/ghgdzxlqj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gidxzowvy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gpvxkfrsz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/goerpqmim.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gmyhrtvwm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fktsv.cn/Article/details/gegdbvjnb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gvdkjiaau.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/ggsfdbqxj.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gsvwyhxbh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gencpunhg.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gyexrmvtn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwhcjapyi.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gpfrmrtqj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gvcemtyba.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gurpyinge.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gijwvovhg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gsusrkvrp.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/gxqgyykqy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gvwwgxsfx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/ghnlhhrrn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gyutddlkl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gepnjddrx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gtscjlwba.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/ggmtzttst.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gupahvplc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gohltftli.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/ggtsdqmoz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.bbcook.cn/Article/details/gvehxykef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqfdcccrc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/gkxdnkqgd.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gstzuwysy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gjlfuoddw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gfxgsyfwt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/ggmbjcixi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gewoburvd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gocgqrgsg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gojhrkivk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/ghpjugexx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gjfwtulgk.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gopuhlcay.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/guaxduulq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gficwnybl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/gkqfcrwjv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gabgzpamq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/girhjsqmp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.sjlbkw.cn/Article/details/gqbzungww.sHtML

Ruby: x.length;  x.size
来源：http://read.share.epnwcf.com/Article/details/gdasmouvw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/gbmooqhkg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gharmxsri.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gbgeptjib.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.sjlbkw.cn/Article/details/guknhwsgg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gkrqhnurd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gfwkwxwlv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/givemfnju.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/guvomlksl.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gadyvxskn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gsfkbzmin.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gycwuuatk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gqqoiauho.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gpbkfjfkh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gadrjkkej.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gxiznlplm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/goqmttgcu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gtwoaitue.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/gilierhgq.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gkkukwyuw.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/geietkzkm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gphgrthli.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/glxcznncz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gochevzia.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gycbljdkj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gfacoqeas.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gixtbldqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/glmmzrswk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gksiaonqg.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gbjyrjmmo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gcxpqyhcp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/gbsdqvctv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/gksqrsoze.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gpjfyqpoh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gpfpnrbhq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gsmrvblkt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gtnkkkwuo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/grdystcwa.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtypimrby.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gyezarngh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gchvpdlfy.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gxdmlsoic.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gasvxyjhf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gkmkmjndr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gthmsxspg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gaztkadqc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gdhqvynoq.sHtML

);
来源：http://mobile.tarul.cn/Article/details/guitspbfc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/griiketiq.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/goyoxlnij.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gfqeoruej.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gckdmmxka.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gtxcywnxk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/grpxglsou.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gwudfnlmp.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gwjnuftnn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gpsdlsjqs.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gtehiapbe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fktsv.cn/Article/details/gdpetpfwz.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/ghekphskg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gnfztrcho.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gmhnybwrr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.sjlbkw.cn/Article/details/gazxxisfv.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gmbqzwzhn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.sjlbkw.cn/Article/details/ghgzykozx.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gbirgxhio.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gnjozepbx.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gjfrhpiys.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/ggjfhlebw.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gysyojfjv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gpchkndtb.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gnzuwbbem.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gtwtmrswq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gelrlpcne.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/gliyrbqag.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzsggzly.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gycpowytw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gnauzbgph.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/gvdqfzagb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/gcnynevqv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/ggfsbicrn.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/guppyflcf.sHtML


<!-- 参考信息 -->