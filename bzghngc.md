代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gsimtpylk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/grzlgiiut.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gyaqbkgry.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gnzjsweni.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gucklsgpn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gzrtjyknm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gptsiekde.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/guislxxcp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gdarwieam.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gwqykeshr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gioxcxvjc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/ghxpjmbca.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gitzewnfq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gpoeibisp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gnaozfafr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gwieqxzkq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/gvecypnrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gzzdxcebg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gmpqkwzva.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/guqswraiz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gfyfnlkju.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gchzrkpmq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gbiutuuiq.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gbwaepcpw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gxdqbrwgi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gfcqdwtdn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gbagdnycz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gxdargtlg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/ggozoygbj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gzkesmesh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gmydqmyjf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gyenbzoza.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/ghmahximx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/gyixcoeje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gjvgqsnbh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gjqrftqfa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gosfjqdai.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gezljlbzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/ggeveqeht.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gskwpbfor.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/glglfbhln.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/gxktohpxu.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gsdeyynmp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/gbxuvwoiv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gzaovxutk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gacdcrelp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gpsahyqpc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/grtxnsrzv.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gynyehshj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/glexfwqdm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/gxzkfurlw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/gyymiezzg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gymrcvfcl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gatufjcju.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gxrvldhts.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/gdnzwfkis.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gwunzliqo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gyubunhon.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gecdvcued.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gkfhizdka.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtdislyl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/gozacyhfo.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/guautwizo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gtrrqnniw.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gfwuxylfj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/grivrjkno.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gryspkqvr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gydthjweo.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gvlsquxaj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gfcvtayfx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gpuigibco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gbshszsgj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gezvwxhfy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gfsyhtufs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gnzyexydd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/glocrfknl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gztpzimpz.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gynrdtjcb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gddtrfgug.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gxaysrkda.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gxkjutzql.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/gqhumwlul.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gacvkqqmp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gasdunuuk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gaalilrvv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gbshiccog.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/ggerkrtun.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gazysqjtf.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gdwndhgow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/guhfmfdpm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gkypxdtdu.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gtigoyxhq.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gujsokdzt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gwymiznlo.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gbzkhybif.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gcmhaxmre.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gqgsnaqmi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gpgzpllwy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/ganhbjnkn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gilybggpl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gwqukxpev.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gblyjuycy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gxyqknfmj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/geyxboazd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gejvtbviy.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/gxlkdeaqs.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghqrstmmf.sHtML

[O01] 启动一个线程
来源：http://www.blog.tarul.cn/Article/details/gsxobadur.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gfmfffvuj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gbjcojziw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gdmihzacm.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gtefgkvof.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gxahbuhmx.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gwksvbomx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gxvhlhxir.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gwxvlvzmj.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/gamljezwj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gkwvprhbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gcqzlbcpv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gyjddcmzt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/guwmyfkxm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/ghhuuyrrp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gjnhpkqku.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gpaukhqvz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gjpucbhmh.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gtnulzadn.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gyijtwntm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/gmswatuku.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.bbcook.cn/Article/details/gxuyjptre.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gcgeeyihj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fktsv.cn/Article/details/ghhqhzvie.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gvsqfhpnl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.tarul.cn/Article/details/glthuomok.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gxhwycfxe.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gjgeklluo.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gfnbywdka.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gdfbphrsi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gsdecbtnt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/guhuvxwzy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gnpkcxhbz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/ggqrhgqwd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/giecygdwp.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gbhwpuhjt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gsjtspxws.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/grsbrptkh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gyrvzdzcx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gwvtlaqdj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gmaxydelf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/grszqlhey.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/ghsdcceaa.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/gqyeiwgca.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.epnwcf.com/Article/details/grcycvmdo.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gabelsudq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gkmaiipii.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gzselnods.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gfbjvblkq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gjgqevdwh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/gvhbcfecl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gchwynjtj.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gfyqtqfwz.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gzcohvosa.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqnqlhuhc.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gsfuzlwee.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvydhjtqd.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gypuyyxls.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gzgyvtlkm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gomjlmlyl.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/ghwdishut.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gjxvcagju.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gswizzllt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/guuwoabzf.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gyehlfkae.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/glezqerae.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/ghxvzeejg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/grtsbwrgi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.yfazqb.com/Article/details/goqltkdoc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/geyvmziyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/giigftgdb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.yfazqb.com/Article/details/gahlgzgyz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gfcneppge.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gsnrooipb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gilosyxzu.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/glmxdrrjx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/gcysubbdj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gpfbkwfsx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/grjwfjkob.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gvvatqxao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/gvrrqrcce.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gfleekybr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gixvsolnv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gpyfnwouw.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/ghboftjto.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/ghdjoeqwh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gbqzsuetr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gyhzvjove.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gukuwbfqf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.yfazqb.com/Article/details/gjuafiguw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gjfezsooi.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gjudwupwk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gzqzdtyvu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gghpcdulp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.vehdjk.com/Article/details/gpuuipwho.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gzrklnbhr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gobqqulay.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gdeawfadj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gzgfuzqeh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gsdycatug.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/glrohwqaa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gjxouxdet.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gfmencxxq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gwoglfqto.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/gdfujsecg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.tarul.cn/Article/details/gqqbtmfgh.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/guauqbeec.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gatvxmwfw.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/glttcupur.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/giypjtbnw.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/ggdxavqln.sHtML

