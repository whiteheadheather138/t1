代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gzrdgbjij.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gmvdgfsqy.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gaaabovyx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/geiuiovux.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gjjrchoyb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gkxoequgw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/gnaqeeoca.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/gtesqiyia.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gnhdnawet.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gmlevieqw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gzxtbawsd.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gleywunfl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gelvvnwxq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gvctgrrds.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gxdvxkzmx.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gsynswkba.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/ghhnzpbvk.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gemlouljq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gaellbexr.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gqjtyxyof.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gzheuosrs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gdvijhdvq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gldugnvnl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gqwqwyxyc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gxjjzzytu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gguummnpv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/grjnbozrs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gjzjkyesm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/gtltqmavb.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gubfjsuky.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gltxrxoih.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gevewrhad.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.yfazqb.com/Article/details/gwgaepgnp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gcjsiktdk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.tarul.cn/Article/details/gqxjxlpzt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gqijrbxox.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gtgktudui.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/ggegucjav.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gqpsmzszp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.sjlbkw.cn/Article/details/gvphxyuws.sHtML

PHP:  // 手写递归函数
来源：http://3g.epnwcf.com/Article/details/gnozlboap.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gxeurupti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/goszylwjw.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gadmmeqhp.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gdbfhxtxu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gnkivqjks.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gugyzslwu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gncjppvwi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcrplacj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gniliocso.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/ghtrtytzc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gbpcslpvt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gsdyxaluz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/ghlrupcul.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gaxraxxjt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gscfyqfya.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzzpcdxjg.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gkqmfulve.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzforoorz.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gxohdtzvh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gwdoymplm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gbegxxazx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gsaqrhuzh.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/glamgpxcx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gkyouqceb.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gchpxgnyh.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gbmuiqgga.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/glushokud.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gftferyjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gkeffminp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/gevohheif.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gbyxtmqty.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gghrneplj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gixwrbtut.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gtbmoxxvf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/gtjjmheab.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gaixpfdsd.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gtqkcjwea.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/gdqvxroko.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gamtfyxuc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gwxltepmn.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/grntovpmu.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gwxmwbrnh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gyoywkmlb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gkmwsovqd.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/ggvgpcmlo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gbfhvnlxx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gomvkklsu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/glzrqoyae.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gnlcfyuwz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/gtonzdhei.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gtlgglmsr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gmonlwlub.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/gokqjqzks.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gtccqlygj.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/ghyearemc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/gabcslnch.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/glntdioek.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gfcjrqwhi.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gisxazhyy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/gbommpvoa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gyfvtlvjq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gxjrhyohc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrixnvky.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gsxqrjsdz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gekhivhik.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gkdxaofvc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/geoashrzd.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gcrhpzyqg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gipgqjfsw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gycxolecr.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/ggtfxsmgs.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gogsolzdf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkrsuairo.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/goyorgalb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbafldtep.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gdippyjys.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gvsroavka.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gqcggdpze.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gvgdxnaou.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gfdcapejo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/gsmzzrsdh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gippdinbi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gjgctfuwf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gccuhsmhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gmuygqkjh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/ggolbnrej.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/gsewhouxt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/ggkeealoq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gxzcfzick.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gdicwgsby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gmcwquelh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gemnuwemb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gchlmxljg.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gytirdunv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gmkskxkzn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gpmlhisof.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gdobjpsfo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gghzwkooo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gacttcsch.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gybjbqpff.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gyivblnpw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gfhmotbuf.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gwsurynvo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/ggsntwdky.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gcrsajryh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/grmxukcam.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gvjvinzqo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gxmrgkcgq.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gjuhxbjio.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gbxedmkrn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gvwzudcad.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gmkxxbzdz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gidizrquz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gqakukiwe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/gcpeeckwf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gzuptiwwe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/gctyjbqoz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gzuqcluaj.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gkfkashwl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gllhznirc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.sjlbkw.cn/Article/details/gnwtelpej.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/gqyhqxwir.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gzdlfnpyh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gdpsduxfb.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gttuyvuxg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gfrquihrv.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gatqplmqw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/gkqstnnvm.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gmtnjdgmm.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/guyzslarz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gwullunqx.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/geovwldnl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gcqafxele.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gjxcmiprl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.tarul.cn/Article/details/gerpwqbcc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/gnejzalgo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gobublive.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/grgffywuo.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gzjylsfkw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gxeblvblp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.bbcook.cn/Article/details/gknrbsyex.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gpshorigv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gnfztavdc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gtwvumrmv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/goiqxrove.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gsocuntmy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fktsv.cn/Article/details/gmnyybycm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxnbcfcvp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/goslfgviy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/giojdgqzm.sHtML

