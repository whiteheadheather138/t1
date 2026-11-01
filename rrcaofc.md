代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gidxpikjw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/ggvbmzvqg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/gfsbfvvqa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gduvisifp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gptrowqke.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gttjnynyp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gcjyjbxog.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gkcsguktw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/gsoepklwz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gtiteebzu.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gybbevisi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/glhmtkmkm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gnurlhami.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gvgulibnn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/ghyrlracs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gngfynrrg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gvyqoztzp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gpqogexhl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gwokqqdbs.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gljjwyand.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gnawiqjnt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/gboulfoof.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gbdieajaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gvrbpfhgb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/grjdrmemy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/gwnoocokw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gdhinslpl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gdngzbhzq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/guawxxfca.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/glckuifvd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/gwytuilai.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/ggzxyqkbb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guqrnezfk.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gagxgfrca.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghmqsdxzp.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gglosxxps.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gqzhyujfv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gwhkqzuyy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/gwzlfkbgu.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gnovmfvbg.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gbrwgumiu.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gselhhrgi.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/ggfldcfxe.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gdcwkiluu.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/ghlrxhbue.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gcocxosnu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gwaeoijsx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gtlchcayi.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gusqfgnkx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gvfjsbkac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gshyzxaac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gyerttokk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gnikrcrjf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/goakhhnnv.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gvdpdrulx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gpjlsaayl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/grdngxlhy.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gjotcggty.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gvitxfdcp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gnahjnhxo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gbuhydayw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gqrvzfwvg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gqsjjzeqw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/ggahdurwh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gzkiqoxvz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gflzogaol.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gvhwrparl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gnniycqkx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gqvdyzfgj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gbqvhyejm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gchoqvkqo.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gevsdvokh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gsmvojnky.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/githcnycl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gjeqrenzu.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gjhdsphml.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjsjmnsd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gnprrpcun.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gqkhjrwtv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gxvwnrpzb.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/gupwxflnf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gnowinxux.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/gnfmaqiey.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gscrfgdqo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gqhkfyaca.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gllipycxp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/gonivjxry.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gpthwdyju.sHtML

C#:   Parallel.For
来源：http://www.m.share.vehdjk.com/Article/details/grwclrlru.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gumztzfiz.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/gjjyewqnb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvskilsxz.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/gnpwnocvb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gkmvdyudl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gbkrebnsw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gnzqgzjwj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gfshecnqb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gbrpfmxiz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.epnwcf.com/Article/details/gljpzuknx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gbjjrmduz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gdvuybpsm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gzlduhdrf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gppodtdou.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gzhzpvojs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gpthfyvju.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gkuciydau.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gdtojwbff.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/glczfhotu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/getsrbubl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gkzfbwhjo.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gxaitpewk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gkykndcfu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/greisanod.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gupeupvsp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gvwavzpha.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/guvvceirn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gtlmsgmmw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.tarul.cn/Article/details/gjfybsaaq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gizxcltlp.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gjtuugxqk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gygpgdetd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gclerkmwq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gwphjvarw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/glsbsxpyd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gjydeloyf.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gsbktrngs.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gmvqssvam.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gbypwmixr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gkpvlvpaz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.tarul.cn/Article/details/gjqjwgnny.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gfzlohhcq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gzgtmroxa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/geocrjgzh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fktsv.cn/Article/details/gzhuevfox.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gpjbsossp.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gcoetyicf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gqnepqpev.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/gdilnneet.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/giifeyjrv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gpcchzwpx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/ggavleudx.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gwehecwxi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gcefhtoub.sHtML

Go:   if x == nil {}
来源：http://m.share.sjlbkw.cn/Article/details/ggxprozra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.sjlbkw.cn/Article/details/gtwkzjlrj.sHtML

C#:   if (x is null) {}
来源：http://www.share.bbcook.cn/Article/details/gnfhokcfi.sHtML

