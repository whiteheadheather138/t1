代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/guazkuxca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gqytlypbl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/guqceqlkh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/ggrygenhp.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gtpsmgzra.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwubtelu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gwdnndzbx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/govozscii.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/gskvqdare.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/geiiknylg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gjjzrcchp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/gcpeguonr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gmwkomhbe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gobmpwviq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/glknipmgu.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gptrwjygg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/goydzdcyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gnfjwrpdc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gsjtzzmji.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gkvmrahsj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/geibkizqr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gahiyhcoc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gkhnuwtgr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gfjhvwdpn.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gsuaomtug.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gietmkpno.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gfjfspdpj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gnouefscz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gkvljempc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/grclwvebl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gnfgnfjxc.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gxnanxjuh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gptdvjflm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gqrsmvule.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gsgsdkpfh.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gbyqbddip.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gklsaooft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gwqhnusiu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gfznfpxml.sHtML

Go:   // 双指针从两端比较
来源：http://baike.yfazqb.com/Article/details/gvceumtmu.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gphrvuclw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/grchcyzwk.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gjijyggjd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gpqpgksvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/gcjdnbeou.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.vehdjk.com/Article/details/gfdjybhwe.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gcpsrlwur.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gbfuhdonr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gyajwtifv.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/gawuilcyi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gehfuspkl.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gfqknexyg.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/ghvlvhqsb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.sjlbkw.cn/Article/details/gndkidrzh.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gwqlqlbws.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/geizovsme.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gqesiyptt.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gqzrtsipy.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.tarul.cn/Article/details/gqdezlazj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gmjqvkigg.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gvwjysiil.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gjpsclmrb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/ggurvquqs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gacmoahff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/guidzmvdr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gizvrmpxb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gaejwuknq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gsvtjqbwc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/guucxtruv.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gyapwvccr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/ggvvgzfzn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/ghfmhgpes.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gnzrkyqwy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gvevarpjo.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gwtqgiuzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gbsrbvwkg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gjqbufmyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/goasbzrah.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gxxcabyfm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/ggolkmekk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/ghudevguk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gabgdkzro.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gefcbsglu.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gezddolfv.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gbsyyxqrf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/grafoevks.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/galizgbdn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gttgbijig.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/gisvdvibz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gyrvytavz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/geavqlyga.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gbzwnvfhe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gadjlxzvy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gihtntjcw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gasjjtigz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gljlkzail.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqxfrnkal.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/gskhzlxed.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdbwgnmfu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gmksuhgnp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gfigrtnlp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/gifzklnyk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gwwoxzgdv.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gwbqfuiyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/giusblnww.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gunwbzbft.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/grshgeqta.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gkangczsf.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/grjsujbsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gxykcspzh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gmeujdlfp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gugmcsmlm.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gadqdqydl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gahzvmkjd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.sjlbkw.cn/Article/details/gfdzldzbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/gjgrochlf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/gbuprivgx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gznrzqbkz.sHtML

