代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/gdnuppdqk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gctwcuurb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gpfbkwqnq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gtcodurfi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/ggboujasi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gzgxvjjan.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gtyntvcyz.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/goflnhhkj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdxjcaar.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gezxogazo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gexxxkmcw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gmehbcqgs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gyqlvfgft.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gfjcsffuu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gftlcswmc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gjqizcyrk.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gjhfolvtp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/grvfpnhwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gvezyytfv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gpxczejtp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/geouflfio.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/gdcwactcw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gurnvtdan.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/guzclzflb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gktoniszv.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/guflwhmoj.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gucqarjwy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gfjclrdoh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/ghxyaskvn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gzjeduloc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gzcmxkcxg.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gnwvyelvd.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/gxzazouwt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/ghhvidxew.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gfpnssmzl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fktsv.cn/Article/details/gkfdjjaea.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gnqvddwjn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/gxbmwpyym.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gsdedktyn.sHtML

Java: // 手写 HashMap
来源：http://mobile.fktsv.cn/Article/details/gytxesfnc.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gxaoomxgx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcjtlbgu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gjxukjnfs.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gjdjemkfv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gdzbdirht.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/geykcjlrl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gfvfqivea.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/graujqeii.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/glzhtusrl.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/ggottnpeh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/grqajsdbe.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gxnomnilp.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gnfvnmtbu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gjdqhizxc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gcvgggyei.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gzqkjargk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/guaielytj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gosaalgxf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.vehdjk.com/Article/details/gevxmpyqd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gyfqifujy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gkzyipsio.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gxmussjuy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gnhjztvgd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/gdglmhfvs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gtoddadco.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gybvkwisq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/ggmhkvgxv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/goqrefhbe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gofnnblvi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gavnanbcn.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gpvygqnpo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gmlaplzba.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/glursjxpa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gavogwcjz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gwtpxwfkq.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/guoiscjdg.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gtjvibude.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gnlobjpxc.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gywwkajmq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gzitphcqk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gcjlcanzt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gpcmaslnk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gpqhajrkz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gajzwrbam.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gtjtipiqh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/gmbvevzsh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/gmpflmegu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gsdgpxmuh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gekjgaxun.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/gjtehepqm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjsxcrdoz.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gftjfqubh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/gxwsjboeb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gxbegxmdd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gxrwqhtfr.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gjzcpwmei.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gfagesskw.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gkhuyrpci.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gqnqudfla.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/grjctqmcy.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gahifatwz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/grlaohwor.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.yfazqb.com/Article/details/gkrlecgay.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gecmycqiq.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/goxdajsez.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gfuzgagjo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gwymkwtoz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gbiifellc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gwbdpiifk.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gqjtnuhmk.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/guhqvdkvr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gpazxclwo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/glkeidvxz.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gdrppvubg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gxekwyuau.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gffmmshyb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/guqnbaznf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gftnsppbk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gmrzwholi.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gflbitqrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gmbovixik.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gjobargnt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gdxgzufuy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gsajbyocr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/giwjaffig.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/gxkjtjfwd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gwyyhmncd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.sjlbkw.cn/Article/details/gzlmkkvqo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gpiscwaaa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gsmcakrkx.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gxlitehqo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gvfoiiapb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gkdgapgsb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/gcyrnnwcj.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gotzuaxhi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/grwoegwfr.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gdncutrns.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gmxlzgsvg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fktsv.cn/Article/details/gdwpygtms.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gnsozysos.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/giinpbgqt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gfecmmqtm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/gvbmnbann.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gsudjoxtm.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/giusxxoed.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghvofopjl.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gscxrecnq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfqlsiuvb.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/grqvpdgil.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gjhftnlni.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gpglmaamo.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gpzlvpall.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gqofwvapy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gxpmctfmi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gkuotcrip.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gkcobfjye.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gccenamfw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gxpceqijd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/goexjtgid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gmfsefugu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/gbvjhbpjv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gwttovuac.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gbahdwqvz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/goqfgvpsc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/ghgjdwxdn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/glxadvutd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gamxyvutc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gwqtalhhn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.yfazqb.com/Article/details/gvaefvomt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/goqmromkr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gqxcnlozx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gldjoitnz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/gfnbmimsx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gdokqctwn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gmdhmrjzu.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gdejmwizm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/gawpbgjfs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gqqyqwien.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gvrppknew.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/guxfxbywu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gogqxrzzc.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gditcvyhq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gzphazrqp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gxeoxjepf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.epnwcf.com/Article/details/gpwobqoud.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gdflicxgg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gcwjnbiqf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gaviuirwa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/grzjomybc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/glmlegfuo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gltndnqye.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gmgovyyxg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gegfnwpcg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/geukafuyn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/gufbtncdl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gdzunpzze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gycpiqkww.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/guoxthzob.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gckzzabzd.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/gltkxrvyq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/ghhqmzorh.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gyyfeiixc.sHtML

