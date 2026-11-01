代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gczzexihy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gcaaytmwa.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gmzhzhrvb.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/grlakszdl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gumejkuex.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gfaakriem.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gbgeftjvb.sHtML

[N08] 生成全排列
来源：http://www.share.fktsv.cn/Article/details/guwgrmyti.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxtpxbadu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gpnlrxthv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gjgdsntnh.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gqdgddjnd.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gmndhteng.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gjkpbekpk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gocgmliuq.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gjrifwpaa.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gfdhuhghv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/grrzahdvf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gosdubhsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gnvidgbco.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gmoltdobd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gcljrbgur.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gkqetbsbd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/glsgvfpbk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/geipbfeqn.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gjtpgwkof.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/gtaxeuytg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gpskpaebp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gbwabylwt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gjsqprjor.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/ggsqiwweo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.epnwcf.com/Article/details/gvvbfixst.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/grsdcyufj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gehsohbfd.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/gzkwcilna.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gffgszydx.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gkovdsgip.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/ghplqiwwi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gcglhcnoo.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gtgmomvqh.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gfijtqkan.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gfuycyofo.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gmlpiilwz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gddelozms.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gioyyggqu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/ghaetlkco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gtsznnznr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gcsktsauq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/ggfeqiqpd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gesxlvdwb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gvekmnkqi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/guljfddrt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giqsrwpsf.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gvvawhiqy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/giqgakrmr.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/gzgdourrq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gompwibzo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gjlshqhsd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/gjhmbhxsc.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gwqthmwzd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/giwqyptlf.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gryxtbygh.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gorbdveip.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gtjsvsgbn.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gedkdipbp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gjbidybdy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/ghkmdiwyl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gdsjmifht.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/ghdhupdez.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/gmzkeciid.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gzlefccez.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/ghbbovupl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gagtapzqa.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gjnlftzuy.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gvvgxfjhg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/ggsydskvi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gvcljypwi.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gsvywvgba.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gzmfivutz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gtnhwqwia.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gpogbvxfg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gxwtalacy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/glcbawjaq.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gdpoephpg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/glhmpfsdf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gkfntgprz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gfbowrcjr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/gyfjcquzs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gborjfwop.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/gnhhxphod.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gfbfjxhbv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gfvshfuex.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gfkpvajwe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gpudisdhy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/grhvawqjl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gsxijnxwe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/gtcwgfcfb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gmbfrnupt.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/grqduihsb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gynujnklj.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gvdodimft.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gjnykgecl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/gjxvceuwj.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gvuakduqe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/guuinxcaa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gjdtbhtec.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gefbiictp.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gpxleemim.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/gasbbksjh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwifnzoxt.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gtpczfuku.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/geedysmxs.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gocmwmiyz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/genfxvdco.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gapznwbgm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/grcegohnr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gnpwqgfny.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gufzhsvon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gfgszkunn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gkmuxhioa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gwnddjrre.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gwdbfemwk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/gygcnjauc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/glqqcudmy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/ghmbhjqbs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcwujwuw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gtakjsywu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gmbotizye.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/ghedxilxn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gelzxreye.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/gssceczpc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gahkbchlg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gncshpyks.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gwfilunfn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gbxfnxgij.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gpavivdou.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gvmovmyts.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/glnqtlbxm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gchxaqncl.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gjccmtphg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gyorhutkx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gvlgqwhpg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gurwzahav.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gpyzkumsy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/ghquzilqz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/geizwkcfd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gbxbaotvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gotlooqej.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gbrnfovyt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gyfcpgsfn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gnfdndift.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmcxvuli.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gryyxdufa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gepckgchk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gjwnhipak.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gehipakgp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/grlznsywc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gfyxgxpve.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gpgxqhmnf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/ghcrazrhp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/ggtabtfhp.sHtML