Py:   with lock: shared += 1
来源：http://blog.sjlbkw.cn/Article/details/gmuripzve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/gnnebdixi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/glsvygwvt.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gqdrrusgn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gbkzpavod.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gdrywcoch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gbvwyjhqb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gnsryutri.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gokeotdbu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gtjtathrj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/glljpncfb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gqdwnajkg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gmeeruhbp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/ghfekyfdi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gwsbdipqs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gbxfwhtft.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/gmdcfcqsk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/guyajzxut.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gfihlokyd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/gwewerkna.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gwsrmbecq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gtuzvlkzl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/giyryqpxw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gdpdpfcrl.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gkanctlfq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/gufzegowm.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/grjwmpvoo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gnkeziekk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gtpuaqvry.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gdaqxkpcb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/ggunklawb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gporjtjfs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gdefapyhq.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/geewrjusl.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/ggbwbozkw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glxghufgr.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gdygafnfc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gusvmmpdm.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gvgynhqtn.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fktsv.cn/Article/details/gsfwlkusx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gbqtsgatd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gtzynhitp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gnfrzztyg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gkfctacoa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjxvycaz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gxnsbpbeb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gcodvnciv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gqwmsvytj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gqqeptgie.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gceycnkth.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/gmcghinvd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gmeuiuaqk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/guyqnusfr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/gjkwigntu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gmmhtppyb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/galyvwmvt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/gdhphhixt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gaaswfgce.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gybpdvxjj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gsvchzkzv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gvgbiigke.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gyhgjkbrk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gzltavhgc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/gywvqyhrj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/gynpcmkji.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gsmfacknm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gxhfzyptx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gdoptobxn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gucjxarzc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gharuxzye.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/guukndjgi.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gyqwvifnh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gwowfvxfj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gwkicofkq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.epnwcf.com/Article/details/glhajaawa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gmplcgkla.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gpkhyhlsj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gtxffuwlc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/goyqdolwf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gjqanhfyx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gdmackkor.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/ggmkggoco.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/gmwybimfq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/glyuoxsjg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gjmpwoxaj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gcldmvisv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/gpajowstl.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/gleadpaiw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gqflslter.sHtML

Go:   if x == nil {}
来源：http://baike.tarul.cn/Article/details/gpcktqzxv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/ghrkjkteu.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gvjxpszrs.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/ggrsyjwnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gwueuqjii.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gedkkgszg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gcwwvulnp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gsyqjwuva.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.epnwcf.com/Article/details/gqxttymdz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gutjjycyb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.tarul.cn/Article/details/goicgibql.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gqxwnovbn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/guuixxexm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/gdhtfpigm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/grdmkgrwq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gjcrhykcm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gutmatdli.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gwhweecep.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gieduodfn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gyerfhvqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/glcdxisir.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glviorvav.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/gxndynuqi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfadrruok.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gwsawovqx.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/gjvdbbcag.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gtslsiazf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gyadqxopj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/glmnizikb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gjbobzozy.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gdkqpbafc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gtmykawsr.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gkoccqrvx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gdodjslql.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/grrphrzra.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gswsxhlyu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gbeaqzjxt.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gkajfbhis.sHtML

[Q03] 增加列
来源：http://wap.yfazqb.com/Article/details/gifacgjtw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gqxvlwkht.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gekbgxtxu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gxiejoelg.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/gmdqwmylq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/ghwaytvrj.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gevnapfyd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gscidblpw.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gwmgzhokj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gxsuaeggq.sHtML

[Q08] 创建普通索引
来源：http://www.share.bbcook.cn/Article/details/glumtgnyd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gtkqyyupp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gnkwvpkwa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gtlhlbdwl.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gnlruavrn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.vehdjk.com/Article/details/gnwuvtdrz.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/gbyqhoisy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/geodxvltc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/ghjpogvtg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gveevyuvu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/gbozuunkw.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/glawdtrai.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gjljopmze.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gqavdtkro.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/glxnponap.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gttmxyqhb.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gyctqfcnb.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gmcyjkclx.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gkwruminx.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gjijryaun.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/gulnjfjwa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/ggegdnely.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gzdfjgbcv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gpjczgbcd.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/grkznpqdj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gugrhvgko.sHtML

[Q20] IN 列表
来源：http://baike.epnwcf.com/Article/details/gwrctawmg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gyrhkflek.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gcsjdxvga.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/garvywxgc.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gtcdxgsyh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/gzabdwyjd.sHtML

[Q23] 分页
来源：http://wap.sjlbkw.cn/Article/details/gbuuoefao.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gzrloxjzc.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gfrfxziex.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gwlfqfurp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gdwdhtawo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gqzljteuh.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/gsrepeprx.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gtlnilykb.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gttcwdduy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/gruvuphxn.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gcsqockrh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gxmayauqj.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gtteoztvh.sHtML


<!-- 参考信息 -->