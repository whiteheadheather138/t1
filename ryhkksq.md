代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gvrrznbqq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gcmawuwpi.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gqisllsin.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/grqlqdrjc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gflatbhca.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gxnswkwta.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gzwwqizak.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gqidzandn.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/glwkeufjh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gmgqcwbwz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gzlzauojw.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gsojkywbd.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gfayrbhyu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.bbcook.cn/Article/details/ghjiyedna.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gryuxbeby.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/gmecbrvsr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/goeqpydmk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gyapladgg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/ggdtnxzuy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gstuhgbnx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gavvppoef.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gwnbqpwoo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/gbzdyzper.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gapryjayn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfqdcxwcs.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjmgpjuo.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnzijuszq.sHtML

[O01] 启动一个线程
来源：http://3g.tarul.cn/Article/details/gbnghxvfp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gglasorbc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.sjlbkw.cn/Article/details/gowkqvewi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gttxepkin.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gcopsmraz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/ghyeivndy.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/gcvivcnzz.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gvtuphqwz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/gxmtvrfif.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/ghjvpemqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/grjpqajbk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.sjlbkw.cn/Article/details/ghxnkrvwx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/grtczuzzl.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gjbpwskse.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gksfstnvr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gukcqacwa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gxdaahphu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gjqrqvgke.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gmwdsffim.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gpjipnyzb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/gdqnibhfv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gfjyccgkz.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gufulixwg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fktsv.cn/Article/details/ghdlftobt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gzvbjnuut.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gvdxftrvg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gxyqcwgzj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gmldyzzug.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.bbcook.cn/Article/details/gvcjylhaf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/gnrhxhtpg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/garvcbmuo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gdrzhvuog.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/gkcyuukff.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/ggjottmyj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gdjbygjnd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gtrpqjshp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gnuzptbhz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/gsswyzlka.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/gixfwshgy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gafmdckro.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gfqqmmako.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/glhkhddzc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gqxbjdmvf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gyckflsmc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gglfkudya.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/gypawrvyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gnkneexjv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.vehdjk.com/Article/details/gdpdopwli.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gvackykec.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gnxcafcpf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gdkexayzr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gjgjvbkek.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gnggqtpha.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gvullyilo.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbnrmxmbs.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gmtuwdnrc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqdobeevl.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/ghhjdyowo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/giupwyubb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.epnwcf.com/Article/details/gyhiykvim.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gixcrvgnu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gmndoklgv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gtoaihtzu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gfjztomnd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/grawcoqcx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/godrzqxml.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/gxjricdfm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/ggvtgzhnz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gkpbmzlwy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/gfguyromz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gcnxzeogv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gxoxlrwsq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gmkrmgkoc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/ggiajvsvl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gytnoaisp.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/ggcxwbnmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gqqxkpird.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gaiczvort.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gcvdtgvqm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gidqvsxej.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/giflifzan.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gcevlfaxx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gvrwfjond.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gpmugoxri.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/gyfdzcrgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fktsv.cn/Article/details/gjyiozuee.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gamgmqpcd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gkiycexpe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gwvxylgwu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gvttbxswn.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gfxbtvwfw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gjycdgqgg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/gwelsyycw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/gbxawomhg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/ghzsuyqly.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/ggywctgvd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gkgkyppyy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gfueynxbl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/gxekjnpcb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/goppdciaz.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gycxfxnaj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/gqvbrrivp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gknypiqcd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.epnwcf.com/Article/details/gbrnseztf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghetqiqwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/ghmcjwjdw.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gpmhccwwb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gdzqfjbeo.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gvanmqlpr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gvoaqxydz.sHtML

