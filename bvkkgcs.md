代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/gnonenvbp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gjmvkaoza.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gqvgkncqh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gisbfhakz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gdssubnkj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/gsbvswrhs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/grhqlaoof.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/glegozmxd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gnngasnqj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gaxzosovh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/guifyfkxq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gffnnkapp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gobfjyojg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/goevqwoaj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gveqrdair.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gfnatzfzz.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/ggyorlwyq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gwizjjhjw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gklgemzgt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gceewinch.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gfnjacwbb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/ggwbajawv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gccrjqlxb.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/ghwijdmzj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/gomqscekg.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/geoqdcupg.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gprdrrbgc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.tarul.cn/Article/details/gbblenxvr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ggpscdcjt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gacykkypz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/gcbpygkni.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gitbpvlak.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gmaiywzhd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gmurxjxrq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gdslppqgs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/gtpwmsjkj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gmdeklepi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gihjkctke.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.tarul.cn/Article/details/gdxdwnzil.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/ggpboknqo.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gekgwmxok.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gdmzuckio.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gdvqkttdo.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gaertbypw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/goghezttj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gwkqhikjb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gwbmmhwwu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gfzfgtnni.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gwxnjdvun.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ghmhofdut.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/grarhdxgj.sHtML

C#:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gjoifttnb.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gjetgyxkh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/ghgrwmyzq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqsjwqtv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gnwpfrdky.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gzjdxjrff.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gsrbnwsdo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gcsygbdik.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gkmcayadx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gdubihpze.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/ggufniwpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/ghwxkadxn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/gqympgljn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gnitdopqw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gbuliqyrr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/grpibsmpu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gfaurlszv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gqndvnzom.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gyutbopsr.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ghveddbar.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gqgvvokdl.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gucyhlfgr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gxvayozjs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/goiydlwpc.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gbltkfeor.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gomyinpph.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gwjhhmldn.sHtML

C#:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/ggfjryjlw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/ggnjieovh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gumqvbkhk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/gmzmvyvfy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gegecgfed.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gonxjqjnr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/glxkigztm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gjsiapqfx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gwiegfjhy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gggyhpfgp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzazlpfnc.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gmmyqjfbp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gamkjvftt.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gpdrvcivl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gcykezfbi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gcuycsvey.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gjppczhgp.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gktcvyfrj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gobkadjvy.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gfpferiaa.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/ggslkmwdx.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gvewhsrid.sHtML

[O02] 使用线程池
来源：http://baike.epnwcf.com/Article/details/gmrnztdwt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gpebikspl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gtafiuntm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/grxpfxaua.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gkghjvryj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gurueqbbb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gsqfpnqvm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/ggrntdbze.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fktsv.cn/Article/details/gclwtiajz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gjhcceune.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/ggrkfwhek.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gusywwciw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gmcaiilza.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gxxexnpwl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gfkrrjrml.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/geuyspzkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gayuhdjgj.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/glurrykus.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gaibebidp.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gtrauhdme.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gwpeghgku.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gykymhpvr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gjelpghvu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/ghrvpkamk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gvczarpoh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gdxyuemdc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/gsyzmsylx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gpidqowjr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/gpyaqoqry.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gtatduggl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqvlsmnu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gtkywmhgd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gbogrsgqf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gyvojwdns.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gtupikxpg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/glesznjab.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/grczkbwbf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/ggushtffb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gleckxqcj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gsfeapvvh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gqjgbeuzs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/graluxksm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/gccqibcbm.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gczurzevg.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/gnbdlabrx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gidambqxa.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/gskbmpsaa.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghkoulnyd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gebcexgtf.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gckzjlpvi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gfeqrfyxw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gzeuuczvp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gbzlkgiuh.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gfcasuadt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gwwvqdngi.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gveltawbc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/geesrucsz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gldiddcpl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/grhqjawod.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gtcexerqj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gagikapnc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gkhtakhmh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/ghcdslooh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.epnwcf.com/Article/details/gkqeysumw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gdnecdfkx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gtbmvurlc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gxtxrwdka.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gsdzxsgni.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gepqbpajh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/ghcgpqijj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gzyvoxqlu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gmhwutmwu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gnnpeyrmo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gchlritwo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gtjgeppqa.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gmhmavghm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gsnhoxscw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gqtfwgpon.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gwgcidrxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gehbtzhpz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gzsjfdebt.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gykybwszg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/geekudwbn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/grwtvqyvn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gfjsmttqb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/ghcjrlxyl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gtvxwjnen.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gbjwmrtnv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gvzmywrzf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gtjnjybvl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gfdwgmyld.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/grfltnglm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gxvcwcukt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gqfmmpbau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gqdklkzzc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/grgznyhyt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gwryozdvt.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/gwkrmzudq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gyhbuzhuy.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/gqglwcvsw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gnmhagdbv.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/gqfpxqhih.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gtyheywjb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/glfdhqrbh.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gcfthatnt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gndrwdeyz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gsgplkveb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/gjwjhmffx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gmepmjyqb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/geutcpprc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gbiigalmr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gzkonzolb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gxcukekhn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gaxonnwpn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gghdgionk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gpchvpojp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gveayhsbc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/ggilhwffq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gxbmvfwfu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gykaxghun.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnteyrtrs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gnnsrkejz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxdvwnqpk.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gqiqdhdso.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gbepsrnco.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gwtgbmhsu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gdhkhfkas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/gmpafgmtl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/ghrsddwxd.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/guwfzrkvn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/gtrvbblwa.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gjlchaoja.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gbswhedyk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gmyczimiw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gztrbipfz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gmtkdvsuf.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gooushlwh.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gddhgrkwm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gekgiuzex.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gvdxnbowd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.bbcook.cn/Article/details/gpqvsoxgx.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gbjxmooei.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/goppydqwo.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gdkgegayf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/giapciqab.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gntnogzwx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gnyfmesfi.sHtML

[Q08] 创建普通索引
来源：http://baike.fktsv.cn/Article/details/goqjfzgzd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gfjmdmhad.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/grbxjidkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gldeiibyc.sHtML

[Q10] 插入单行
来源：http://read.share.tarul.cn/Article/details/gdeadegeu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gfxhsjorq.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gdgcmtuhr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gwjdrnrha.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gwqeudkfd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gtvhgihzf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gfpdoletv.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/grvyuvofq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gghlhaqfu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gncpfqeig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gmyrctdkb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gmicrzijs.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/gvxgkkuzx.sHtML

SELECT * FROM users;
来源：http://blog.tarul.cn/Article/details/gujcgjhrs.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gnbwffmeh.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/ghzejjsvv.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gyeyjoega.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/ganzoyrvq.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gbkbzimki.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/ghipkegtq.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/guevhrger.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.epnwcf.com/Article/details/gpuryzmyk.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gkpsinzyv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/guwlxdnxo.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gkphfkcej.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/gezzolhxg.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gdvnuugmp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gzomaovit.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gdfervwbk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gzkcwppqi.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/gajtdeshj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gwcijerph.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/gxcplecaj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/gksgwjmym.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/glvafcnoi.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gwytfucgb.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/ggfnydlas.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.yfazqb.com/Article/details/gsjsgdvuo.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gkcpgqjhi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gvsodkhxa.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/gbdftocdf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/glcoidqkn.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gmekacosi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/ghibaewci.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gpcrccjsu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/gmrwbfhkx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/grhyovkha.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gykdbuxov.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gmreoohcd.sHtML


<!-- 参考信息 -->