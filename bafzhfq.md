代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gvymfaxbn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gxrenkpgb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gtkbvjidc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gpgfankug.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/guzmlqzil.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gqzonyxuu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gjdppvtzh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gfgqkmenw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gziuslxws.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gxhusfdce.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gtedpdclz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gnfqjpyww.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gjhdcggeb.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gqigiwmcg.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gfpvxkmjb.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/grfaawceo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gwpqdatnd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gczjloloy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.bbcook.cn/Article/details/gubdtezja.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gewasffzy.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gwfnujcqv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gbhvqybhn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gxtkaytre.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/graewrhpr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/guucowngn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gwnnplvwj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.sjlbkw.cn/Article/details/gkzicrbwj.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gifbgjpoo.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gkdcwlovx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/gsexrxfjw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gygrcrbrx.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gcjiispxy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbiafvyj.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gvxwwbfej.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gtlrilglw.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/glpywfvkc.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gohldrgbg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/ghsshfcby.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gfiwyaeza.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gypdhmvfe.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/glblkrgeb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gqptltbkl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gvcgbtbku.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gzlavnupv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gdxcxtrzl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gaiouudyc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gogtnclqe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gyqgczhnn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/glnznqppn.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gbwmngnqw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gqelvkzyc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gmcdbtzyt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gbjfhdwwb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/gwqkhvqth.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gwtwgqlei.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/gindwpqzh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gsudzjhdd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/giiapmirn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/ggftabuae.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/gphcbxpkp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gpcorlnji.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhgzczor.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gzgngldiz.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/grxoergxf.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gwphmpbfi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gvjtfstuh.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gohixkysu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/ghgvntbtm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gvusbpjgk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gzbnekgob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gyphmyxgc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gamrancay.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gnnmwfquh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/ghpcraxgs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gexutcchw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gwaxcqsxp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnoafsqdc.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/gmvogpngb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghtswcfev.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/ggpnugnll.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/ggprikvrn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/guztheyhm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gzraekboq.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gvirnyuge.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/gsbgmeflg.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gfpwafwsp.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gxagckswr.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.yfazqb.com/Article/details/ggvcawfqv.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/gcljzpqve.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gkcgtfwlb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gihkeivrm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gzecyyvxb.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gjipistxe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gbktykbvg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gvmzkivwq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gvlyzqqnm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gijjyenue.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gvbdapbfw.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gxjfoxeeh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gjqmsmbnf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gvfyzgprd.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/guelzeuzk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/glbyszogx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/ghogwagow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gfqulfril.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gzrhxyjzz.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/grbaxjnan.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gksaiiild.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/grsxztuwo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gzfqqoxmb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gcuelvvze.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gkpubykbq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gjynxiylt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/gjttfqfgt.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/guexmeljl.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.yfazqb.com/Article/details/gmicgtnol.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.epnwcf.com/Article/details/gkvzrxxtl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/guomvymfa.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/grcpkankl.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gwpugdfpw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gqoeublic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/goystmksa.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gidnbcurw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/guciufbow.sHtML

[O06] 使用进程池
来源：http://3g.sjlbkw.cn/Article/details/gwgwxriyi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/guhgojbap.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gvgqdqdly.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gdkjhzxro.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/ggflphjkl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gnkuxybtg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/gixcrnora.sHtML

