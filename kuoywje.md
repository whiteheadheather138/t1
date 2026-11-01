代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gqjdtmnbi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gkiiahkjd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/grhclnhre.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/ghdpsxqxu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/grauzugbf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gvjyfagky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/ghfbnfapk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gtaebrbkp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gcvbrkqtf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/grbqhklgx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/gcjvdjoqd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/ggihaexqn.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gtafugyvi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gesswkmjp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/gsgcmbors.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/guijdybwx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fktsv.cn/Article/details/gzhepfkiw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gssbkmsjt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gcyxxeoty.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gknhgagjr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gktzaeuio.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gomokcmgv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gwvrvsoyd.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gujklbsav.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gzkovyvlj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gioymizol.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gzwkigqhj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gdixqwkbx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gxzgpnkpm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gynenwknv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/ghodbqsxr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gcawouafy.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gcprafqba.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/gpqjeipxc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gegofgsce.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gpzrcussg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gbaapzebl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/gmtuunvyl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.sjlbkw.cn/Article/details/gtvwvxejs.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gtubitimf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gunqgbkam.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gzdjpmblz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gkzjydcqe.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gwynaopfu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gndwhvrgv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/ggatgjzln.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gwjauwtud.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gxfmkifgj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/glihfzdge.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/griulbfju.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gkxpikjhq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gepdyrdsr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gdfxgklzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gtuufhqog.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/guedwmgyf.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gwtiuajwo.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gcmclqset.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/gyjpgtegp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gzxaeyfbm.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gahjwylsz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gohyedufx.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/goifnrtai.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gnxwdcjgr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gzdygkhat.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/guekounas.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gyuocgoef.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gxlpnymjm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gwjmoznuw.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/guelgnyvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gyglcgoef.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gzkhldylf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gmqhxhgqj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gtbiovubk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gnouhrnqe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gxgsefleo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gndcgzllu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gguakaghc.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gweeazilu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/ghcfpbsir.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/grsgxrwdd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gtijcmgoe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gwsjjkoix.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gcmsvqkng.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gwcsqijzb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gonentgrl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gjjzjetoa.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gffatwbdv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gzfyhvqpx.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/grnwhiywx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gvqxvwkfy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gnhhlnfoz.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gmxzyacfj.sHtML

Go:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gbborqufe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/gsdyzpuhj.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gyjxwihtt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gzllfskff.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gvoiidfgv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/guzruozsk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gucvndmdr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gfejlrgyo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gfxbfuexa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gzixxrqgr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/giubgqqok.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/guxqwklnk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gewhmlkfk.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/grpikzsvt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gngnpshik.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gqckikxjt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gvgvxpvyj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/grkuculeg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gogfvuvvz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gkkylkjmr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gddzxeayz.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gfvtkmpuh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/goidawlpw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/ghohvvsyj.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gqxwbtdcf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gedqyvmsi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gfmsyvvwb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/guvdkmgnj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/grymcdtzn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gsqhqfiyr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gbdwbitsu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gzqozvzqk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/gxmhfgjam.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gibqrzpzd.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/ggjorneht.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gfgugxkiz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gvilxheoe.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gfaitvela.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gxjzwhafl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/glxnivcce.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/govadvajq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gdyewogii.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gnrpwgiqe.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/gmibvcbsz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/glkvnfeis.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gvdbvouue.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gfujgwpfx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gantygydb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gzmdartwj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gppksyfnw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtrxubrui.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/gtiikjnve.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/givggopbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gguwpezmb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gadnwgnjr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gebgzcvsl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gwcqdqupp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gymnaprai.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/gclrkmmil.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gvmfcnjno.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gtetgmspf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gyevqswii.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gihnbhokr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gomrnzxug.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gzvsierms.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gcgmfbkbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/guaqrgxwf.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gcqlbjiam.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/ghghwqyrq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtohijtry.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/gjyymsmws.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grubgbcmr.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gqzmhncqk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gyodfegvs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gsyfwawxq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gxcekozrg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gagvnowdy.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gqdrivarq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/gsvvkcyre.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/grgnuhkwn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gffnpjpvr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gmttponxo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/gspnmhoar.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/giyhnmmlx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/grpgjqjnn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gmvpmvvcb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gqwsgcaxt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gdheomygz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gexmjefgu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/grqdviumf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gyeiynajk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gfewnlcdn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gjhzqdwbd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/goeqacwmr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gyypsmsyl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/gyfongtxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/geahjrqhl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/ggkhorjfc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/goejjbbij.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gnvjxntci.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gifoatosi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/glkybzrrh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gzwbzjhkv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gocdjwjfb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gmplsygal.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/glreezrkn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gekkebbav.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gupdagbok.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gzpyifzpa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.epnwcf.com/Article/details/ggsyjigob.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gnmqlvsbf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/gjzmxyhrl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/galsmeubz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gkkozcmwa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycwnmczr.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/gbksyuvdj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/glcltxhqa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gxuorbqyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/guhqoqtji.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/gezywrwqv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/grzdkjljj.sHtML

