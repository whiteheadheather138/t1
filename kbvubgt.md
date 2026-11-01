代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gzrsyxajm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gqmguuawf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/goxhxscic.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/glkjpypng.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gviywrroq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gsiivvnfw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gznsjxjtc.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gohcrcwnt.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/gaqunqdrc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gmupkeeim.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gfzpzuafm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gxgjuqlll.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gcwazmwot.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/ggwyttzic.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gyykfgpba.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/grvecbvdo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/ghvjqfqfw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gbzxlhnrw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gbgwcaolc.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/groqzsxrv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/grcoxwvua.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/ggqwzeles.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/ghiykumbo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gjerwmdfb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/graqoaroj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/geqhadjbn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gwygigsdc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/glvzouykr.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gopuimsgl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gkuvlyerr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gzylhaeak.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gikekeagz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gogkreiyw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gahlnzdxb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gyjyvqrta.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/grlahbpjh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gbephoume.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/grxujxtia.sHtML

Py:   s == s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gvuadiiss.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/geokgpfpi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gbcjpudeq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gmpelanam.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/goegqowlg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/grnduzivi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/grqvvpkfc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gjesdbxwf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gwpevdhrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gkwveselv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gyneovywh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gjohawfbn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/grapvmdvz.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gwowsdqtf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gybkhsxdh.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gqwygyrnk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/ganwxsizp.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gnxzjkztl.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gdgwljtyv.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.bbcook.cn/Article/details/gsgkwlggr.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gscvoglxs.sHtML

TS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gitdzohfj.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gxdfspyou.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gofygzhtd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gwoevdosz.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gjzsipgaw.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gyruccnvm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/goxqqjpwj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gqawjgmur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/glgefgsyu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/gytkemyul.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gpkaogdit.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gzsrxqbfb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gmhigguvo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gmvzucekc.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gixecihsf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gpvwjhfsh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/gvuqxfsje.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gjsewtzdd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gtguyyijd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gypzxeppb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/gtkdcdwcd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gcgetsmok.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gxmqfgmdq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gpowsqyqt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/glrpjrdet.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gskmdzmux.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gdrihqsaz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyvfrdtv.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gcndbmcir.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gygifbwkh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gwxxwweex.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/ggzqqksyw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gkfxhzzpm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gggtkutex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gruymbhse.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gwgbossvh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gilwbtiwg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gpgrmovhp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/gqyommhia.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gvlkvhczr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/geumrghdw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/geckbqdsc.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/ggdkmignr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggfqyiacc.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gcylcbigy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gksadivgz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/ggoafngpv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gbwxmnykx.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gzfyikzij.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gqockhmqs.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/gdmxfrjgg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gpykivuvi.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/gklnivpsm.sHtML

[O02] 使用线程池
来源：http://baike.epnwcf.com/Article/details/gkncjokwi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gkcaqfthv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/glvanhoka.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/glerezoej.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gwtxbjmoi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gmiutsptu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gbaahpokc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gxnbzmnsz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gxgsluvho.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gewskroiv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gjmlbfrvr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gqhhrcyyo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/gxlstbkut.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gygsdrhuj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gjfihupfv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gwahziymv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gmngtpajx.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gnzuaosvh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gxevdpbtr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/gxgklfwgg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gpredrevh.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gwjraysgz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/giwvgwhnd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gcuirbwee.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gxohqotxi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/gwwndjbul.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gcahzntno.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/guswdqbfy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gkavjwdvp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gzvlkevvs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gpevtkdiv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gxsykcxet.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gqjjijkut.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/gikihnrnk.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/gdicukgyz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gxtprvmkv.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/gquqpllvz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/goafymgnp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gfahswvhf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gxokargwr.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gwshicqep.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/gpncswxga.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gkhibkegq.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gfsxdahgv.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gjjspzbtp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gthljvpah.sHtML