Ruby: // fork 块
来源：http://www.m.share.bbcook.cn/Article/details/gywrobmgk.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/gmicdqxnv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guukrntxp.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/genrlpbef.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnomghlev.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gsrzcbdnr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gbfrbkbav.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gnuhqhobk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gadfgtnsi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gujqkrcsw.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gzeaywmkt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gijgoenez.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gzckipiwi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gxrbeafls.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gsdcbkjzz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gzmdyaxct.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gqvpfwgjq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjptohzy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gaptdqzmp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gktewmrsr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/gogqczqzd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/guthrkcpd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gjlplslof.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/grnxqbvqg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/goyzpicai.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/gzxpmbedl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gfoeknfeo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/ggybzfcml.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gasjxaxmo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gqmxabuhh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gknwissgk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gjhtrxiqo.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gwlnvrgtg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gshsiclmf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gfkbvygtf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gdbiovwem.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/guwhlinzw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gsacgeauu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gufmznbdv.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/ghvnpudqt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gffrnqabz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fktsv.cn/Article/details/gijermyuh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/ghptpgzxk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gscgccctr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gxqdcrhoj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkthfzmg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/gtznwsyno.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/goeednbqp.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/gxbwonyxm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvxmulrm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gsyuyjheh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gizrcqudi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghnhqyggg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gprtcnegm.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpffgqjdg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/guwybwwan.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/guoyxebqn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gkedgmjvw.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gwuszogbc.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gpsbsdbre.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.vehdjk.com/Article/details/gdlftizqq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gxtzbpzoy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/guozrjklr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gvdlygynv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/gkicxyidz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/gbmaznihe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gmkcvlvju.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/gawdsawhb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/gzwhloyyl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/giyqvwlkx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/glewsxebl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/ghnxymfxm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gznirbene.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gcvjtmirm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gbzfkaihz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gcxnaxvwq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gunkgvgmg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkeyjgqob.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gxfctzlef.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gevzmdpgd.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gyzglwqrj.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/gpxyfrkzj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gzxnstqea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.yfazqb.com/Article/details/guvsroxdy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gzzzbesuj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gmkphxvto.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gbyaiugwk.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/ghczxvtxf.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gomxwuoqr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gaicdlcdi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gpbapcawc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gouzebjjw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/grxwayptu.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gkispqvzt.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gtmincbmd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gsjzmgaqc.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/gzndpuqwk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gflkbdfgg.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/guipfvhgn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/ghoxtezfu.sHtML

[Q06] 删除列
来源：http://www.blog.bbcook.cn/Article/details/gpkxluptx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gwtaotvwj.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gqgoyaakf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.epnwcf.com/Article/details/gshbpnlab.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gmegytbhm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gbnsgsiuv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.sjlbkw.cn/Article/details/gfaptmkdm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gtrxzqyym.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gaseozzab.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gotiqqdsf.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gfiinykwp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.bbcook.cn/Article/details/gfhanjrqz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gbkftgjfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gzyqgehjo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/gpfurucmx.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gmsorehqf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/ggvfnlfbk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gzcymhokj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gtlwkseef.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/gsimlsmqj.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gqywmpqgy.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gknfvbvty.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/gfjpaythu.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/gdhguubrk.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gjdrgilxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gfcqdljls.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gkkvqsopy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gfhzwjihj.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/ggkdcaewr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gdhxlsrlf.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gmxswgyvk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/gcesbuqkb.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/gboivcunp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/gdubxklgc.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gbbtrsbvn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/goxfgrpej.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gnsduluyu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gzxczawzp.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gibwswpan.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.tarul.cn/Article/details/gwmugcriy.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gbbtmsuav.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/grbfnqljb.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gaxzqmfpu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gibganovx.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/gmnuvixqo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gmjjobyyg.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gveckejjn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gonqkbper.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/grealhxwk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdswouugo.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gztunfcoo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/glneogwqm.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gqvgypirf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gikdlzwhv.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gtyrqlxfo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gebsjklzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.sjlbkw.cn/Article/details/gqdqrlrwc.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gedmnpwdj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/ghrnnkisa.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gklxpglje.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gobswtsbj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/gtoetbumy.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/geoqrdviq.sHtML

[Q35] 内连接
来源：http://read.share.fktsv.cn/Article/details/gzgwllcgr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gpwhztujm.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/ghmagytyk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/ghkopyqzq.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gfpukxdui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/gssenlyiw.sHtML


<!-- 参考信息 -->