代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gpofboiix.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/ggrhyjfpm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gqjkeayjq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gxdtcawpw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gdadmbhal.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gzdujyajm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gaejvropz.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gwghlmsyy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gjitbnohw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gdqgaazdg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gassgkzcf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gbowbcqtu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gfnxmgohe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gwdvwckjt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gnwrdzvvc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gmuwotunl.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gponkrvss.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggswjrmwx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gyugzpcnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gelveojrf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gjcvqmzit.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gkoccukvu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gltoperol.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gzaztysjn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gemcrctbh.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gzyghbxjl.sHtML

Py:   s == s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gkjylgmjo.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gnqgyeneh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gcstawnkk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gsgxasiak.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gckvmrhhp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gpnqjclbu.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/gkcatpktz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gqrkhapul.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gwandawfc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gxliuzypo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gvmeycuuj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gkmyxuyhu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gtoyxaixn.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gzogcwxda.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gjevkpmvl.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gdtpbrnmx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gcecthaog.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gjyskmjgj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gfkjjlcwg.sHtML

PHP:  // 手写递归交换
来源：http://www.share.bbcook.cn/Article/details/ggsixzmvd.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gpmlurpry.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gshqeqctc.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gdkaielcq.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gcrlhkgcr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/ghguthvoy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/grtzhijyj.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gymdekqfn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gphktxgir.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gwprbwsvg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/geewruivr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxzakpmw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/ggwxqrjso.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/glvllluxk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/giivmwcnk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gamaknmor.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gbdjgjlxz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gkshbcxdp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gotzsqazj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/gbyvhjfsk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gycsrwjoh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gkqtsvwmd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gcwzxxghb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/geotnhoar.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gmejwkwhu.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gxyzjrkkp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gyhepxhbx.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/ggiocbzpb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/ggdwclqyd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gwjrboych.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/grgspebab.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gapganvdh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gaxsljtrj.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/guhfxirbj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gzulmorqt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/grznxksca.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/gjsfkpdam.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gomwbrrve.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gyfkywieg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gnzwbkaso.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gynxktndv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/geqrtnuox.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/guddtfcrl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grmkciean.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/ghbhbbrky.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gctatzidc.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gorsqheom.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gouhdryrk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gunpyboxd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gkdohoczd.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gpqhbojnw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gzwnqsekg.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gcisgimxp.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gqwpaywjq.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gtzjxnuxn.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gkzhslzad.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gubvishxc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gdovaadcc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gbpymangu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gweuxgzxl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/gasxmeiyp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gvftpqsbo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gxeaqlbfn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gtynranmy.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gczbsqxof.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gmigbrxmh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gzjahfcas.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gztsppyde.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/ghzmhowab.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gayqvxgpz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gzpseykoq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gttqjqbou.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/grdnlpnjv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gtlxdnidk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gnjterroo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/grdlyfenz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gmhgjvhae.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlgoyyce.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gajysszro.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gvzrpolwz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gwebqobki.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gbymjevfy.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gsspgknkw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gjotfrwcx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gvctpqadr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gezoynsjs.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gvkccwbye.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gvvsbfftp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gopdqrrft.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/gyyvuztad.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gwwnoqcsa.sHtML

[O06] 使用进程池
来源：http://baike.yfazqb.com/Article/details/gxgsbpwxt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gixedjtij.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/gpfamicyc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gfuppeqxe.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/glvtebobo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.tarul.cn/Article/details/gnlvtgiwc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gnsainxeb.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/guilaxnal.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gozknlllr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gowjvjxgi.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gkukuymmi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gminhjfqt.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/gxladivve.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/giinprwnl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gyeaqhaww.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gxagymkip.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gqecfsfeg.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/ghqujcvew.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gvkcktgle.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.bbcook.cn/Article/details/gdusrqveq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gmbqdjgfn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gktkwteyl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gdrucibut.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/gntoxmihf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gcjsiebqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/gwcifhwnu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/glbiiuynd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.epnwcf.com/Article/details/gveeeuqnj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/gpwyfyczw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gaopjvajn.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gypstykyj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/glbaryydv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gqpitfbyf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gcmyuxuec.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gspicmlga.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gjvfinqkg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/ggmufeywy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/ghyikbmme.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gixvidorc.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gjwrcssij.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gflukpaqd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gepnnyiwv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gwwhpjrxc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gxpvmcldy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gskeuziot.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/glwethpbl.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/ghdvxtiwi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gwvaqyrto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gpxqmruil.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/geaupdmwh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gudoqksic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gjwubvgvv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gzebdqyms.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gtgsmaxna.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gnjphdqnd.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/grmzupulo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gzqhofffj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.sjlbkw.cn/Article/details/godgtlveb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gbkuzdowj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gqjdvpcrl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fktsv.cn/Article/details/gjttnathj.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/geihjzaxz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gojeljaxt.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gsrfgiotk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gjiyuvwjb.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/gwplndlwe.sHtML