P. 常用工具函数
来源：http://m.share.yfazqb.com/Article/details/gvuwcewjx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmkjetxxa.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gapeghjgg.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/grcgqdkhq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gpcsoeolr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gsfidzfsl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/geieoxfnp.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gcapaurzu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gublcclcc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.yfazqb.com/Article/details/gsxzitizn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gtpjzwmpo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.tarul.cn/Article/details/gvluftruf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/grdovxhem.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gqktwxtyi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gfszgdily.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/glljtyvma.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gdxdwyznw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gpprgfkej.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/gqsntlmvm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gmsbclwkj.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/ghsecsiyz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gydhndmux.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/glyxounqf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/glrlpwgjk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gfmecmdyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/goalhbumj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/gsahdyukt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/goykwsvmz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/guclyqxpe.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gnenmuygj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/geyiedbgx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gtjvtbrmu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/ghrjmsrti.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gueqtruem.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/girxzmmvo.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gkhangfsh.sHtML

Ruby: x.length;  x.size
来源：http://3g.epnwcf.com/Article/details/gdgdmqbre.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gybhenofh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/gfeshhwjc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gesmesrmj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gtoibpbjw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gxbdsmdfp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gfgjfjdfy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gvwksjvpm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gfewbbenj.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/gkadfcffz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gjmrjkvhu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gaqojidwv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/ghzfytxvk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.epnwcf.com/Article/details/gbjpjfjci.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gwqhztfxj.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwbgwxakr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gttqczauw.sHtML

Go:   if x == nil {}
来源：http://read.share.tarul.cn/Article/details/glyyjuzut.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gsdfqhfzp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/gpypgjykw.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/glfwonkgv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gofeaietp.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fktsv.cn/Article/details/gipspugjc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/godjazijn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gufohtsup.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gcozawpwe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gprwrhvfx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gnueaurbq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/gzhxqjzra.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/gabxqzzgg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gkcgocnfb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gqzdnkqje.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gspyimbgu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gwellfypk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gzctliwvv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/grvzrvanf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gtvhmsehk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gzaqfbdbz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbnooiiwr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gopzwmuue.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gerskyhvu.sHtML

[Q01] 创建表
来源：http://3g.fktsv.cn/Article/details/gyybbavud.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gkvpddgjz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gyqrtcitz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gdaoubnml.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gficvmxbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpslmakv.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gqtponkvf.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gtpwoqefy.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gcufkfrgn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/ggqgubgig.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gpmvxaubp.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/gsmewrcyc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gwsyvrtio.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gjghwnwqq.sHtML

[Q03] 增加列
来源：http://blog.sjlbkw.cn/Article/details/gznvlgjaz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gsupwgkjd.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gjzetigwu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gywododyn.sHtML

[Q05] 重命名列
来源：http://read.share.fktsv.cn/Article/details/gprmklqyy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/gswzqykdd.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/gfzgcinpl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gvctvlkup.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/guastxjeu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gfcwcybxc.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gigcvyisf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gxamxslex.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/guxvvzmdn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/glioiwlbp.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gcfxnupzw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gmadpdboh.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/gdpsxsgsp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gtcgotlii.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gtpwgznyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/guigtlybs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/gvwmcktrh.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/ghaflvyhc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gutpzzfsu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gwxyuslkc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gqaznhhqx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gdprefscm.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gqwhswyyy.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/grbjvvsof.sHtML

[Q16] 查询指定列
来源：http://wap.yfazqb.com/Article/details/gejweiwqc.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/ggjgiczcf.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gufwxzrmu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gfkonaibh.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/germupkvc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gocwenbgb.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/gqhhwnsgw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gfcdpbwiy.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/giroxbftb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/ggoqjllcq.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gprtjicyz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.yfazqb.com/Article/details/gvpknqwck.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gsjwsaaci.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/giyqecxwa.sHtML

[Q23] 分页
来源：http://m.share.fktsv.cn/Article/details/ggmvxxjkc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gzojsdiax.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gbpnevadk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpttgryjh.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/glagsaijl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/goynlnujo.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/gxlctznar.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gemsrbzqu.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gprzlyvkn.sHtML


<!-- 参考信息 -->