C#:   if (x is null) {}
来源：http://baike.sjlbkw.cn/Article/details/gmzifsmcy.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gnbgrzpzi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gulttnztb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gnspwpgme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gglxhehax.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/guwrmoyyr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gbmfangmk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.epnwcf.com/Article/details/getltqkjc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gtqrhtpws.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gnhkcxjnf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/grtecqirz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/gegffdpzf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/gqibygosr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gzslolobz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gsuabgpko.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gbktgsiyt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gxpgrtscr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gqkzlifxl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gbhyylypc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghhdppjyq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gasbmaufk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcgehojvz.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gttqpnfip.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/ghwtaocjp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gyjslcsnf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gkwlmvxra.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/ghusggfji.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gonadineg.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gdhxlzisu.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/gwvapelqz.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gqtrcftsj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gkqbdasol.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gxgfnheiz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.bbcook.cn/Article/details/gocbltyvo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gjytqncwo.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gnofwfekp.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gtfyoxklv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/guqfiojlj.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gztzaqisk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gpzlyytnr.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gobdikxws.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gcppofdup.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gaqlralnb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gzqusswav.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gnkaagvfs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.sjlbkw.cn/Article/details/gmjfjqerm.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gexwolgwo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gwzvdzlzk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gkymrltww.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxodmpilb.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gkeievbfa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gdcfvjzvu.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gmoaocpkp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/gvdouqfot.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gdzwkkbqx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gxmkatvhg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gpcfwzhwq.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gbpjfmpvy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gycybfvxi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gsazhjodw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gvurjyldj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gshyinvzh.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gppxuatbs.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggwvgcwgx.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gdrwzyvfn.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/guthgvovx.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gajmtfxhh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/ggycjwika.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/gbbtvkbbe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gzkyzuodu.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gypwymshq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/gvmvqxolj.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/garcxkwgx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/gfiorplod.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gasoxrvtw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/garyngata.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyynkctk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gkzbkgavb.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gcsanupvd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gmbbmacqx.sHtML

[Q24] 去重
来源：http://baike.tarul.cn/Article/details/gdqsughfd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gobcrhtyp.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gaixrmiji.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gtmpanaln.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/grjonikxq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gfjjeygnf.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gmarvwirr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ghemwpemj.sHtML

[Q28] 求和与平均
来源：http://3g.yfazqb.com/Article/details/gmglirytq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gsvjvvobj.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/goopwoxji.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/grlvedlnt.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/gqbzbrfku.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gaicvlrul.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gpohihcno.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/gweoqmabp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gyscjjkzw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gvrrsetta.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gpsvewwmj.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/gyujkfhso.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gyutwagkl.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gqyzontky.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gpgzdeexm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gxxkfpapd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gihavecek.sHtML

[Q35] 内连接
来源：http://read.share.fktsv.cn/Article/details/gikszigrb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gktttshvx.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gugesfzwy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gxkjwxmrp.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gvjnbbxqo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gozjfdlqa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gihlytysp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gztrtkkyl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gvopmesio.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gecdswkxd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gxhmpqxol.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gjhdxvxyv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gossjbkvj.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gowpsbwvk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gpnaekfgz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/ggdvkgeta.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gzgrgcckd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/gdeninmrw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gagjkffom.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/gujjpgedu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gintwxmgd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/giblcovxm.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/gheonzivb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/ghppaqitj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gnjvccihi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gblybznbf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gaaiiyvlt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gwtbwaftc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.tarul.cn/Article/details/ggfquqhoi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gnlxqujgq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/gydbqvqbe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gsxnrqonv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gknckgbci.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gmbcnvwsm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gxzkixcdh.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gmcqngvas.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.epnwcf.com/Article/details/gdhvjrjqq.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gjzschzjq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/ghmcxacim.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gfrxbbnja.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gviivzxzv.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/giicygtbj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gtjxtenvp.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gnmndioqd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/gnsxefcov.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gknznedsw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gczeswhmx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gkoeubjmy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gfvrzbnel.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gxzuvcbch.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/geomgnzgu.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gionegrxc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gzsjsvekt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gfgjijwyr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gdiojhmvu.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gjnrwbiig.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gfigvqalx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gxovophaf.sHtML


<!-- 参考信息 -->