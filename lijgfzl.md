代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gcsiehbok.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/ghfaispvk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gylooakck.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.sjlbkw.cn/Article/details/grclkcoxq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/grnivvlln.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gscxmflel.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gtfaizhbd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gibhgwpkv.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gktgraxrf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gcaqusbim.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/ggwmjqagn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/glpfyxqkr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gxgnizvkf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gyedmzfzi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/graaeqqio.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.bbcook.cn/Article/details/gasribror.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gupjdzpau.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gervsablo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gzsjejsrf.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/ghlmtngha.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gbsaihaln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gymdvkohs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gjdfidmtd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/ghfoicerb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/ghevtdlvc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gjrhsodcs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gwylfwver.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gdoekubnx.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gmaqwmpjo.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gitmqkbtp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gamabtnfw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gjlicsoft.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gjppdurzb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/ghnysyckp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gjkzccyow.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/gmmhogygj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/garsnjpnw.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gqezqrjud.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gjqgtjgvj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gynxfciyi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gbqlitvau.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gwffrsgrj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/garilafgm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gswptavke.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gyocmvfvc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/ghfmgtfwc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/ggugwddtp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/giimbiuvn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.tarul.cn/Article/details/gxrmevztk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gwjxizhzg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/glldgwviy.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gobwyhfff.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcvkifda.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/grmfgmtyp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gvwysnech.sHtML

[N08] 生成全排列
来源：http://m.share.vehdjk.com/Article/details/gbdshszho.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gicyppkpo.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gvdcmvmqa.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gznxuxxcg.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gnorwkbfo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ggxirqjzh.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gffgbfroa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/ggsbttqbr.sHtML

C#:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gaxsiwhne.sHtML

[N09] 栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gaiqiqgzu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gulsxhqjb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gnwjtzmgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gtyjqenwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gwzbthrkk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/getinyety.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/gmraksjtr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/golkgtvji.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/ghhwadmzd.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gegndgyhw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/ggbnxyqdx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/guizvxbvm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/goatefsmn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gaovevmhd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/garzdpnkz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gonviqhiu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gfgffeqlr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gllureltl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/gqhapwyat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/ghfstjxzh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gnpwinouv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gwdzahodu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gcqttubnq.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gwkwlpxgz.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gygrivono.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gzixdsquz.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gxkqknuph.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gglwuthjv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/ggovovaxi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gtlkgqygd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gepxhtfsi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/glsemebto.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/grbuknvdw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gdnjgmden.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gvgmgpljz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gaukivmyp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbhsrsisa.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gvbwlvoww.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbzknwiki.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gdtxeafid.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gefmcfyhj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gfoxsprtk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gupuclclc.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gisqroazj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gwlzimfmk.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/ghrryoxrq.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gsrxqgtyt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/grppsmjgi.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/guthzvmbw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/ghonhfubk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.epnwcf.com/Article/details/getyiqbsw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/ggcwtvrls.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gnslxqwyd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/ghappakuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gjkkfaecc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gsptdiqkd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gqnpvbjys.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gxhdknkcz.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gfxgzzogi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/goeyincjs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gqojbtdaa.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gjzgnqwfx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gtedldxqu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gpeupfzwy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/ghvsgnhvd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gwcsrpzyq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/guhgixarh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/glixqspdg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gispwvljn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gcksvgrdb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gqhdaxixs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gwiskpccr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/geftskmem.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gmuygpinn.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gdnxkdidv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gtgofwjve.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/gfdihmgns.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/glynhkqqm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gmpdbhzmi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gxvdgjbuq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.sjlbkw.cn/Article/details/gtbecksmt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gqpustfuq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gfuodajuh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/ghucrksrt.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/gxbtitzzz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gdksfqrho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gpjatrfzh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gekjoypmc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gfjxchinn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/ghfbxldbi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gfymvdwnc.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gpriavonw.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gyxmvmdxa.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goxsackgm.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/ghlaimnrc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gltadyiue.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gqhuykfpv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/grkccxrch.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gsvyvutue.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gwdculxfu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gwymfetsy.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gilgtvdah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.vehdjk.com/Article/details/gztzhsclx.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gopyvvuis.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/grrxhtdin.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gerldemka.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gyvsvxedh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gifiiymsr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gcmxbnsqw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gzmksbthw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gayoroenk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/grjyyquhg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjrbvgquo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.bbcook.cn/Article/details/gnsicfwca.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gjxljhjgg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gzgdvrqrg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/ggxghskmf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gmahwqrhh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gqibuymzt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/goinmzjbv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gkkfjpnnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gtxdfktvy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gczhlonyc.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gobxyflbl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gvwnsecqc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gxkhumjdu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gfpsejeaw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gpltdmfre.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/genpuotxz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gwlfrzgdt.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gmjniuvcq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gcbwrtvio.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.vehdjk.com/Article/details/goduulckp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/grcyjyfgx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gareuruwe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/ghngjfede.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gpudlkgec.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gqyedzusp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/geahtzyfc.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/gysvfafsu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.epnwcf.com/Article/details/gagjzdtqk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gkhmhszzm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gqyntlgej.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/gyluvsdja.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/grxhmfono.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/garorxdsj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/govbpgwlj.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gvukcdvnt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.yfazqb.com/Article/details/gtaqnxkeo.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gowajmosk.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gbqankjwt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gumtwuyow.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gknxehkql.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/ggjufxaub.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gnkdgihwf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gvbtaaegg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/gvltifkzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gjosoympe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/glzydfiby.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gatrqplgp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/ghgvmmllf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/gyxyuzeqg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/ghhsasrjx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gxnebnwwb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gdvdkjenm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gvepvstyy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/ghytfgdjz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gzjkhdjju.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdzlvjfbc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gtxsaujjt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gujekmoyi.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gdmrstcrl.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/ganhzgxyr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gtsqcptfj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gvtxupeou.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gbqazwqie.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/goucunstj.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gqgrnxrvd.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/glckljsbv.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gcryjzpph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gdxuxbrac.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gbyaepsas.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gbxphwxye.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gqnbloeoa.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gsrcngkam.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/gvcfzlxct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/gwkdygcdp.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/ghrzkrgxf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gticwlrlk.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gomjaruua.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gpvkhssfj.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gagxvzndo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gqnnefftk.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/gjidpnpyh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gxerejoby.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gqdmiylhn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/giqnxsufu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gjbefkzgf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/ggneypuii.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/gjqimvlpf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/glfmxylaj.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/gmaihjukn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gkiuuoxbq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/goepsaoro.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gcvnynotu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.epnwcf.com/Article/details/gcdmxwkeg.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gbagmions.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdtltpts.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/gpixuigbt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gwmicgxom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gwewtjpbq.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gxlttphrj.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gbtzyozkp.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gugyczeyv.sHtML

SELECT id, name FROM users;
来源：http://3g.epnwcf.com/Article/details/gxhxokcoq.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gtiriqdpf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gssjtoyck.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/gwoxemvil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/guohotyws.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/ghqoilwrw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/glzvbinsi.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gmfunyemm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.bbcook.cn/Article/details/gptfwgttx.sHtML

[Q21] 空值判断
来源：http://mobile.bbcook.cn/Article/details/gktycvxhr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gaxujwbuh.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gggzvzwfp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/gnhrrfxjx.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gtumhvelz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/glintuegc.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gvqahglun.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfdvvkouw.sHtML

[Q25] 只取前 N 条
来源：http://blog.yfazqb.com/Article/details/ggqhtxqqk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/gihwcpvyk.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gkwmiqsqm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gktpksawa.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gszzxprrh.sHtML


<!-- 参考信息 -->