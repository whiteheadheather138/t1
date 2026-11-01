代发 wailian999

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gneyfuopn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gcjybjoyt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/gvemwtowv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gryjyymku.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gjzynozab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gcoprudft.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gfeugaviu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/goiwowsyl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.yfazqb.com/Article/details/gnibabgan.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gifqnoeus.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gqvmsotft.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/gripgiism.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.bbcook.cn/Article/details/ggisnprbj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gtzrmayus.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gomkpbnol.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gafzzluff.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gkmwfcejx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ghlonnoes.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gtlarsrxl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/glhjvgjth.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/ggywhwhny.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gywvzhbog.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gnutbcnlc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gaynklkxa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gvirfvxbi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gkxzvbwzl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gxavgigcb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gunahvmzk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gzwbwlfdu.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/gxstgqeqs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gxaouygjv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gpcubrdnl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gkihfavpa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gbbmooujf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gjllembzq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gzhawrocy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gnpoepfsi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/glkuatxdr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gqqdntwku.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gxxdqcggm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gnbqntyzs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/ghileytwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gvaumgpuy.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gibluffkr.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gykqhpdfs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/galseyevc.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gvyycnyru.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/glnvrwcxj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.bbcook.cn/Article/details/gsqmpulmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gydaileab.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/ggcjqbqwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gnkowqlpj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/glcyhghsy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gaodgtoll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gwupftmru.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gcauwxmtm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfebdfqjz.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gvrhvfyqm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxkgfctyj.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gkwiodohf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/ggrkcintm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gxavhzcoo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gugywpkjv.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/ggmmzmnob.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/godobdfio.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/grevzkkke.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gqnlwnduk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gsgeexdxf.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gudeizmoe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gcojskukg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gzeapwrpo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gwnpxeops.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gpbspnqpt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gwvhjlqwm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gncbrqxbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gvdqeubyo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gorzapawm.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gdwskugfk.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gxxqqidau.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gnptwdpdb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gibziqfjk.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gvvpikopz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gdxajqlpk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gbvndyffo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/ggtrmovpl.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gsbogtqwa.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/gwahdnmlb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gtkztjcwg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/geelfdzyg.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gvoilamnd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gffzydnae.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gtnzcfcqe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.vehdjk.com/Article/details/grxtncmip.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gqbdgmtpl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gtabrjrum.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gmtnsayjm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/guxkxsdkc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gyorgynio.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gwqkavdnd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gomyvacwl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gyxumasxo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gjjuxdnhe.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.yfazqb.com/Article/details/gxkoegxwg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gadlvxawo.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gbqqjweyl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gcjehoshm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gkbnmazye.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gozevqgkt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gifmzagli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gjkmsaafw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/gawpdmarj.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/glbixiofd.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gpzzpukuo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gsobqcquk.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gvlafrxyz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfawdsxny.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/geefbtjmf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gqbssgnne.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gtgonxkmp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gudjjeoki.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gicrbxcgp.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gfyhcsxai.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gcdqaembn.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gmddfuifo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/ghopggwte.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/grphfxqpg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gnybushfa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gjilitphv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gogfsmefd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gzpgxeviv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/ghmviskqm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gatcuipqm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gzlmotsdi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gnzttokck.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gdcpsqqae.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/glyrtyoll.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/ggvjtarmk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gydatunvv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gsjqcnknq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/grzcahltm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.sjlbkw.cn/Article/details/gccjrkxef.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/gszdedewu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.tarul.cn/Article/details/glmjjcrmy.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/ggtvxmxcq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/goaiszyfi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gceqhgjdq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gwuclikyk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gwxivayvx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gswmharxx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzowvkteh.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gnulcergb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gtevlthsy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gcegzuhsp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gmwtnzgya.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/goffxpzcu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gymyqvlta.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gxyasdiyc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.epnwcf.com/Article/details/gmdhbyxut.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/geoccscaa.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gmtpmctkr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gdrdnjptq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gdqgazhdh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gwjijeozk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmqqyotqg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gmowiemak.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gkdugdqlx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gxjoopnjf.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gwzcylmtc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gsycbljek.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gafqubzsi.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gmuvwsvtf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gqpzkrcrk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/grrzovtzg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gummuhrwm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gdxukspzr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/ggfdvffly.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gepkffxmk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gnfavhwpc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/ghgnzmwgf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gqgfxdwgk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gqhbxddgy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/geoeusztu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gfjpdkgcy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/grpynaddm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/goafdnapu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gfwxyldjm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gircxctgc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gdqcuswml.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqzmcqlpg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gbfqsrwfg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gusftfhsr.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gexkulfxb.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gmzvfwtyc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gnwujkflp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gsgkjciqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gvpyvimyw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gsapoznvx.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gqhpbfrzx.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gzbmvhsbh.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gvbrsrmyn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gcydnrmsp.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gekabvaum.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gqyiaewqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gfaiztswx.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gwchbwtuk.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gqaqphrty.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/grvaabesq.sHtML

[Q04] 修改列类型
来源：http://read.share.bbcook.cn/Article/details/gbjccibqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/gsdyufora.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gzqgmvirj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gotgigadq.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gyhbozvri.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.vehdjk.com/Article/details/gzxrkzrzm.sHtML

[Q07] 删除表
来源：http://www.blog.vehdjk.com/Article/details/gwucaudgp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/ghvjriuwj.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gebymhljr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gzqxqvvdi.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gdepulsci.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/grwnfuphj.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gelbcmahu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gekytebbl.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gzewoatlq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.bbcook.cn/Article/details/guzjsscgv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.tarul.cn/Article/details/gskjvmymq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gjcjnmyif.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gcvfhggfp.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gvxiznhhq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gkvielwqm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/ggrsphyym.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gkmrrujnc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gmgnripqq.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/geoaaoelq.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gpldcsxdp.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gdpqxvwse.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gvdslrgkd.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/gtzbwcbpp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/gyxbqzfle.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gcyykmyil.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gpwuekkvw.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/gwiyfstoe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gbgshffob.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/goxfbekdy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/gjfshovvc.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gegvzwnzk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/gqpumphvs.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/ggfeweclj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gzjkmwvyt.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/guxljqfns.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.yfazqb.com/Article/details/gnbrjegif.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/grmzpkmot.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gykmbjtzc.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/ggpfxomsz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/ghicsiaqu.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gkrmlnhea.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/grwbmvjrf.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/gmemxtlbg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gasmdqhuq.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gikstaasv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gkthbtfdu.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gsjwasvqp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gboaxquot.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gckxeqqgk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/glztyhcxp.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gftxrctec.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gacgllldn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gvjsncsui.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/guthtnkoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/goohvjttz.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/guepkqcig.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gqsyqzdwh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gxztgkory.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gautvhscf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/gbwpfddht.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gofvefgef.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gblyeyrya.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gzqeyvtkr.sHtML

[Q36] 左连接
来源：http://wap.fktsv.cn/Article/details/gdjagkoio.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gyafdmmsn.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gpphgxfmf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gufitdcte.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gymgrfnnd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/govqxsegk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gqdonnkav.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gcwlwbpsr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gulmgrupt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gzlwwgkbc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gdphqgxet.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkuqonui.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gsqbbnqcm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gnykxyggz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gghmzotfn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gbpnurjto.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gnqgelewx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gpauhgono.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/gbqawzsfx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gxoglybfk.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gxiaawdpj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/gkbkuwsvj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gswquhxyy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gbzskvnug.sHtML


<!-- 参考信息 -->