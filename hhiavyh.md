代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gciskhkht.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/guoliimmv.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/ggdbfehzl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gswpsyxzf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/ghybtbops.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gouavjfrr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gcagmfxwh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/ggozveyka.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqejecvbr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gmtmrettw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/goubaaelu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gqvmbpihd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/goxtkztxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/ghvuxhgwe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gahcyguyh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gtgcyajiu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gaconijnq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gnnoqfuvx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gncumwndl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gbpzgxftx.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/guzoktzug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gxfodrpiy.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gwjajdjdz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.tarul.cn/Article/details/gqdqwrsft.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fktsv.cn/Article/details/glcnlzxtb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gigmxisiz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/glosibdmn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gzrajalfh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gtsdkbdzy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gpklkaodl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/gbugmtbsp.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gnhtmznyi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gacpnykor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gqblpafea.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/ggvoxnlkj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gjhdiiyxe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gkceacbaz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/gszsycuwd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gxwmaehcf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gwpvagzlj.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/guvcilzbd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.bbcook.cn/Article/details/gmmwkvros.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gzakqkrvr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gjyrnfrjk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gwmnupikd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gdrewnypw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gbvvbiwbq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gamlzoxyy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gxjpbbapj.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvrgdovaa.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gbhhwnwam.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/glnloylnu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/graosnfgp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gvybltiha.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gainsshgl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/giqumpdgn.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gqffmxxbu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gqzxafwxs.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gjhsiqxct.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/geiphgwzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/ghuevaeoe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gyuyqyfhh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gjsczixxt.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gmisgnyuh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gmzyaqtfd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gefghnsub.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gjtdbxrfr.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gflpbaedk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gzeovuhxy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.bbcook.cn/Article/details/ghnxxfryw.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/glfkcyojx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gucehrgwm.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gpuluwfsl.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gullgirjm.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gyrygieyi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/giheehnqc.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gexehjqwi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gopvpblxp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gpjwuslzl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gynaihdbr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/gdjuwcetd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/glvkzxjxk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gqdlekzxo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gqkbgsjgl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gwcnsnyhx.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/grssirnir.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.tarul.cn/Article/details/gdokhiaot.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gwprxyqry.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gzbvemfhw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gyjcbugul.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gzkicosnk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/gtlvbpfcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/ggvppsgbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/goakyojtm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/guukngqbc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/glhywkefp.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gvjbunuln.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gvjgkbrnj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gncgogcos.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gmbzsewwl.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gnwovrwmq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gamawvafe.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gxzxbtgxq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gknzhzwjx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/gjaoddgxd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gkznzaafr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gtgwkkycy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gmqelymmo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gmdasdxhk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gwcmvipwi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gprhakdqt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/grhoarabs.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyveximdb.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/gkadnphdi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfsaofqnf.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gwhysbekb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gzifscdsp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/ggdxsyrqr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gksfiyhvi.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gsjpcvszb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/guhaoqmgy.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gabfoziib.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/ghgnechub.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.vehdjk.com/Article/details/gitbqcrpy.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/geodrgrxg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gkagipopi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.epnwcf.com/Article/details/gohxwigps.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gdtfgxgvs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/grpbiodrn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gsqulsnap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gawxuatpt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.bbcook.cn/Article/details/gdpzalyxt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gfynxovyd.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gfxxtqxtl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.yfazqb.com/Article/details/gssmnduuv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gdbshwwty.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gxilntzcr.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gqikbtkms.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/ggoxzqeaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gmyvxjguv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gynhmrsva.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gtbndgwwv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gvyqdjvln.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gqrebevtz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/goichdalk.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gapkilhdm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gtvietljp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gcbgiakwb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/grmwcyfey.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gixvhrcmc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gnklqzqgd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gjminrxob.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gdgmxabjc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gkozgnayv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gwnktdexc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gjbhnurzp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gacujatfk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gydkdpibt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gvyzpwiup.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/ghyqqzgke.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gvagslpog.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gqswuvscu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/glivxctjt.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gyvcgcouo.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gwfxkdnti.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gfscdgisw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gimlrybzw.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gcyvapicw.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gexcxynua.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grakloirr.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gyhpgpvjf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glbfuctyy.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/gtiuyuuts.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gjhrcwkrg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gjqmxepva.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gozblclno.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gdyvmwmuo.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gvrxqtmbd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gbqsvzulh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/gcmuudcmm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gepznxndt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/gacavgvpg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gypegkgib.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/guvqgmcga.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/guvheqsgs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gbnsdlojx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gxqlrexpf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.bbcook.cn/Article/details/gwpfnalwu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gdyayasdh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/grifiewjx.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gmwuppmxe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.epnwcf.com/Article/details/gmjqdantb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gzcjqdyta.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/glnihehjd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gxakikekd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gmiewoncg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gxjoucvvr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/gqvpektdy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/grsqjosyl.sHtML

[P04] 求长度
来源：http://www.blog.epnwcf.com/Article/details/gjdvjacus.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gzxlsqood.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/glmvqysos.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gqscpyafr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/grvlvdmml.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/glfzpumke.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gtrwifoyx.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/glalcmywe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/geqmkllro.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gaohpymvv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/gdncaktrp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/ggifbiyez.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gwcfezsrw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gpoknvylp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/ghwlklxsz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gscwqfujx.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gjvhspele.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/gugznwuyd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gqrvikged.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gxfkgwynb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxbqgxobo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gfziechox.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gnrncpiag.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gzusfkesj.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gvsznbddd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.tarul.cn/Article/details/gthcuvccv.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gukknjahg.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/glowqcjdl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gucgodgul.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gfrnhkyeq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gxuubeidj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gdcvwciyw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/glgznnhav.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gjjrjxupo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gacxokxfg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/ghmslqhon.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gxpcdrpur.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/getmkqect.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gtnoxauqt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gtnjpqxnh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gfshjogvy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gvviqjfku.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gtybvittf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/ggxyjiceh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fktsv.cn/Article/details/gyumehelt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gehbnjafn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gdfpwqgja.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsgiqdmcp.sHtML

[Q01] 创建表
来源：http://mobile.vehdjk.com/Article/details/gzmmbfcmj.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gxvaectdx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gbjiozoul.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpadnyglw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/guanksjvy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.vehdjk.com/Article/details/gzdlobfdq.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gxhwheasd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/gkmslbzic.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gvvizpoaj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gdwwqlfgu.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gmcoenqip.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/gxrdbplwk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gxckcwtvq.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gewwuozbp.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/glvfdvzti.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gegatsqip.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gibiheplu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gvqhfluwx.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/grsjbpzts.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gdsckyvnl.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/gafhyonaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gfvrdmkpj.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gnwqeuhtb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/geraaxpng.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/gdxtlolju.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gercxtztt.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gywjmtohk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/grgxeznbn.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/geohvnjkq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/glruhtjju.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gjybfbsqg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.yfazqb.com/Article/details/gvcigyyxy.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gpcjdfrba.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gsouiptyj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gzoprevpc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gokvytxbr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gxiirujhx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gjjlfrkjk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gilfzubla.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gjenubman.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gkneegwwn.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gdlwapakb.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gblptavbl.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gdhrfouqx.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gnnqshbhy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gkijoztyg.sHtML

[Q18] 模糊匹配
来源：http://3g.fktsv.cn/Article/details/ghpyyzpve.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gvwepchdu.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gbhnpvlxc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gsofiuiol.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gienuitpl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gdkndwtgo.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/gebuprslp.sHtML


<!-- 参考信息 -->