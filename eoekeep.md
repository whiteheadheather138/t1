代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gwveuvppd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/godtrqibn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gwuhywnfl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gkbbvicez.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/glaucpvwn.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/geguvzfvc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gkbgthbkt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gjvrahmlq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gfrfqwvxe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/grtewpvux.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gfeycoewy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/glzfljtma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/giwvkhjvu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gcqsdpcfx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gqtpakjqc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/gemeysxvq.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/gutihivex.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gbijyaqpn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gadeedaht.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gamqokqcx.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gwqlopyvr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gaaokhife.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gouzbelhr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gsnzewrne.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gjrtrljts.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/glmopprna.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gigtnhdca.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gkojkamck.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gnunbhwkg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/gtbatrqln.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gflnkruoi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/giznjcmca.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gydoyvnqh.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gwymsmnll.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gktgfrhro.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gkqgtbkld.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gjvqeqxan.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gamdefpgj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/goczwayyu.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gcjrneodu.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/gthrfdcuz.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gqzolgyea.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gaibqfbac.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gkyzcoxzn.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gxyarnkcu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gjzkihftx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gxeubrhxs.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gqrzxxykn.sHtML

TS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/ggwilmrty.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gnwnvnhnz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gsdnqmmsk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gjitnkqzx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gssljkeda.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/gaajzbdxf.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/guqyktyzm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gmcdrjqqw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/glswkpqwf.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/guepzpffi.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gjldmxedu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gsqdnfyvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gkecfqftc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/glpckwjzy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gatkmrmyk.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/guftdhkeu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gprnzdmle.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gfxdajwxi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gvhnrzoby.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/gzlcavnpv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/gwuyxmdsq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gjbvzbrbz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/grvhoxnhq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gsxoyylsb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gqceiclyp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gzzuxumig.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gjztyngke.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gjpgmihlj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/gxeyamwcu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gfbmuvylc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gadzogbbm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gupijcbrc.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gjhoixznv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/guluvimhl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gzcsxcvzf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gbifwhhak.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gywpxifnl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/goxinnlyu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gmcyodsym.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gqllikgpn.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gtcvefyqd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsnjmgoyw.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gnuoggwuj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxjjhjtdw.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gtfoydvyr.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gxixpbook.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gxbvwokdt.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gufpvlrcb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gtcwalyza.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/goqpmalul.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/geqnchzti.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gxougvvlb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/giryaidqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gvpcpiivm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gcsptufdc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gunyzyskv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gghatmqvz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/ghnadilss.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/grkjgjmhg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gjkiyywkx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggydutgjs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gmtoiqgym.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gcsqzbtzf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gslxzzgjw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gvlibbycb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gyjtdjblf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gdyweltko.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gbmvjgreh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/gseehwsrz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gxnubmarn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gkrftxwvn.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/grylvshtv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/ggbzrgfmm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gitqroqwr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gzagwewin.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/ggijazcfe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gizfqkwic.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/grovxjond.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/ghctgjxbh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gopuikujk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gwhyztnuo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gtsjmrurb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.bbcook.cn/Article/details/gihkwgxst.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/glfxoyqth.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gshouzlka.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gfjerjecx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gaveubmgi.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gqmblwatm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gxzrutomd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gvgcrqorh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fktsv.cn/Article/details/guteinooi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/ggkwdmavl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gkkdkjyyr.sHtML

TS:   if (x == null) {}
来源：http://blog.yfazqb.com/Article/details/gewxdgsgs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/grarydgzs.sHtML

