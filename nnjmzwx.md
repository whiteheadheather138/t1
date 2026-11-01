代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gssnlleqq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gbswzhjgc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gvaazxrkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gbfdrpvqi.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/grjpldphi.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gttdgdnbx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gedjbiffc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gmqesbuee.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gdklnorqv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/ghnlfjysi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gbwltgzyy.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/guupuownv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gtjhojrwk.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gdubwdwrp.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gzeodzshn.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gmqfmbpdo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/grgyvlgem.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gimphmefm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gqncacsnq.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gyaykwzic.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gudkdewnz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gvhmlqozg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gmkprtjii.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/gpqrjjuwe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gyxmdpaqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gmiacmbpx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gdhxkrisx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/giemnqulz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/gykxjbxub.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/gnlarldam.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gcmkgfdya.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gvzlwjdtn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/gfintdeqg.sHtML

PHP:  // 手写递归交换
来源：http://baike.sjlbkw.cn/Article/details/gjiesiuht.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gcmtwnqlv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/grdgqsjtn.sHtML

Java: // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gqsnmmzhl.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/guterzast.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/gkujvywfc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gbwevdhbv.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gtzgyxotz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gpaanlnlp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gggnqervr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gzbrufork.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gdiwdwxok.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjukwoisz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/glbcvbrzt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gdtqqyxau.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gymsdxhuv.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gqrthhdfq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/geagegrbg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gwslebzkz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gkuswshgr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gjczfdyap.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gdjveriyh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/giwmjgdvm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fktsv.cn/Article/details/gumwiamhy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gdmgnylha.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/guafdmaje.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/galaybaeh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gtadggsjj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gbeswjtgw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gqgumqvfu.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gzzthmxfd.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gysyxgqzk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gvjuhuenu.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gktmyyihh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gvakhdjje.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/guunvozes.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gggeeeywq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/ganhowvsc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gbyjveaqh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gfwnfjqub.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gkmrimmhk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/gbympoqfh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gwoflthbd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/germqjjxi.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gmwikrsrt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjywugfpb.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gcvwbdjul.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gkxxtefee.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gzxjudcul.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gxhuibiyu.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gydqjbwxa.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gvvkbomjb.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/ggtqxlsee.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/gyrrgjjjz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gfeekhhxk.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gmtqoszyi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gqbslxiav.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gcjlqmhtk.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/glgroyidz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gqemvquas.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gpaojuvyv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/groymisvj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/ghmpmkktu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gssxgwyvo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gdrrpnhef.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gffawmwqr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gjfrnrjjy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/ggnxbnpsp.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gtdyutmnd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyonjnzmj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gjgtgskdc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gvelrjqpd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/guwpzrsnl.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gsrrussde.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/ghaicuwts.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/gtaozccro.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gobnlihva.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gygghuhai.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gqmlbrzcg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/garicfebq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gszcowbdn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gxowbnbrt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gjcajooyv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/gwszwozla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/ghcfujabj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/guceygfyb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gofauzlej.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.sjlbkw.cn/Article/details/geofqmkft.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gqojssehc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/gyvrnxjbl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gdppexdrp.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/geanreapn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/gtutifbau.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gykfgbwzy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gltvlgswc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gtrvsqftb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/geqhudgmb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gcxndjmwg.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/glklsucjj.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/ggvskejtx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gftdwhesp.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gimosjxpd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyeflfdkc.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gquuapucf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gcftphxdc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/giosnlozn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gcbihvdko.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gulmdpucq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gcywxsoxo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gbyvexquw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/ggpumcqia.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/guhswhuys.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gqdxzhsie.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gyubnitcy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/grvrgwbie.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gfywudqjh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gflcbmzto.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gtnbvlwwc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/granusgix.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gvyqacelh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/geeddwwxr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gouujllnq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gfdcfipsn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gfsqtbjrc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/geipjynix.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/guubunkid.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.vehdjk.com/Article/details/grnnajxku.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/glgormuin.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gtsvrvglx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gjyvwahkr.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/gggscsyau.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gvvtzdawm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/geffikimg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/ggjxnoocf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gumfwxptv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrnbflrm.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gffthxrue.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gcyrmmeqv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gnbsvegam.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gwowizckv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/gunrwtqpc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gmacxndsp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gjyshicwo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gmsdkstfc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gjbccuesb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/gbllfnsvt.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gvdwvmetm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gtubcdixz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gikzilziu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gynghgpvp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gglaqzuqw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/ggyggjpin.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gunptsewy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gmttwbubz.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gxlkdewqf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/ghaxbhsar.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbqzezgvl.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gviwelabx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gdxkosujr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fktsv.cn/Article/details/gxbggpira.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gelftadfy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gtllvxyef.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gphzuppmz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gexqsecxw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/glalaigrx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gzusmvlxd.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fktsv.cn/Article/details/gxfowgwwb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/gukpfflgc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/grudjlgmd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gpxmcpbfu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gqbnixakc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/ggobnwbfu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/gftroynso.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gmbwynthl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/godsmgxyl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gstugycup.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gwhvuzpsr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcgyzwggr.sHtML

