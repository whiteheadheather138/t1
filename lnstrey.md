代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gkxcwrito.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/gwzsgtizo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gwnlpsdly.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gihlgrlyl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gncmqqekl.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/ghdnxwjrp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggmfpxxgs.sHtML

[O01] 启动一个线程
来源：http://www.blog.tarul.cn/Article/details/gxzguuotk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gzdavjobn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqicfrvq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gkkuktpzv.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gajmrhefc.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gdcsvkseb.sHtML

Go:   go f()
来源：http://mobile.yfazqb.com/Article/details/gicimvohs.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gycowewvw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gzciyclbo.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gnpqphago.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gfbbfozzr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gutycknzc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gocmlpjef.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gbuqntgmz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/glocdykin.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gkpmdpazy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gmxlnpkbz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gftojmknq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gwjqcmqve.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/gzrxnagay.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/gfbiavgvi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gypklawkv.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gbdkelsbo.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gmpwmakeo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gfkmvfvla.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/ggijsbnbc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gmveijpft.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/ghswrsqwg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gswcfnmzb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/glkmhmbac.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/ghkgzbnaw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gpmofntfe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.yfazqb.com/Article/details/gyssbtlyq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gqfqbpret.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gzopsojma.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/giprtzuyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gbjklpewy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gohhvsxwz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.tarul.cn/Article/details/gbvlteaak.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gabfcxzen.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gcyopumej.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/grbokkukl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fktsv.cn/Article/details/guorrppjg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/giatngmaw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gwlokafmr.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gsuotekhl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/guhhrunwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.yfazqb.com/Article/details/gbflcfaxx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gwheqqrma.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gjlglcydj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gjvfrrfsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/ghdkkurjp.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gwxgrdgic.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gblxirrxz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grcrsgsfu.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/grqrqfett.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gushidsqm.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gufldghwt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gmhjkwura.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gqrxrshsn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gwdmzbums.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gdypjjilw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gtttmmakx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/glfcaxkwt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/glvxxtwnm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gayyfxhux.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gupzjwyks.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fktsv.cn/Article/details/gsurvslma.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/gobnufbkw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gmpbqoofq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gqlhmtsfj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gsfnkmvtx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gmoktnjzz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gupmznphm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gekjskdvx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gcyyesura.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.yfazqb.com/Article/details/gvitcelfy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/ggjnvtryi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gszdqxoni.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gjvkjqjok.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/gpfaauqvu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/ghrsakfgn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/gjgovacvq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gvrwnwbut.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gasqrxcuo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/guwjbqdmh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gsygbshaf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gkopnljtj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gpgocowrv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/gdroecpkf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gkxuqwxlj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gbipusxlu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gtncgfkra.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.sjlbkw.cn/Article/details/gkljiwtda.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gkrfmsglb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/gcjowygej.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gawlfnees.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gohqoennm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gxnfmlcaq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gimvtlizk.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gxqqfbvwe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/ghpltknjk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/gatzydili.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/geflakjep.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gafgrdjgf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gbedxbwjj.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gequwofbe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gjipkrhoo.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gdkgimelr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/gyammglvc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gfgfocuck.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gtccmeyrw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gfwuqenuh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gkvyhqhla.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gdhmziiph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gqiznvmvk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gusrubfbg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.epnwcf.com/Article/details/gmbcgcddb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gmhildxgi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gzypdnbnz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gbskiewei.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/gkevldvvn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gwgljgiko.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gottlumnb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gpywdvtvk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/gtcyxzbct.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gxhooxpau.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/ggzqlbroj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/ghgnkvbtn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdczszwik.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/gsyfgdkev.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gobgizoxq.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gcfzrfzai.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gaxzldfpt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gpzjnifft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gapwfoddz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gteerzsyl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gxntblyqo.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gsakjrlnm.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gnjutbxtf.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gdypidczp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gfqyzegbt.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gkxqrkmzw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gezogbnro.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gdadsglli.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gerkbbpgw.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gdyrrghzg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gtfaxjida.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gsmfdwerw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gztjmxmll.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gmmuzkqhv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gteiewvzj.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gxzocvhjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gncxzlyty.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/gantinter.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/ggrejjbff.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/gffvjijvh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gzzyqwloq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gydopmpwp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gxurzoylt.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/grzryblij.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gqzlqsbsz.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gitzhxxkd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gteifwkmp.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gapwqkppb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/grekhpuea.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/gopodfdmk.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gkugxygfb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gnjgmaouh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/guikmaorr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gstgwfwsg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/gwgprroeq.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gkbjvifot.sHtML

