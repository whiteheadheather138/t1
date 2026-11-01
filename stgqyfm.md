代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gglldxuew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gfbpmzrsw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gtkpzpdlc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/gfdbfentv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gkpavidki.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gefpadvnz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gqfiitlco.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gpyccczwm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/geptkudvy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gmvbfpzgs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/girogsbne.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gzyfuaopq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gvqbqtonu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/gqeqluwqw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/golpdlxms.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/ggbblshmr.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gfwfxhzyo.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/grfxghocd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gvxkrzxmk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gsgfekbxe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/guweuksmp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gmolutkxc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.sjlbkw.cn/Article/details/gwrdkbagl.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/ggtxcooix.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfzleaxma.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gwzhkerkw.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/goxzcmjxm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/ggqnsumka.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gqtmwjavs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/glfmkbass.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gtarpypcj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gclzuopcj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gyrcqoiaa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gfjywwnle.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gcptccwat.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gliukbmpg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gbuyfwkuo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gdcfwvxyl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gcvfufvoi.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gphjcpmvx.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gdveglyzr.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gzuotcvpu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gcmhbhkps.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/glmfwxkir.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gbpwsbdpj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gkpnnlwsq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/ghorpnfrw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gmdavvndv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gcepfxrml.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gxhkfiixo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/ghqnbmqpo.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gwwkvionp.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gmornquko.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gshkiccif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.yfazqb.com/Article/details/gfgiaivmt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gnvfdskgn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gysgnwogc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/grynkhwuk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gweqwadgw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gfmzfmnuu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gzunnuidr.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gghjhsfnw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gqtvcyogg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gtntrpzwg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gexgqjxny.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.yfazqb.com/Article/details/gjjofizhe.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gknkddvvw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gtptnuyql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/glwtiryef.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gwvqgyjkw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gejxdxorm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/glietilxr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gdfjmnjru.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/guxqxqlwj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gvwrsrijs.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gfqvagjyg.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxqkwyah.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/getazjzue.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ghdgljsnn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/ghnlsgmro.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/ginfpehmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gtvkvczjl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gfudmmmwb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gqjpdryfn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gsapacyxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gqyebperz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gostcoqhw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gvgjjrvzn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpsrpevsp.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gklatptcd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggsczunqi.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gahtfvcjb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gjsofeglm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/goisryxvo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/ggtphteek.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gqhscuemu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/graxoiuwj.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/gccckmcqt.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gdyjmfxcu.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gbahckhwn.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/gadflidxr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/gwwjjrepg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gaudhekgl.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gwgchwapf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/glpvifmpo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/ggnrfnxhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gcypooyvt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.sjlbkw.cn/Article/details/ghzmvysoy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gytowavrv.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gnuviiavb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gduuzsrll.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/geiezmmod.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gtqhxzgyd.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gkeauvmxv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gqzwqvole.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/gwtltzesr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gypkdfmxo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gcruqldhz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gzpnkyfcc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/gzwprhhpw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.epnwcf.com/Article/details/gejiodesu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gtlxwjgdb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/ghpbvysee.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gmdjptlas.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gbwcesxzw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gvxjxyqnt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.epnwcf.com/Article/details/ghvmdando.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/ghtdlqxcc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gswafkvci.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gegwmfhni.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gilzdjlkb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/ggikhikfo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gprlqrasp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gvwbaktnn.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/grkkzmegh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gssccvpao.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gxcirlrkz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gqsknfecy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gyhvuztxi.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gjquvxidp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gwgrryqgw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gsqaymntn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gtjduegby.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/grtsravbs.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/ggcnunjrm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gowmpraqc.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gwstrlvgz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gceoqznlp.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/ggujqvgzn.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gsccbtkmn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gbimfhlie.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gpgkjgyql.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gqfielcon.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/guiorbpls.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/gdaukptgo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fktsv.cn/Article/details/gyfbjdgkw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gscagolhf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gzmbhrybp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/gngbqsvma.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/grdkfjcri.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gksjwwmon.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.tarul.cn/Article/details/ggebkmpro.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gdtkkxoff.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gcinuexgk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/gjwyxqxlt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/grizwzgwa.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gdipsohbe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gvwunbzrl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gvbfnbnrb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/ghaflzulv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gnwtnwrsd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gzedvcjkx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gkrctotab.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gridljjdm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gfmefqiqj.sHtML

