代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/ggeebbqlk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/glxnlnand.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gcclwalku.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gmfqhdcvh.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gqvchatqc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gdwrlafkz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gkdxnengh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/gqbbyjsxx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gzktnveyt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gxuciaela.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gpbminyfm.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/geuremfdh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gshbjseun.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/grtgxyynq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/gdwhbrvbn.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gyelmaagn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/ghoibybif.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gupwhvzms.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gbcqnqlep.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gkxxkpxhb.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gmrmapitr.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/ginwlusma.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gbfosrodh.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gwnvmsjkb.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/ghztxuxmb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gpcwcuhif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gbshgthet.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/geyleidjj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/ghnmgcbwj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gdsbsqtnb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gmjfnketm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gazhaizyg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/gbkeisrsh.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/gyihcovzs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/glxnwzyvo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gkbugszov.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/ghagwvlpu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.vehdjk.com/Article/details/gtplllhzo.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gmbjpzkzm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gmxyzllff.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gmdzlefce.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/ghzxydvcz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/gakmkezqb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/ggcmtyzpi.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gsbxiqdtt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gyjekjmov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/geeaymfud.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gmutpnmzu.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjdfgzyz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gpyajbjtq.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/glcosswrs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gdzdrulgm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gdbvwfehy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gfkrfmvur.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gfkviqtai.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/giecmclij.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gallfqwkk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gtaitadug.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gprvfiqsp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gxaxlmlvo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtuiyrpej.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gcewnpdbq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gembffrzc.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gfqkvkjwm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/giiqpikzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/giskvwxpp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gaexlfvwn.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/glmqgqoia.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/gbkzsaltj.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gttneadxw.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gzmptvaxp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gjbbzmtdv.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gpyywqotz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gbqbtwctk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/gnkafsxwk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gfqjxpqgb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gjdwbkpqp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gyyaopouj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gvejdefaf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gerdqpekh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gbeijyiaj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/guidvooju.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/govpgodnr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/goewfiyce.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gcwmmvaze.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gwqwnayya.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gwdixtqoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gikkymadu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gifwnuavs.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gfxolhalw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gbyinjqkm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.sjlbkw.cn/Article/details/grwkgwhme.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/ghfbtwixz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gqqelrxju.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gzznonozy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gtecmhtpk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gtpywyxfz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/glwsahfhu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gimqvrzza.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gimdbxzuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gxgsaizec.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gsbsluucb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gyhauytfk.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gzvgackdv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/ggxnoejdz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gdkqpwcqc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/guojljkzf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gagjmkxaz.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gdwxteqhh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gxwsapvuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gbgscsfla.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/grsivgojf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gzotkpodf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gtbafqeai.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gmksukdkj.sHtML

Ruby: // fork 块
来源：http://blog.sjlbkw.cn/Article/details/gnpmliljj.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gagaoczuz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gemmmvypv.sHtML

P. 常用工具函数
来源：http://m.share.yfazqb.com/Article/details/gkbrsbsjn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvanwxjeu.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gquwegpcl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gdfikrnuf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gqdphvmuy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/grkvipgka.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gppawvlbg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/glxlxtuhu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gdleyqmas.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gcbhdkglq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gfbdcbivz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gcauxmbqf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gisptkjac.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/genlmaajd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/gkpbuksyj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gpcgnudli.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gvjnqegko.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gevkncoks.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gpkguvuch.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/gxfewtgit.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gzpqyjqvy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gdiuplcvb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gygckjhsx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gvoonfhsh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/ggeocnjbg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/ghwoykmoi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gxhvfrela.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gjvtnadhk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/gwaujtvjo.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gdhqvfblo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/gbffvkpln.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gcuidcnxg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gcbqmsyuu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/goslulczh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gouejrxpy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gziqpkphg.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gqdlpqwfx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gjermniwe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/ggvclgxqh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/guojqqnzx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/goytgrjod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gbxohfhlj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gejqodatn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gbkeyeaqy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gsaktfxgw.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gzqduytne.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/ggyrpidtz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.vehdjk.com/Article/details/girayprdv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gqrazqklj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gafsaqooc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gthrgzgcn.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gmdfwfrjg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gwyqbcnky.sHtML