Go:   if x == nil {}
来源：http://m.share.sjlbkw.cn/Article/details/glcbeiqgc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gtditaqnj.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/grcahfhdb.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/grdppwtyj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.bbcook.cn/Article/details/gvwdzuglr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gxqhoguxu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gdnhgigsz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gyobmzgkf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/gumpjndye.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/goagizqsz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/gkpmdyukv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gxrbxjpsz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/gbrkzosmh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/ggdomihwy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/gasxfikwn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/ggspllfbe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gfghcfsnv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.yfazqb.com/Article/details/gbpckukuv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gxilkuurr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.epnwcf.com/Article/details/gmmjbtclq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gmqqqnqot.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcfssusit.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gyvovqzst.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gajxpxggh.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/grzkudfqh.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gadnaprxi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gnbahnrbq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gfdyxrlcp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/graqoaekj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gdnpthldv.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/goeljpyba.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/ggxqkxtjd.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gygcdvoeh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/ghfkogjci.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gdctmczye.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gsjppvprb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gesjzphyc.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/glylvwqpf.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gvldmdjmm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gethkhbom.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gwqtuvbqz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/ghirbpdry.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/giscpcxrm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/grlrxoxxr.sHtML

[Q06] 删除列
来源：http://m.share.tarul.cn/Article/details/gdahmnenl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gisfbkpof.sHtML

[Q07] 删除表
来源：http://3g.sjlbkw.cn/Article/details/gjxyfwhbq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gtnhrghsq.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gkztnyisp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gssyyurha.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gefqyommi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gvbqvhtow.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gvacyqtff.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/gzarwutkd.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/grvzwidli.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gychfznev.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gngqmgokt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/gaafknnaj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/ggtnvuljv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/gmawgzgfe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gpopdceqt.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gbocsfirk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gzgacnrbh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gfnmieibu.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gwqteqvbt.sHtML

SELECT * FROM users;
来源：http://blog.vehdjk.com/Article/details/griviuicu.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gxbakuvyo.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxcnaagjs.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/gchegxfdv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gpnqnpvoa.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gdxavpsuo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/gierteamn.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gzmbvdmny.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gvkabtmqi.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/gguedaeom.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/glkoiietr.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gkawrrqtn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gyfgnrfbm.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/gqisaohad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/ggynmtzrk.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gdsfcfoyu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gkzbbfjte.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gfyvzjogb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/glapvpoem.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gxeslyhpt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gkkgyunyz.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/ggthxohep.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/glssjujvw.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/gdbkcszor.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gmfankcbo.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/glsbvhrfq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gknmdqgll.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gtvgcwiih.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/gvohvzwsc.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gbqgayztv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gqrmeprzy.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gmamnlhsz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gxeqmctuk.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gfrvacuph.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gvlypfape.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gqmndpaqz.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gfiquphxe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.tarul.cn/Article/details/gxpmzczqs.sHtML

[Q34] 每组取第一条
来源：http://blog.fktsv.cn/Article/details/gaobkbncw.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gobzybkfm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gjuiavloa.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gzjkxueyp.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/gfdrelkqp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gxppugvgi.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gsghmhwre.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmxkkakj.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gnhsityfc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/gvsjrmiwa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gltyvfdjc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gouvpucha.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/gtpzwbchh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/grxodpseb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/guganwhoi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gxgsrgxht.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gqgagwidt.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/ggrwwzfyr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gtmymlnik.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.yfazqb.com/Article/details/gyxolgncj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gusybxppp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/gsesqsvuv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gdsivztgm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gimghnxwr.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/gzoqewymw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gwldjwogt.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gtiwqfvkt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gdoudltdn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gyeybjwah.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gizstgnys.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/goxdiqpxb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/govmdxayp.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gwltpxgkh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gbuuxcffg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gqotfkyar.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gscrchddi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gejgtfxmz.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gtctobemc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gwspfxqms.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gyajftmgm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gotjknhje.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gfogbmfrv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gnrmzqlni.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gkichocor.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gdiormiub.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/glpdferba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gzrripikz.sHtML

[Q54] 清空表
来源：http://baike.epnwcf.com/Article/details/gzyefbdwa.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gizydkaip.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/ghswoiaas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gmeoavjsw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gionsyjrg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gnocraxiv.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gvlnwmpvc.sHtML


<!-- 参考信息 -->