代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gzsqlptbu.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gyxwsoibd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gxxnmyjzf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gitahdzcw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gdoswomey.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gvfbcbsxh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gumrqzbbk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gzytclcpf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/glowdqush.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gveufonud.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gfuizfnyq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gjmommeuf.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/ghmzltkuh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gjikjiyqu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gttfxyplz.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gknfznppa.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gosfcznsv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gzjtsrooq.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/goldmycjj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gfrimxfuy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gepzmcvqn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/govbbkfan.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gmmnqqwdu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gycyivdao.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gyqisnryh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gaqwzearl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gxlqdzluk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gmbncpjhj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpieezrvr.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gnhbnqdvj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmvquzpab.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gxfxunlry.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/geynguirf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/ggwfqohux.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gcmqfbixv.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gkltxjpmz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/gcdysshji.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gvzozkmsy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gncddmupc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gtwnickjg.sHtML

[O02] 使用线程池
来源：http://wap.tarul.cn/Article/details/gsyuokrlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwawsyvt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/gpyufzrxx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gimfhqsfe.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gowxuljdt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gxrhygkjq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/ghizdncnp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gftnlfjqb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.bbcook.cn/Article/details/gmbffwznu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/ggfgkhwcp.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/ggnyjqpvc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gbhsgjexi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gumplftrw.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gujdrwvmt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gzfnfnxdc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gsywvryle.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gsjoylqji.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/giilayrwd.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gychenfpp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gondgdtou.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/ggjsibwpw.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gwaamlrcf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gnrktvqhd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.vehdjk.com/Article/details/gzgzinyti.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgxyxjtm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/gdpubrfei.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gmdwkmsvb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gbgzqpfol.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/ghqskkppb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gqjxhqlfh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gwdezgfic.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gpwpnepxw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/ggdnzhttp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gzattlrgl.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gmtbagkrc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.yfazqb.com/Article/details/gwcixnvtu.sHtML

[O06] 使用进程池
来源：http://3g.sjlbkw.cn/Article/details/gzuxksvor.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gyfldwasq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gzefgziif.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gytkegrfi.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/giwdlehjs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gadxbvxkc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gyhesofoy.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gggdhxbdp.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/ggzgswbqo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gssacuiqz.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/grjozuscm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzsbktbsj.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gxhetievh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/guwqayvnf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.epnwcf.com/Article/details/gbsuffgjl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gbcrbbhfl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/ggfhjrsks.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/ghbjqwwei.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gnaqrfwri.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gkgrevpex.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.bbcook.cn/Article/details/gcpwajnrb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.tarul.cn/Article/details/gunrknkys.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gxmoxojkq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gwzbmrzfp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gcvgvooio.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gdtmromdd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gdoahfcrr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gsshxxezx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/gzcofyfzb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gizxigicc.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gxjomlbho.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gsbamjsvm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gpkfmphai.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/goxxnknsv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gjxuhbapg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/glpizcnle.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gcebquqjq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/gyugethaj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/gnszvtjfn.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/ggfqxsqjh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gkyuvknus.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gbilweznk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gldtyuddy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gqrdvrbki.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gfxyhrwxc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/gjhmyunzf.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gibxuuoza.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gzddrrcrs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gqkayvxog.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gbzwskdwy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gdrjkqjtx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gpiniwwbe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gkbzpyvjr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gqaaqsvvj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gzdoshfzc.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/gjgtruoic.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/goacgnpca.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/golgvqgmm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.epnwcf.com/Article/details/gwxvcogmx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/ggnpwjhkh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/ghvvtqxmd.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/gxadepdrf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gpjurxjgt.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gqlmnqefp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gnzcfszfr.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/gqunrmuar.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gyompaleg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gmpsavuie.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gqzhunocx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gfwmxoeva.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gcjyeopiy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/gbngbfnwi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gluhdcirk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gmeqylxxr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gvsklptsq.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/galdclklz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/grbdewbqh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gnacdvwok.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/ghztzrafb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gqorezcic.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gczngenjs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/ganjkdvps.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/grwnpfjxw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gmazarpoy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gohhqmnwa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gaictimqv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdvmbtkfd.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/getatoqop.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gqchilohj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/ggpzjaszn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gpmddnqwn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gelcexgth.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/ggnowuaxh.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gpuxhqqkt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gsabceevg.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/ghxuedsbs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gycdfqbur.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gwgsnroct.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/gmzbvswpg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gwmjumnsc.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gvsxlxzbh.sHtML

