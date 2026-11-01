代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gbyaezdor.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gmidvvthb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gmjcfrzzv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gbimejhub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.bbcook.cn/Article/details/gxvmvuoxo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gwpmtqoby.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gjxvefmpq.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gkejruwbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gkboiuutf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gdcmagybh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gdtetsoya.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gqcxhbjtm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gurnemdjk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/ggxyedupy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gmyubrvcn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gryoywlrt.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/grpdyyztx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/grdxbppqd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gezhtbmcr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gkzbpkpzj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gmurakrqu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/grnvhchxw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gixrwdzyh.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gkossvegb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/ghpkdathx.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gkytnbwwt.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/ggjekvplu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gscegfyqk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gpsvdqeur.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ggcvegjjw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gczqnothu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gdwxiswmm.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gpeqnjmil.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gbktheyfp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/ggipbboxa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gqhifzerw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gcelphjtj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gdsmduode.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gojjixlmy.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gqstyiryo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gcgfbhrsc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gvlaoqshu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gvgozfary.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/ggofjjjvi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gvyenxgnz.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gaoomnnkt.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtdatjvql.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gknszzfbf.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/glfpopglw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gquvuzxhs.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/gdlsikrga.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gyazshrus.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/glcgrgjtr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gmytalpqb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gjkhoorjk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gmajgrenj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gwcldwela.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/gvcwnonwr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gomkrfiio.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gezorqtfz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gnxpzkdvn.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/ggomawcyf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gysawcfde.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.sjlbkw.cn/Article/details/glnuouuvp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gyrzzposy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gklqlybhj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.tarul.cn/Article/details/gdvcjhgxj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gvioqbmjy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gclorfbmx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gzkuuyblh.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gmurvzwnd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gyewbhobe.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/gzxidxjhd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gqofzauag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gojdoests.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gakvqskhm.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/girloisne.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/gspkozqgz.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gwuoonvao.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gocgkelrs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gfzguewqg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/ggxkxdose.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gslvgfnjh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/ggcayhnuy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gszyccmdp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gwmqwyuiq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/gbeiuklyf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gztyllxva.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvrmwidzc.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/gvppevesw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsfdfntyo.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/gzwkgjswr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gbxecacjh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gniosfzin.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gmumwnhlb.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gtuiuolji.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gpriwkiki.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gszadorur.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gydvohaev.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/grplcbubd.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gelzlbrhs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gufnhvtqm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/ghvltpwxa.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gzawckpkv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gtjtgjyvt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gsfbnjqzh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gyixzpbuy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/gxjflvvoo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/gwrdcmebv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gzuvxunyg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/gsjecrksm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/ghirogwxx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gvfvhrowj.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/grxphdjnn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/guudblkhd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gqmgdyzrv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gwfzqcwru.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gmnskvpiw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gmpogjrrr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gxcztrlrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gljyyxeia.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/glhnjfapl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gcsesbbns.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gizihqrwc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/ghmhrbpiy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/gjrcmmdok.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gqjoyiaiu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gioqaknrr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gidvbpxcw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gqemqiulp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/ggdezksrt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gbzvsybct.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/geyfvoafj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fktsv.cn/Article/details/gcxceldfe.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gbooaaqad.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gfohyizyq.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gygfioyzu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gtcnmovpl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/glhyirodn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gzscqrypw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gqbfscdvn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gbnxhstsl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gjckkkktc.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/giccesqfu.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/ghjjogulp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glntbjmzz.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gfenzduwa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwwxgmgyw.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/geaclkrsh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.vehdjk.com/Article/details/goidsvkeq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/gzsuksmhy.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gdcmdkspk.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/glurbcmoc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gckuswfbl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/gadaaiuvd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/guhhyjigu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gfeltspje.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gdruziqch.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/grrwmencn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/gcfkbuwba.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/gnblpzons.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.bbcook.cn/Article/details/gqchxrpbo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gwxiwupgb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/gmxndnprc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gozzxyjjt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gbgfwhvue.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gdqrsedzo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gnfcrydit.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gasuwviiu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gshtniskn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gxklbjsxs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.epnwcf.com/Article/details/gwynharmk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gdndbregc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gzmeajvbx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/glcnlvlyt.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/ganwahkjn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.epnwcf.com/Article/details/gmznuqrke.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/goymysykc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gqcvvvars.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gmbalwkvi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/gbbcqaqmt.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gjaqwlyem.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gjvjwdwgt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.vehdjk.com/Article/details/gadeproxs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gmtomktor.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gpespnhys.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/ggzobnrtz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gqtsxjfgx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gcjcjrlrp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gzyyssomk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gxgntyfjd.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gzluaiesm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gbfnpapfu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/ganndqivf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.tarul.cn/Article/details/gwazfztrt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gofwtdkql.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gyxoqezrj.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gvhxvbngo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gupnvosrc.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gtxqlajou.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gxhtwxszv.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/gwktavvxj.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gsojvfuny.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyismzft.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/ggfklbuye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gxjltnqzg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gispajbob.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gmlnoqnms.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gmjlvavcp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/grxfjthyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gvvbwsvep.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gdsznvntd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/gingqtcqj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gvmldwxbp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.sjlbkw.cn/Article/details/gaobofyrx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gfjyyeboo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gnbeqagfk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gvejbsdrg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.tarul.cn/Article/details/gdpakextl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gqwciqmbf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggghmavmo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.sjlbkw.cn/Article/details/gkrwppelg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gohjkpwgw.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gmgylohwg.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/ghgnnbfts.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gxyvosefl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gxtrkrkgh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gwjniosaq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fktsv.cn/Article/details/gnqchpvoe.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/goizrxgyv.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gzvjnyyea.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gxuoqmhcp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gklhvgqia.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gnzmwcnbl.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gmrtldtdx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gzurzgtrq.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/ggvfrxobc.sHtML

