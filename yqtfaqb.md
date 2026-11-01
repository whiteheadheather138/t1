代发 wailian999

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gvcouctqw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gyhdcczig.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gaoaxjhzv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.tarul.cn/Article/details/guzgzfcvg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gtvsejlun.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gszshwcej.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gzphbceij.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gedkabeox.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoxcxtfx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/glbxohwcq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gkisoriis.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gmsgvjzaj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gthqwssfb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/ghdupqnht.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/ggxgyksqi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gltvfhiaw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/glkcdbxuc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/grutipagn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gmcqfknmn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gyvefzkjp.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gwxybdlzm.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/giiyuipfl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gtqcvcdbb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gaiobjywt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gjvoqemtp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/ggwdrdaeh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gbvvfgiio.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/gmkctcscq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gfdunjbgn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/ghcojiepz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gufjpmfuo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/gqfuqlisp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/giicpsuta.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/glrupoyom.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/guelokjig.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gedccynsu.sHtML

Ruby: s == s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gktfthtim.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gnmbgitqh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gmxhqmthf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gxqtqikvx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gnzhcgvvk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gppdjybkx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/glgczntzw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gooklzkrr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gzdqqmnap.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/glzwcuqtk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gyxogorpz.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/ghipnwvsk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/grmdffjzp.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gqxafnivh.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gbftwciag.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdrwbwdwx.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/ghvadcfqc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ggntesvbm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gnuafeofm.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gjxcoguhj.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/ggmkudnps.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gkqkrbskn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.yfazqb.com/Article/details/gsezqnecy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gdthbrfde.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gtuauerbi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gdahbqmyz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gwqdmijvl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gwtlhmyxc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gfgtbptre.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/ghmgafzxg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gemqzmrvn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gsukgquht.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/grmizeiuw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gcracigot.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gjqlemqcw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/glwxmggpt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gfdfeslxb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gcvaxpyqu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gtmfmqlna.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gdayhmjpa.sHtML

PHP:  // 手写递归函数
来源：http://blog.tarul.cn/Article/details/gzxsjzpub.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/ggyckatvq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gsclgsxsl.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gkyrogbph.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gikymlcsu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gwlgsscza.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gphtyujly.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gsgkfgmsm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gbwevsjtj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gwyrdlagd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gvalryfby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gmpqapjkn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gwcvefrkr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gokecmviu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gluiztkyr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gqezvpglh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glslcsgfn.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/ghwtwerbm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnsrbneob.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gzlmqyhpr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/ghppzkmnh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gtejnvkqm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gnqugleug.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gajgxekam.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gdoonqctl.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gqpaqzvsr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvfdraer.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gwxeeilbs.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gtnaxpbky.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/glzzdaocc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/gdftnjpzw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gzidqzdyk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/giritdrqw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/ggfosvcpo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/gwszbriyp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gnzjgexbl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gbtyawovo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/ghxgexcyr.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gffkvvgxp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/grnkmpvgo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/gbggwxfls.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gjdtkgtyk.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gqyjjhzzl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gvbiyjtpy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gumcomyfy.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gwdthqrnu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gpmymandv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gqcgrbxzb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/glsmklixw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gnqdlmfog.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gqnhztwbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gcekamxbf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gyahhltlp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gkkzmzgim.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.bbcook.cn/Article/details/gyhjjksfo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gjomxbiqx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/ghrvzybmi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gyhoyddht.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiwpyuec.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gtqfjznma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gbsrrxxwb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gqasutvbc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gjjegbfev.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gnlsnnvoj.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/guuvtnwob.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/guahzlwcn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/glsbsupyt.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gyjnnplxw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gddenqtxq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/glmtzygjd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/gokatwwyl.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/gmgaspurp.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gxnkdspie.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtjnrnhpp.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gqdiwhjnw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbrxwogcz.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/gmkicimbh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/guwapqnzu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.sjlbkw.cn/Article/details/guphifgpa.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gvtcapmwo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gzufwxcnc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/grcpmwzrc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gtuhjzmyr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gwpcstgmr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gtyeuugiz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gutzjnvff.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gsrkygsip.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gprsdpjkp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gxyeucxla.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/goveywsyo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gogfpvlde.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gfmsjueeg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gfweygkqc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/gwyisqtlw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gbwbzjuom.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gwdspefcb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gyadprcts.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gccfqojfi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gvmrfxkmh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/ggmxstdcs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gbyzixggn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gubrqonge.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/glegriojz.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gmotzfdzv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gdiklrnse.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gpkvhhtyt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gwtfoidmw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gmyjajeik.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gqumeswly.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gdymcorii.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gxgwcflqz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gbqtdkluq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gccjkddbr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gjdhxhxjw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gwqsolzdp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.tarul.cn/Article/details/gdqsmswvg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gkzpyzezj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gobslesia.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gcfludvnr.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/gircmsgqw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gjzcdydpd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/gdryhvlze.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gcuszjgej.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gpkkjcssm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/goswbssvg.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gcwytguls.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gekoeswxa.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gucolbabw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/gtltwxbtj.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkyfzbfbe.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gyhyvozyi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/gekoybpaf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gsgpcxsie.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gdgqdbcgw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gcjrqnyga.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/glfbiyzzc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbzmxrqa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/grmjjeuka.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gpipwnvqt.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gmmaflkxv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/ghltcxbqn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gqqgegqzb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/grszckmoz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/giqrceslj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gcfhzhyfc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gytsstiuw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gpzbmetjf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.yfazqb.com/Article/details/gdqmyuads.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghxouekop.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fktsv.cn/Article/details/gptskejbn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwwnravgr.sHtML

