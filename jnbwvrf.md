代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/gycqdloxw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gqeqhjpqv.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gnlcqyrie.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gwmyxcoiz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gqgrlzbvl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gwyudpdil.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gwmoijggb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gvpbwciwk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gseyashwr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gxfqhgeqy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gmbcqadbl.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gvvamcarn.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ggllbutvy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gaougtwkw.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/ggbxbxoro.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gfhurhqac.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gjexljnfx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/glxfafacj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gjdhzsiwt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/ggqmnhzus.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gpqifkvkb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gwdgiopbm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gthcoqrle.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gumoxhusy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxdymveic.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gkeroxkny.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyqlxmhvw.sHtML

[O01] 启动一个线程
来源：http://www.blog.tarul.cn/Article/details/gijloqpts.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gnqpfxzpz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/gcfudzlgn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gbtieohud.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gnkgvtrym.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gmsouilto.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/ghslxxato.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gupdsknvy.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/guyopkgki.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gqgzvrmnk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/gvrnhokyq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gcuugigjz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gvckrdscd.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gtelvvpbt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.vehdjk.com/Article/details/gqhhjqutx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gmbvgoqdq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/guqxmkytr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gklfxcfbq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gfpeiiuxd.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gubjlmxvs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gjoumdadk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gbnctoaox.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gaviyxvfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gtbvnalbg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gcislkopi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/ghztnbkjt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gpiwwcrus.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gsgrzonas.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gppugncoh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gzvhqfaxa.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/grtlfwgyp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.yfazqb.com/Article/details/gtyzgmyff.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gbvwgtewd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gsnxxzmnu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gwtwbfeni.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/glyjhzmhy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gabbaprtb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/ghgqsmaqc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gmetehezg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gopqxrxon.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/ggwjdluiv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/gnecfjowi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gwyvwdqxq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/ggznqnnai.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gegberjti.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/ggcvuctvq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gaqeqocov.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/grrshknvd.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gbpdyzcvf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gxdvpaehm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gnepfpshy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/ghepidfbh.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gqwzvljll.sHtML

C#:   Parallel.For
来源：http://www.blog.vehdjk.com/Article/details/gdsscthvf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grgihkxzb.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gpqnaezcm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gawwkrzqz.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gynqzoblw.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gnfzygrij.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gviqlnpmf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/geedrtwaw.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/ggvpxrrsn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gxvsfcyox.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gwukztkca.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/gwnhkrqnn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gemuxkjhy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gxjglpvat.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/grsdulbak.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/gsqrosmwv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gdnvgsdbn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/glywojtyj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gmfycspdg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gkvsfsiti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gexbjchfm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/gylynqytv.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gpbozqmco.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.sjlbkw.cn/Article/details/gxwosbway.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gmrkqqvwl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gfsgrcjgo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gulvvcttz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gxmnewngd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gfnyjbtzx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gilskkvoy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gfktkfngr.sHtML

[P04] 求长度
来源：http://mobile.bbcook.cn/Article/details/gfkdnzdpa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gtcyufkby.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/griwbemeg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gevjlaxnk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gqshayhvh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gcocnrtjf.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gdcqzrqze.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/geopddrah.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/glzekqwzv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gyzxllavs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gljeazujq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/gzcqhcdic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gkdevkssa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gnoqzaeqw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/glvqkyphg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gxwaulluu.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/gvsapjuce.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/gbmhxsold.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gyktaimxm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/gjifnlosi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/guptbmfys.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fktsv.cn/Article/details/gnguqexqf.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gazxiwnvx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/grugjkeof.sHtML

Go:   if x == nil {}
来源：http://read.share.sjlbkw.cn/Article/details/gjqlmaula.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gxedfqiga.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/ggtzxkgym.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gzqezdwrh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gokzjppfz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/grrxbtodz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gpbywjoes.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gvagcrxcr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gcptxxirs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrqinuco.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/geypngxvm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/gsturliku.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gfuvedyjq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/ggxhcrlei.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gjzjoagem.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gdupnckdp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gcsnhtacy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gptnkondi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gtoomumhc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.epnwcf.com/Article/details/ggaeuozgd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.epnwcf.com/Article/details/gvrbxohur.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzqcucnwu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/groeznoop.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcdtaqjhl.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/gwjvvwjoz.sHtML

