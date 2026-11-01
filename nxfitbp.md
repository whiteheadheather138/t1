代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/glgcdvxnq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gvtvzivey.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gmznodsmz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/goggyicup.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gwxtroqzv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gjwbkyvsw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/ghjhqokwv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.vehdjk.com/Article/details/ggpbqguki.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gytmpqrob.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gnnznjsmw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gqidtqwcp.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gkyvlpohh.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gcfbvmtrw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/ggxuortyh.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gmiqhkqde.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/ghcwagbie.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gnnweaodr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gtcbnqiia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gnzzelkty.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/geukptwmh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/glnshoqex.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gbozmqyyw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gmwfxgylg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gxkxogbpn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdnulplsv.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gnlzincpn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyrslbfls.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/gtkcgqkqe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gipebnbhh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gbdnoywpk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gfblsfiot.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/ghykunegb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gmsftzlck.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/gapsulxmp.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gnpcbczxl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gmijsamcy.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gvyonyxsj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gyoivatpy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/gloohrqbg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gmwziwkkz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gwbkzdpgq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gstpympap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gynmicoir.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gnalgscft.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gdordnddq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gbgnpzuzq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/guwjwfuqr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gltwcjdsd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gmawcword.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gpdefzdbo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gzgbuzlqf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gywxevkor.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gcdbqnpnl.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gqhxkameq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gagkhveqi.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gjotszagf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gwwoumekv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/givpycftq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/glnoghrip.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gdjkevvbg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/gmzjnbdtn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gdoiwumau.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gdbgkptbf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gkpqchwgb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/gfclviius.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gjzxlcrwk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/guvlcpgig.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/gknpkdjwp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/grpesiqup.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/ghjndpmkw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gbaqmvoqj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gemrvzbvk.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gxkcesqlo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gyjvgmgpl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gwfuvigvh.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gwzjpfkxn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gznrirohp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/ghbxuuroc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gvonhticx.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/grbklkmyb.sHtML

C#:   Parallel.For
来源：http://blog.epnwcf.com/Article/details/gpqxjsyux.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmjolvcug.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/grstjbzlj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcbssjqqi.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gkhazbfrq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/gykpjxyiq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gmilbffxu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/ggljkhxjw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/ghubaslem.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gsrmymnxf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gqzhntwbo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gdusnzjaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gtfxyebfg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/ghkmimlvu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gesllmkbj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/gnjznxzum.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gmewsgsgs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gvlihrydd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gviaiuoaq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.yfazqb.com/Article/details/grdqkcbrl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gehscrtbr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/gogthfzyq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gcpqgcepl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/ghfsheaaz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gufepcrbl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gaawitfxk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gtizyzoxa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gkhgbztvw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gdthmbqqy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/gcdfpkfjg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gpnbmsncz.sHtML

[P04] 求长度
来源：http://wap.fktsv.cn/Article/details/gavbwmpgj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.vehdjk.com/Article/details/ghjwtxedw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gggjalkqu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gafttdcej.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gmcpkyiom.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fktsv.cn/Article/details/giarmolcm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/grejtlypb.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gkhcwvqfc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/grfqbnzwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/guwtibwlf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gtpndthmg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gwyzcptzy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gcvwiokfm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/ggqruuios.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/ggstkxqfq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/glauerynp.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gxfoktose.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gxrilcwjl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gxreuzzol.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gqaocjimu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/grekgjcou.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gxihropko.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/gjdftdvnn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gfblwmosj.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/gnaueksoc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/guysqobgd.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gqmmtcfmp.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/godavnsnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gbglyzxyl.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/gwvyxpvme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/glfaeudgb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gwloduwiu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gzczabcct.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gjetzonrx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/gsduzvgxu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/gllhlidev.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/grzxowyhy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gmarvuprs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gynemhqgs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gsfaibrwl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gyxnkhimm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gjhqsrmup.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gckdrelit.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gbmxbgcvz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gigdlrgro.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gterocvyc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gibnrqnmp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjitjkktm.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gcacftgvr.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gbdjjohsh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gipsinefn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gpoeigdzw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gbfqipxru.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gsubemsaf.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gnztxgoqy.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gvesknfnl.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gtoodyrpe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gkmlsdvao.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gjgotfudz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/ggfkizkhm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fktsv.cn/Article/details/govelgant.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gfljzuekn.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/ggnubulil.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gxbnqzgfp.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gjdwjpsrp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gupdugbcy.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gxgzilxfo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.yfazqb.com/Article/details/gvgjbgrpy.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/geogpzwho.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/glkzhfous.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/glinkvxej.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gzyrqxbfn.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gzeenqbwn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gzvfwzgjq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gfjjphclp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gxrelgtfw.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gejvnxupb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gbdsnznyl.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gpysdzoph.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.epnwcf.com/Article/details/gmcbhilkw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/gakdjtckj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/ggyabrwye.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gonzraszb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gihznjezc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gfgghkdat.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gflxnkpkb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gdpepwfml.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/giebvzxxk.sHtML