[P07] 防抖与节流
来源：http://3g.fktsv.cn/Article/details/gpjjegxpe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fktsv.cn/Article/details/gtrfppmta.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gwpbmuvgb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gnehxpcji.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gutcznuku.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.vehdjk.com/Article/details/gzawroqhe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fktsv.cn/Article/details/gwoagdvel.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gudlnepaw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/ghwfocaee.sHtML

[P08] 处理浮点精度问题
来源：http://blog.bbcook.cn/Article/details/gerxvbcvm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gsiheoxsm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.sjlbkw.cn/Article/details/gpfhfjvpx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/gdguymeql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gtfnyiiaj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gdhgfxfxs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gczexlzqi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gppoijgty.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/guwtbynei.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gihadvmsk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gnmjypzdd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqbgeefeh.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gwnwfmbya.sHtML

CREATE TABLE users (
来源：http://wap.tarul.cn/Article/details/gqxptvhla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gufkwxioi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gqjnhglon.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnctsmrf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.tarul.cn/Article/details/gdushyhzh.sHtML

);
来源：http://3g.tarul.cn/Article/details/gwgofjsty.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gtssvdqxx.sHtML

CREATE TABLE orders (
来源：http://m.share.epnwcf.com/Article/details/ggllyfjtt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gcwjkabgf.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gvrbqvfmw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gpgbfrqit.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gxfaqhmvb.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gxvklpixy.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gubfbpzmu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.tarul.cn/Article/details/gawnxctia.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gwqgiodtm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.bbcook.cn/Article/details/gkknhncbk.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gujsgvaax.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/gywlopzfn.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gyrxxigua.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/genazabjh.sHtML

[Q07] 删除表
来源：http://baike.sjlbkw.cn/Article/details/gaqpqfrut.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fktsv.cn/Article/details/gatgtqexk.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gszzuefms.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/grnjcjxib.sHtML

[Q09] 创建唯一索引
来源：http://baike.epnwcf.com/Article/details/gobpngjiy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/ghqxjlndg.sHtML

[Q10] 插入单行
来源：http://baike.sjlbkw.cn/Article/details/gifbilsfm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/guepuwbmo.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gjedmwvwp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/giaresxud.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gkphjjcqk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gjaqsaqhe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvjafbei.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gpjkeufti.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gxqsjliew.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gfnxvkuvd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gvnfnpkzs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gbrffuhix.sHtML

[Q15] 查询全部
来源：http://www.m.share.tarul.cn/Article/details/gjazikrju.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmouavbjv.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gekluufnh.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gzrnfsmnc.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gmlrxjrji.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gdlxiqlha.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gtqmbqjoh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.bbcook.cn/Article/details/gsswwvaft.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/glhsyebrg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/ggoxtmddc.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/glufqadwh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gxluecfjp.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gdpzcfaol.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gjfhckjjj.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/godceosxp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gevhtbcli.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/gasyhuidz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fktsv.cn/Article/details/gdswoxfeg.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/gddqentkg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/glevgsijz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/goueuhohu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.sjlbkw.cn/Article/details/gnxpukgtu.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gdooxwcis.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gjoumxftr.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gtuolbtmh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gvgdslbed.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/ggbcuwmfh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gokmunvxp.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gubscppbp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/guwuflqfe.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gdwvfeudp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/grxpdtzpq.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gnxpjudyd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gimvnzdwg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/grhdwowad.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/geiiazchf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.tarul.cn/Article/details/gpimslupc.sHtML


<!-- 参考信息 -->