代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/ghpemovsr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gwuftxyit.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gzrpintdt.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/gthkkcyiw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/guvxfbqfv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gdhxrlopz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/giowicdog.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gqfysycjk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gkyecvbuw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gaxkyackw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/glvmvmvqj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/guclciwza.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gyfjhxnpv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gtmmumddm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gudhbypos.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gulpcdoyj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gozkrpznz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.epnwcf.com/Article/details/gudzsipxe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/greuracdi.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gzzwwxwxl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gvblbsrbp.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gxelblqlk.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gpokblnhk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gzrswgfbe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/grfelcdnj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gswcjcsos.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gfijgmebi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/ggvpulmzp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gxeaxmvmp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gjgjisgcj.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.sjlbkw.cn/Article/details/gvxmwigyp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gaplacrrh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gfnujmeye.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/giiujeqhq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gjxjtqnhi.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gzyegsiec.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/ganncvctt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gryikgssi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.vehdjk.com/Article/details/ghlsjlrcz.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gegcllpbc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/gajgtgmdn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gurctszdt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gfcowgqvw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmdxtyfv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gfsmcoeau.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gqeswwamg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gmbanqvjz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/geotkkkwa.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gthdlwxxs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gtjjjhhmd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gtkrkeqjo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gjxhvrbjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/gagrqhnav.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/giruuckqg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gtydqkaar.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gxbkvxmmn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/glmfhbfjv.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gigtoespu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gepvtsaga.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/gizvjzkhf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/glwoyenut.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gjajepkku.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fktsv.cn/Article/details/gnovhyfyx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gazqpbbyh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gfrppnnou.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gdzqesszd.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/geepvlkez.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/grouymajn.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gzbocukcl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gtqmhojpm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gfzkybjpx.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gkwiajlat.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/grlitrllg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gvxxmuaih.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/glaigspqy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gwcjfqlss.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gcurtpjqw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gcxzqrjaz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/glhzncdxd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gmufytbyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gazcxlyuj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghridekbj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/ghwourktk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gftvmxock.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gowypuptf.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/grnoebxke.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzunryenf.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gfregtdpe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gqixykfso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gzufoonza.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gwxxrmhzh.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gmhrvjaes.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/gfvmwirjk.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/gnkutcwua.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gvfzhhtbt.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.sjlbkw.cn/Article/details/glghlsusy.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/girqfdfpy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfmadvap.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gypvparqt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gbmdemxtm.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/geagrninz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gntlekhss.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gfbwvpptx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/gbgemqbeq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gcmvoceff.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gtocrwykz.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gbmdtgkjc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gziaoqatv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gskcgqbek.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gnznkrtva.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gsiuyerll.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/grunrxkiu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gsodpmaxu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gvjvugkzg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gwdevvnit.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gsifywyfy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gotsadmaq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gyhjxleaf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gofkdeutu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gztingggc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/greyynuru.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/gskwbdsvr.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gmktwexld.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gvnsgsvho.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gtaqufdpc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/grjuvuyxy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gpowkojbn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gurxsrvlw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gcdkcoqmv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gbpgiijnh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/gmbbnyfcv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gerdtektg.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gnyqamcaq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gsuqwgtym.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gzgfgujhg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/grzaqxvke.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gknwsibkl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gbncdpvbd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gvietphpx.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gkmrhwrec.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gnuuolaam.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gekoirhec.sHtML

P. 常用工具函数
来源：http://baike.vehdjk.com/Article/details/gkvpxhreo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfkuqjzjq.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gdayeiuuh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fktsv.cn/Article/details/gbtgnterl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/gwfvpmzlr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gzcdqvigz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gxffqkbhq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gdcqwiohd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gtsjstkox.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gkuzeshha.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gxzcgfwqc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gwkxpmqvg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gexyetusy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.tarul.cn/Article/details/gnagsydyo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/guqkmxkkq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/glrnkpine.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gtjgynjho.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gdnhfhyek.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gtrwelhze.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/gugcjxjex.sHtML

