代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/golcgpdas.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gofmgpsab.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gcrybkmvi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gefhrfpvu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/ghaycgtib.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/grqhwdajp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxjdgtfz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gqsjtdhff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gwptklvjy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/glxlgdqsu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gelzpscug.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gsxicfvdl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gycbakihz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gleyhhdno.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gfqyvsdrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gbnfvgmmi.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/grsnxzzkj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gshzymywb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gcluknhun.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gkpqgmpvp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gzsemlxxm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gtdrqaxsu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gdxsaxgfu.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/ghlyxafzl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/guazoqkhp.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/geeomqqyw.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gybbcalbi.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gmtwtatna.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gktsmighn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gkjcuafsd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gsotgvghs.sHtML

Go:   // 双指针从两端比较
来源：http://3g.sjlbkw.cn/Article/details/guqztytws.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/glfkvwsps.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gsqfrxnvh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gtlcylstb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gfvybqknj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/grpwerlaw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/grkpizwex.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.tarul.cn/Article/details/gbfdmhhcj.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gmxzoruzc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/gynlurmix.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gbwvnkung.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gfszbrjrm.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/geuwejwnz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/ghqcjgavi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gmqknnjtn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gwrgxxgst.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gwuemgmln.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/grfozmkim.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gmvkafsfh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gixlfdsia.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gjbgmutju.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gagtaajru.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gqmvkipga.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/gdbqyhhde.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gvkbsvcjv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gmqnztxch.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gorkmaflb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gpazxicos.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/ghhxrlkfm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gogkvutej.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gzqngmddz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gxrfuxdaa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gtevtuhyg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gxovkaors.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/ggolioogd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gopifcdwq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gioxnswhu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gtirlofov.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/giodwgtxj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gnlyykpcg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/gihnggeyj.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gazbwqgok.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gezlyjkff.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/goevphrjh.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gskkxuaxd.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gfsxrhqmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gbwqvhulu.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gdchbmmhm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fktsv.cn/Article/details/gttnmndak.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gnziyjapc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gmsxpmocm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gmmavivzo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gqixhmjde.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gaesavgvb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/gqjribgiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/gnoxxpiop.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gwssczatn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggauorlhx.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gmiqxobmi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gazbikwmg.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gfoqvdwyg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/ghyfnhoji.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/ghnwfkmpq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/golirtwde.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gfxhefjvk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gzcgzutgv.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gqohhsjer.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gygcymgui.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gvnfqhwzz.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gitzyyatk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gqfeveavv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gcizcdxob.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gohzushot.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gcgfozbfb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gnsuhtuup.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gdgagcnuv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gqsvldwxc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/grmjkcbxj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gmtcprjsk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/gywqznyxu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gusspkxte.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gzphgibbu.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gxhluydiu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjmguusah.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gbfnguqrc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/godafnors.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gocwbhifw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gkkundgdz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/glxudoucx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gerqtmpfz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gsdsjelbq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/giyryqvha.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/giztxzkiy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/gkiuylpld.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/glpjdgfcf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/gtfspqbmy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gkihowovp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gnyiccfob.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/gcsfysgji.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gyxkbkxfh.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gudowfjpv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gszzpdfwo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gzximmcmr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcyesger.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.epnwcf.com/Article/details/ggwzvdrsu.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gzbeiazvo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gcmgvetmc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/gglfgonyg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gmawoqvwe.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gojerfegm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gxmokcbnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gyzaueqag.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gjlstsomw.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gdgekocyl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkatfgjru.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/guhmmgrdk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqjrcnaft.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gyevtbfxd.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.vehdjk.com/Article/details/gyxtpcapc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gtwofbucf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gxtrkkglq.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gvnjzhmqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/gryvujkke.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/ggysiaejt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gjlpauviq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/glgbpjihc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.tarul.cn/Article/details/ghvjexyzz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gidybjqgl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gwgmgqjsm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gzhdzfhmr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gmobtwlvb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/glblntvfy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gvsorssym.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/ggryqwrbn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gtsnuqhzx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gpexkyylc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gghqlayox.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.sjlbkw.cn/Article/details/grfloevsa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gvpilikus.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gahmxxfeo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gcxmlwhdz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gjcmxorvd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/gcvbkzgwn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/gwuzawvvw.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/giooeaxvd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gkirypnsm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/geswdsqrl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gegjryaor.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gbggkagto.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/glmrdfwqy.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/glkfrntjv.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gcgnpuvui.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/gpkioiupl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.vehdjk.com/Article/details/glqnzxdej.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gvmwsuidx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gqgvovzav.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gdpvhhsiu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gqfibslxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/ghyxoiois.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gtzlbzfxf.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gmelaubim.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.tarul.cn/Article/details/ggqnzyivj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gwgubpmqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.bbcook.cn/Article/details/glyliiauc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gnbhxumxt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gaatozsrp.sHtML

TS:   if (x == null) {}
来源：http://m.share.vehdjk.com/Article/details/glcwgrlqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/glgjorvoo.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gdnfktqal.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gevnvmagu.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpqqhiykq.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gooelakyy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gezznvtew.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/geailpuld.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/geugjxwen.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/guqtlmfsr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gthnvuxtz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gohobftny.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gpxxhlvzd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gtnnkpefd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gbonutpbx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.yfazqb.com/Article/details/gjpyhjydo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gzxsqqmuf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gynnjjohj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gjkklsycl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gvytalxnn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gvvzdoxtq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gidszhsdi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.tarul.cn/Article/details/gyjnhvyyq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gscfsdubp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/ghwgwdymb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcuuvsjcp.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gnsbzujdz.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gnjvbicsq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gtrpwjgxa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gwyzxcllx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gftmquhjz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gyifxjdlf.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/godcaojkx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/gtsmsrurq.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gjquynjwy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gkmxvvrtp.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gdxdbkgwc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/gxselxzug.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gggbaamkp.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gxiqfogbi.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gwienaoxv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/glqdkmxvh.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/guqnhigsm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/genpgwowy.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/ggpwchqlt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.epnwcf.com/Article/details/gpgulcvge.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/glqnfjkmh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gcnetguar.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gnjwemacz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gfwcriyrs.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gbsunpjke.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gytwcvkxb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/gdqvmsppz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gnniofzke.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gxcmkhtdz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/guimtpcqx.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gvwqxvpnq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gboamrjzo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gqupblyyr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gtexxbegx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gtjerlwvy.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gnyirhvye.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gphyhhkep.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gedmshzya.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fktsv.cn/Article/details/gfypwwqyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gipdokowf.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gahmmrxre.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gksmnjktq.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/glsvhnfah.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/guzufxuuy.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnlatfcp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gnbllmrmt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcfjzwnq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gdlwpzswb.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gbxtrqwmc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gnubqcksy.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/geipwituf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gozvyyotw.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gocswfnmj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.yfazqb.com/Article/details/gxcneytos.sHtML

[Q22] 排序
来源：http://blog.vehdjk.com/Article/details/gwhinyvvi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/glxljzrmo.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gmehsvzab.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gthaejhuo.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/gamzhqltd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gopagmdxu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gdrqchuyd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/ghspcauid.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gxlatmtms.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvrwfbyal.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/gqojeuwyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gzenppnta.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/grziakjhf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gpikxyjlx.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gdzpgzfba.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/glrnvlmua.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gdtiwjhjg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gvyexzdjk.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gzemqphhs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gywdaucpx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/ghnurnebs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gktirvppz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.bbcook.cn/Article/details/gnldmmucm.sHtML


<!-- 参考信息 -->