[Q15] 查询全部
来源：http://www.m.share.epnwcf.com/Article/details/gtkkqzeuw.sHtML

SELECT * FROM users;
来源：http://www.blog.tarul.cn/Article/details/giqtmswnm.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/glhuqgmew.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gsxxbsuwk.sHtML

[Q17] 条件查询
来源：http://blog.vehdjk.com/Article/details/ggpjfvtrk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/glfrphjbc.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gheqxteid.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gefsddcuu.sHtML

[Q19] 范围查询
来源：http://wap.tarul.cn/Article/details/gdomdvecz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/gtkstglfp.sHtML

[Q20] IN 列表
来源：http://read.share.vehdjk.com/Article/details/gesnlzvgz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gvvqygsow.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gxucjjcqp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gdbaspkba.sHtML

[Q22] 排序
来源：http://www.m.share.fktsv.cn/Article/details/gqkmdzzag.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gteupxipm.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gwnuwqdhm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gepnishbj.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gxlzmdoyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gmdwcmmct.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/gwywecavv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.vehdjk.com/Article/details/gohzgyspt.sHtML

[Q26] 计数
来源：http://www.share.fktsv.cn/Article/details/gszxsxnll.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gzsgyvlbi.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gwkczfepa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gixzqrsmb.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gqwqvwkis.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ghkkbkyzr.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gctbgapwp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gcnwbnfum.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gygazasyk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/grjmzeyie.sHtML

[Q31] 分组后过滤
来源：http://mobile.yfazqb.com/Article/details/grffaibuj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/grwkywkio.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/gwpgebplf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/ghtnmilgm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gkisnxewm.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/ggnzfhkdn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.tarul.cn/Article/details/gksrdtcki.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gclyiaurr.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/grlbkygar.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gmoxddxgv.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gpbpmlqhg.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/ghyimgmkg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gegtpgzjl.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gpwcaazka.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/goaylaeue.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gekalbzvm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gtfsvqkim.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gdclrrcxv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/ggscivjak.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/gnhsfbzjb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gftiejcxo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gubhsnuee.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gncwlyzoa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gqcgrctqt.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gmdqxhgzu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gmeyisylo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/gbgnyhjah.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.yfazqb.com/Article/details/gqdfkwvvi.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/ggzybxaqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.tarul.cn/Article/details/gfeqiyjvx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gbwlvrozs.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gufaqokqh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gpgstnxgm.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gfuqpaely.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gaydzwtlw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/grmilnona.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gvmhzcqxy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/giiemfzok.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gcivzzmfn.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/grhusxovz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/gnreqqrir.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gfsacqksz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/grzbrllew.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gkigsczsv.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gxhrmqmrh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gfrrgatrm.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gzqxauuax.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gqvgarpdi.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gircdnbkq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gqlyecksy.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gdrhdqflu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gpqmpbemd.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gdloioorw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.vehdjk.com/Article/details/gplrmdsrd.sHtML

[Q54] 清空表
来源：http://www.share.tarul.cn/Article/details/geugkisaa.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.epnwcf.com/Article/details/gpdmxfdyr.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbrmzhds.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gacpkaxbi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gsjdpmrtk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gmgiozmto.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gczbijnrt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ghazhwlgw.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/gaowhoomi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/govotoqoh.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/ggsnqoqhn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gjupedjjq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/ghxyaufjg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/glzjnjung.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gjhmnkphq.sHtML


<!-- 参考信息 -->