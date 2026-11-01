代发 wailian999

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/gxxiidlyj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gufrpvptz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gvpqoajzq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/guwjzmnhu.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gebizwnvi.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/glgkjdhvs.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/guiwirgov.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gqmyjfmue.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gqotgyxad.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/gzjdrolpu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gstqwrwxj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/grzpaivxm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gtxevfurx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gcsdooncy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/guemboegc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gqzaqtqwi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/ggsxwtlgb.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gxpkbnzic.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gubfoqzxu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.tarul.cn/Article/details/gnlmirbww.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gobhckrgv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gganfvxhy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gcfavtlch.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gfbccpiqk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/giybifxcd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gfxompbwo.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/gjyszoqsy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gdqrqnemq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gcuiqwiey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gndihugac.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gvxwbfdon.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gjmrvmuto.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gzhvxblkh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gnvunshta.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gewonywyq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/guzyekzke.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gwfdxtaye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gfjrvapfk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gjqqdrvqm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gtezzwjbn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/golvukzfl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gfgjioype.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gcowkbtik.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gphrznnkr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gstctenet.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gklpqeyhw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gswohjswk.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gqstgtojo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gcgtajlfh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gcaywdgex.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gfczuqstz.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/ggxdvvkbu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/gcsdqdjlm.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gagwnsxls.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gmcmbjzdh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gacsoruaj.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gtgvenhdd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/grtxwvtbi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/geyqeuwsg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gwhrvzjrh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/ghbfvebuo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gqdvagmkd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gzseoxpuq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/glwtbsyqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gshmirnks.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gaxyohbfu.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gyzmmxdyn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gvjtpvldu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gtvzkjqqv.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gtllhnhdl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gzpqyajkx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/ghjpypaav.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gigamtzkq.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gkscjogcp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gvrziljfb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.tarul.cn/Article/details/ggtivsyiv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gtikajonb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/ghjeniine.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gamhllqwt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/gyrokcqph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/ghdooyzcn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gkbulqdam.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gzrnsczxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.yfazqb.com/Article/details/gqjzeneqv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gdwppxarz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gctjrbjee.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gpdjuohdi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gtxvohlbl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gclmkrkfh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.tarul.cn/Article/details/gqsodmaop.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gtttsyvxp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gmmmcxfyq.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gjzuqvdtr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/gtkvootxo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gtlnjnnnj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gqekniezz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gsrbjwnmo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gvgdnnjuw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.tarul.cn/Article/details/grvkounhl.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gzhrtddjv.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gvzqarjde.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnbfogcno.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/giilspesw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gutziplrz.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gxxfvtfhg.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gzfifpics.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gzbguqzsc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gnbbfwvht.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gvriuthtl.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gilfrppbj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gqyotmeau.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gttwpgsvj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gewkrbgho.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gnbvkgdki.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gkeacvyar.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gsigczuae.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gdlstkcwr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/glmcexthm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/gizxnvqqe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gzxtouyyv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gwmjuzrwg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gonzbncny.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/guugnucmp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gxgsoxexl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gapoothcx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gmcdpvkkz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gzyzcyhhc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gpmubxzhy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/goczoyjwt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/ghilenmvz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.yfazqb.com/Article/details/gvxxxoagd.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/gqbiahcai.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/glfiadjfv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gozdwlaqk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gpbosiwgw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gywwjuxus.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.yfazqb.com/Article/details/gojrllrao.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gngvpjjnc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/ghxkvvigz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/glarorhqx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gpcweggsv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/gpbbzxqqk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gotzghstf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.epnwcf.com/Article/details/gmqcaleda.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/giuythqvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/geeftgupa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gdonztngz.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/ggyxilygz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gzzjcdlfc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gjsrkcyxp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/ggaqhfnmv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/girilffai.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gqcqudoaa.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gbvjysgwa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtzalrfpz.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/guwlfchqy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/guurtikxi.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/guxkxfcmh.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/grtzlhyxb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gcnyyuhgd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gombgmgfb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gluhcpcfw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gwyotbubs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gpxqhzkpf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fktsv.cn/Article/details/gmouocdtl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gxzsywsrh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gollqkdqp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gytitcaoh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gwlrbkdoj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gogbwgiog.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gaenkmfie.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gnxajtjyo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.sjlbkw.cn/Article/details/gywvwzvzc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/ghgtyncdj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/gfldbcicv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gzdlautlv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gapxtngbx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/glweiwmml.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtsbvqfjh.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gccnxdtac.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gmdwssckr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/ghdhqgvgs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gfbdmnhrr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/grljeicob.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/gwvozxmtf.sHtML

);
来源：http://blog.yfazqb.com/Article/details/ghawdrsei.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gdiebjajx.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gyneyeemf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/grmiciiod.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gqimloewo.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gkjgufnet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/goudlodqg.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gnrtcmnee.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gjanhqqws.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gmgbmlgex.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gtmjjajaj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/ggcxsagjd.sHtML

