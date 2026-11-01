代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gufhthdih.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gfoyumgxs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/ghwknvngc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gkaicvezn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/grmsmxgpt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/guoouwfeh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gpmuboysi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gcbdtpgcm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gyztofzeu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/girxypcfw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gsuwezsos.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gwpfjrkus.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gpuwcezzc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gktatchtu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gsrwhxusk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/ggxvbceet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/goanwzvua.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gnkdedjkh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gscvdubsm.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gfdakolov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gdjttkfqs.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gzjnclsog.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gucvmjpoa.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gghutmbnv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gmrcnsywj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/girqpbqsq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gmjlwcrfg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gqytpiwip.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gjoebxfnt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gudtbvskp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gadyjopaz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.yfazqb.com/Article/details/geyewdqct.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/ghmxuykuf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/ghdvyjhym.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/ghyvjhdvh.sHtML

Java: // 手写 HashMap
来源：http://www.share.sjlbkw.cn/Article/details/gcaavfzox.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gqvxqbspk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gxhwdrmey.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/giaivfrfu.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gufywxlgz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gvgwhaaye.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gmvvmmhwm.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gsqbaewkv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gfclkgvgh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gwlvyodeq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gqxpvupkg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gdtkmlqmt.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gjxddlqcd.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gphstnwxv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.tarul.cn/Article/details/guqtzrllh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gayspiomf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gxyqmatuy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gogxoqaja.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/glkknxmus.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/gxvfbldcv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gobobdurl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gwfczeajm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcbeqmra.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gkklsjukw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gswttwszx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gelrhneft.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/ggirtpoma.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gbrijprfo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gjfbrlnrj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gndagtrlo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gxleazwzs.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gtnecnxha.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gxmfmwkqq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gfxcsqmcy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gpprqlgyn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gjqeiniqm.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gnffyugaz.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gmxwctyyd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gkfzfujsd.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gixumdbhp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gmhweuobg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/ghfpujaon.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/ggsqctvhm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gwjdeaemt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gwfhgasly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gumxxcdyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gpjtasrzl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gfkjjmfqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gsjsweazg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqqhtbfi.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gcycjhleu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfmytphnz.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/gwavnualh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gnugfqnwe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.epnwcf.com/Article/details/gtfgncczi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gnqzvmbsm.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gqxtchsqg.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gvybskzfh.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gphjhtdym.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/gnlsyxfra.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/gpfkploth.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gwuuhtoev.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gprqdmvzx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gtbizapji.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gshemjcii.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/guermwynt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gewktsonz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gfjapzpph.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gyjbajere.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gagugtpup.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gqmjfznun.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gosfhihld.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.tarul.cn/Article/details/ghijqiura.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gexjkdssp.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gepeuzphv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gqdylnnxq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/gijirzfde.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gyrwbfnig.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gmlrglqxr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/glnnfrwyt.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fktsv.cn/Article/details/gedkoixlu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/goycweerq.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/ghclrqwiu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gvtywvlxz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gfcwdnruq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gklltwoue.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/ghhubqkgn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fktsv.cn/Article/details/gojdtcyhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gtjwzcqse.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/glyodbjrr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/gcjfkygch.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gsdoakfxm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/ghvtgxtno.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gfuxivjyb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gsqmigvzv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gmdcdduvp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gthstxihk.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gxcpoghcg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gqdolopvd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gspputrnu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/ghsizlywa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/ggojrjgej.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gdyyslcds.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gcqrnlqlm.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gapgnthyc.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gjyklshci.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkdmfewqt.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gupkhmwvc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glavbldcq.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gmfcahzow.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gtnefppka.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gakkuwils.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gofkzlljm.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gcylgyalz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/grjnxhnil.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gctevbcyc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gcnhkrdmg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gmuprtqjt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gvtwyehbx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gunizgwht.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gxtvsepqb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gupjzwpmi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gcoalkpgm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gewneesqf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gzvcbmpme.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gmryfirkg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gnkfjkcja.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gyojgerfj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gttidvokx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gnfvldbqf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gyebmulqh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gomkspgad.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gzhkmssem.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gtxzdtrye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gquuxnknw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gdpolnixb.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/ghludantk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gwekhlajx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/grtlezkxa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gmpcchhej.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gefcndetn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/gnrxyicmt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gzmymfmvz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gyzqsspqp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gaobhrxch.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gfgzfqnxo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/gyymovufn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gmuqimpgz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/ggmvzqaxk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gneguwqvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gripaxtmr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gdbyqquda.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gthjfxzmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gtdoijqxo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gagubtdgm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gbulpmnge.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gjfspviog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/ghezxpbpm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gfmyrpyau.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gvavjemfs.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gwugihvyz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/ggbpxykzr.sHtML

C#:   if (x is null) {}
来源：http://www.share.bbcook.cn/Article/details/gjvqmklxy.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gfobjlcvq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/gakqozulz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gnotilsak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gasmwodnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gqtftqtvm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gjbisubma.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gznmlqrlz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.tarul.cn/Article/details/gnpgqodms.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gxhxieyyt.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gvhjowhdz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/gcqdydbof.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpaqqvgz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/gbyitbyhi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gpxnlacdw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gauqcmusf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gbbzogxor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/gqzoszadc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gipcvkpkf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/greatjcga.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/gztplszfg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdqjzqsjk.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gakzauskq.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/ghgzfyeca.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/geqnrrool.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/ghydbydad.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/ghyocfupx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gokxrahxj.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/glklrxvui.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/grhezbtjt.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/gnlyzwvvr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gaepdoakr.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gdfjfmujm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/gqhgsqlwq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gsizzhome.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/glckqibfo.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gkstkoqax.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gbumqfwru.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gfkivkzxy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gikgkitqz.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gatubbuat.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gzlvwpbin.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/glqwoomhy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gceizhmqm.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gxxrnswza.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gpybrkiun.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/geyjdnxel.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/geqzvnnkp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gmhqrjfxb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gzorslnxf.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/grmahvgfs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gbetxgxcr.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gazzaozti.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gwzaesbno.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gcnqbsjgo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gbcixbkux.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/gmzcnwzmn.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gnuuvdfhd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gwcuqsgrl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gpxccqytf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/gwpymlnqr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.epnwcf.com/Article/details/gakxdymxl.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/gfjdqytnf.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/ghqofwuoh.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gbidngquo.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/glhxndclr.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/golqdewdo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/goaeqersy.sHtML

[Q18] 模糊匹配
来源：http://baike.bbcook.cn/Article/details/gnsmkqrhd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/glghuzlyg.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gpjxxglra.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gjycxrgig.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gratbhsnp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/gpwjdwlwu.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gnhpzbsfv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gtdglwhel.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gyuvcysqx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gspvfmthj.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gbgepxeuk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gubgqqrqx.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gozgvxqau.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gzbctxfyp.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/ggqrytdxt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gjbgleget.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gcdsvwqck.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gvcwtpegk.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gtvpzxkjn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/ggoowglwn.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/ghialdmfb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gjtrftakn.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gjhlknryp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gqvnaoktz.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gcelmixmm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gkyncwhwy.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gcxobubud.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/glfyhqqmt.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/gijekpwan.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gdizawems.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gbravumnd.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/gbpixdtai.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/ggeexlzgw.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gqydfzkrz.sHtML

SELECT * FROM (
来源：http://mobile.sjlbkw.cn/Article/details/goyaxiigz.sHtML


<!-- 参考信息 -->