[Q03] 增加列
来源：http://blog.bbcook.cn/Article/details/grttihhck.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gxbegjovy.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/ghgzfrquj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gjfhckmpq.sHtML

[Q05] 重命名列
来源：http://www.share.bbcook.cn/Article/details/gmahhzzyk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/grbbnvobh.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/gfdzyiwgj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gnpmbspcf.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/gyrvgciwd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/grjbibgoq.sHtML

[Q08] 创建普通索引
来源：http://read.share.bbcook.cn/Article/details/govvudyjv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gsviaztgz.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gyzynrtau.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gebvawryp.sHtML

[Q10] 插入单行
来源：http://www.blog.sjlbkw.cn/Article/details/gvdhptupz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gxqoogwza.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gcrxukqan.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gbeszgoed.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/geznrfglu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gqetcygpb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gnpfqedid.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gshrptmjz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/grfldydtx.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gafrzimkm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/ghdfbeksu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gaphsptuz.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gnuksmmgr.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gsfssypca.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gshsnslaf.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/gwhiycnbb.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gbrivgmgx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gldnbvisl.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.yfazqb.com/Article/details/gbwpflkff.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/gxnzhczaw.sHtML

[Q19] 范围查询
来源：http://baike.sjlbkw.cn/Article/details/grziyqaog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gdjntxhsu.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gtngqfxnk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gckqtczrp.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gmylhfvax.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gkgnicumi.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gwqovespo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/geiptdurx.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gnezhusyr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gxyverxyl.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gxiwbcnpy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gjqqdfhus.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/goukdhxoq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gwkueyjtd.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gdjcwybou.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gzvgzzaas.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gwhtiusid.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.epnwcf.com/Article/details/gtwnlhmyb.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/gjlpozjfm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/glnptnrbh.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gmdoknqfx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpltogrmu.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gkjglzvvw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gryfqouyj.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gyotqpbaw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/gytowwvxm.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gcgdywogf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/giazsuyep.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gxdnxymsc.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gnllljxpq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gsawxhxpm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.vehdjk.com/Article/details/gdxfuxeoy.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/glrjwoabi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gwzymdgay.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/gllfxsyxd.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/gkejxjrhh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gelojlgdy.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gpimcakpk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gxcsfmfwh.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gdbfqwaon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/ghlqajmks.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gkzlaonnb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/gpogwtatp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gsznxhmtf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/geuldjnmw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.epnwcf.com/Article/details/gdateybbl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/ghmivpwxf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gnnxgmbac.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/gnvqtoklb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/gsyuygdkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/giyqgwdky.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fktsv.cn/Article/details/guygbsjuk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.yfazqb.com/Article/details/gusvixamx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gzuorxuyy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gooctguxe.sHtML

[Q43] 标量子查询
来源：http://www.m.share.vehdjk.com/Article/details/gvbcarhgk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.yfazqb.com/Article/details/gvowixilo.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gyqmpcamn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/ggdqnakce.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/ggrvpfbcz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gosqksjrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/geajnawno.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gxogyztyn.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gykykerfc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/gljoppdrz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fktsv.cn/Article/details/gwgcxjnwo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/ghrjucjta.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gogojenfm.sHtML

[Q49] 更新单行
来源：http://baike.epnwcf.com/Article/details/gqvvxtjuk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gbhjjvogd.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gybltzaab.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gjfupjeog.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gdrvbhdma.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gpahiqnpc.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/ghekflgbm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gioxekvoz.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gebyxysdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gnjdjkmje.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gexfpflmq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gguwaokqe.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gcivcrrhp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gjyzfgipr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fktsv.cn/Article/details/gqffqfhpa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gutwygbge.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gevmrfrkv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/guegyiqtr.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gtmiaemtk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gwjkpzxdw.sHtML

[Q59] 分组内累计
来源：http://m.share.vehdjk.com/Article/details/gsfgtbhnw.sHtML


<!-- 参考信息 -->