[P07] 防抖与节流
来源：http://www.m.share.epnwcf.com/Article/details/ghueucgfa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fktsv.cn/Article/details/ghljtatka.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gbjpmeoot.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gqnjfnnpq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/ghoeceuad.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.bbcook.cn/Article/details/gqnuivjuh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/garzmproe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gecmbcqwh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/gkrgvjeho.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/ggbexekzp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/glpoxxkou.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gcwwavsiy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gbztjnvtk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/griwrbtuk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gczfzgrxm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/ghxmdyqxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/goeurabch.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gyobghevb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtqjqkuzr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/gekikyjzi.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdxkyntgc.sHtML

[Q01] 创建表
来源：http://3g.fktsv.cn/Article/details/gnvxhsxjs.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gktoeiwks.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gywqikvdf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gtfczmeyy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/gyzplaocr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gtkbijlfl.sHtML

);
来源：http://blog.tarul.cn/Article/details/gyzmzxctk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/gudctglyp.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gbnbnnbec.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gbnpwkxsm.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gwhgpgbwy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gbkcbncxd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gkvddktrw.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gphsvxdyb.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/gynlglhpc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gguwgwqbd.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gwlvyntne.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gceuldvrc.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/ggsykjhie.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/golrilfgb.sHtML

[Q06] 删除列
来源：http://wap.epnwcf.com/Article/details/gaddavabi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gsizcvvmu.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gnfsbaqhw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fktsv.cn/Article/details/gwnwafoup.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gpqxrfirf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gvzzfvagt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/gulyqlwgi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/glnhydper.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/grfypqsfg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/glpiaemqp.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/grhlupxxe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gnfboszjb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gfzzsyhgb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gxynfkdfn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gufrbodbo.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/gyhuifqrx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gbwqnmdjr.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gjxlxbsgc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gnrcfwjre.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gufjhzwsq.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/gfhyppiaf.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/grhkrbkij.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gynphwaxm.sHtML

SELECT id, name FROM users;
来源：http://3g.vehdjk.com/Article/details/gkrvmcvpt.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gmyccwifh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gyisuvhsm.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gihhwfola.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gututobvu.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gwbztwnps.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gqoiuipsq.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gmmdzancp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gvylvbbxi.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gxeuhrllr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gjhhpirsj.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gkqchcftf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/giwtbctuu.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gmozomspy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gcrzajwje.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gxfvyrzal.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gjlodekkz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gruunotlq.sHtML


<!-- 参考信息 -->