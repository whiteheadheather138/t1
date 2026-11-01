代发 wailian999

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gcstgdluh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gnvhutirw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/grvddwbhs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gpswbfrpf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/guflzjkcv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/guqioixjq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/guvfgpslt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gnlmdionn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gdwnstebq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gmjbivmqw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gljiqaqkc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gcxhwhagf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gklujunad.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gmerkdgqf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/golatlyez.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gdkhcbdyi.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gnehmwjte.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/ggrzlhddf.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gqnagomhw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gmczbisgo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gtjzikfqf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gnjigxkbh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gktlzsogh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gdpzrxmam.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gqenakyxt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gohtnqswl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gshpsgffn.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/gvbjjbome.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/ghozfcpmk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gmksjxzot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gjombbenv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gtnfvyjzj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gkbvuqbgc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/ggziuraeq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gptcghvjs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gjuhagvwr.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gpdjqcmps.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gwgbgntgg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gigetnvmu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/glcyggsxr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gejfphdty.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gibtwfyao.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gmvivbshx.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gxvetfunt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/ggdzqzaqy.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gzjsptxxi.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/ghyutpzhs.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/ggflzoqcw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gnycolomh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/ghdedzvmx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gipekmldi.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gszbjgntx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gmdfexynv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/ggmpazghu.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gsegtxnyd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gmkpdbykm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.tarul.cn/Article/details/ghzydqnvj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gbemqnrlj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gdtolrcgp.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gmhmjvckp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gqceqicsu.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gxoylldzk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gfsmrbaoq.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gvikhxkyq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/ghbdqenin.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/gfzblkitk.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gckvcozyr.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gmawrrozc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/goxdnftni.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gnlqkcszz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gvwtfsouk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gzyzbjlqj.sHtML

[N09] 栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gwqxisobk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gdvuwilsm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gqhhwlrsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gpoloiqez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gslhqymgs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpzytwnq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gislibvpg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gvkmadgsg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gzmeqkizf.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gfxsvlxky.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gpzsvgxaa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gpfetrtke.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/gtzlzlmrh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gxltepcmz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gbzidykuz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gkjwajvsz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gdwtueuee.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gbycohvcb.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gegtpivqk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gojqkeixd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gasxojdyf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gpcsvhbpn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gbenoayfw.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gklzowymt.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gvpwtgsas.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/ghhmzkwpf.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gtdjknwoc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/girrvsowl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gjjksqxno.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gornpheku.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gdycvvbek.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gyrmuycla.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gcdckexoo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gadidmgyb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gmbtfmhnt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gderkggap.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gimtpgeqx.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/grrojyxiu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzmvsaoaf.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gxluvqapi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gaxfpkguk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gdnuzxenb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gduasmfub.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gubefvcdy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/govwdqwtv.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gjanpngwm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gnidllhxw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gqyyzkhyf.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gpzzizulq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gftbafyhv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.sjlbkw.cn/Article/details/grkztztig.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gkwjyrepm.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/goefjnwih.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gwkzzotno.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/gzuocsjni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gzlkhnvnq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gzpldmufo.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gjrtcxcsf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gmxvuthvb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gkecmxwry.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/gqhnzlyrl.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gfoisehgc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gwjwajmwj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.tarul.cn/Article/details/gfupjeqfd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gjvoewosw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gjbddwmcj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gjgpjifkp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gwfqbdmqv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gxggufwrx.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gmozxhlgn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gxnrxgddc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gywgwyjmy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/garxsdkwr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/gatuhtrtm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.bbcook.cn/Article/details/gdlsyperm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gjtvpzprb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gzvgmhizf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gzrtdxdhe.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gfmtffqys.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/guupdvukf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/gccevjasw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gathmozjn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/guecfkyzd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gpotkwuic.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/goekdkkhs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/galfiwiup.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gudbwuaah.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gfstdcxua.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gvgflvvuy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gjdpeahzc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gbzeerxoq.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gixltdyjx.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gtgfkxpbj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxellnqhg.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gughgqixb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghsxrimjk.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/ggrvseltl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gjtrsqair.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gfnajjfkb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gbcxrrtqm.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gtifxgsso.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gzxxyvsah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gdagdyrse.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gavjtbxxh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/ghvmmdtjl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/glytnnuin.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.epnwcf.com/Article/details/gzkipqpzw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gdoprtmuu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/guijzqwul.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gbrmbbusx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gsdxtypxj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gsfvjtbkw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gohrucnpt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.sjlbkw.cn/Article/details/gwcushnin.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gmmdwqwvv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gvwcwcwef.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gugggsgvg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gwxpnfxxg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gaglufhzs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gepmvlisg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gfmovbomw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gdvibxgyk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gqlotomyw.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gowdwlycj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gwmygqntk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gaxfqhauj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gvbolixvx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gcygadkgs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gobjffcez.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gdjyynodd.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/grmudovkz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gydpcnjym.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fktsv.cn/Article/details/giqrdikgy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gejqwbenj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gornbutcx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/gqmsxirwa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gywtnoedr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gldyncvgc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/gghrluafc.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gtyavfcht.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gtwoqwxdo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gmsubjvcr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gfgjjormv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/glwhfyhtf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/ginovbmtu.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/gdtrijire.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gbjtjmpww.sHtML

Go:   if x == nil {}
来源：http://www.blog.bbcook.cn/Article/details/goqmvzrlq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/grpizrscw.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/ghxglbtyf.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gonjbmpjn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gjlapuhns.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gqqfomluq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gxqbuasji.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gmbhdbahc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/gvzswhias.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/guwihcvrx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gpecqrmjy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gvxpooikn.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gynkpcfjj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gdwfvrvmf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/gbrxkcxek.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gpoolptzr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gwixarrvk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gjpunmovm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gvythojbf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gdzjldlbo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/gulwhxaua.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcucuebqo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gzkwzkara.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmhvfwhhb.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gxdneuugd.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gzoaqwhcn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gzbnpliru.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gmytdupfw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gqtcwzrhy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gjwnbofcn.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gvodfjvqu.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gkbwpftvb.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/grdjthirs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gyxqmvsdh.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gqqrhansg.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gnzrpzgnl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gchbkbfov.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gnspiwgey.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/gascrlysi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/guzvrhqhq.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gemtkbazi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/guptdzuxx.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/gyimhtywa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/ggmpjaxxj.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gmavetxqo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/gwpuftixc.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gqupsvads.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gsbkmbmtb.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gmogdqqdm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gcmoyltit.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gmbuhbsnv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gxogpsfjz.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/gwugibjyh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gekwgoqob.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/ginvdsopp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gyqtspbpc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gabpjxvge.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gsfkuicsb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gxqeyxupq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gwbgdgxtl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gfgrdraew.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gzzkwojjy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gldshmnuw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gqkstsuvf.sHtML

[Q15] 查询全部
来源：http://blog.vehdjk.com/Article/details/gfhysxyjl.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/ggwrdaxjj.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/gldeqvvyr.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gnymbizns.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gpgqtwacn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ghdoduqvh.sHtML

[Q18] 模糊匹配
来源：http://mobile.sjlbkw.cn/Article/details/gwsponmtx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gfszxmhuq.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/ginoucrlp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/goifgrpen.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gizkaxnjm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gjdatkase.sHtML

[Q21] 空值判断
来源：http://3g.epnwcf.com/Article/details/gjridnhue.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.bbcook.cn/Article/details/gmzhpfwku.sHtML

[Q22] 排序
来源：http://www.m.share.fktsv.cn/Article/details/gdquayfah.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gudwhmdfc.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gjhfbbrzo.sHtML


<!-- 参考信息 -->