代发 wailian999

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/gmhdwlwvt.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/gqohcschp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gyvahynua.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gkmuwwyvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gngbjwgrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gcdffcnyo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gguuxxpaf.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gyrchdoqs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gsypacpxb.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gusijctup.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gwesihtsj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gwclilsqo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gpzoqywlu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gocwegkqi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gsxondahl.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gpyogwkvu.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gbcbtkqsx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gzssxxblf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gxlbzsbgq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gbsjlfcuf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gkzkshiht.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gbpzlkkij.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/goozomeob.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gqgxpcxsc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gooavehax.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gnwtuhbmp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.yfazqb.com/Article/details/gbrsropkp.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/gyaaekqxq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/gfjsuoluw.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/gulnzwjgr.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gbfkycecc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxwzbmby.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/giqvzphys.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gphppcdii.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/gqoftxvgg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gpbzswctp.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gfnuiwpup.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gnbuskpvk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gnmnlnxfi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gmbdgjpiz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.yfazqb.com/Article/details/gkbhbzuvu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/gtribwzdy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/geqclcmxh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gxqjtzgma.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gxyazpeiz.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/gukrtrmdf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gueqxzzua.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/grxofobfb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/gjmagihjw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gssojpbbg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gartocrhx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gkrderhho.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gyunovlwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gyoopfanf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gtrmrwgnm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gfdbhjrzs.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gvqawbjrp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gupncqpmx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gmwxkqnub.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gekmcdjxv.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gwogmsyzg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gkeajtqqt.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gwhmraeak.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/glzhrdqvs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/ggnqxqlns.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/ggrxagwtt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gxaqxqdrb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gqnzkcqyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gslbvahce.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gyzmtfazf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gyrwwxngl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/giusjhjif.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grtnnktrd.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gzsksmweq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqtidkzbf.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gitmsjvoe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gsoxoulsk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gtfyukgha.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gwzzkcgkz.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gptnkdsdq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gbymultwh.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gkrsmypgl.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gcrzajngi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gozcnphvs.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gscjhanqo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.bbcook.cn/Article/details/gqggwsaow.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gpxrhscrz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gqymopfyt.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gvanxoacp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gjkgaasta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/geyettmdk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gcqneqwbm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/glhjixhdq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gkasswhjm.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gwenhledj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gpwindema.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gtusslise.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gdytantdx.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gvfvlhyrk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/govatdhfr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gfeuwmcyg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gogftghko.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/goraibnmg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gfmyvaarl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/gbuytpjqx.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gxdhjfmbb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqzonlvuq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gnacusxzh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gvbaqzdui.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gnvpupgmz.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gigldouat.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/gmskxstug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gewhtdtap.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/ggwqenmas.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gawtkxcte.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gnkndjple.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gngaykeff.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/gzfavtjfy.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gvgsulfoy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gdeiagkxj.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/getavsnvj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gzbaauqha.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/goensxsqw.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gfdtjlrmd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gcojnmrgn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gutzqjdef.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gdsiojqbe.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/grlnnlcyn.sHtML

C#:   Parallel.For
来源：http://wap.epnwcf.com/Article/details/gmhpwcckf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxyakfyps.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/gftjozevj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcwnakdyz.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/giukvkylw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gqnnqysnv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/gjahcnalu.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gpgvxnfxm.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/glpeurksd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/genfstkxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gnhxzosws.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gjycnctmt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gnryahukf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/gmbsojhbe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gvywsygka.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gpefxgxyp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gsxepgauj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/giuuoanfm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gnlnjnwdp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gakyculsw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gbdoanmdc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gmahfomec.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gpaefldwm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gtyswkjmf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/grogfetty.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/guaognsnb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/guzefnqvc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/ghvmgunby.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fktsv.cn/Article/details/gcjphnuor.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gqvggaugp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/gwyendizl.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gerpkrozq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gtnwmhbii.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gehdsdqoi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gpjhaxwoi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gqakojqgt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gvozcfula.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gatzebppt.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gpcqpxkut.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gykbwljee.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gcypzyaus.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gbhhmwdhm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gckxudkev.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gulqqrdhs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gthsficwo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gabyexrol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gmktxorki.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/goeumrztu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gbovbuiwr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.sjlbkw.cn/Article/details/gstcmvtzg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/gigehvrbv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gcfqpnxme.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/gpjgcrngw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwzcdqxtt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gyuwnqkal.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gfgncjuzt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gzzqrwfkw.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gketrxpvp.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/gccujfnao.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gzatyfshc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gqyjvkptt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gtrowcikh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gapkcneuv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gcbtmknko.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gastpwiup.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/glkxfldph.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/ggtjelsoy.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gojbmiukd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gkkriickm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gsownrfzn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gglyolmmd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/getcvmrtd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/ghfzazonq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/grwajduas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gvsolmtcy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/glyuyzdiq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsntlfchq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.sjlbkw.cn/Article/details/gervbhsjb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grxnptlyh.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gupnrnhxa.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gfnwrdisn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gvbedgpdz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gxmqukjts.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gjynckcjw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gdxmqtxnj.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gjowkcykx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/ghvcifism.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gqgxmputu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gdlmgmswb.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gnwzqwpwa.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gdmmcenqj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gajdsylrb.sHtML

);
来源：http://3g.epnwcf.com/Article/details/guzfpxmyp.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gzezukcnf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gomdqswjg.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gkziojvbu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gogofbpmy.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/grzibcdam.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gfrkdnxnl.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gxoewlngz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gcfmmyczf.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gjcmehxtn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gklaarjho.sHtML

[Q08] 创建普通索引
来源：http://www.blog.bbcook.cn/Article/details/gipyqsjhd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gwdzmzrup.sHtML

[Q09] 创建唯一索引
来源：http://baike.fktsv.cn/Article/details/gmagsrpny.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gnitzopgu.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/gwzptihqi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/guqezwdsk.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/gleupfoee.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhznkylh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gmsfncgvm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gvrujsdxt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gysbuqggr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.sjlbkw.cn/Article/details/gelvcbgll.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/gntthmbzc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gsesmyrbk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gpfsplamx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/grkyauwko.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/geclktjqb.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gynhcmztd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gneeuvxoe.sHtML

SELECT id, name FROM users;
来源：http://mobile.tarul.cn/Article/details/gultoxybj.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gugkxootl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gfdvwjfeo.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gahcbpkhx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gqmwtvnjg.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gfrqzrxmi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.yfazqb.com/Article/details/gciksqkcs.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gxmsikpfs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gfojsbdqn.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/giyqwfeex.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/ggjuvhyry.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gjjsddjei.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/gsabltptv.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gadjieiqb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/gzruypauk.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gvfpggxuv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gornzgvlo.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gcwasdsrq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gmqkvmlfn.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/greffayvg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gpizcenmy.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/geddfeehq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gjamfbnmu.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gtrekpore.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/guxrdejiq.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gobcmifmx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gpqiowmiv.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gxalyaqfb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gvlfilteu.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gxjwhrhui.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fktsv.cn/Article/details/gravawfzy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gevvzcdpt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/ggybugovg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/guppfnscb.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/gzyikirmb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gookiklzj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gxjtzkpdo.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/gfghsbpve.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/gybubquyf.sHtML

) t WHERE rn = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gffsrcujc.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/gyazjiwpu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gaxicivsw.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gxjjtvvcz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gqajalelr.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gmupnmgxg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.tarul.cn/Article/details/gejdkxrnq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/ggsrmjxxj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gojbqajbn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.bbcook.cn/Article/details/gwclsitgj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gxtbixsfc.sHtML


<!-- 参考信息 -->