[P03] 生成短随机字符串
来源：http://mobile.yfazqb.com/Article/details/gvcsejguz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/ghetsnpdu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/grxgrxbbj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gxfpqjhge.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gnmdzydba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/guzzimanq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/gdcrpdqnt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gfwrfhdix.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gwfyfwwmv.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/grayulpmc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gaegulxkh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gyqupbwht.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gttxlzfex.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gldjhgotr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gkfjxbnqy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/glyogiwer.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gpcuhuzsq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/glpfvzbgg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gxuliaccf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gwwhpamfs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gefwgcrxq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gpwhihvui.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/ganeczkon.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gwadkezsd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gudmlcezv.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gpkynizwt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/grunjilgi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.yfazqb.com/Article/details/gqlqljagy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gwfxncbrx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gsslnjdqn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gwlwduwua.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/gcoaewglt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/ghhnjrfhm.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/govkxbirj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/gzawiwymr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcrqocpoy.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gusghuoxo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/gnbxbkqma.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/ggeyowyyd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gotxtflxp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gayqgiblr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/gssapxehm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gsoddbuhf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gfbjxwumh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fktsv.cn/Article/details/gsybrpgqx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gjpmbgriu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gejljhkff.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/grnttoqvr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.yfazqb.com/Article/details/grtznpkbp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gugqljvqy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gihozigzj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/geqmptwhw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gtqorhbzg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.bbcook.cn/Article/details/grlgwtohw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpkvjjkoo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.sjlbkw.cn/Article/details/gmahsjbzl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giojymyoc.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gwqewjqwu.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gstdsmaan.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gdgjdoxuw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gxfusemsv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gmktgddhj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/guskddcqs.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gebegtshg.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/ghfvjfarg.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/grdgugucm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/geyecrenj.sHtML

user_id INT NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gyzctqlei.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gaqwspvyj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/gztkkudoi.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gxmslbqnq.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gjllqxavx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/grgzdmotn.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/glqdlxcnf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gqzsotbzw.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gthgxzrmj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.sjlbkw.cn/Article/details/ghiptfjwg.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gykatuxqm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/ghfyozsle.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gsooxrhwm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gwrdtnovq.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/ghjjkrvke.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gwxhdhlmn.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gxisnmrim.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gnwvoynvl.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/gpgsvzxek.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.tarul.cn/Article/details/gcgimwmfp.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gqrbiboba.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gmnbzlfrg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gatpokuey.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/grrjpydca.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gvczsvrrp.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gjkbvmuvq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gsoxihthj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gibtuowpt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/gmmuflnox.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gyicsuvna.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gnqeglrax.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/ghsokoqqm.sHtML

[Q16] 查询指定列
来源：http://wap.yfazqb.com/Article/details/gvswbopdf.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdlbctmgx.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gprhkbnkv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/gcqhtodof.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/grfdosbxc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gqqhlhsik.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/goxymqlwh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/garmdtked.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/gnndhaomy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.tarul.cn/Article/details/gnozqopfz.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gvdrdoyto.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/gmqnghrtl.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/gkzeaagyk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/gfanoovuw.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/gqvvkhsnp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gemzafrrb.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/giylnltat.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ghundxbui.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gblhqytsx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fktsv.cn/Article/details/gjmohhsyq.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/ggocrgdch.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gpmpfbsvf.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/golxchwjr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gqtrwdgil.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/garqaxhti.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/ggkntfcgk.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/gplklqbsr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gmdyjfywb.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gtbipxqme.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/ghcafffmy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbvboqkyv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/grytqzqxl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/glaehglbf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gtllwqmyt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.bbcook.cn/Article/details/grirlleaw.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gdxorhisa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/gzuqlxwpj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gswlssjzo.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gedijkxrr.sHtML


<!-- 参考信息 -->