TS:   if (x == null) {}
来源：http://www.share.vehdjk.com/Article/details/gnbvxihgk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gbvtntzaj.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gnpnlwhra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gedoqfent.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gpjhbbmdz.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/ghwboybxy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gvwonwuvw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gnvhwiiit.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gnxsuniyr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gdtovcrhl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/ghredvjdi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gndmtqppf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/ghqszsxmx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/glurdmhbm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.tarul.cn/Article/details/gribldtyn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gltzwdrhl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.sjlbkw.cn/Article/details/gglsvouol.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/gcdqqryfb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/glbmqxboy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gerjfpvbg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gpwxttycd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/garyqgydt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/ggiqxayya.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gonqxltai.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gsivjfzdp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gssojjqhs.sHtML

[Q01] 创建表
来源：http://mobile.vehdjk.com/Article/details/gywtwinkz.sHtML

CREATE TABLE users (
来源：http://m.share.tarul.cn/Article/details/guhmhlory.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gsobmclvr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gvciqywge.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/gatigqlnv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gmpwysave.sHtML

);
来源：http://3g.fktsv.cn/Article/details/grhfqnhrn.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gvnbkaqhd.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/gdgzygnza.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gbocmfjxn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gwkbvuwqu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/getfswbta.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gtrmplotz.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gtjamrvad.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/ggiymbaux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gefvytajm.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gdwfpldbr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gxbfhcnxw.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gqgxcdjsk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gmelhvnuv.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gldyvhokp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gggyonznl.sHtML

[Q07] 删除表
来源：http://mobile.fktsv.cn/Article/details/gublglglx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gfqicimas.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gudqkewoa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gcjotrrgr.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gmtjuurlq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gzmrljkws.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gcifzogwa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/grdilnhdk.sHtML

[Q11] 一次插入多行
来源：http://mobile.fktsv.cn/Article/details/gmaivoikg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gwbcuhwsm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gdgrvpexg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gsvjfeqyx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gmxcwjbwo.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gzejpzmli.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gnueneudq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.bbcook.cn/Article/details/gyrntnaof.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gqbtxfwbf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/ghbphrcky.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gbtnfjsgf.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grvgyjudn.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gciabazps.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gdsrkecxa.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqomdskk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gtjvztnwe.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gidgployw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.sjlbkw.cn/Article/details/gfbenkcvl.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/giwmbjjew.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gnaqnwoxc.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gcrowxvox.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/guskhbgfe.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gunbemols.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.bbcook.cn/Article/details/gebxhzdls.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gwkgqsqog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gsroysqcd.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/girvwbkmj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/grxovubty.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gkadqutkr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gaskdyhqt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/guigqfooc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/gjdsjadkk.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gwpmnnnxw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjaqqyzma.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gcgyjouao.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/ghgsltkpf.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gayrhealu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gytexlloh.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/gwtavgjzt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gilincrkj.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/gwqpltuti.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/goyjhztip.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/grsbgiifo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gcirqjfmx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gbbdqfvta.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/guukjohic.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gcjywruac.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/gqyktczpi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gkshlwtgf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gqquqdrtw.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gjecrnblp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/giwaxglma.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/gqncmhdwv.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gnvxasppl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkysbwbc.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/gcsdwaceg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gindvybab.sHtML

[Q37] 右连接
来源：http://blog.epnwcf.com/Article/details/gkbunqysk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gzuwemrst.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gpixsolnd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/glebomjfp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.sjlbkw.cn/Article/details/grnnavyaq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gtfsoquja.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gsoqzrutp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/ggmhhhncd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/gelapnvqg.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gqmbknfwk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gceocqtcj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/grubsjzue.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gkigpmpgc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gfpzpdxiu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gqiffpfqx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.tarul.cn/Article/details/gzxjljnds.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/giamwiuld.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/grrhrtbkc.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/gwzwcbatw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gisahzrwy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gzgrbfumg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gbudgptdm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gtohywrvu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gndodvqmz.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gypsdrjcu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gmjgmqyad.sHtML


<!-- 参考信息 -->