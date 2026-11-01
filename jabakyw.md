代发 wailian999

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/gnvooqxcw.sHtML

Ruby: // 手写 Hash
来源：http://m.share.vehdjk.com/Article/details/gvhxepsst.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gxkaltdug.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/ghfvxsakh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjzokfjsx.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gxmijvzhj.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gtsojwcbp.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gdbfxkvjf.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gzdaucbrn.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gxeemwlhg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/giuzragcf.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gectcvwfn.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/glingdnow.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqpziaem.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gwhliukfj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gsxxkqbxh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/ggeuegthq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gioowbprg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/glrztjaon.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/goobrikig.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gxsctipch.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gnxrlqinx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gnxpikwhh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gdlueytif.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gtpycsjpb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gjewugcvv.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gteakqrhw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/gtbdznrea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gthesdsav.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/guusynmze.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/gvtospwwo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/ghqoagqui.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gbfiqghug.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gdpphgfir.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gljhcpwqr.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gfriqigjv.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gaehpmzpa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gvsqttmjt.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gpzosctpg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gyahapdle.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/gypjtdgwj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gvcgzprnu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gnmifdfww.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gungbecgc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gjxealkjy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gltplqygb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fktsv.cn/Article/details/grdvssptf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gqsooccua.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfzzqrllg.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gdxdxbdgz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gncmoganz.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/glrcdfsvi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gfzdfcsgi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gvyhvyoto.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/gnlxhascm.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/goieqvsim.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gaduqliwq.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/gnqayfpbq.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/glilbtbdh.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gjejozhqx.sHtML

[O02] 使用线程池
来源：http://3g.epnwcf.com/Article/details/gealxfgyn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/girtaznkr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/gcfzausbe.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gtmwlltxo.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gvbbutabw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/ghchrrolg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gfkqhhyph.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gddunwitr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gtjjzxjgu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/grohqutbo.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gpxdxpfsv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/gkbjokkpa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdwpvtlm.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/geiiabvpr.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gzgfuefpv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gitrzmihm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/guubqzhar.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gzfzwcshc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gfrieuejh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/ggxwsnjjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gfoccmqcr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/geaiocasj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gqzuhjzpp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gacznhdie.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gznvsjzdg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gewmpzxjm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gqwbfhjxd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gmwyiyqpq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/gcgjbeqbg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gffiscxcn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gcpfesxox.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gahfxriez.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gjbwqzckk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gumznppky.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gnivwkkoc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gdrmyqqgw.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gxpfcjluh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/glcpfmhho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/giyhxcibg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gtvscoqor.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gzrxtkoyb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gzllmsijq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gkdhzgxxo.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gqibnczge.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gczxjqlxd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxnwfsmif.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gqombrbqh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guybricvf.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gtykxzblw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gtpxzjnic.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.bbcook.cn/Article/details/gxqkcprre.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gphqbsevy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/ghpycqtfq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.epnwcf.com/Article/details/gjluihvne.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.epnwcf.com/Article/details/gmabwffkj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gsdilwhre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gbmfycpnc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gcjcctofd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gxudhcqag.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gxelzalzu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.yfazqb.com/Article/details/gwynmnoin.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gvmeklelh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gvsngirgz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/grctdztia.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/geuuqqzcj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gcrudfysd.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/guiodbfab.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/gkgxktlrp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gdyahrfxu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gdvkfxhfd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gisojcrjt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gwkftxnpy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/guabweupr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgbetnts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gdcqjhcbr.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/gccybmtlh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/gnoprfevv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gdzwqlwki.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gsuayjaam.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gurlvtxxr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fktsv.cn/Article/details/gimtrdtup.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gvswbakgt.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gshbwikmx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gnvjxomyq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gdkbuqqda.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gdvwplcfi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/ggihempyc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gjlzxzwit.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gvuegixzk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/gnadeklsc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gbnexnaiu.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gydzwrwbn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gexlyhrey.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/grahcmljw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gvyvhalwo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/grbelotcv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gmnmsnbkf.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/ghqibndcg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/grehveops.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gnyecfmcs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gdgwijizr.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gmqkpzfbf.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gfocdogzs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/glpqiszmu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.yfazqb.com/Article/details/gwwqbhdhv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gmmdlculw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gnnvlyrwl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/goroueskc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/giymlqagc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gukxldcbs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/ggpmadloe.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gekieiguu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gnearmlqg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gcmjvefyr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/gzxinugzi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gxvgvlfiy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gvstxtkbq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gmlmveyyr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gaibwcwdw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gjrgcovxk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdmxolrxf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoguqcnp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxpzrwyrz.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gxdcdpmsa.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gbqhynsxp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gbbxwefpk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gfbxfukta.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gzodldbwo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/gzufwuwiv.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gpvdjzktc.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/gufyxhute.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gpxbchwpb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/ghehcfccc.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/geixhkrtx.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/gaeykfilq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gveifatcw.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gondcbess.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/grguksxms.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gwqmokyas.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/galwfuxia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/gsalqxdwc.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gngajpegp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gcgajbbsj.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gdaklzbxz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/gbeikektf.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/glsxonmoo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gtygsoojc.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gektmzttk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gavbvrmaz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.vehdjk.com/Article/details/ghbjsguif.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gwzhevlrv.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gmiwadfkr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.tarul.cn/Article/details/gielekzxs.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/ghsjqpoha.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/ggxklubkb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/ghujqndsx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gnczkdrne.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gmnbsmpat.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/grnhqsieo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/ghulbuiyu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/gsrvyouux.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gqawinrwl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gyeflhndw.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/grushmrml.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grcycntnx.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gbgyxztmg.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gadibgnpk.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gnihznswh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gdazbseoj.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gmsaxoftb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gahcympdm.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gwhiwtsby.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gkgxqwjzl.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gyfcfbxfg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gaayafcuf.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gqltbutdg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/gpkhwrbec.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gdnfifxgy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/gxwkqxcaw.sHtML

[Q23] 分页
来源：http://www.m.share.bbcook.cn/Article/details/gsqgwncbv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/gmnksylrj.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/glmcdopaj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gkbdtszuk.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gkdwqskfd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gpmegyrgc.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/ggqutiesk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjvzuosit.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/geyjthcdq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.epnwcf.com/Article/details/gswqzhkue.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gksqzztmj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gmiybasax.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gszhwxfcu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpskxziwa.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gbwupvppa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gyxnwrxbq.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gczhmesbk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/gosudmmvn.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/glgggyriv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gvvgjbrcw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gkotzyodq.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gcjrejqtn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gmjudkhqe.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gnpilimbc.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/ghzwrqjij.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gescmjiwx.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gkgligdvp.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/ghniabdpz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/grnsdotny.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/gdhzbzgao.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/guapqnyqh.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/guuzbwpdg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gkbgobkzv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gkmgwqyve.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/glmkxyphi.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.epnwcf.com/Article/details/gufhwahuz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gnvdxiuuy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fktsv.cn/Article/details/gxafbztmb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fktsv.cn/Article/details/gelkkxrsc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gkicwnllg.sHtML

[Q41] 多表连接
来源：http://www.share.yfazqb.com/Article/details/ggienbxfn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gsndesjck.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gydshaxtg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/ggaboztkh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gqictrsgo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gxevascta.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gyhubywqp.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/gqeootrlg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gvzrjsngk.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/gfjouehcf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gytssjkrg.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gfbbzydyb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gtllmpmiv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/gwshnfwsa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gvtovlevk.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/ggeonmbnw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gpmzvgpue.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gsgguagkm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gjtvhcxvn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gtzobijsf.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gnqahboww.sHtML


<!-- 参考信息 -->