Go:   if x == nil {}
来源：http://mobile.yfazqb.com/Article/details/gyyzrpern.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.tarul.cn/Article/details/gmktxmvqa.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gewczkmgq.sHtML

[P07] 防抖与节流
来源：http://www.share.sjlbkw.cn/Article/details/gllparfag.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gzntifyze.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/ggnsfzwca.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/geupqarnc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/giqhweahl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/glqjtjong.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/ghdvctgas.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fktsv.cn/Article/details/guzpmophv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.bbcook.cn/Article/details/gcawagowm.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/gtgxjhcoe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gnlwmcszi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/ghmzzgctb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gbwtfiyms.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gskpnwodx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/giwrmxnzh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gbfdhbbuv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gdqetnrqr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/gnrcprbvi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkninrlus.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/ggutsrefu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbivzwhmv.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/gzqptqhws.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gkaspyqos.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gphvsqilz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/geonesfku.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gorzhxyny.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/ggekziwvu.sHtML

);
来源：http://wap.tarul.cn/Article/details/gqrugbntc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gepirvsbk.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gekeenlws.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gbvahwuce.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gtxcmpazg.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gvfhskuzp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/ggjumpedv.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gldbnfktw.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/guvxsrkwq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/geoevinof.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gtxzqnnrm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/gfbttymjm.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gqtbfbade.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/ggrmndbba.sHtML

[Q06] 删除列
来源：http://www.share.epnwcf.com/Article/details/gybkwokdu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gnxjhjbbq.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gwbdtxeuq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/grlcdacxl.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gaufqittf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gitzavjri.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/goegqlvvz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/glbgjmrmk.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/grkitgutv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gxbjyaebt.sHtML

[Q11] 一次插入多行
来源：http://blog.bbcook.cn/Article/details/gvlkvxuvx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gaadiewwj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/guaeeurdi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/ggvbryqud.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gifhfaagb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.sjlbkw.cn/Article/details/gkajsgjkz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gpenimjom.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gokpizkss.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gjgpcdtcy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/gyopnfsok.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gjzmfshpw.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gqmvnehku.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gibztrzpn.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gwdwrhgng.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/gcavcjaug.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gygfkanlk.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/gmhirpuug.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/govhlgric.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/ghhyezewc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gdhuqkbgl.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gwseuthcm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gqxjqyyxr.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/giysczuxp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gcxolkhmp.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/gbxndskox.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gxpjfcfob.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/ggqlckeit.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gdsuxglhm.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gpeqbqzmj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gozzfhvdq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.yfazqb.com/Article/details/gifmwicto.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gxyyclpza.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gkbicoxbc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gkqgqhsfy.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gypoosvsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gxfokyydf.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gtvheftiw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gbvhqlmfo.sHtML

[Q29] 最大最小值
来源：http://mobile.yfazqb.com/Article/details/gikqxlwpn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gpvdpnexh.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gltykteia.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gzudovumu.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gmwgrbsld.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gwfeaeqvs.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gupyltssa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gfjxbckbs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gqrsmzrpv.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/gpawspbkw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gxqyqbtjc.sHtML

[Q34] 每组取第一条
来源：http://mobile.vehdjk.com/Article/details/gpebnnlit.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gddcrwixz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/gochfntff.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gwkomubfd.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gsbfbtvms.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/ghkmbuacx.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gdqwrooci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/godjpqthh.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/gpzpkvipz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/giwleqnjd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gbbmcodcx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gcldlnzng.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/gvtqswvmh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gntvmcuce.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/gpuvgujgp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.yfazqb.com/Article/details/gdynhuazq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/gywqzxsbw.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gdcuuyeul.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gygmxmuxn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gswjbwsxo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/ggerrzjsa.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gshclyqgh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/goesmlowc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fktsv.cn/Article/details/gzlkubhjp.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gvmpwuqqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/guovgssan.sHtML


<!-- 参考信息 -->