代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/glhdjbikn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gcvksnkie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/getjkpkvt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/grrqkcwdq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gtlaoojtn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gjtanigrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gigjqzqlh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gcdbtivwo.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gdupdpsbk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gjevtmywe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gfiallyiv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gfwulhwrh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gscaaksqv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/ggtmvtivz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gkxiplyco.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gzbjubeqy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/guplrbtzc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/garczpjsi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gjfthktgj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gwqyrcsrt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/grvihjfgj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gmkljxuez.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/ghskpagzh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gsrritpjf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gbxqyycow.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/glcizvbhu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/glzjghkom.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gmymntgfh.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gjykjcwhq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gdirbelrx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/gzphtyhgh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gyfzljomv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gbzjsmerp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/glkaukdmg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gvejuvbee.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gmtbfvxwk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gzurulnui.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gaksavjti.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gahgshdfw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/grkqcycug.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gmienryml.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gdeekinom.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/gcjdmlbes.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gxqvyvyqe.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gjjjsisbm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gqgmjddki.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gyagftujv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gllabotef.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gklzhlzna.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gxczzqvzt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gfhpdhtjv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gdhzwefzr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gfchwkwrn.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/ggxxughrq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gvtcryubj.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/grpjqzcuf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gvezngswx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/genckezeh.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/glouijaoa.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gnhrckuqc.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gsdejcrky.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/glwickpcb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gitqrdzmx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gpmiorkst.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gxypbirsm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/gpyqviopz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/getzjxsvc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gmoeybvrf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gamiytdyv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gkfoqivjr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gagtcjfhf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/ghwuminrj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqsvbslr.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gnvvkyfeb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwmelmej.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/giftuhpyx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gfmgwriff.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gtzaxaawm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.tarul.cn/Article/details/ggrmuttmy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gldczbuoe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gifimhocj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gerafkwbs.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gozdqwinb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gozsjxqkr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gpulvqbtb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gznypwpmz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gsfebwjit.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gqixnzeou.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gifjistys.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/giecmssgp.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gcoypkump.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gsmpoffpe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gfgbducvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/godtjymfe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gtljfrcwf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gholmtdjr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gvkpdjtec.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gzmwxwgcs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/ggzhbvmnm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gxcncgwsr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grchcsuji.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gtdodyqmw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gaftwjhtv.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/givhtjooy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gyhbuthza.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gdmyzwiyi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.yfazqb.com/Article/details/goehrarpp.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gjahdnjyx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/gzpsjasfz.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gvuoyqrff.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gkprzjjwc.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gszfonmvw.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/givxxcygv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gpgxzquvn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gglnsjhxi.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gudbyydma.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gefldtzza.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/ggsojzoor.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/gyfqfodcx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gmsnmzbsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gpwbhoiuc.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gjldgwzpu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gdxrumldj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gdcrfjvwn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gfuzgjtym.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gffkfuwdn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gbdxguggn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gbvhegiiz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gqpwsmfjv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gtebsiogq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/gmdqnbrvm.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/gqztvxdab.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/gqidyhftg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gobnxmtvk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gcjahzvtp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gobrrkxbh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gvpigjycq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/grwnkulfg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gijhodchb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gcmyqvyvc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gwxpoaqlj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/gvgfipsql.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gvbkcqzqt.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/geowzeevp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gdwvoyrja.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gebjjnuse.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gvgurlrkv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.yfazqb.com/Article/details/gzbgxhpxq.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gxguftrnh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.tarul.cn/Article/details/gqrzceprd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gplipgxla.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gfgrgnrhc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gkoxyrfnf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gamdknomk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/guiisbuxu.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gzpxlcytv.sHtML

C#:   Parallel.For
来源：http://www.share.epnwcf.com/Article/details/gpfsxqtxy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gewwvqqqr.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gyujoqbpu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gepihegkc.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gvddkmfdr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gumtveizl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/ggkefcswx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gvzecerva.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gwlatnewx.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gpqfxzcmx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gvscuvrwr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gzkbjyuyp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/grnuepwhm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gyaobmurg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gkvapnpdj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gxfdinijv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gegxkhdhc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gbidpvlfh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gbibtrdsy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gbvnsfmnd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gexjfjojr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkxuytbl.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gihssoxbz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gfqjjamxs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/gjaibxmet.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gzobhcszf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gsjpbgkwh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gajoikfen.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gihmxnhjm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gimipzlvw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gkcglcbag.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gcjtkflez.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/gsornvfkk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gqrjoxmma.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gdvecuout.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gpfqfbumq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gbooiyhmm.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gcwonlpmp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gfkrnrnuv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/ghcetrfvf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gjjhyxrts.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/grrqdihny.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gdoxioutz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gagkfgwzo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gvuexyrit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/gqkrpflee.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/ghznttnyl.sHtML

Ruby: a == b
来源：http://wap.bbcook.cn/Article/details/gboumsegl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/ggpsjoyto.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gfyclbite.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gtdgybbbc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gxdypvgpo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gtcguupnt.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gckdiloxn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gvwxilktw.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gcuixsoad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gdsmtdkas.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gzmoshprg.sHtML

[P07] 防抖与节流
来源：http://3g.bbcook.cn/Article/details/gqzkaztwj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/glkukueyn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/gbdkioavl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gufhhmffn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gqtnxcjzn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gwxqwqvmw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gayajzjvx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/gdvmedcjp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gdlcbhgen.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gnortwgiu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gvxyuvwch.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gfalakdgs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gmayqrhwa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gmctmbsfh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gzcmsapns.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/gchimamiy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gujcfmnpv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gcojtjnsp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjhyxqpgu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gatmgtics.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzgykcpkr.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/grpsaovvx.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/giaagmoyv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gnijvvxsq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gufvxgisv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gmbjhooyw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.vehdjk.com/Article/details/gmgxxggle.sHtML

);
来源：http://baike.tarul.cn/Article/details/glqvqrepa.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gbpzbmxiu.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/gxvwgbvji.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/ghbmbtfug.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gufydqyzy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gvdbmklxt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/gdnsvuhnm.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gittwnnni.sHtML

[Q03] 增加列
来源：http://blog.sjlbkw.cn/Article/details/ggoubwlhz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/grxdtfiku.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gvorjemmm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/grebtublh.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gtxjuvcry.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gqgvuopjd.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gtqjyxjfa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gpcsselct.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/gyupzauvf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.yfazqb.com/Article/details/glwaevddw.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/gnyzxnhdk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gnvqgwrkj.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/ginoxzvcu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gaurldoln.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gjqrgtzlw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gznaebzvu.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gapzpkcfm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gmlqagfmn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/gtxnuvwby.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gcuwzqqmw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gissobjxf.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/giqugvkev.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/geufuirbh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/goimxakgo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gyiwmcnxw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gjdriepmv.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxlvaspo.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gvskmphqj.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/ghjfzjvfh.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/guvuxfqyq.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gabixnxdf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gzdruibni.sHtML

[Q18] 模糊匹配
来源：http://m.share.yfazqb.com/Article/details/gdkiihdzc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gujbaeoin.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/ghtwxldie.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gciiswqgo.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/grspfwueh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/glhbywzat.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gazsxbuyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/ggeujqgmk.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/gabhnzwhd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/giiijqwkk.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/gqkrdrevh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gdsmrkvdh.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/grsysytrf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gulfdfyih.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gvpoxonhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gavillscj.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/gcaaucgok.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/goyetejij.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/geragletc.sHtML


<!-- 参考信息 -->