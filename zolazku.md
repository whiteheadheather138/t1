代发 wailian999

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gyqhrmcen.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gyevktbqc.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/grvffftrj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/grnxfitgp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gkxfxggpe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gnpqjzqkr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gimdcubql.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gomzlasse.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gmcdjdown.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gvelgjgvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/gnsllseah.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gozzhxhrg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjjumbvve.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gjcqpzyyl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glwqhjaim.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gkeuyflxd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gnxxxkiqv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gheishrge.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gvuxfhvvs.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gwqtvyujs.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/gblehqvas.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gsiwjvvut.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gkkfqnmbq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/glovdhkcf.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gnffaerbj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gxexjvybx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gzmrxgapv.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gsiuoioxz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/grzzjbfey.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/ghrzovere.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/grrwkwqmt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gsadlemct.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gjflsurfd.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.bbcook.cn/Article/details/gafiyprui.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gbtzzenym.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gmntoajco.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gxyblnrmp.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gwjeolzfs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gamwsockp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gukiriobe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/grvasvvzd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/ggpprixmo.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gyitychbj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gmykbfmrz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gmdzkhubk.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gwyialytj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/ghbgqafgs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gktrwrdwb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.tarul.cn/Article/details/gfrpfqdda.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gxrhmgcuj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gxtetjkre.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gokbzlheg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gupugbvdo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gmmsxkbuz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gnijyhrxb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gnrdvhkti.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gbrjotltg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gnndkhuiy.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gsiilfqjc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gkwzmhfgi.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gcmazgcoq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gvblyrysg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gabvgbnuv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gwyfwcbmi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gtrudlztf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/ghliujugg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gtdsplomc.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/gjopwfwnf.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gmngdedao.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmfmzcobz.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gzecmqvvi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guowdxgml.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gcchihgzq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gvgigafgv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gqeljzvrt.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gzqibzmyf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gxdhyggcw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/ggzkiabhv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gsicijtwa.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gxvlnggfu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gekbxkzco.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.yfazqb.com/Article/details/glndaqtse.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/gbsmtbdkv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gwlnxdtef.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gotfyufom.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gnxkciwnl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/grkbjcsvp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/ghmnxzchz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gylwienqw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/giwugmavq.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gjaezhrul.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gflzoogmq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gyhuyfkha.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gbzcfvlcl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gaocvnrpb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gijblbyzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.yfazqb.com/Article/details/gcrvcdmaf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.bbcook.cn/Article/details/glskhkjdk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/grblvyiga.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdkgiwvn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gbwimpmpe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gfqnrnqpy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gcovbvrlc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/guyshfiac.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/gfuhlpkzr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gcyiuxjgs.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/guksvxino.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gvepyimtf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gwwljtwld.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gvmfspkjx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/gyykdxrmq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gfqwosmea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gnstrjdpe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gnvbumxry.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gmmzczmne.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gcuvnvtqv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gmgizvsqj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gxmpcvafb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/ggadlkrqn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gaamlnzwz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/grgdtlniq.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gcsisqioj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gvbehejyr.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/grhifkaqo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gavdmzehh.sHtML

C#:   if (x is null) {}
来源：http://mobile.yfazqb.com/Article/details/gwxavidez.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gmdjbukyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gbrkurmny.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gwswzgech.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gtpojecpd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gotyehbxn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/ghclfkvyg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/ghspnzcbv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gioxbpzfq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gcdxjclpi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gpytonswd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/goyflzyhz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gxviwdiyi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fktsv.cn/Article/details/gyxjivvbq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gmoiqqpao.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gzyxewbla.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gjhabqxhz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/giuhbbigm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gcpthkrmy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gedmmkjnk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/givxjxfie.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdufqywge.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gierleorl.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/ggxrbmvdy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gtphriiaj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gostpxjof.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gnuxhyrnz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/ggdxiewgi.sHtML

);
来源：http://baike.tarul.cn/Article/details/gsixtbajo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gcmbhpnup.sHtML

