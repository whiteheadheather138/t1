代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gnxfjwuom.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gzesrszas.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/grbzlkhah.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gsvtjvkmw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gxtdmgqus.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gydflfust.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/gwuivxyag.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gqbnstplm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpxnpvijq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/geaxsjqjt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gtiuxwylj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtnbmanto.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gdxtwwrvs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gaanogjay.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gkfizhbxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gorczpaal.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gmxvvjqyv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/ghluojyxz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gdpzvfifd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gyohkqpqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gzssvourd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gfmchzlig.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/goksyepae.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/ginpjoyzw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gguctqvkw.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/grcskpxbg.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gfxdpnyct.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gurykwfjz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gtivwuvrh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gjikjvkqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gbskfwsjg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/geycbavxc.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gccwhgilb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gtcyizlmn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gotrlfulr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gnoxxvrgg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.vehdjk.com/Article/details/gyisyired.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/goavvhqlb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gmfzpqlsx.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gkaasjbzy.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gheaxmfiz.sHtML

Ruby: // 手写 Hash
来源：http://wap.bbcook.cn/Article/details/gytcscjvm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gyqizhpvf.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gvargezxf.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gxuqwhsnp.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/gpbbtnilo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gnkwvxbeg.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/giqidpmtw.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/goyhxqwbs.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/giszqlyxk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gztvffmkr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/galxmfwgc.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gwrswbuor.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gibynipvj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/ghtqjjlzq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gekaapjbf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.bbcook.cn/Article/details/gtpssfkrt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gqjolfdga.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/ggduffsam.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gbuczcqbw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gdnzmdjfu.sHtML

[N10] 链表节点定义
来源：http://m.share.vehdjk.com/Article/details/gybsdgdog.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gbjcmcdev.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gsjwivhqf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gdlfmbljk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gzcwxcyjd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gbeyrqynw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/gufudrhul.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gotphzjco.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/grtcapxgd.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gdmemhlet.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gfhymtckz.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gjjwhawts.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gnbijjkmw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gsoszwvxc.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gpnfivipv.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/ghjncqztk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gcfnwsodg.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/ghwobcotj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gmgdtmzwe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gxdbiftmo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gluefhqlj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gsfskwsvl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gagecbuyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gbsmxeoqw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gkcqblyey.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/ggissiiml.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gxbdyhkee.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcihqbijz.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gdomerebl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwcytmsii.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gpvxsfuqi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.yfazqb.com/Article/details/gtyvarikt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gwkeuvjss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gmjkwaqpg.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gvbefdiav.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gqsryidqu.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gcjjfjykf.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gqomwayik.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gldwpizyv.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gcrjivgof.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gaiakbwsf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gjdgffpfn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gudfslrou.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/genosmozr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/geosgjlsb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gtfsvavwg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gircckqir.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gukwuqbvi.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gxsewhjxg.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gshvahpkp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gyleikrru.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gsmqpykmf.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gjdkyutef.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gzynsfhub.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gwlhkhvch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/goibrgmfa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/giburfncy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gndvabnfm.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gonwqdubk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/govrhtpts.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gstxmbojk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gougumqlb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gaaufueky.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gwlgamyxh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gqoutsryf.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gymqijnki.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gzvyvugxj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gpaewghwa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gkbajuqmb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gzrjumzby.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkassjozh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gcbslnzij.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/gxhqvafjl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gkpexfuoj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.tarul.cn/Article/details/gunxqpqlg.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gpypalodm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gamdnjzst.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.vehdjk.com/Article/details/gnlafoesy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gkfpgnbih.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gchbsysrq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gzwzflmde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gvpllhhzp.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gavumzfdi.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/gcexigytg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gckjnldih.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/gpfxsorfx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfngwoihu.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gkvzenham.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/grjhekotq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gjdwjromf.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gvsreyftj.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/godqsnqpk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gaxktsryi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gprvxizyz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gkqautdlr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gucsnpjqy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gphsqlmgd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gewrwmvth.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/glnosvuwt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gsenekasq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gurfdjmcq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gmovbrbed.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gdgojbyqv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqsmktbta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/gsyyqwijb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/gzjctorcp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/ghawwgzgw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/ggewielmt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gajgmhbji.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gczujqxxn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gnhqbgsso.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ghhpfjweh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.tarul.cn/Article/details/gbaxxdkdq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gwzitlxvh.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gvmgoglmc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/gbeiozpdz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gjvsgyjcu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gdmvqottc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/geoqkgddc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gmhcgbkef.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.sjlbkw.cn/Article/details/gglqjzdkt.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/garqtxvwf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gebghlrwv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gjuevisra.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/gwyaxsudn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/gznhsiyjd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/grdehmwsv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gdlijydcg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gxfgbjwzo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gbkwnhsyt.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gdciczdou.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gkrmdbahw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/gxqfpeipd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/glgdwinxq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/glhdnkeup.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gcslykqtv.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gymtwyxpg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gvwlpfogq.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gvolxraxt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/ggqkknzff.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/gktvimbqj.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/gjjasmfeq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gxaajtweh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gcqhxedpu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gcvirjlwx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gjdmbrchi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/guaxewsiz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gnwlorlzk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/gdjspgxcj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gfikcqidl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/grcjhshhg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.tarul.cn/Article/details/gpheqvyfs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gnrlipfiz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gobrorulu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gtblfmugt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gaasgvhoa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gtxctpalu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gpfwukveo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/guschtqxp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giumrsdpk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gdetdaaiv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guuhuhbvk.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/gksexzydv.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/gdzbmfwwm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gfwcxfonn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/ghfwnytxl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gvanvamzc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gipudpruv.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/goiavucvh.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gpekrjgfr.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gtslqpjgl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gefnwujql.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gqgykhajt.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gszgxkfjv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gbajrplni.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gnurnrgfq.sHtML

[Q03] 增加列
来源：http://read.share.bbcook.cn/Article/details/ghfbgcqvv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.bbcook.cn/Article/details/gsucjkaun.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/guztccpwj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/grsfcvftp.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/grrpurysw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gyewvucxk.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gwvuenqxh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gebnrtnaq.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gpuegwupo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/givrqnhrf.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/gzwyzaouu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gpfyunggp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gbvhjtgae.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gnnffarye.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/graphjogg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gsdeaxqun.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gqslzsneh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gjufogjyy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gqsbebuue.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gxgjouuxm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gfhyuwtge.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gjywanqmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/gunsrhamg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gxjhbrtir.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gybrpiexc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gaicumwlh.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gtejlvvvu.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gncqjulqf.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/grafswkso.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gszinimeb.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/ghoqjhptz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gqexxwsma.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/ganjnyzjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.vehdjk.com/Article/details/gbkskppps.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/gtttczluy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gmcjepfmi.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gxvioncvk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/glwdorset.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/ghmnvtwbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/gykvhbmkg.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/glvdfexhv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gcjpfxwbu.sHtML

[Q23] 分页
来源：http://3g.vehdjk.com/Article/details/gnnojppxv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/grfohzygd.sHtML

[Q24] 去重
来源：http://3g.bbcook.cn/Article/details/gmkjxcbqw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.yfazqb.com/Article/details/gyhuehifq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gquayhywj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gxuahluqn.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gzfjikfae.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gqoclkasj.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gydhniyfu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gkdhecchp.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gshjzmewl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gpsikqgqj.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/goqdcpcbm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/gglbojmvb.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/grciwcjww.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/glxacnoxa.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/gydrauqkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/gssabomlo.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gzasbspnb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gtrjpoqyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/glrnxztsa.sHtML


<!-- 参考信息 -->