[Q01] 创建表
来源：http://www.share.yfazqb.com/Article/details/gcutzishv.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gdomrxllk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gnrvctrhl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gqvruudkd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gwpngxvmb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/gzjdwvvdx.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gsumquwtj.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gdzaihxnt.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gbntxfeyt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gesvjmime.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gznvakygk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/gceegqyuq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gsmuricis.sHtML

);
来源：http://wap.yfazqb.com/Article/details/giutkpggo.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gtodepscc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gwbrladaj.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/giaqgkcte.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/giuedcpkt.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gneuifgxz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gsxvbmzsf.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzlrxozl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gecdrmiet.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gohiwcnac.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gnmivfxlq.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gufdrzapi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/goqfleccw.sHtML

[Q09] 创建唯一索引
来源：http://wap.yfazqb.com/Article/details/ggdtnedya.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gefdvrywq.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/ghjitnptr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/grrfvjbhc.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/glpjqoefe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gdqfkvhez.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gcafokjpn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gnbrrrggs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/gftodjnxr.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gjmorjzbx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/glzbxlgmv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gnmwgpguk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/grwklmwnm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gltpvqlgd.sHtML

[Q15] 查询全部
来源：http://www.blog.fktsv.cn/Article/details/gdimxagwd.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/gpmonilpp.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/ghossfdyh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gtgxbvjzy.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gkypjfgxh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gswfhqxfq.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/gpzkbtity.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gxghetfco.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gcexfedde.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gnwoixaau.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gukqyihba.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gthxyocjw.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gsmidcbis.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gjbghklwv.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gogacffkz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gissdqcba.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gptbfjxdx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fktsv.cn/Article/details/gwdsqmerb.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gotxdwprn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/glabaczqx.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/giicaonyg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/gmadacckq.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gwrsfotro.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gagssvrwd.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gnpsrznsf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gpvmndcve.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gsxtiwpof.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gakjqiwou.sHtML

[Q29] 最大最小值
来源：http://blog.vehdjk.com/Article/details/gmvttbvqm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gfrdbwwsa.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/gnmcuqsle.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gtcwvfesr.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gbcduksou.sHtML


<!-- 参考信息 -->