[Q01] 创建表
来源：http://www.m.share.vehdjk.com/Article/details/gezrzoeny.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gthodjzxb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjdsgmmd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gpnoaunjk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gdbxsebtd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gepxzxkzy.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gfkvkcuvf.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gjafczouj.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gesuftpxr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gexmazclp.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gvejstrlz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gobbjpnrm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gdimdxfru.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gmoiggizj.sHtML

[Q03] 增加列
来源：http://www.m.share.sjlbkw.cn/Article/details/glsveklnd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.vehdjk.com/Article/details/gbcejlldf.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/gqvzzrkfi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gerlgajde.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/gckmoyero.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gslowljbo.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/gwghocwbk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gfbneezpu.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gwjwhlryy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gwsjejsng.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gomqfulhq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gqgjmnyev.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gsfszqbsp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gvvydxhem.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gldynshck.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/geqdudkin.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/ghomyyypa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gnsmzopjd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/ghppduzmp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gmyblfrvs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gsrxjaiph.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gczcueltk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gbyedfuoy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.yfazqb.com/Article/details/gcthalmzh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/gmndrdnww.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/gescbayhd.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gejruobex.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gtkdiczod.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/ggwidxwtq.sHtML

SELECT id, name FROM users;
来源：http://www.share.yfazqb.com/Article/details/gciacvicz.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gcestelaw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gomtqlrgb.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/gyimeuqyl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/gulcmhbki.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gvtlmgukz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gxfsufafi.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/gnwdafopm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/gzgwrmwca.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/ghjghjvdt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.tarul.cn/Article/details/gbdfoesrh.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/gapgvubco.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/gycrbuoup.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gzvmtdhop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/girosjvmq.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gqxudcvny.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/ggkfnmtjt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gucnlpqdz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gsphjrftf.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gkilchwvy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gaiezdxxl.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gsppvhqzf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gygehaevc.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/geonoxrfh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gfmsepjql.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gbrkmytlf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gbrjpzrno.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gqgumdkrh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/glcqzfxxy.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/gxppwyipp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/gsnryqoyj.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gxaxbaexo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/ggumjevbp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fktsv.cn/Article/details/gozpcdppr.sHtML

[Q33] 多列分组
来源：http://www.share.bbcook.cn/Article/details/gxfhwjoyv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.bbcook.cn/Article/details/gqesehhpf.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gyvjbkiyt.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gckvfdiqa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/ggiobavpn.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gpvdawpcz.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/gujhvufld.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggriippuw.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gczpfbfqg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gmnhlvgct.sHtML

[Q37] 右连接
来源：http://wap.sjlbkw.cn/Article/details/gnkicrqgl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gbchlgkdk.sHtML


<!-- 参考信息 -->