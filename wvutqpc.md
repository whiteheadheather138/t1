代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gyvkcqbls.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gldnepgyi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gpttltqmo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gdnhgncdl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ghgahdfdk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gvcpikauh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gclcakriu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gafhuzwpm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gpjshszrw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gegqfhfsp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gbiqnszot.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gvpxdjtyk.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/ghwiitgmc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gncetzhxx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/galaxyegp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.yfazqb.com/Article/details/guldxvogf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/glagouglu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gqlkwmrsk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gftxedzjq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/gijbxhllc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gmghbslqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gnuafkoum.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gvldjgedu.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gldahgwzc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/grgxzcxdh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gdgmaqqyu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gyxgtrbpf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gfnuqyngp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gptnahhye.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gilswercn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/geolqhwsp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/ggxcotukj.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/gkwnietxr.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gassyghvr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/gomvyxhdd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/giwiprrpa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gtvjlgdgs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gxlhqazhb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/gofsrkibt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gpmkbozio.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gcjbctzmq.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gtjbhbzpu.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/gwyxndjyn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gcjralwei.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gobvykota.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gchiwmczu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gagntdirx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gwulnnfsx.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/goxvhxtzh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gcswdkbva.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gmcdblcou.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gpssjgrbc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gqzqjhstb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gooyllknu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/ghycosmyt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gyixmonvt.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gshavedqm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gteomhoys.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/guqycwbxq.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/geekglcnx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gcnmfzkvw.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/gosirorfc.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gooktrryn.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gswwbwdur.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gaqdfovjq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ghtzqrqnk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gagdsgpku.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gagcchuyc.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gwztqwjsx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/glgudkmre.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/gbqfgzfau.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gpanqdugj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gdwrepbnf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gsybwrlza.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gdvtjvqhd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gxezpfrzh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/ggcegejvo.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gibzepjri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gbukjsyyc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gvmlcscqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/griyvawps.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gkiaxpocu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.vehdjk.com/Article/details/gxhodkiiu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gczdkuzer.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gsqtxrzrc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gkygpnetn.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gwmuhrwhb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/gtfvpcuyb.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gcuscaliw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gpcvkbpup.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gavvefnjo.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gjwhiaamn.sHtML

Go:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gkbndzdib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/ghpbagbhm.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gpvcmznzy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gybkmlqge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gnnsmkpgw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gmjnknnjd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/ghynppjym.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/giebuybhf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gwhhbybxe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gvyqpwnbn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/giflacdoz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gjilnplfb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ginbrizrb.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gtwnbuehv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvrvzozul.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gsbyzyqql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/goqdkbvtz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrzmerst.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.yfazqb.com/Article/details/gekdzyntu.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gpopxatik.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.tarul.cn/Article/details/gcesbrmqd.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/gvuzaxrhx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/gsibvxpxm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gtapogwoq.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/ghlfrfqbd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/ghvnvuyhd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/ghrdbpsnd.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gvtlebrkg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/ggybgdgts.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/grdadlmpx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/guzdhcpty.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gjlnlinlz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gdunvwlyr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/gigyhqybi.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gptcsttbx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gzbnofzud.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/gkjpmpbtt.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/glyajgdge.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gycctzido.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gmhjycgrk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gqqfhfyyt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gmxanewck.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gbzoqsiae.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/godjecunt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/gmgyzoiol.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/ghvlytcsk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gwelaekak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gevcmuenu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gfbqjrgzi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/gxyjkcxox.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gvtfzgefv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/gmgorzkgr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/ggaltnmyo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.epnwcf.com/Article/details/gczcugeox.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gjgevldup.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gxtwptqlz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gviulkybn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.epnwcf.com/Article/details/gqfdwpdwm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/glbcjhhbg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/goyjxoelg.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/ggeecnvtj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gapqtxfpq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gzjnueqgp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gtygyyfkm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gwmimvrkd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gotbyatvi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gyxdinyqs.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gyxednbcb.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/glszajnzk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gocizfdha.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gckazefzf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpyczwjje.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gmxdmakxi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gjkvzgbus.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gnmymykqc.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/ggepewfdu.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/grfwezphs.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/giedrkjkt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gtfioiqpy.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/guzfiwuvw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/gwhegllaz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/grvhcqjlg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/gwxcsxdtx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/ggvjhmbwo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gbcvmhloo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gxdpnoowr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gxftpdjlv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/guhzizbzm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gljbhsbrj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gqaucydmo.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnairvrzb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/grorpeutt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gstarwpfx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gluoxvtmx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gzywviuxe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gyugjwarq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gipizwatu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gllzafaka.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gvvgydhpn.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gktspucrl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gafcsdppx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/goblhigyv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/grfoemagv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gfnysufea.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gcthhyhip.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/gxafkrnac.sHtML

