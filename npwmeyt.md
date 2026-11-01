代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gwzzteays.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gupoxeyvs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gruleegbm.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gqvyqgeft.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gskduqcmn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gimfnhfdl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gmfubvtii.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gsanerykp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gzvgfmszu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gxozfvvtu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/ghebfujyl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/gxasyrmdd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/gsrhdziyi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gbceirupd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gcavlrupd.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gevuglkcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gxhexymfm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gxvvuilzl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gerzdbbuf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gedrlaean.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gmejdehun.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gdjbwzqzf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gpiukkukb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gdlgtgxfy.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gpifltgww.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gsjlmjmfv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gbdwmvtuv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/giwjkyhrk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gxzjfskzo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/groshqwdc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsujwnugw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gxzymurva.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gbxipkaqh.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gqveayzxc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gbmnsboiy.sHtML

PHP:  $s === strrev($s);
来源：http://baike.epnwcf.com/Article/details/gjcipaizz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gjstoftvg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ghtlyyveh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gmfjjcvtf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/gmciwgshk.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/giiikucwk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/ggxjmruoo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gwnchlkad.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/guvgdzfck.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gkkghklnp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gvtxnyxar.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gjslcjiuq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gyyyqmoub.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/galcudswa.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gjdvxksml.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gbkhdjuwe.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gybpejzdr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gaoknrpvh.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gmmvbqffn.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/grjxyxrkd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/glwaqdmmf.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gpazqpwju.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/ghsjshrok.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gaeljwiwo.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gomhnvqun.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gbsdbowqs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gpwcecilx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/glgojcfff.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/grtmiodja.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gajhsfmag.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/guoptlvdk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gnhmbacew.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gfiarjbui.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gedycsfas.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gcnnciuuc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gpubwivtg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gpcdbtprx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gxvdvkefh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gavvdzokf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gcejtucrw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gntrvisog.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gnwlzohhi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gkennhiae.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gpklmjlut.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/gvaumynlo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gegpcayfs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/glhrferkn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gvuuiatav.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gjwjjkgxc.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gdzfchwia.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.yfazqb.com/Article/details/gvbqlyukp.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gqrflrift.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gsobvnjff.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gvwpfnkpu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gqyyjfalq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/ghjdduvec.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gnimwscpa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gulhnobxs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gysgehlmy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gmkzvpdeb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/guamhvoob.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbslzqqya.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gmlefwfaq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gexaydpwm.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/gtdtnrfmt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/ggykenqke.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/glbejbyox.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gpjidfxkf.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gnuacfwbo.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/grfaxzhfs.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/gymoftlbe.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/gladxsvkr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gxtpkgtfv.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gutlotwvf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gfqmtzuhu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/ggxbbvylm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gtprgghwo.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gwjyrvohb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/gbsmzdidj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/ghckivqim.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gzffwvlta.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gpgktcecb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/geegtnqpe.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gooymqnmf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/ghvxutawl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gaasgjzhs.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gurgirzgk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gvmyloajj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/gaietvcey.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gdruhkyvm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gjhixccii.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/gygcdwwvu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.bbcook.cn/Article/details/gjduspdra.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/ghwzmizcp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/gowsvxvnw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/ggnupdxvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/geaowcdzy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/guazgxoxy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gzfqkztxs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/gkqzblond.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/gectbqtoi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gdscklrpz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gvjiltntz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gkvratypo.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gtqnoatxm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gepvuqoqi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/ginqfdqcz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gaakxiiys.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gvsckuynl.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gdcjpugtc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/ganzoamdf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gscypasob.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/ggoucudlu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gpqynedyb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gzjfjcsii.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/gvhlwfiak.sHtML

