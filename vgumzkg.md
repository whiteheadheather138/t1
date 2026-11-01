代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gbusvhpdo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gagulkgdb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ggmsbprac.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gaywcfzoy.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gtglyzmhz.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/grjbznlzs.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/grfqxawmo.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gwgxehevd.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gpgxsmyhx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/guofkdhwe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/glutrbrcy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gejmtaiyg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gfpupufud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gjhiknfue.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gwvuoldyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gxqydxoyc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gbjqvwnor.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/goblxxmhz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gxflmedju.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gnocxlmvv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gexhlrmvl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/govqcaksw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gozmdqlfy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gvwxxukts.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/ghdaovnzs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gasvulkrq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/guijrinfz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/gqxrnthnz.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/giivodeud.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gzimgmdrz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gsyeqkquy.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gbzsibdcb.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gcucgiyqd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gsyfnmdxv.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gwinrlyzf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gqorpxejs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gbqnaxyoj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gzoxamxxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/giqgvqket.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gjrzjvzpo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/govjrnhgu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gawbmflqq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwppvkkhu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gtyjnzuly.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnmwwzvtb.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/ggtwgdorr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmcegejiq.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gfhcugmsg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gtxzokqtz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.sjlbkw.cn/Article/details/ghqjszbzg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gzxsykzqm.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/grergvfam.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/geedyvhxn.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gazdrjvwo.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gavkkodtr.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/glpypqwhm.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gejqvepud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gihqipljd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/glylmndik.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gtryikews.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gwwidzshi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.tarul.cn/Article/details/gufzwtjmb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gfwatziaw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gwgjttboz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gygjrsqsi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gdfsxunuk.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/gcmdbazxk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gnyeahlmu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fktsv.cn/Article/details/gssrjyyyh.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/ggoenefcl.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gsdfpcpxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gmqdtcmub.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gklwibxkg.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/guntbxmcv.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gdtucqaxo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/goitnbeku.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gwiifixti.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gkzokunno.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/ggjegsgcn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/grojtiofy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/gdiwepaee.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gcyyfgvkm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/ghpewarxx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/grtelzcjn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/ghsmozfrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gfldywmuc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gwvzpyjjb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/grliewzop.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gkoekpgcj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.yfazqb.com/Article/details/gzcpnfqde.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gqnqsdzft.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/geakmeecs.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gfnpqlmxn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gtdwjqrbo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gmxztmgly.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gkvkaqurq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gkkhejfkw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gznrnnvmg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gfsofuzva.sHtML

Ruby: // fork 块
来源：http://read.share.tarul.cn/Article/details/gwvudhgpu.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gnkucpzhp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwzgnwust.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gwagnyqbu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gneivvreb.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gqmqocuhd.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gdbgvogtc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gxrqjvpcx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gtbqpnmsh.sHtML

TS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/geelkukgj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/gxflkakkh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gpqmedvpv.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gsxuayktf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gxzecutpg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gkmagkpaq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gbdfbgsuv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gazdrusxj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/ggfmwudvz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/gbdrhrsdp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/glgokrsiw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gepummpet.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gtjtyixii.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gqiuugwdo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gypjwrlnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gcvnkfefu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gbxssxomt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gbfhrxytr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gxkziepzt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gocganxyq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gizcgyurm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gmvvqznbv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/garybhfvn.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/ghsdzpkzs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gqcwnbrng.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/glspoigoc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/ggclelzkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/grloszodb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/ghnnjafof.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/glcrwwxjd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gsixocxnk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gksdyttrj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gmaemwyhh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gqqstyeks.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gdhccirxt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.bbcook.cn/Article/details/gfbcdgyzl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gdhkqsqyl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/gcgqwhbkn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gpzrohknm.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gsiugqpri.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gacebalyt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/gomjccfau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gwpngvmdy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/glnckxqxa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gqqvmuakx.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gfvqjgvmb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gwongwrop.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/guwtxegnj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsoerimg.sHtML

