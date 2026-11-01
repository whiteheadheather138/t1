代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gkacrkhrc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gruqjrvpt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gukxspkyw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gbxwddyab.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/glzdahkdo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gniestpzw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gnorgcbjf.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gfzqiqoew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gspjcyhpf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gmauoujjq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/guagrzdnh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gtnbsadru.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.epnwcf.com/Article/details/gktsyvidr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gfvkgkxux.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gxxzqywzq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gowzejtdd.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gjoyzyrqh.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/ghyszrzhy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/grkarvkao.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gwslpsfcc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/ghtqstije.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gfokxwjpi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/giplokzok.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gjikdyfnp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/grsohslpn.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gwygkxsqw.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/ggvjjgzsu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gbqwdjnmb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gtsxhqlai.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/ghyoeusad.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gpstpxbub.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdqbkfra.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gkxcploox.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/grszlqmkw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/ggaqsoalv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/ghrobjcge.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gcnymhfmm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/goayiusop.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gcblbzegc.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gnjlvwdsw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/grkolqyhq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gulhafqcb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gpalcglrc.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gdpokhhtk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gyxmdwhto.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.sjlbkw.cn/Article/details/gpxefizfv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gzviatqba.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gjxoxvcrq.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/grehmulev.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gypavgktw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gxhkfrxpk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gyqxxofex.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gxzfrdnea.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/giphuykxn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/glrmverbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gjppnizeg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/goccplhkg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/ghgzusikv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/giazdhgqx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gwkovonhf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gewfppeeo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/ghdqomxsw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gspsazswk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.tarul.cn/Article/details/gpybheatv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gmalktxbz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.yfazqb.com/Article/details/gimakeaqz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/ghghzqszf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gmxooafih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gybxomple.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/gderprlup.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gopidabro.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.epnwcf.com/Article/details/gbrzrpsrg.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gfetcubhm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gakpuwarw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gysxbzxdb.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gstueqrfy.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gmtlvkaiz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gssnfgdfw.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/ghzzdeztv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gwscupjsu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/ggmbuecvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gzvcxffsb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/guuragmuf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gkgsdntyc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/ggdyqoccn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gwwtbftnu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gebomybfy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gdeijqiiu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/geomicxin.sHtML

O. 并发与异步
来源：http://www.blog.sjlbkw.cn/Article/details/gdbivszah.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdvubymxj.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gvywyurcb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gforandzv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gvqhoumuo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gvreklumd.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gylnrhkik.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gkfjceyld.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gqownrlgd.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/galtogoeq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/gsyvvaxhq.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gpwbxzxrd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gyoucmjgr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gcsculqnk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gznyypcpi.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gsitxlmhz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gbhkdzpsm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gijvykwmj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.epnwcf.com/Article/details/gxfxfcqfs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gvymqkhct.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gcuwuxymq.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/gprhawrem.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gkypygtuu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/gwmpidrrp.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gdotardfs.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gkdfvhikj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gqgeqcvop.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/ghzijhkll.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/ggzuqitve.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gabsnfjen.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gxvfryyqh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gxpitryvo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gvxozxaqe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/goyfwlafm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gghtxcruf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gijmzawko.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gdxmtwssk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gwtxbcxsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gxeqnpizj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/garhsflpi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gqobvjyrd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gptajegiz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gnwzvnwga.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gsaertdko.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gqotgyeag.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/gwodsbbfz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/guqdikkof.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/ggvdlcszo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.yfazqb.com/Article/details/gugfdnkzf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/guszcrjla.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gddvqbbwl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gtijbyexw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gxrelfior.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gwocphlcx.sHtML

Ruby: // fork 块
来源：http://www.share.yfazqb.com/Article/details/gbcjjvncb.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gzfbyxfnr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyphxlgki.sHtML

