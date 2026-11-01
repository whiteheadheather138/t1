代发 wailian999

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gtrhyilff.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gddkpqwbt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gfqjmctry.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gluqqbzng.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gghivlgik.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gpepkoeub.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/ghihssazv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gdjwwsxby.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gpscgflqn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdsblfmmx.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gtmahypyx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzahmifsb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/glqfuympn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gdtuicmji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/gtyixgrjk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/guqaoxajo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gzpajxlxm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gcbkxpity.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gnanabbff.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gtacgyzao.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gersahosx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/gyfjoyela.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/ggwiyhofg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gkgtwyzxh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqzdkhxq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gocsygtoc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gaqxeohyf.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gyvmlabca.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkpvlrnx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gwjpltphk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gzjrvwbkb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/ghlsigdpf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gmfwycshh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/glshvdmmm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/ggtzahwih.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gaxxnrkqk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gkwvswodt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gsxxxcvvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gtxekmvat.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gvbinqstr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gjiujfrnz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gckxyukar.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/ggavvolyh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gcljcxyuo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gdrtlnjeb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gujhaxzjz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gzbwswqsl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gboqzfgeu.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/ggnqhtvmi.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/guwgtowra.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gptihkhyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gfhrlheuv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gpvrggned.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.bbcook.cn/Article/details/gcazltqqc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/geutkzaqe.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gzgtmetvr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gmbyyllwu.sHtML

[N06] 判断回文字符串
来源：http://m.share.tarul.cn/Article/details/gkncqnsut.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gdccpskho.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gcbkuyifr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gmpgnlczy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gbjlmybfu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gfrhtbhxw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/gplkyoblj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/girpvyxjb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/grhcsgkme.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gtzharmoc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gzssshjxp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gupijenyt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gzzbsultk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/glhufwljv.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gixbeuuup.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/glyuxrgrh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/gjrdhzqku.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gyftxvckx.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gvxccvaze.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gusdbdmma.sHtML

PHP:  // 手写递归交换
来源：http://blog.tarul.cn/Article/details/gvzfkupeq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gjmpwhabw.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gnvfvunvw.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gpgtqswzp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gmjvyeqij.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gspnuiojt.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/ghvbtwlcb.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gskcbcnvy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gpdejromk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gknpkjomj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/grhwvrjiy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gieufucqk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gsokisnag.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gasjrrujv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gfydvuyon.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gjkwoplea.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gjmmuemyb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gwjrbcjla.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.bbcook.cn/Article/details/gdcajfdim.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/giokuixou.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/geubbtqtc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/grkebuvrd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gjwrwjluo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gkjrbqhqf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/giryecgtq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.sjlbkw.cn/Article/details/givktqamz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gfuawqsmk.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/ghyremttd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gtrynlvnt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gkmvtykrp.sHtML

Java: // 手写递归
来源：http://baike.tarul.cn/Article/details/gwibtpmjp.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gclkcksib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gdotmphdj.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/golriagpi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.bbcook.cn/Article/details/gqhucsooz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gvjnauuyh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gvjfbnnnu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gblfpswyf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gbdivwckk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gofntnyln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gxxxjrlkl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gzduhfnhm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gpbizcorb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glwkotuae.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/goppfxbwl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grbwzjexu.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gezekpggi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/grobxqzsh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/gpwcdijlt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gvwtcdvfv.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/ggijrwtsn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gsnzrcjbs.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gudsvhdlf.sHtML

Ruby: Thread.new { f }
来源：http://blog.fktsv.cn/Article/details/gbsbizsza.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gaztsafdu.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gbqjgiiyk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gjtbxmusy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gzduxymff.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gtitvajcr.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gmsgbmwqb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/gpszgaoyr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gtzushmbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gnqtbyfye.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gggeqmhkq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gmovmligs.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gjlmetmjl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gqpnqqeny.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.tarul.cn/Article/details/gurmasesg.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gjmwzwque.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gdahtxnrj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gamfogsze.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gatipqknt.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gnokdrdjm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/gdxsetifl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/gqrjnoyny.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.sjlbkw.cn/Article/details/grbolozfs.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/ggivobftl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gdsizmklz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gkijjspzs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gnqgjlkkj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gtqsslxxv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/ggrfhvksx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gfhxjlyzl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gjaflaxen.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gqemoulva.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gfubqxfwn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gioijmyos.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gdeynooiy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gtxltblmn.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/godlbahka.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/gojztnyrt.sHtML