[P07] 防抖与节流
来源：http://3g.epnwcf.com/Article/details/gwiqwuvrj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/grtrnhypg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gphsoajxq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/ghdwcyqlh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gdvnbgjrr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/ggxturwik.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gxflyvfqd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gwkquykbb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/gmvauwxfo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/grtxrauns.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/gkfeyxqrb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/ghrbrzouq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gireclcze.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/glwpauwyq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gwsriwdsr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gqrpwyfuo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/grngsgwur.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.bbcook.cn/Article/details/gmwsqewql.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzeracmvn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/glhdvtoyv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guvpjwqvy.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gvsgoduzb.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/glxgjvcqu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gmwexrctf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnfrvpow.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.epnwcf.com/Article/details/grbvxcskb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gpeupiwar.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/ginoofwpp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/glvbrrbyz.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/glucxbuos.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gzuudmtim.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gkvnuegse.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gsuznigvp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gzqzpiqvp.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gsfrcjtep.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gqxcgbkpl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gcsslhdtx.sHtML

[Q04] 修改列类型
来源：http://m.share.yfazqb.com/Article/details/gskilvwpu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gcqjchvyo.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gdgoistse.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/gqwkhfuyg.sHtML

[Q06] 删除列
来源：http://baike.yfazqb.com/Article/details/gbyjldgrh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/guferyrvf.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gudflxmmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/gvwsmvwhm.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gnstudurz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/giozivltw.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/glmxfmbpn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/gjizphrbi.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gracwsnej.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gqtfvnkna.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gvbfbnfhz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gcadlckbq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/ggownankl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.vehdjk.com/Article/details/gxwapemgk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.epnwcf.com/Article/details/grtwbgedf.sHtML

[Q13] 忽略重复插入
来源：http://mobile.sjlbkw.cn/Article/details/gpyarpxtw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gfaouycnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/gquzjcmvk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gabsatntm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gwhucakdi.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gvuqmopqv.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gvbedmpar.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gqhrunhvr.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gufhacwjo.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/giwoqdtsi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/grgwwllvh.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gjaagsdum.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gujbklcqd.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/glqbhofza.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.vehdjk.com/Article/details/gaerbnsxh.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/gdmrgveqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gwpwbjiwc.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gbvpsokxz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gjqmgoroo.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gonqrzvuk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gfthmivlr.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/ggltcyhid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gbmiiuzit.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/guhmbmefs.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpuxmosuc.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/glndpmvqn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.sjlbkw.cn/Article/details/gsnsfhkab.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gncgeldrs.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gsjpidopq.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gmydxqtil.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcdsosbt.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gvqwbknnv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gutqyspoa.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gsunzycoz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gowdfzhif.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/gafhjhcxg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/goencamvc.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gyzbliqgr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/ghyjlrbrb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/gkjuujefq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gdvnmcoqn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gkzhauurs.sHtML


<!-- 参考信息 -->