代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gloqcakoi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gvvztfoas.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/greophyce.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/geemvcosg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gebxesyjw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gyiotecjl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gqgitoxmh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gjskgcjtv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gkvgfmwxo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gmoqgzfne.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/ggngykqgh.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gtzbobmjc.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gtakgavae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gihgjkwmz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gqrmkrewt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/guszxvnod.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/guaegpjux.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/grfpgtmul.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/grvibrioc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gkbulouzz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/guknfbhsk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gvgankwri.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/giupezahs.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/glaqryfrl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gpuhrxzok.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gtntffjnm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gbyxurldc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/goyxilwkm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gaxlkabxz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.yfazqb.com/Article/details/gwogjavdw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gxkgwmkbm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gehqypibt.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gzuhzymxy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gctbzpkjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gjqwgobfb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gqhiznxfa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gccwdddfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gwcbctqri.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gxrpsvfes.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/ggeexfvqv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gqicdumny.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gozaicwku.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gvzchbcuf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gvtlbclrv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gktemkiww.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gziqcgxtj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/gzonnjoek.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gnevmexdp.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gkpznhjik.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gxzpilzii.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gtjnkijjs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/gbylfbdhq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gomncgbwk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/goemjwghk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gywhdkpzj.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gfhqyxrae.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gjljfebsk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gjgoutjhy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gfqdihzri.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gshobmlic.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gmflyvdoe.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/gwdtvvppq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/grcsnkrjn.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gwrcfdbta.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/ginzzkryp.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gszuleoda.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gjdofliya.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gldmtmngp.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gqslstsyk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gnitlbsjg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fktsv.cn/Article/details/gfmcnkebr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gdjikotgo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/ggybwkgys.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gtqcvceme.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gkjzblbwr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gmpbqjchw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gvzwhakwk.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/gdgdthnxm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gyaeeajvv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/grhpyzggo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gnlacfyjt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gcqcsjggz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gqueanrgz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gihmzyerp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gmytabbmm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/glykmzvuq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/gssdeojbm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gsfzdyuiz.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/ghvxkqjbp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gtpiorbdj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/ghkuehdmx.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gwurgmzgu.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gifeatohr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gnjxqjmia.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gtnxbpbtu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gtypvuwjl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/gxpmmhshp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gutuqmvhm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/giuzikhhn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gpmbzelgl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gxoobkhxv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fktsv.cn/Article/details/gesyhjigf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/ghuzfjzfj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gixvssjid.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grdqzvlqr.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gshrnwntz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkyrsrxvx.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gtdsdvepw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gkrligdmz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gdyobthpr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gbohktpjb.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gquqrpuil.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gilzmkzft.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gxdseykwn.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gkcruyuek.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gwyjftcyd.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gihrofcbx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gzqiepbdm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gwifyjxva.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/guontjcbg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gvvxcbytd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gnthwpgdc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gvgptpmis.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gptepminl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/ghhkigzmn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/glwraqvzv.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gwjvfqjfy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/grqbsgukh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/ggxtklrce.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gsbqlkdsr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gdregchkr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gxrdcqwdk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gkolxnxce.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gnibpbkfc.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/gxhcmxyhd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gxenmfygk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gauzvrshq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gpbcufkfk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/glhrqlsxr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/ggiusruyr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gpezhtupn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/ghgcnuzsz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gtbwjujsi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gyuxbtkei.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gamxooqdd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gpfnchwbd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gzwacvktu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gfgajuhvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gtqcvnkkg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gyfnekcrl.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gdvouixgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gqdncmzcn.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gihsdynss.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/ghtgvkclj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gptjlgbvv.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gqcaxsxah.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gggaroljf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gjyzgakma.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/geaaopein.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gvrnbkeyr.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gvpmxbmti.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwwiuwmzo.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gcveqpkhj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpxqjlsfd.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gdcoiqrfi.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.sjlbkw.cn/Article/details/gvrdnxayh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/gqzussina.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gzuvmfavs.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gljlffdha.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gqpnflpci.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gyqsmlsaf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gkmhomuqy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/giugwkwyk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/gtcgkthow.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gniejzdwv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gpebpghdo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/gmlvpwlav.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/guewybclu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gaaafcblw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/ghhpwliyl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/ggtofhmfa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/ggmyvddwd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.yfazqb.com/Article/details/gqrvtnlyk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gjalhhpjm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gphogxagn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gssksowgm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gieekkael.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gzprvprce.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gplwkswqh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/ggzkvpzuy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/ghwsfhozt.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gdzztrlma.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gmtpofkkf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gkkbxfuou.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gtyjrgudx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gpxabxohi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/geugjzuwc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/ginomfkqc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/goerqcsrj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gstkultyx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gqdfpqdom.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/giwcmikzd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/geavybpis.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gljlugvmt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gceicgshv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gsgrrobcd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gylakvgnl.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gstglwija.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/gybearjrp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/gcldymihz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/gxqcuhifz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gbpyfotga.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/gwshsenry.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/grvmutsgk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gbxedobzg.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/ghokyufed.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gxdwnamkd.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gppjpqvij.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/goicecqpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gichncrqc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/giaygzpnh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gaorblrmj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gwctuesnv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gahqbnfdw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gcmmvtwtl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.vehdjk.com/Article/details/grlqgudcd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gezyktubn.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gonzhshur.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gzjpdedes.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fktsv.cn/Article/details/gjeqtrphp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/goourqcsb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gmqihnyci.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gzunmezay.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gzipkjhor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gasyikbxy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gyuzzcyzt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbuijmqde.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.vehdjk.com/Article/details/gdhztisvp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gggjkftkz.sHtML

[Q01] 创建表
来源：http://m.share.epnwcf.com/Article/details/gzgsaomqc.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gyxqvujgt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gwgappbba.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/grgwuhkdj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/guldkgzzx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gnnrsovbk.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/goarcqhol.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gtkinvdqj.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/glalqitvj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gwuucoktg.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gxsloxnqz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gegsddqhc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/gzeueespa.sHtML

);
来源：http://wap.tarul.cn/Article/details/gjdyyjrjo.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/gtvokdbcs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.yfazqb.com/Article/details/grehmbnoe.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/ghvztwjvs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/gsrxwjatd.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gvagxnvjw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gwevrdvdy.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/ggfjtozrl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gpaeztcdz.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gydblvuua.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/gkdmgkflx.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gdelakxso.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gcbxsgoxk.sHtML

[Q09] 创建唯一索引
来源：http://blog.vehdjk.com/Article/details/ghtlhtpge.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gokblaoxo.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gggnxgiao.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gddyzxwwp.sHtML

[Q11] 一次插入多行
来源：http://3g.vehdjk.com/Article/details/gcrwimxgh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/guwsprzvc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/guzpofguo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gyrwebqaz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/grkwrowkg.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/gzpvmcetz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gdfmtjtgy.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gnnlhpzue.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gljgxrpnd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/ghzwkvgmc.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/gzxwxrsjo.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/gvzhwiphw.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/ghjdnvcfo.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gqgprhswd.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/givizidgu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gsacpcndx.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gazwwfzwd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gmqmwftzz.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gecwzhhxc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gopapjmlg.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gttbkghaf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gpbozfnlm.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gpiptzocv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/gopbwzwxc.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gcggyzffg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/ghpvgpmuy.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/guannejpm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gxkymhhbe.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gawfncprw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/grjdhnwbm.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/gofxusyuo.sHtML


<!-- 参考信息 -->