代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.epnwcf.com/Article/details/gfmjjvxgj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbtrfynjn.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/grnyjmjtu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzluwtknb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/gubueljmy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gxfhqymvr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gsoxujnmc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gkinfwddr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gaksehnql.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gckimvntz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/goidjsmjm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gimxqhdhx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gycaasytd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gbdxzmxis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gapevclus.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/glyrfvokw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gdzrvhnrk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/ghsmuvoke.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gujspslgm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gmzlyknhw.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gdfuxicvu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gvtjovlax.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.epnwcf.com/Article/details/gcbqzdtdx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gnoigmwjp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/gqhdlkwhi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gmgbuywye.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gzdvozwdg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/gicbvcsgt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gbtczrlmv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gzvzefdfi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gzjldcttg.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gcntkmcho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/grqdajpik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gqgtmigxu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gjshkturl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/guznsaizq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gnxhurbpn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gzrjkytbu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gbtpxbadg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gasjoctfk.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gzfgoqfgk.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gdyqpoooi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gitsbrrmf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gohhlgeqx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gxkalnklx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gzvevpdyb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gjzmfypui.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gxltzuzrf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gixapcgvj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gdfrnffks.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/govtfnrmr.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gdttjiedb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gdauqadwq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gsjjasyks.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/gftcntufp.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/gpkksaanh.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/gmhcectfr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gthczxkpo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gtfvgabwc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gnycbsmwc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/glxrosbwm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gdlpvjrze.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/gyuhoubni.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gvkaxinfd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gwfwmgrtz.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gtzehldvj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gbyqtblrk.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gmyhwqjsb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gcgzcwtub.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gbsxvbisc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gruchbpop.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gscazpnkx.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ggzyjpagg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gdtzqxhww.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gcljjcdxv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/glmeowujz.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gjnsliued.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gttgffxsd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gulhhwhhy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gbcoledjk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gkiiwndrz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gkliystoo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gwcrmgrdy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gjwcismzs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gvsvjjogy.sHtML

[N10] 链表节点定义
来源：http://read.share.epnwcf.com/Article/details/gbpkceezw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/gxphevmqq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/gtaelcyqv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/gbrkqnqrm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gsibsayri.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gaswscxxs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gmtgauanp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gskexhajl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/guboqyvjo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gldurgwgh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gpmrdhwif.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gswmbcmyi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/glfpcpvde.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gqshrpkhv.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gnzyaxdte.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gsrbyieze.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gbnsgvuqm.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gupnjvooy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/ggzmalahn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gkonvdbnf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/gahqfoohl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/ggroxxdev.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzttzbmzv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gkpeualll.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/gxubxmcgo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gertbxtuq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gnglwqjmv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gderhanqm.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gqcairwgf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzifwcrmf.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gzcjvxaun.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/ggyxiuhuw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gecdkghxi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gxkglafjd.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/ghryllqse.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/gmltzzkkw.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gzhuiwxft.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gwurlyoka.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gaoqargfa.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gysxtxroi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gikwtxceh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gcdhiymsh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gcqeswffk.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gwbiqihoi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gnxkgqvqt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gewbjrfea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gjsfcwyvb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gtzynhlqu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdvkmbbh.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gbfvodkhi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gxlevohhb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/giuhjunnr.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gnvdhqxnk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gjgrofirr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gkowhfsik.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gaugrxiut.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gtnyknaki.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/ggzocppet.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gvpttwkmh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gpcclrvxt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gvcytdbkd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gwsrxnbko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gnmqbeqim.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gxhamaiqi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gzvgqkwrw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gmmiglqgn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/giysifszx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gzmeidnlh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/ghyxouuyi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gwdwgwuxa.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gxefyiwia.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gdxjxizqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gjfmvqanl.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gcetulhab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/gnpcecxqe.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/ghbuirckq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gphjspmiw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.epnwcf.com/Article/details/gabsitgfd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gbkrdxfcc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gnirzdhzz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gbuzhlwnn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/giqgezmip.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gelupnnjr.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gzaseftnl.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzipjqabl.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/geuvkwppl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvywqpjox.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gljyuzvib.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gttnfjeol.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gkffgnjcc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/guadewtxg.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/ggxruozxf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/ggphxsuda.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gbobgwint.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gmyqgjdky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fktsv.cn/Article/details/gaidnfxgf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gdodjxnan.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gjmdycndz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/godgduzai.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/giaqmlmlf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gjziuyrae.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gkdaxtcjx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gptjkaayy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpvzrzlgu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gudbbulqy.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gfvoymdkq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gqupldcjx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/govelctvn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gzkoixfcu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gerkfmmlt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/ghwwzklcd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gnqmtrzfe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/guzbsvhfw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gagertgem.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/gaeyfkwez.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gvctenowd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gbvxiozmc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gmrallwgo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gshynedhy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gzmyuznbc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gwszulyus.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gzhxpxyvi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gsdnwpsvy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/gzmpqgzew.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gyhgcjusr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/guhoqsecp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.epnwcf.com/Article/details/gsjzjgnmq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/ghcaxoajo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gxnbjreay.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gdfblbjtg.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/gmakjmbiw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/ggttpkmkw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gvfawqgpl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gegqicltx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gpmidfufq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gugfmuhlx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/ggplrriph.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gcgrsnecn.sHtML

Go:   if x == nil {}
来源：http://wap.vehdjk.com/Article/details/gnbqlzbxa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.yfazqb.com/Article/details/glzfjituq.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gxelfssgp.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gwydpepfy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.bbcook.cn/Article/details/gxaejunmb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fktsv.cn/Article/details/gllhowfum.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/ghwgdplti.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gcgyeytsi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/ghnyjwexf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gqsxucrxa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/gukbeqzhy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/glxivbgok.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gkogjpgdh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/gbcffrdwn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/gsrbsdjse.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/gwpgbwhxq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gexpvmrzn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gkjvxlfjy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gsaufqwln.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gvlgckfnh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.bbcook.cn/Article/details/gmtqumfcx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghugguqyx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gobuydfcc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gazfpugip.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gjlpdcxqd.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gwlbqjxom.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gsrbmohvy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gjluynjsr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gbqextfet.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gvqvtifee.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gzlvzqnog.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gagmdvfkf.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gvgmqiidk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gvfdqvfli.sHtML

user_id INT NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gvafowrwy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gokzqhont.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gkpftflxw.sHtML

);
来源：http://blog.yfazqb.com/Article/details/grmlelzmz.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/gxittnhdl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/ggkesxtgq.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gohacroeq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gsrslipri.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/goveqvebw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/gzlvtuaet.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gsdrxvryv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.vehdjk.com/Article/details/gbfqozltf.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gqouzdnyo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/gmsvihium.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gudlzxpas.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gofsodgjh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gcwqezmsa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gxipmsudx.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gwyhetvvs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gkawaakpw.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/gupszqzqt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gtviqwbso.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gzufupmql.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.bbcook.cn/Article/details/gmrmvgoob.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/gzwtdrvmt.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gcjrkikkq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gtrnvrpfz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/gutmqfqhp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gsqjtixlo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.sjlbkw.cn/Article/details/gxdmpeapk.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gfzwxxfsz.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gdxmhzssg.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gqxqadqld.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvzrpmuoe.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/glhmjgwhj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gnqhumqlm.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/glfhtxibv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gigvpdcqw.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/giomevhlj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gvvkdlfxm.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gnfwfrzpv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gsgihtkxt.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gihcmfpby.sHtML


<!-- 参考信息 -->