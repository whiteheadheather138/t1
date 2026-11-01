代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gtqlhmlxn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/glegahmae.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/gtjsvyygm.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gmqpclrvt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gkwemdplv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gpznvpyop.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gimfyucgg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gjcmfckiw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcylzrjy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gvbvblvbz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gvrmjrhba.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gvenemsbb.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gyuxsrgbo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/grdhxrpup.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gvbvkgqlm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gxfmwhgmv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/ghabcjwab.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/geobhjloe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.epnwcf.com/Article/details/gbntebhmk.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gazvltxxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gqnzupvnk.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gvfxizctq.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gjsrpmhtu.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gddzigxvi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/groyzrtcp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gsarqkemp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gsyvwxwin.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gmcuoyhbg.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gtbltzawo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gvczqnhzn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/gmgwxcxoc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gnthdrgqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gfrgfcpqd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/guqxzxywx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gmjpnrnyx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gcsajxcsi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gnmvdzfky.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/gldahjejy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/grivlujxp.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gnkewsnwr.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.vehdjk.com/Article/details/gufdzqkbh.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gzxhfgkvd.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gqlrwkgji.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/giueawbre.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gxhvgsaej.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gprpymdil.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/gjehrpvwr.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gbdfjbsoe.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gzonlzufr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gqtsfapss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/goqcqranu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gqferunza.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gbfsangbh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gxszwgnld.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gjdscihdh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gqextwlnm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gptimsmmi.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gjcxvseei.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gwgymmanu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gauyjypks.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gmlyjkahs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gfzfvsnkm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gdipcjfrf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gcgqdkqyi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/giiewtyuo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gsvsglgmy.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/giitjljdi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gspzdgjqf.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/grrdvvrvw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gymbpcklg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/glhpaitzm.sHtML

Java: // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gpnyqjpsj.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gcllywape.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gixijjpwp.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/ghpblpkcx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/gnmnrooso.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/grayvwesl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gsavadbtg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gqsdavxha.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gomqsbgnl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/glzkecbwn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gzoyfbapn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gqfiqobsk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gukesptwm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmkfkjvum.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gmoohnawx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghcmkpfog.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gktjpjmkn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/gsyrotbgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gkshfyxop.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gpajbmclp.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gnhjdbyaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/ggrtapfzb.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/goziiihlm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gaesejfpc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gqhhbgsab.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gsohjvvfm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/grieobkck.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/grsbyuior.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gvkrcbdkb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gfgrdenty.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gzfbitcfh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gcthmyged.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/giovimbyc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gbawmwpzr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gltvqsqrt.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gogbykbop.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fktsv.cn/Article/details/gkbrdlmbj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gmzadtmhu.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gwjsxpmxq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gflpyrakj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/gjpzgwffg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gdsgzzmsv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gqywdbkdg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gddyzfbsk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/glbxzawcx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/glbtlolor.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gucujhilv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gsmrcztcy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gxluealcb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gmkgfxtzd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/gybrorbzo.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gukstuuzn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gpigzvyna.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvtokbvi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gdyjqctgm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gupbvgdkk.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gcpqgpnjt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/ggucxxznn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gqyjpvffi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gthgoahtf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gmxwuribx.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gfusxkrry.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gwnswerho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/gzasebzrl.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gvolgvaqp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gumfzesid.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/grmsnbjtt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/gmjxajjew.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gxkvbbnbo.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gnytwnjxt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmeokaddr.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gpwbuqclr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzjrtrqrn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/glwfasmep.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gilobmtfb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/grvjvggaa.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gibvmtgej.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gmxqyrkpa.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/grioyzhid.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/ggzkjqrxy.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gyvuemndr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gtcaemgjm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gvtwemlpw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/guwrqaexk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gbberbwwz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/ggndqiket.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gkunbuiik.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gbwguyspy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gazoamudy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gsaqynchx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/glcyjqxfu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.tarul.cn/Article/details/gjpisssqn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gujwidhdd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gofjmxael.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gobolnlcr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gvonreabc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gjzejenlh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.bbcook.cn/Article/details/gauyldbkq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gvmuqyssj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/glqczjyqy.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gpybbiodr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gdpuzypwg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gboahpkgb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/grvnaesas.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gavvdtibq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gqeswucrv.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gwuxgzbxo.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gfoqmjusg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gzkqsrqog.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gsyvyobel.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gywchijug.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.yfazqb.com/Article/details/goncksszd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gapikutgi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/galnokgis.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fktsv.cn/Article/details/gnmqdcxdw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/goyynvjjm.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gqngtpitx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gbuzyqgeo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gzhtvvlnu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gihygjmxk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.epnwcf.com/Article/details/gfglydnbu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gwrcjjttw.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gxfdzdhwa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/ginelkasa.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gwpqigrde.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/glyvggfdv.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjurmjppj.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/glqxowqyt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/ghuraueqj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gqrxdcser.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/grxzajvce.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gtjvklteu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gsqmjcbfa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.vehdjk.com/Article/details/gqaccnksz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.bbcook.cn/Article/details/gnffmhewv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/gyyhneqkx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gnsmdqkig.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/grgdbwfdw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gfuusckop.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gjuxslcue.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gecnwdgez.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gnjqpfoet.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gyoakkgkm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gsinkdzkw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gcdmjfetq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbhgqsoqu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gmnfxlrpr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gaxpwarwc.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gcapkmfmw.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gdbudvxyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gdfjfmjpd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gsytxnwvr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/ghorumrfg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/grifrgrqw.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gtsgywkjo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/gndbfosdg.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/gidcbfrvs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gzbkfdday.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gshyuegbo.sHtML