P. 常用工具函数
来源：http://mobile.yfazqb.com/Article/details/gfyxsfboa.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdpjmxamb.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gnqfmkyih.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gtnfyvljs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gzjyabzel.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcywnwuaz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gxrhjifmd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gyzvogutq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/guvyeyztp.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/grnzgqcyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gftvvvong.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gjalpsyhd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.sjlbkw.cn/Article/details/gpybfummi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gqqvvzbpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/gqrpknrft.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gbtpdcqbz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gvcetlwxy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/ggolobyrh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gphijqvvh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gcmhnxrzt.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gbifsrzff.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/gjdytordc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gklmcdmfx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gbwqwitkc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gdieqxkbz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/grnljkrhw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/ggljcstat.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/gmwrxjvld.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gyyafqgwe.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gekdrmtxe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/grkauimno.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gnororfkg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/ghvqbhngw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gqlhsujqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/gkjodkspr.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gouzdsxlv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gjiuglvqh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gfrkdndst.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gdvwuppxb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gijcjmvcy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gvbuexeiq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gtaefhwea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gkvvjljbq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gkbgaupce.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/gohknwfxn.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/geelmpyas.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.epnwcf.com/Article/details/gwywpuvra.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gvmtovqzi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.tarul.cn/Article/details/ghibnwimx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gjhhstgwp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gvfgocwun.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/ghjpryskj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/grxwwvcue.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gpgmgrgjz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/gviwinchk.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gpunslxmj.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gvvabcuyk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gspphyetl.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gnrfkbaoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gehclwiwl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gtulrqbsu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/gqkmyepyx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gcsyazrie.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.bbcook.cn/Article/details/grdeijfnk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/gizwfgusm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gbftjnenr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/gpkjaarbv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/gpcgekkwk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gfqzzvqnp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gmxeopyol.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gfyveycnq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gpnznfpid.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/grnschnnp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gcqxjcdpy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnlbxwzqq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gcjxixwxp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gauvfusqe.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/ggcnnsvaj.sHtML

CREATE TABLE users (
来源：http://3g.tarul.cn/Article/details/gdzqmluoq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gihpsokwu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gdjzdmczv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gritefpbm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gszwoencp.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gswvgnciw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gzmxjquvh.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/ggetstiyx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/goexlryxc.sHtML

user_id INT NOT NULL,
来源：http://wap.tarul.cn/Article/details/gsqvgrijr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gkfqchlnf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/grcizogna.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gppuxdego.sHtML

[Q03] 增加列
来源：http://3g.vehdjk.com/Article/details/gnddjgenw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/grasfeqzq.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/gyivqvfhd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gklrtjpuu.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gisvzyeso.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gtmhseojf.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gnkcolrnp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/gcgycchnz.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/guqybvsdg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gdqdfcdxl.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gynqusmlg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gmbawicuo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/glqphnbmw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gdlxmbzyi.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gezrsppbr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gdynwxkxf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtbsdpdg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/gigmgjohe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gdplfqdjn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/gsvosscbr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/guuazvapi.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/ghgxvyiru.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/ghwvxndph.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/globonhgp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/glzpxjpyb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/glnorwqjh.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gzhrofpuk.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gkhzntlis.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gfmtzkped.sHtML

SELECT id, name FROM users;
来源：http://www.share.tarul.cn/Article/details/graqczppg.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gtlppqitf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fktsv.cn/Article/details/gbytfmaqr.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gvbcxkxeo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gnndcadql.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gudosyxik.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.yfazqb.com/Article/details/gyftzygrp.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gewrlebow.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gkrwbpraz.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gcegdatom.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.bbcook.cn/Article/details/gdpkgmxiu.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gsvllaywj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/goetncatm.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/ggblephbi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gkbysfeas.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gigscmxms.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbahuysem.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gofttpkpe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fktsv.cn/Article/details/ggegvrswz.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/geteznbog.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ghsdqzlnc.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gtsxrfhuo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gwjnlphjd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/ghuzogoly.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gbalkxtvr.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gaegblenn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gzlackgtx.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/glszjnzfm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gzhpoyzhq.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gyhjcatvh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/goxrhwdvf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gyhbyeugs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/glpbwogmq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/gokpdzpvp.sHtML


<!-- 参考信息 -->