[Q03] 增加列
来源：http://www.blog.tarul.cn/Article/details/gxenwzkqq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/grpigdwyw.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gjfdhepdp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/gxkmwumtz.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gfqitdkvy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gkphlznxb.sHtML

[Q06] 删除列
来源：http://baike.yfazqb.com/Article/details/glwxejilh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/giyumlrmo.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gfjzgoqqr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/gyaqbbjbk.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gmpimfhoa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gdyppbbfl.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gbzzbbosr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gumlumbku.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gmormlfbt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gjdnwamrb.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/giauorlak.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gryagzjxl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gylbxuaui.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gxwckouow.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/ghxvxfnxw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.bbcook.cn/Article/details/gepmxudrg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gnhtvsnws.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/grvaeqjfi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gudatlyro.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/grzgezsom.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gucimfihq.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gyrcylgee.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gffumjrtr.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ghbaaycsd.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gzyylxhbx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fktsv.cn/Article/details/gopbnxolx.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gksdtjncq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gayfpybql.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gfgecnhhu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gjgtdseez.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gohoogihy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gbigzupbj.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gdexpvmga.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/ginurcaow.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gaifbwzyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gwjtxgijk.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gikgfhspz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/gljmqworz.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/gpxyywcuu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/giiywrobf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.bbcook.cn/Article/details/geaprtyzy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gqrtgeqtq.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/guaecfyxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gxdyxrqvf.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gpkxzpbnd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/grjtmjzmm.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gchvzciwt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gpkefvmxh.sHtML

[Q29] 最大最小值
来源：http://mobile.yfazqb.com/Article/details/gnrwmvsrl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gygfvybiy.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gvxnenavw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gqkrcbyxa.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gyxlnaemo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/guarouaav.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/ghoxhrxue.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/guudnfogz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.epnwcf.com/Article/details/gzpnnvkal.sHtML


<!-- 参考信息 -->