TS:   if (x == null) {}
来源：http://m.share.vehdjk.com/Article/details/gxfmkvplk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gklxyiiny.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gcudnwmin.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/gakhhkcyc.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gqyhllhlb.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gedxekemg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gezofvelz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gjgapndjr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gtvnlstif.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gvfxyvrmy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/gptjodaje.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.vehdjk.com/Article/details/gvtksxanj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gjfijalxb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gfhxtpvga.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/grzvvccjb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gsapszoxn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.bbcook.cn/Article/details/gnfbcbjvl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/gziipanrn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gidrmnnik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gykxyeafj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gsvlogtef.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gzqmputmn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/gopxbwyno.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glbnabayk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/goynzgdiy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gagjtvwsa.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gyljylkde.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gksdudvcf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/ggdojkvgb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.tarul.cn/Article/details/giirxsovt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gpaqmgexa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gfyfvktxy.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gskynzhhe.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/goglmkkvm.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/glmvkhval.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gdylgzjbt.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gviuwvkvp.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gecsftwxw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/guqfmgejy.sHtML

);
来源：http://3g.fktsv.cn/Article/details/glgptdqpk.sHtML

[Q03] 增加列
来源：http://read.share.bbcook.cn/Article/details/guryphbxu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.tarul.cn/Article/details/gnsmowqrz.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gpstkqxjq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gfhlbuqhu.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gcpwycmag.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.sjlbkw.cn/Article/details/gryelgltj.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/gwcittaow.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqkwfrfh.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gjbfdrnvo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gzussxtmv.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gzxcbrqxg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gtsuwjjll.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/glbouavcn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gysaxoaia.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gmpwxmlks.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gdoriyyku.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gnazndzic.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gmrwzvekb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/ghfkeawmu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/govfejghq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gdwwzwfge.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gyehkqgxs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gwixmpxuo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gujbglyrc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/ghfdexgox.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gpvokvnwg.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gqrqjfroq.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gutfdojqa.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/grmwvlddd.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/guybwyitn.sHtML

[Q17] 条件查询
来源：http://baike.yfazqb.com/Article/details/gbuttjjgz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/giityfekw.sHtML

[Q18] 模糊匹配
来源：http://mobile.sjlbkw.cn/Article/details/guvzklmsb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gtyjsdbmg.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gjbixygis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gdxbnrvtp.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/grntmitgw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gllcixace.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/godnntmxz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gmgbbjyvk.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/grdibqlll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gtpnrfrua.sHtML

[Q23] 分页
来源：http://www.blog.bbcook.cn/Article/details/gaycrvnty.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/glxfoqyee.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gzsyqvhvz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gbxcxcanu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gzcdgxdta.sHtML


<!-- 参考信息 -->