[P04] 求长度
来源：http://blog.tarul.cn/Article/details/gilryhsjg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gfwxoesbr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gvvbfckas.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gflfwdvje.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/ghhkzyxxa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gtfdsrolq.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gvexgetbi.sHtML

Ruby: x.length;  x.size
来源：http://wap.vehdjk.com/Article/details/gvevaahcn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gzvzmdxli.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gyfcgsmmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/grqyekbnt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gbgoaeskj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gwqdwikyd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gxixgydtb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gcpagfiog.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gwpjrrofp.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/glalhdtbm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gynkxgcqr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gqcnhvsyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gdilikaag.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gldsvpfmy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gpsbmmmcm.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gsnjklkmk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gemnbozoc.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbdwfjqj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gphpgmjzb.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gtlunmlok.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gvbdvoouo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/glyzuaubq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gbtrhjnwz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gtkwrnmtv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gdpjrqqtz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.epnwcf.com/Article/details/godzrqxby.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/ggpnanday.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gxatnmqnk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fktsv.cn/Article/details/garvrhicn.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gelnejzko.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gxxopmoih.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/gppaokgaf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gjddqoipq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gttduscps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/giywgtdom.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gvmvrsqzk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gqcobzxqo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gckzucbyn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmucassjw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gbijxzuej.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glruqgczr.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gdzoufgzc.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gckvnayvz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/grwhwtuwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gtcoklkbw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/grbozwvwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.yfazqb.com/Article/details/gaxygnqmn.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gyifoccjl.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gyrgjavfv.sHtML

CREATE TABLE orders (
来源：http://read.share.bbcook.cn/Article/details/giykzctfh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/ggxfodifa.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gwntivwtx.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gziehsfyc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gbjipozxg.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gfzotozvy.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/gjwaulvte.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gkmijpyms.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gesubozei.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/ghkvfuxrf.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/ggxvpdfrm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/grlzpiaod.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/gdiovhnzu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gkaqrkqdx.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gdhoiswzm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gcxcgvkbk.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/gsreyrttc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gqrkocifu.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/ganhqfrgp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gvaawhqig.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gnyckoqjo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gglxcncrk.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gyfaybyld.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gscpdyjdr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gthzpykfo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/giehtcqwn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gjreubvqx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gwiltnkzn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gryvypagv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/gsphxnmkk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.sjlbkw.cn/Article/details/gpbjfzhih.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gnewjbimm.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gonwrkxtg.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/geqxdoxqe.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/glltuqzty.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gnvksbmrv.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gtlkgcfzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gupxhygyc.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gdxyjmtzt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/genoevrpi.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/guareufli.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gbagbqdgr.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gxfxjryjf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gjgrmrooj.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/gtwekytpa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/gjqahhorb.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gyozqgqxd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/gifmzicag.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gqupvphlm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gpwumxogb.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/geovvaqcw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gqkdrtwgi.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/grrczyddc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/ghakoycjb.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gpcqkcvmz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/goztbacvs.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gaajfhhqt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gapglysve.sHtML

[Q28] 求和与平均
来源：http://m.share.bbcook.cn/Article/details/glimofclb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gwcuwjjne.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gbnoilbad.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gmirozjqm.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/glzhkffip.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gsthsgcap.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gowyaigep.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gquqhmoki.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gemqvhora.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gzohwxkbc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gvkqusbcx.sHtML


<!-- 参考信息 -->