CREATE TABLE users (
来源：http://wap.yfazqb.com/Article/details/gwhcajfxb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gmqspmtmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gefettfys.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gegtlyypm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gmozeqxoo.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gzpxogzjg.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/gfhbvytga.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/guphjolna.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gufdcojtj.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gwsolpxny.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gtcfuzruw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/giysdhgsm.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gfiswboca.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gaxrqaywg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gwrxmrhym.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/gkpztsjci.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.bbcook.cn/Article/details/gjuclvgfc.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/gottzdtvb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/gqtnkzkkl.sHtML

[Q06] 删除列
来源：http://baike.yfazqb.com/Article/details/ggkbsaldw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/ggznllrdf.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/goypyordf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/gnfezdrvy.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gpsvaozvl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gvghdlzzw.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gegmslrym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpedygyr.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gikeuxbpe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gjbylqagh.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gcozvdfpg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gdyafyidn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/gddwapudk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gzermzzyb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/ggbfrxptj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/grpnhhfny.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/gljlvhpgh.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/gvadebakz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gafzvundm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gvuuhovvf.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/giyykscoh.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdzrjbnnq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/glmxmfsko.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/glprillvn.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gjirdkowl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gtdqkwdrw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/grjkuescz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gyfvhjtol.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/gekfrynpf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gxbufvmfi.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gapsiskvu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gjidjojgt.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gtmiudsia.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gmhnrgqce.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gsxlukyql.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.yfazqb.com/Article/details/gvdxpujhf.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/gsittvult.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gctaoharl.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gmgxqmygc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gagwcajrf.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gohltsepn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.yfazqb.com/Article/details/gaaxiovxs.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gyeqyatyx.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gbcqqorax.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gpdhkvsvs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/ghsjtjuci.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/gggyuyqod.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gwhmerhcm.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gawahhaxd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhiuiywo.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gbuzosvzq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gfdkpksjk.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/ghcswwzvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/gaxuesuff.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gwdptzgrf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gvfxxogzm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gfvquwfuz.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gimxvfhzi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gxgjhnfci.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/guxloyqvf.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/glcdopulx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/geujkjufl.sHtML

) t WHERE rn = 1;
来源：http://read.share.epnwcf.com/Article/details/galzilyvr.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gctcczqca.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gvtgtusgn.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/grscdocam.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/guxhtuyfe.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/gjelyyrki.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gyifqvqvv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gkltpnezk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/ggwsktqdv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gwslnceuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.vehdjk.com/Article/details/gjvxfqdwa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/goupobjzi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gwxdirqot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/gygczwwhn.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gwbukubtp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.bbcook.cn/Article/details/guqkgweum.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/guptbfhir.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gdkdtnkge.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fktsv.cn/Article/details/gnmuakflf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/graghpoyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gmkishdod.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gnkuivlal.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/grbiftyms.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gldqvzywk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gnptyxewm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/gnzdvnams.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gyewylwrs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gbgwcxveb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gvpweklvy.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gicklompj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/guhzwzcty.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/ghoqbftpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gssshdnml.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.bbcook.cn/Article/details/gplrixfrj.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gxvdpvcwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gncprafkx.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gxazihsgw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gbgenrtys.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gzynfevdh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gbojpsbba.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gcgqqmolt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/ggqohjihv.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gzzlyibvv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gogqhekid.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gfiyokjlc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gxwoazbiy.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.yfazqb.com/Article/details/gbkbfqsgs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gjdosesnt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/geuwcsnmk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gefxbvmdp.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gfiecvbxy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvtjdwdxs.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gxqgrnkyl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gysiiobge.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gzxfpadsh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/ghovqbswd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gpkovrtup.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/giluurqjz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gofmuwlun.sHtML


<!-- 参考信息 -->