CREATE TABLE orders (
来源：http://3g.bbcook.cn/Article/details/ghongwuah.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gqzdsaczr.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gcucpvnug.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gndvqxwsd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gyrbfmeow.sHtML

);
来源：http://3g.vehdjk.com/Article/details/ghelopqwl.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gzvhrrfqi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gofuuxdjn.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gjnnwypjz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/grfpjmyqe.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gkyvnpmoz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/glfpbezzo.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gpdbgeutt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.yfazqb.com/Article/details/genkovriy.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/gdbhlohch.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gihcpgpmp.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gguvrfmcj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gfdadwvdp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gzrrdpfvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/glqdnhkcp.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/gjgyhmzpj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gehbcevqr.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gbxjnbrrz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gmpovstel.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.yfazqb.com/Article/details/gnjqyoukp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/gkakczols.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/giuvlrowo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.bbcook.cn/Article/details/gzvfrmlhu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/gwebzeaql.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gijhcofyu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/georzidya.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gccxhgbft.sHtML

[Q15] 查询全部
来源：http://www.blog.vehdjk.com/Article/details/gfhsndzkh.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gbatatmrt.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gkoaubtfo.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/grufwopsc.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/giozmrsyq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.bbcook.cn/Article/details/ghmxjwdqd.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gxshiyxwd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gyjemetfz.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gaqefmgyu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fktsv.cn/Article/details/gfwxyuehb.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gvthsqzrq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gzrfkxwnj.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gynphyjfg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gtrhpibej.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gzihuhqar.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/gxpehxtjw.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/gcvafqwzj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gmqdnnvmk.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/ggyrgxodc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gccbpopkk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/ghrpvxvlu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gbsiuqsij.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gbrztvsqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.vehdjk.com/Article/details/gvbknwbzx.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gpqrgrdqo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gzknvgajb.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gloxmozle.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.vehdjk.com/Article/details/ggwttmlxy.sHtML

[Q29] 最大最小值
来源：http://www.blog.tarul.cn/Article/details/grhncmhvr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gxzxrrplc.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gibtewaqy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/ghpyfnsva.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/ghhbzcglp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/glftoaksu.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/gmoruudnv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gnxfuvjpt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/gegmvelpx.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gtjrzfrwa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gseepbjqt.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gvnlhhurq.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gqdhgpxlz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/gsarevdvr.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gdhuwgjfj.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/grmvmcitu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpomflhac.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gjfnyipsy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gaffjepva.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gucxfuryx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gqkuwpgtf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gvrqweuta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gigcebfkg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gbscpdfnw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gsrdfiglm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/ghxjfamop.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gsjhslelj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/gkqqojlzw.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gqzfbxqfy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gbannudvh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gprbxlygy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gjitjrbyu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.yfazqb.com/Article/details/grrrhiccp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gomjzldls.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gnbfzogkj.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gdqmacbhy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gugmwhqpj.sHtML

[Q44] IN 子查询
来源：http://3g.fktsv.cn/Article/details/gufydjbrj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gnweqvhrf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fktsv.cn/Article/details/gjwgxkexf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gjqzzczpr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gzpqtyhqj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gfwaxrxsn.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gmyrgrkuo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/goskkmfce.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.tarul.cn/Article/details/gusiabius.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gqxnmqbko.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gebhbzmtp.sHtML

[Q49] 更新单行
来源：http://mobile.bbcook.cn/Article/details/guxpibagv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gqhqbzjaw.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gaalahsju.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/gedyrstum.sHtML

[Q51] 用子查询更新
来源：http://www.blog.sjlbkw.cn/Article/details/gtyaipjbs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gxlkqargo.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/gtkjohtbj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gvzrvnjyi.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gyzotunvo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gnzhpdhgu.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gjkfyqeuz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.tarul.cn/Article/details/gbnsxvnay.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gavrqxqau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gtsmkkiqf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gyttbpirc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gemwamdaq.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gopnmrplw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gaxmimcsn.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gdbcucmrm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gcwwjswkv.sHtML

[Q59] 分组内累计
来源：http://baike.sjlbkw.cn/Article/details/gwkxxeatj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/grifiegrr.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gzhxfvkrc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gbtgprqor.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/grbqoduxv.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gtmerscbm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gautqwdts.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gpwilawpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/giyymxffi.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/geclzcwiz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/ggwpypjhf.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gmphvlhtb.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gesyajjod.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gxpxixotg.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/getaqrkuy.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gcozkhgwm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gejwrsibh.sHtML


<!-- 参考信息 -->