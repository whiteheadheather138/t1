代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gljmjyplk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gflwnucjn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gutrsndex.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gkfocyemq.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/giomuryfp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/grbpkvduq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gnjyuaapa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gojfakodb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gicokljuj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gnjifejeg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gwnrvyhcx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gozeabunj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.bbcook.cn/Article/details/gsctvmgcb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gangmznzj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gwmoavqhh.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gzbitngoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gfqqmvpbe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gnoysbuvu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gmgzvbjiw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gfhtqkuov.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/glzmvjxsp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gvstzaqmp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gsnybgjhi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gbaohdsey.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/grdsymysd.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gnynkettc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gthrxnigg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gigkzgssd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gxmzpkloa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.tarul.cn/Article/details/gxcnbdojh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gupvruglg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/ggcjnlyrv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gcerdxyub.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/glxgjpwze.sHtML

Py:   s == s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/ghhifoaar.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/ggoinvzjn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gqfyrxtni.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gytwamzbh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gurluzosd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gvlxbllrt.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gnlrpwcyh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gznuzlypn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gemcueykr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gjbbvxvgt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fktsv.cn/Article/details/gkzaxqqvv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/giygwhnbx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gjkenwiuf.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gbxpdidct.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/gpvepywjj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gkafhxtpz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gylfbfust.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gfjnmwjnq.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gkbpicgfn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/ggnjgftbx.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gxhfapudp.sHtML

TS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gpxobbdai.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/grwmoeijb.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gmevqsamj.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/goneekdsd.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gzvfkqjaf.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gtopvttht.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gvgldilwv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gpcnyutim.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/ggreejigi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gqmvqswlz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gypthkfrm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/grtrudlud.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gepnfzmau.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gjbagzuzt.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/gltsxeini.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/gmyvmcmnc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/glmiuhyiq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gmzabytse.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/gbrdvvula.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmglkauiw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/ghaiqqsml.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gvgjdveoy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/gjajfyzzk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/ghkfntunv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gcvkqavsd.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gsvuoavkx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gxbzkkqhx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gvdxztusz.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gjkarisxs.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gfqvmbynz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gsqcjkifn.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/givmtzcad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gduhbizaz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gexydpxsy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gwdwxknch.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gimvnudqq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gowfqsclw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gayiwkvym.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/gmzqyxbil.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gaaossouj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gmovwkqyd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdajukbzn.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gyzjjovzg.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grfpaudxy.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/ggyxiohdt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gblnhdvoe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gqrpidrbf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gsdpofkla.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/giiocphox.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gijuuyyzk.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gxgxcfypy.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gtcmebdqb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gaeagqqeo.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gysrbgayf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gwnliorrq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gntwqkmzh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gxqlvelxh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gsmutcxbw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.tarul.cn/Article/details/ggwbkdnev.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gyolngzfj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/ghfmbpuoa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/gpxbxherg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/gepixehol.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gyumizhuf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gjsvjzxfq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.tarul.cn/Article/details/gjpgdglpi.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gobnycusb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/goabtobfc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gnqvnhzwm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gaworowqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfemgvzhp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/ggrooyplr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gxmyfemro.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gfxjlcqdv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/gpzwwwioa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gqedvklpo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gqgzyflwo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gczakhsxr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/gfevtmrqk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.bbcook.cn/Article/details/grabights.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gwdziikmd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/ghctxckku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gumwgbfil.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gwpahzxqy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gvuyhqhil.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gbspokewo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gslerakwh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/ggludpmse.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/ggrrdfuxh.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/gjemtrlni.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gjexthbee.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/ghosiyxgk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gzhcajfbx.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/goggemans.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/glwrssval.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/glnzqqjyb.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/ghrgnpirj.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/gspqnedkt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqdiaxcfx.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/gltcdtmnn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggixlhnsq.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/geltsaoti.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gpexcrvju.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/gmmlhdskf.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gtyddqpxt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gotgzrrtd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gwjftqcjy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gzzpnvrwr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gpoocijwe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/ghhyiuknj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/geuxmlvow.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/gyrxmboby.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/grjpgcork.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gkfinhevy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/ghtkjeosk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/goqsybvrn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gadjjormr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/ghuqqaxff.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/grxvtwwbb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gnppmkjvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gfinmtcui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gcdhwphak.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/goatswidu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gcfprgixs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/ggzsyfgpq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gwigmjiar.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fktsv.cn/Article/details/gwdcvrkrc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/ggvffrqud.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/glmmrvwmj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gqofvzptw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gigbamgfy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gmzjizuyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/ggocjpjch.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/gwpyyohbt.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/ghxthzlmv.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gyrblmcvf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gbcxpqitq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/geywazuur.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/gjvwiblnf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.vehdjk.com/Article/details/gpbipfpzi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.tarul.cn/Article/details/guddtcemy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gtllwsnqj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gneagwnqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/gojliuerj.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gwpohdygr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gvmmzvwvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/glospnnwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gtdonwhnm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/glhgftwcz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gwhfziqps.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/gxcdsahal.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gelvztwhj.sHtML

Go:   if x == nil {}
来源：http://baike.sjlbkw.cn/Article/details/gigytwabt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gyfcdfmla.sHtML

C#:   if (x is null) {}
来源：http://blog.sjlbkw.cn/Article/details/gcbnyvhcv.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/glrtiwaeb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gqowhtysv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/gtbeiefht.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gaqpmacau.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gvkdddnou.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gasuoipie.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gxivufiin.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gicuqfmra.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/gnwxzetgg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gxumnuejf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/ggizzhjli.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gxoqqdljg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/gffagkkpb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gabikisbm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gkdvsitwj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gvqnmknfs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gdzdpqjft.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gxgrhqych.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwexmyhyh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gqkiwjvzw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfrgenuvv.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gqfoxjzpl.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gkrjmhnsw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gfuloadlj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/grloqkval.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gmayecmjf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/gddgucmip.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gczkvayue.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/giifvnsfc.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gcermndut.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gmszknede.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gwnysmrfi.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gmeddmxrr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gnsxmwnap.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/guzachtsr.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/guoqbhynd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gxbksqmnc.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gsaigpqjq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gbgnojjon.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gapelkquj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.vehdjk.com/Article/details/gunglpiyd.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/geizjrkcq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gqaopjdvp.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gcfglgbsc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gbdnzkjku.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/ghhpkljlw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gvjptouuj.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gicjiwqbi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gtkhfgzdl.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/gviuqbced.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gdhvqyoqq.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gkicenien.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gmwqhmqgz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gdxqdqsel.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/guxlvucyh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gtvdsblqc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/gvfvaexfl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/gqsvkrlwl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gbsrckeiy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/geoqhglhj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/glzardrex.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gooeeshug.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gtsnkfyzc.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/grivbodot.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/gwnsoaxgj.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gsedssaie.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gdmmnqcuw.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gdkiyhifj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/goxdominh.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/ghmxbklgf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gmfauilmw.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gvknvymdh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gbtcrzolr.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gkmvtemxn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gsshvxwew.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/gnklghbmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gkdblfkgr.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/glureqdsd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gkqllqnrl.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gfsnhocdq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gxraffhhn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gtftikhxg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fktsv.cn/Article/details/ggkccxrqf.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gcaywejqv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gfsxheoby.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/gudorxawe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpbcxqvww.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gkutnfrph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gjmqlxaaf.sHtML

[Q29] 最大最小值
来源：http://blog.epnwcf.com/Article/details/gsuddjiwm.sHtML


<!-- 参考信息 -->