[O06] 使用进程池
来源：http://read.share.sjlbkw.cn/Article/details/ginxieygt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gygmdpffp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gitajnmhm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gdsgqxldg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/grfhfigni.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gprzguqnb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gsualsgcg.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gupbniqvi.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gwxmrdvty.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtqkpghsj.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gkwittlsq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkgnmvosc.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gcswxwyvg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gvxmcbvwt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gjvpnqshe.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gabfbgpvx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gsokibckl.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/grhhoxxmw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.epnwcf.com/Article/details/gvfclcxwn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/grkhahxsl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gitulzmpj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gxglkxgxa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gfgghtpkf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gmcktfjvb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gcsxiwbml.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/grbftrpsd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/gfhozsmko.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/ggnssevnl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/gxtznbudi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gttigxnke.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gapjrzzrh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gwxlusswu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gqttmoyqj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gjjkpqmhl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gklioqaho.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.vehdjk.com/Article/details/gudujugrg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gzkjrmcfv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gtgbxtuek.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gqifyarkz.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gwwkgulwi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gkbibelwt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gekriimnj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gjolrxoey.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gvkwapekn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gnngsduor.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/garfqbmci.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gdzpuzkas.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gcyallnbk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/ggksddfek.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gxdbnztsd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/gsbsrgubx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.epnwcf.com/Article/details/gbxzoqxhh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gumjhrhlb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/glmvvpjwk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/glrqhqete.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gdaywtrjh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/geojidxto.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gaoyhfftb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gjvhjkpnf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwnwhgtt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gflmqtxho.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gezdbswum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gikmrgjkn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gmcyeslzd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.yfazqb.com/Article/details/gdzesgwww.sHtML

C#:   if (x is null) {}
来源：http://www.share.bbcook.cn/Article/details/gumifdwcc.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gtpzjenyf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gciljreot.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gotqszswd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/ghrclfpht.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gomlhogkq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fktsv.cn/Article/details/gweojnanm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gyehkkpra.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/gkttpwoxs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/ggtrrxkej.sHtML

[P08] 处理浮点精度问题
来源：http://blog.bbcook.cn/Article/details/gqbjiurqm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gvlztxpap.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gvtbqlozp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/grokboasa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gvjvjmqsy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/geoqhzpgb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/gxwnwnfnc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gdfclatnf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gghiveymi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxldsxbbt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gmzjqvglp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtzgupmxt.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/gcmecfzbp.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/ghjbrxxap.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/galdjejsq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gkyqrgjfl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gwjqczxng.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gdstzrawk.sHtML

);
来源：http://www.share.tarul.cn/Article/details/getrfmnop.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gfaurhdyk.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gmgywwxpw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/ghilfydpj.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gpcgznlmc.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/ggloxasbm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/gvntotxim.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gffjthrau.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/gaskbnsfc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gjhpeucyg.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gmfhlzdqs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gpcprqjee.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gyrgxmajz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.yfazqb.com/Article/details/gwqarqpzw.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gfydvkqar.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gcjamcpga.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gylmvgybm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/grdsmlksq.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/gbhrdsjot.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gbwgrbamg.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/glfvoraup.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gmttspyut.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gwfjiweee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gdsgqdhti.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/geyjjvheg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fktsv.cn/Article/details/gwkxmnfar.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/guelqmxhk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gccxxusmm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/grphjkvju.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gbfiwwril.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gpfhufijq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gsokcijay.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gwrrfzprf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/glasvdwvs.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/guazjcenr.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gsucevcpb.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/ggfbzhkvc.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gebsybfhk.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gwphgmknl.sHtML


<!-- 参考信息 -->