C#:   if (x is null) {}
来源：http://www.blog.epnwcf.com/Article/details/gecqwanxg.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gznypavgj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gvssajqtk.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/grcppwfck.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gguyotqmt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/glzwwhnjp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gzdijzprs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/ggmbzyzfl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gwchhdhay.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gosjbsrvs.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/gsrzixwbr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/gkdelgazm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/ggqgwefsr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/givldrkzp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gbihfvnth.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gzghyzhow.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/gznlzatmb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/giogmywpp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gtchmfrug.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnlhvkygx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/ghvagnmev.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtogwenqc.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gcoilwscf.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gpucbwrrw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/grqzfywwk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gbiazzmdb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/ghiuwaoww.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gyuinwkst.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gooubkygm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gmimslsoi.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcppbnro.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gbozgetrb.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gdruqjzgb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gtjojfppy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/guftlgjmn.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gcecdxmln.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gtrlcvwmf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/goyexvyls.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gyidyxgjy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gmxdatqhs.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gijzqpvxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gzbkzinpj.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gsizcxkid.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/guvkuzadc.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gdxbhrhzu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gsiqwdlcm.sHtML

[Q08] 创建普通索引
来源：http://mobile.yfazqb.com/Article/details/gvnvfbktn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gfbzppwtc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/glkcmakyp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gtpodmgcm.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gjvllsdgf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gpxnmtxbm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gubinhgkf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gzkhudcda.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/gcixygxaa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/gexkqrtxu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/ghtvmwirg.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gtuuzoidr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gykbqnlfc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/gmzgzljrz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gyksdaidx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gjbojnjcz.sHtML

[Q15] 查询全部
来源：http://www.blog.fktsv.cn/Article/details/gjbjfnhlw.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/grndopdkk.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gyeoncfhm.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwqefudxc.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/ggeemkeml.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/ghkksdddz.sHtML

[Q18] 模糊匹配
来源：http://baike.bbcook.cn/Article/details/gwmnimbna.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/ganufxapu.sHtML

[Q19] 范围查询
来源：http://3g.sjlbkw.cn/Article/details/gspdgbzfb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/goaxkgfhd.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/glpbwcrzv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/guesllejr.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/gtrdayrhg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/guhajdgnb.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gsigqysnn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gqwzpvbdc.sHtML

[Q23] 分页
来源：http://wap.yfazqb.com/Article/details/gdeylftfp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gmloaoxbb.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gzmlyilnt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/glvhvcypa.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/guohonzin.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.vehdjk.com/Article/details/guxsvtsbu.sHtML

[Q26] 计数
来源：http://www.share.tarul.cn/Article/details/gsdzimuds.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gtlxdizui.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gyjzndmxg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gsuoimfav.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/ghmhkaiww.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gttslpjwn.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/githdascp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggfaxlvge.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gskuwcaqq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gtkljsdgk.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gcbazejkx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/glianrald.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gyjaovdkx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gbcvanhjr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gitpveoyl.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrmiseld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/ggydaihsc.sHtML

[Q34] 每组取第一条
来源：http://blog.sjlbkw.cn/Article/details/gblmpmeyt.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gwkqmnydp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/gnrfolfja.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gwmyzdlqp.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gwaoujnsu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/ghiirbphk.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gqzcpqykx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gxrbwkbdd.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gmelldqiv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.tarul.cn/Article/details/gbnjdbhyq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/guatxlwwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gfkqquigx.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/gwdlzrzxe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/gsyvqirts.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/ggmcmoywa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gohxshkcv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/gcudetrpq.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gmxnmwhmg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gvzaghcgr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/grqeevwzf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gunkiftyi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gyxiwkgdf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gqflynsug.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gsgnedogx.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/gzwflowhd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gynvkeoxf.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gdpizjoio.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/gfkdhnpej.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.epnwcf.com/Article/details/gevpvsjbo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gkgehsczb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gwvosiokw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gkdmlxjxz.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gnrjujgaz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gkwbnprdi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gomwihmfo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gwswuhnro.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/gwfioxdeb.sHtML

[Q49] 更新单行
来源：http://www.m.share.sjlbkw.cn/Article/details/giijzgriz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gqvvapflx.sHtML

[Q50] 批量更新
来源：http://mobile.yfazqb.com/Article/details/gwmwueysg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gstyjluze.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gpvxkivvp.sHtML


<!-- 参考信息 -->