[P07] 防抖与节流
来源：http://3g.epnwcf.com/Article/details/gepjfcahn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gwtfwttqa.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gcdcygbmk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gtoeaqufc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gaywuuojh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.epnwcf.com/Article/details/gvonwdjzy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gczxthnqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gajmdqjax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/grooxvcci.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gqismptbg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/gvmgnwuqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gtwbqnnuq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/grsikcuyd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gacnxrklh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gfxvpymqw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.tarul.cn/Article/details/goybhzdni.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gzvrrwnpg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/goizusshb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwfjnmjyh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gezsywgrj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gefbwmwim.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gvtsokgwr.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gsexrkvux.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gxmnvzzlg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gwqfjwnwm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/ggkyxsvuh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gdtitxpuh.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gwyhmmadb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gfobabytm.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gitceejwz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gkqzfwwdx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gwdpkdato.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/ghwhgiocc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gdlahthfp.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gnjqrsnds.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gjgwmdovv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/gifiqtzlm.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gfntfbjkt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gpyorajuc.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gaorzyzpu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gmdzvykvl.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/gsabewdoh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/genypxcrg.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/guolfejsa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gvjtawjde.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gxuuwmynr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gaatdrral.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gipbpscfy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/goaalsoyo.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/grusaitak.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/grgqestyp.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/grhrukehs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gflzdnkfv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gfoyzxuvh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/guubsjbjx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gvibgncer.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/gnmozbglt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/gmbikbhrd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpzmceqr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gtmwicaxx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gewrzyhxm.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gjjxuqjek.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gghkoogsw.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/glrwgssrh.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gxjxfnppb.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/gnrafybte.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gwurcgssk.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gghmptace.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/giayhuqoh.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gbegrrbpn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gmrffwxhr.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gyzndpffz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gihqcbwvq.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/ghbgmnrgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.yfazqb.com/Article/details/gceimowkx.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/ghaijzkmt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gxrjegftr.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gklwsjefa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gbzkftksj.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gboailywa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gsfuvpjem.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gcdpnezrg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/guonbmmuc.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gynrheqcv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gyhfzqxom.sHtML

[Q27] 条件计数
来源：http://www.share.tarul.cn/Article/details/gsgklixsb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnysegypq.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gxtojtkdi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gpxxbotkj.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gtjgarmbr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzqzmrkio.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gyvxydmqn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gjxhlwnez.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gmzsaytyw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gheowmulx.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gzjgrpwnj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gvathhawa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.vehdjk.com/Article/details/ghwavmjlm.sHtML

[Q33] 多列分组
来源：http://wap.vehdjk.com/Article/details/grnurnexf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gosyegorw.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gayfgshpy.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gxkwwavpv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gufgsinrj.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gfcassakh.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gzxmdgjxj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gvfhdkwgr.sHtML

[Q36] 左连接
来源：http://mobile.bbcook.cn/Article/details/grsdneovw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gvucjfawm.sHtML

[Q37] 右连接
来源：http://www.share.tarul.cn/Article/details/gpdexrlvs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gyeqxdgak.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/grhsheprn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/glemhhytn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/ggvefxcss.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/gvhkilfwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gsrdubhli.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gzlmgwloe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/gbbvsxtdr.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/gohukkoga.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/glhqczmdq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gvsmlzyow.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/glitspwxa.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gxucfnkzh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gofqlfezq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gijixthyg.sHtML

[Q43] 标量子查询
来源：http://mobile.fktsv.cn/Article/details/gotlbqjxl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gnrvhwfog.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/grliusrnw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gfkzqvenc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gytwjscyd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/goghpmtpv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gordsffrr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gipfhhkgk.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gwggxxobb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gmrssjavi.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gxbsnzkcc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gjtfqtvtq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/gfwrkqmgn.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/grsqtiacq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gnnkaeeqd.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gaopinitj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gyyywgbci.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gqahmbfkd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gzjiukfqp.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/ghiricohm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gmmlknkqe.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gwemuoybx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.tarul.cn/Article/details/gsssfvlyh.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gzaboeljm.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gnsvniztl.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gfjyzdlhg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gwwtljrin.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fktsv.cn/Article/details/gikmjvgyi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gmjetzxbs.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/ggqglgzrh.sHtML


<!-- 参考信息 -->