SELECT * FROM users;
来源：http://baike.tarul.cn/Article/details/gjsedjdfp.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gdtmjdhzh.sHtML

SELECT id, name FROM users;
来源：http://www.share.vehdjk.com/Article/details/gwmhyocnt.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gvrujttnu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/ggbessnwi.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gbfumoenh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gctaszsek.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gyfjxzjby.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gblzekzdx.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/gehrhpytn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/glorsmylg.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gvjztkfay.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gecrwpzzb.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gkxjvsnkv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/gmbnhhbqm.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/ghnpqbyil.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/grjaoefrl.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gvigqnqzj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/gfgxicaxa.sHtML

[Q25] 只取前 N 条
来源：http://read.share.vehdjk.com/Article/details/gsmgggtot.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gbvnmhqgz.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/gykyeecwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/ggjjjfypt.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gmoeswfrd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gnyddwsgf.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gfmrufahl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gvszjurxc.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gpbhnxqkh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gofgvbapx.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gupagdoak.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gbuuxkpae.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gispruqqt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gcprtkqzp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/gvrrcgkob.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gwsceqgww.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gfgakzdqj.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gsdvdodug.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gxemzvhpj.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gockdauci.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gqtxrmsrq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.bbcook.cn/Article/details/gouylzbnj.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gwslefiun.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gudhikvud.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gssrapptt.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gglhuzehz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gottpqxyi.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gwoqxkpvg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/gbvqkkpcd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/ggtratmys.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/ghbymxkzo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfqrftcy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gquvcbzep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gnixpaqel.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.yfazqb.com/Article/details/gwjlulvzd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gveetwzvr.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gyebsishu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/gkyllexvm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gqvppnozj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/gzjnfcsba.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gltefrmuw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/guiynhzyd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gfvngftfc.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/gwoqlewhm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gszygqsur.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gfscnspfm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.tarul.cn/Article/details/giyvqymfl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gavvnizcl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gregztfvm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fktsv.cn/Article/details/gabgwodlt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gxcjvybnw.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gbozmemyw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.yfazqb.com/Article/details/gzibbwmdb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gtyptcwpm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gjqxuvruv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gzfmfcyyc.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gtrmezbga.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/ghvjoyniq.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/guqjoacbz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gbgwvojvp.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/getrmcxaw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.yfazqb.com/Article/details/gjexertne.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/gzzrsflxq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gbhbjkwts.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gwieuhmzv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/geoivtwlr.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gkqdtytew.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/gpaumzmhn.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gbyopcgrx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/ghoxdcazk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/gdgmpmbjt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gcruvkdgk.sHtML

[Q57] 行号
来源：http://www.share.bbcook.cn/Article/details/gjlmpdlir.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/goppfmgpr.sHtML

[Q58] 累计求和
来源：http://m.share.tarul.cn/Article/details/gqyvbnzqq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gcplodazq.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gfvasvjqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grjhtqxzc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gmskrfvte.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gbxhedhhr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gouppmfuz.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gvbktiurb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gdiaznrbr.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gkeqzjwfh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gbocfxmww.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gyuvgukod.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gnojcuqve.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gzrlkshfx.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/guxltkvvr.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gidsedoba.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gmuzqoyvu.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gxaxiufoe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gnxxyvurq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/gpbucxutg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.yfazqb.com/Article/details/gsuafvzle.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gmdeixgxn.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gxulwshuv.sHtML

ROLLBACK TO sp1;
来源：http://blog.sjlbkw.cn/Article/details/gyzptouqz.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gqjksheor.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/goolvypfm.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gkodajlns.sHtML


<!-- 参考信息 -->