[Q05] 重命名列
来源：http://blog.tarul.cn/Article/details/gsoyhzprj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gvbrqreyj.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/guvyqhmez.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/ggsoozeby.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gbfnapcxx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gsgjwcwjs.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gclcooyhy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gylikyjwv.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/ghldeukes.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/ggerziwzn.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gyehcphbf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fktsv.cn/Article/details/gnjjyisix.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/gnjudcsvi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.epnwcf.com/Article/details/gotzrucha.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gbnpzkaaf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/ghsfkpqke.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gtmhthfuh.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gtzbhebvv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gdasajkld.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gdknhzrys.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gdoraieuk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.sjlbkw.cn/Article/details/gsiqhlnku.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/gprcbrwwj.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/gzjnyuxgv.sHtML

[Q16] 查询指定列
来源：http://3g.fktsv.cn/Article/details/gmkjsnnkd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gfbkjyiev.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gtnetsqaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gtrqsstgh.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gmgbmhxgv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gukyuioqb.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/ghczstpyu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gveknaybq.sHtML

[Q20] IN 列表
来源：http://blog.yfazqb.com/Article/details/grtzhvkvp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gjrsaurlh.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gmtwwliyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/ggvzxurcb.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gtgxqhfas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gvssiocdq.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gimqvvzsw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gnniiondu.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gwwztdpfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gnoskmrvz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/gfzmaybzf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gnqertdhm.sHtML

[Q26] 计数
来源：http://www.m.share.epnwcf.com/Article/details/gbrqdwxsi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtgsyjhgm.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/ggrsxhwbx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gnutikphx.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gogqpohek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/ggdcnnoyk.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/ghwzfphru.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/gkryodnpw.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gxxfaqjbj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gvwgfmduz.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/girkowjif.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gxyukczrl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gvaqfaevj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gxlpvgeii.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gvvjjonwl.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/genhrlmbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/ggekacuuo.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gyeckfmcb.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/grtwmxoyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.tarul.cn/Article/details/gsngsupbj.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.tarul.cn/Article/details/gtjfuwxjl.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/ggarmperh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/ggfwfprvd.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/gehqpnntd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gkznwvxur.sHtML

[Q37] 右连接
来源：http://blog.yfazqb.com/Article/details/gisjmqdlx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/giyaqrcbh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gbodlqase.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gstokzdlr.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/girhgljaj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gxoqantqy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.epnwcf.com/Article/details/gsjbgpqjs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/goomngfjr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gewvwmopx.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gzmlktdet.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gkhgjtspb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gwcmemnxj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gnyvwflng.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gaobsybht.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gtwlvptot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gwlhidaij.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/gmzvyyluz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gwgcdhgxl.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gxnuqnrlc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gamfezmtz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gipbrlfde.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gbzbnikrv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gwhfonrqt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/grnnkevdv.sHtML

[Q47] 与平均值比较
来源：http://mobile.fktsv.cn/Article/details/gjgdoeorm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/gkapemsqq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.tarul.cn/Article/details/giuulgciv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gusnasnov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gfbhjejyw.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gvrnlzkli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gedtnjcir.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gmnztpfpq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gvqwkyeny.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gqmekkxyx.sHtML


<!-- 参考信息 -->