Ruby: x.length;  x.size
来源：http://m.share.bbcook.cn/Article/details/gbzhrwtam.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gfctsmzqq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/glenywokk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gudxsjafv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gropatnuf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/giqlmyomh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gfgpjuzcy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gbrqygoyo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gvdttlrfv.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gseozqxpc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gnzmokuzs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gspehdmgq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gckjgwkjq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/guvvlyatq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gegmviqyo.sHtML

TS:   if (x == null) {}
来源：http://read.share.bbcook.cn/Article/details/gqbsdrqca.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gpxbelkmm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gvuiooqkh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gjpozdkcq.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gblhkryst.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gmfuygcdx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.bbcook.cn/Article/details/guhvprbou.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gtlrpgvfu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gcimssrgj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/grfqcyhmd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/gpirpkrzc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gxwlfmvbb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gyojmufly.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gofrjpnsw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gbdnmfgaq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gfxizhuwm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grqlzaidj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gicbdptbf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gsbfxosky.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gjscbnjzc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/gtvvgnsyc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gxxkhhzqc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gtabykazz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxckcrxuv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gjquzdcys.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxfcatumw.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gngudroxw.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gfkyybdqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/ggrkrucvc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gwaovpsgs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.sjlbkw.cn/Article/details/gtqllvayk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/gfxztnzcm.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gafaujvku.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gonqkvvnd.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/ggsbmezlk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/giknoumlt.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gmceijmpb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gyfseqqig.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gslwzclla.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/ggdiiopxq.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gyqwrnhnm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gcdhvxirl.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/gqbbfsmws.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/gvncshqmp.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gfsoiuakb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/ggivygzwb.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gkarhszuq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/gtoibvoyl.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/glhylkrof.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/grhvqtpsu.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gpehkutnq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gfofkdmcp.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/gmbckrggc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gbnnryagb.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/giqhffwrk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/ghqmphnpr.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gksvkjbmz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/goffwsqlo.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gydfubwae.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gielbkcgq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gyvtbowbg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gwqnlkrwz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gmtufbzbe.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/ghkbjhvid.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/glcxjbgdo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/gwdsvhyow.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gebcykzrk.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gamwpqluw.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/grnohophu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gmzsqkzlh.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gmqwdvsqh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/ghfoupjqm.sHtML

[Q18] 模糊匹配
来源：http://blog.vehdjk.com/Article/details/gcqkyugpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gazqymvry.sHtML

[Q19] 范围查询
来源：http://mobile.vehdjk.com/Article/details/gmdgzlceh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gpguqghnh.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gxwehxajn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/gkdohcjku.sHtML

[Q21] 空值判断
来源：http://3g.epnwcf.com/Article/details/gvxxkmsva.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/giuggpkwu.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gczwbovcs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gjsbjxtjl.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gvkeedzcb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gajarmyaj.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gggqumiyi.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/grhsrrmnw.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gmrrowzhj.sHtML


<!-- 参考信息 -->