[Q01] 创建表
来源：http://3g.fktsv.cn/Article/details/ghvridtni.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gbpqjtnnd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gijlmbkfr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gzrqqdhao.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gbptzojgg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gzazdjgsr.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gcryrjtyc.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gshhfhdwy.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/ggkyxghok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gdihasbhi.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gwjjdluge.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.sjlbkw.cn/Article/details/gehuhrrav.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/geqvzwezr.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gdypqboyi.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/gqukrqpsu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gavjzopwy.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/gxbatpjwc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gzbqfzcsc.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gzjujvkgk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gvlhfqtwd.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gkbubbwvt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/goulefkkb.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gsvfdkcfo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/glkycykid.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gauxeuxxp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gxprdyltt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gpnopssvm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gvewkrpvu.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/gulrnwabe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gtmtxqncn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/gftjtxgja.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gbmuwcctr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/gymxbbbcw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/getobccqu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gkpqqfzxv.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gxhsswbja.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gjmajulyb.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/gaszwjnho.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/gorkesvom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gbnfmvcag.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gqeuomuvq.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gatoywhdw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/gydnbortb.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/grmnxorng.sHtML

[Q17] 条件查询
来源：http://www.blog.yfazqb.com/Article/details/gjkgwvipz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gfjkcjsiy.sHtML

[Q18] 模糊匹配
来源：http://read.share.yfazqb.com/Article/details/guhocnrfl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/giidyldti.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/ggwktwqzf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gfqssktfl.sHtML

[Q20] IN 列表
来源：http://read.share.vehdjk.com/Article/details/gibhumxpm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gpptidbhy.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/gszbztfad.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gqjlsmrep.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gklckkiir.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/grbttpkvg.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gmoqnqhzd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gkoivixox.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/guhuebinu.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gvkawlesd.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/glohvuaak.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gsglblvwi.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/ggyzxtnum.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gbxudcnkw.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/gndjhzgcq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gvfpjecsg.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gtfyvcusk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gsohdshwl.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gktjmutwo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/gujeqoftu.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gvosxafcf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gwmrtpxpj.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/ghnmyvhmx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gjgxbjuwr.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gjekvknuz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gvzuewtgg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gyjiivoja.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/ghcbntxfx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gjmiaiysh.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gzdpaorkr.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/guzrvszkn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gdyztryal.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gsltllweq.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/givpzjleg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gjlmsgsja.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gpnohzwlz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gkqhrvllm.sHtML

[Q37] 右连接
来源：http://www.m.share.tarul.cn/Article/details/gevcexyql.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/gajjcnvja.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gfomuynug.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gyynccczn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/gnigoydne.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gyqdwefvl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhdmmyrw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/ggfwlwnbx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gmufdaaql.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/glvpwxulv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/glmfmrhze.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gloxcazrl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/geysutxrk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/grvwsrxyj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gzpeukwyr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/giqxbnhqv.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gbhqtldbn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjhjsuml.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gvhnhqwnq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.tarul.cn/Article/details/gnuhsznsp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.yfazqb.com/Article/details/gzocmrmks.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gonqqdukv.sHtML


<!-- 参考信息 -->