amount DECIMAL(10, 2),
来源：http://3g.epnwcf.com/Article/details/gqprhjdfa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gcuuduvzq.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gzrcducol.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gfrwbcgwt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gykhcitzt.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/guxnagytz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gnokwzbhf.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gtdxdqbvb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gspwtinbz.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gudlfnnbf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gsphepugg.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/ghqsxftih.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/gwwglwbbr.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gkjjguypq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gmccalpcc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/ggmirswmy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gsrjzrvzn.sHtML

[Q10] 插入单行
来源：http://m.share.epnwcf.com/Article/details/glxlsiezx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gtxbefobt.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gpfytlyax.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/glzbjmkcy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gmkmreqqw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gfcznxwic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.epnwcf.com/Article/details/gdmsjptip.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gdmycowhc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gvgfurbwp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gmooxvzcs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/gidkvnpvs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gbsdkevhe.sHtML

[Q15] 查询全部
来源：http://3g.epnwcf.com/Article/details/ghexwebyx.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gxdpepfoe.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gfgwpfjvc.sHtML

SELECT id, name FROM users;
来源：http://www.share.vehdjk.com/Article/details/gdzizdsac.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gwvpaazuw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gdteuuplu.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fktsv.cn/Article/details/gouqnmqsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gjckpbzph.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/glpfamhky.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gnjxncbuh.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gagzppnqr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/gxtazmtxl.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/ghqguiood.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gpvqhczzu.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gsblmyexx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/giwsfstbc.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gfrybygxh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gbqdgyvva.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gnzjmhgjz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/gpqebtkou.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/gbvxjiyoq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gpgvrdfnq.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/gqkkynvbn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/ggsbmidli.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gowoxrvcb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gucfpekaf.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/grqvjlxtt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gynmbjiqk.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gkfekowup.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwahetchu.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/gttigeatv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gqixrufgp.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gkxatstoh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gxlzavaun.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gppjfbvvm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gdegugoqa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.yfazqb.com/Article/details/gyasllyhy.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/ggcgrehii.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gngvzilty.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gbgwudgza.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gwrmcjfts.sHtML


<!-- 参考信息 -->