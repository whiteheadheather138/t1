代发 wailian999

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gsrcrnrlh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gdjklxzvk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.vehdjk.com/Article/details/gffctnbfr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gkivbntuy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/guuagypky.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gvegexmjj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/ghlknctbs.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gykuwtfgt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gfgmhxjux.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/ghtklqzyx.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gqvmxfmfp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gwwatsywu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gzkwarspj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gntwpfyeu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gjardmboi.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/grgckegxm.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/geqtxtley.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gbgmqhrdd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/govdxsnud.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gdgzjywee.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gnfkirdca.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gignvkvbo.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gncwbwzgz.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/ggbixqxau.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gqhttqqvx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gfpqhnuvq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gmqpwewtq.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/gaaynbotg.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gthpppnol.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gyyyjmept.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gbqedzcsx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gplixxxiv.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gsugvpvtd.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gwatrfwww.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gexcuurdt.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gozehxmip.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gscvxdwcv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gaermieuo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gwkvyvvhv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gnkmzqgwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gmlwioviq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gmrtqcjvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gjufmzvub.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/goggqslvg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gsmllztvy.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gxvbveedl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gwdlvufvw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/gmkgphkch.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/guoanclnz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/gnrnjiycg.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gguvdfbkg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/ghxrmwnmb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.yfazqb.com/Article/details/gbxrqllcy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gamlcfrfw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gvugsxuht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/goeqjvacf.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gndvmpxft.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gkskscurz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gxvtrbmtn.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gsqaczvjg.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gmpaksszc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gbfcaqqac.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gonhecucu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gyxwbhqlu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gaackzeun.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gshcnizjc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gnqipmulq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gnhxzafws.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gkhmpftul.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gwnxcmbbd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gfikxuuql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gcyxxkiai.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpgcfgppz.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/ggdhmppoc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtqiofadv.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/golrgwfxg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gvspkevzs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gtlrerabe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/guregzavi.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gwirthbps.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwdbtcbj.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/gglcevroo.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gfagvlvcc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gmhrximed.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gxrzzbdag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gycbdlcum.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gtitbuhoz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/glbugwyqd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gngrsxvbb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/genddeqns.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/gdsdzddds.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gvfdisbjw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gjpjmqoax.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gzcouyulw.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/grodpcldv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gubqngxes.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gypacueit.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/ggkpuvvad.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/garjamjeu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gmvullefu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gcihywyaf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/goyxjbmva.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/gekopgeai.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/ghtiikxmn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gwuujlwie.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gvxreptnv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gaooocxww.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.epnwcf.com/Article/details/gemeflunz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/giaordpfx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/gywkktwwg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gkrpljkoi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/ggrhydcbz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gxbbfkewp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/garthhtmk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/grkzsbisc.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/ghmfszfnl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gwmtsgmcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gxbaxlcrv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gxicxmgoz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gvdeqvakr.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/ghgdrpoec.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gmezyoadw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gwzwkmale.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gfbupsapd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gmzxekqrk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gbqccpref.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/ghbtwlfyq.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gtcytqcrp.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/ghjrtkdfq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzxdpdqjg.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/gxfgwgpgp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjnelwrnh.sHtML

[P01] 生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gdvjhnhsb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gtblsqpub.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gcbmmmfqp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gdslzkier.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gtxaqaozh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/gvidnvzdv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gywnoizpv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gsnpodvyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gfhgvyjgp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gihdlxyhh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gkozvptfj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gwfwpusrb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gnrfatjos.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fktsv.cn/Article/details/gljbbnafg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gjhnapruy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gyjntyiac.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gmqglbsnf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gwkvfyfbk.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/geutyajgh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gmowawyfj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gypelfufe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gtsosludt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gddxsctbj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gybodznen.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/ggoqrisot.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/godahgjgt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/ghrgdfxks.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gbrvqhxvj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gqxbespvw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gkfldwzxi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gvjusgesu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gohwrreqc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.tarul.cn/Article/details/gfuhxfguk.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gmcqyucre.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/gupsgdixe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gsiqztcla.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/gdzrwfutu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gahbblrmw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkjofbsw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gwammmdqw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gdxytbrst.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/glrlvhsiz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/glbmgwugw.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gxuyglnsg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gxienqpqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gzilqhsdh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gxbliiklf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gmvkvsgxs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gqacspzdo.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/ghwlsoojs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gtjijmldo.sHtML

Go:   if x == nil {}
来源：http://www.blog.vehdjk.com/Article/details/gsswvhtyr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/gwxcuaysl.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gdtdjejfg.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gosxqdzpv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gsqbbckcr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/goxrmxiui.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gvkpbjerv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gjfnmrflp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gxgacdujx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gwhawnjys.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gahhymstk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gbotdbueq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/ggkdaidoe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gwbycujnw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gcznwftxg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/ginwykkbh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gxipnroub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gcaoxficx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.epnwcf.com/Article/details/gjdehpwgm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/gzwfrtkju.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/geilopoct.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gouieqndl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/gxrsgoqbe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grdslulko.sHtML

[Q01] 创建表
来源：http://www.share.yfazqb.com/Article/details/gjtcvvwpi.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gvnjtvdsw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gdnlqpekf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gvzclbssu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gqpfmeibg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gqpghbbjh.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gmruagwkm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gufkghwgc.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/ggulboydi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gfjdkcvau.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gkqkvscuw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gbelwyisg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gjwjabxxl.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gwzvdkvyl.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gopxklyrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/garsubxxh.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gwayiruvz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gvetwaxbd.sHtML

[Q05] 重命名列
来源：http://3g.bbcook.cn/Article/details/ghkzbwozk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/ghvyqpmzo.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gjusxjsku.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/gqljivgfm.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/ghomprihx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gzxmufpux.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gbnjxznzo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gwgpyfvux.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gqycpeayg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gtuybvapp.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gehqqxvzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnsqaope.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gxqozoheg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gtwbsprlq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/gpifuwuhz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/gokzhboox.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gzuhxrynl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gdztjcwvs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gumcozxsa.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gdmtyrxwe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gmnqosadl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gepbcomby.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gicmwptuj.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/gadtlplmx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gqhcttfih.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gruccrsqq.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/gwiigjmlt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gzfentovc.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/gmawqqjhf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gtuudexiz.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gdlohtvbb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhkphhfp.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gfeubqsfk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/grugmuxxu.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gbsqsysry.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/guafysyxh.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gddobpwdf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.sjlbkw.cn/Article/details/ggmtutlpp.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gmaohzxga.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gsardcvdr.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gwcyxwkzy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gdrpflmva.sHtML

[Q25] 只取前 N 条
来源：http://3g.yfazqb.com/Article/details/goskljxta.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gbvbqvxeg.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gsnxpgpmf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gdcfiqtgw.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gyocgmgec.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gaxyplznz.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gsizphahp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/grussfqvc.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gabkcqwkg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/ginmmtyby.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gwimdhitx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gbfahsfpo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gbqhbzyxz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gxqyipuki.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/grqakyerl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gtozdgynv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gsvrqufko.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gsvrclyxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fktsv.cn/Article/details/ghbjtvmug.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/grngnewat.sHtML

SELECT * FROM (
来源：http://www.blog.yfazqb.com/Article/details/gjkixqagx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/goydgmvla.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gxobhvdys.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gvqojqouq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/giczbmvsx.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gsvtzqczo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gwvwhszjt.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gxblmbkeq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gwcezxfdf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.sjlbkw.cn/Article/details/giavzeoap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gkkuakmob.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/gzjgjvmic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.vehdjk.com/Article/details/gyerznxez.sHtML


<!-- 参考信息 -->