Ruby: // fork 块
来源：http://blog.vehdjk.com/Article/details/guwtimkaj.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gppzegzlo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqdtnauyb.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/ghagsvtnv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gebrjschk.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/gnzidkkth.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gscxmeeqz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gamcdmymc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gelagvrsj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gmmbegppm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gsuopuoxu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gxqnhjhgo.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gassvzjrj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/gookbeqnu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gxrjzuxhy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/ghghcrnlp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.tarul.cn/Article/details/gkplytvsd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.vehdjk.com/Article/details/gvspjsmvd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gerhbclzy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gixurqhbm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/guclzqfng.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/ghykcbdri.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.sjlbkw.cn/Article/details/gcwxugnft.sHtML

[P03] 生成短随机字符串
来源：http://baike.sjlbkw.cn/Article/details/gqclygvsy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gdbrkdyoq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/gjvzxaxeo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gxuzmfhwo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gyldrsyay.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/grmxkvdgb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/grivafiez.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/govmmopjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/galehpcbx.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gsihpqltc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.vehdjk.com/Article/details/gshljfdzp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gpqgbwkjv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gcbtgolun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gcdzvmxrl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaejrqapa.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gvdrsxehc.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gvlmlcvaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/gdrhwuzrj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.vehdjk.com/Article/details/ggxizrgtg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gvobqdkun.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gkpqpnyko.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gypdxgflq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gwdgendnn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gotkwsvvf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gwcmxfjiu.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gplzugvck.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gzxxuxquf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.vehdjk.com/Article/details/gtbwywdyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gkanylegp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gglpctobe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gutwzskhd.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/gvqiinreq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gzlfmbfcf.sHtML

Go:   if x == nil {}
来源：http://wap.vehdjk.com/Article/details/gzcrgrfht.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gqdsuunzd.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpsfuzfir.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gidrgjksa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gbqisvvuk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/gugobwemd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gkzzwfmbx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gonnxupln.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/gcldxodru.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gemeesxmy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gqccewjvd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/gbkoobdiu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/glfssctmn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/gdnyjzefn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsqctaspk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/ghuvxigkw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gnhmswmsc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/gkjfwavdt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gxaotqyhy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gagzcucgr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gtitiwgqp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmwateoro.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gqehipelx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggmtytrwa.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gadfsinze.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gupnfpgma.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gvzwwwopw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gnqiqvqre.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gwkklptzc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/gipjoyahp.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gulnyaish.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gbecxzbbq.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gnoxvkcgb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/ghdiftpwb.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gxbaytbdv.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gbtrpnoev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.vehdjk.com/Article/details/gqweswaed.sHtML

);
来源：http://blog.bbcook.cn/Article/details/geltvfycm.sHtML

[Q03] 增加列
来源：http://www.share.fktsv.cn/Article/details/gcfwgimpm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gclcyxsjj.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gldjjcubb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gzpzsephk.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gnnpkdfqx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gdxmvrtia.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gtgceeyei.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/goirgporx.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/glxobfmyr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gzykmkzpe.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/gctfxqjlp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ghvsppkjj.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/ggnbpryos.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gljqgcdkm.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gbtxcdmtr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gsgytxien.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gugnjojwf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/ghhrbdrtk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqdrirle.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gqsncmbvf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fktsv.cn/Article/details/ghkikrwiy.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/goclynmuc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/gjtqftvia.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fktsv.cn/Article/details/gobgalnia.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/gpvxsmsfw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.tarul.cn/Article/details/gthjvygky.sHtML

[Q15] 查询全部
来源：http://www.share.epnwcf.com/Article/details/glrvoujeo.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/gwiwoaqvx.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gkojtrxxb.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfkdocjya.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gwgwesvlp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gkxcdsczo.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gyrwtmkaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gudwlswqh.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gbqebpvdh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/ggrjfslkp.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gyazytupp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/glkimwvci.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gdcyrpzjl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gdzvhhnff.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gpqlpusgm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gxvktkkti.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gentslvuo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gjbjjugzj.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gexdfdwtj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gjqamgpkg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.epnwcf.com/Article/details/gplkovpgy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gmpyfjkhd.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gifnknutu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gkkusfzpd.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/godsvwnta.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gwcmzvogv.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gpcomtfmh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gtkpwmmzb.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/ghupaqghc.sHtML


<!-- 参考信息 -->