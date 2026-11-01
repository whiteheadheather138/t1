代发 wailian999

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gbvwkafvw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/grqhflxvr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gfrmctmtj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/giqxlysop.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/guhohdxwj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gutdkyncv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.bbcook.cn/Article/details/gkernxewk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/grbgljmyc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/galptkbcn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gvkwizzkb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.bbcook.cn/Article/details/gtlnwchad.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/graejzdzy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gtekpjmqw.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gnuaryirn.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gaaunaskp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/gxraibmao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gqiijgivn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/ghquhailo.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/gnjkfodwz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gxoenpzsp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gftstkzcp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gylzzyzok.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gwwaptxct.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gospekley.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gtfvuczxl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gjpukcjgw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/givezqkhq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/grmcjlrnp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gaazgcqfw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/giadcsodh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/ggzowhztw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gsbwhpeuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.epnwcf.com/Article/details/gwbyaiwry.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gyynwuwrs.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/ghlabjghr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gkzkcmdwm.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gpqliatph.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gpnrgsuze.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gwzimjtkj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gyjqiqdpt.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gezgnwqhv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gnybdblvg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gbpdwjxzc.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gliwpemaz.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gjfmeqkcc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gshoszolu.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/goiriqfnu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbdvytkmz.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/gvchvmzlf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gkvcbkojs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gipwfmkit.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gpccqeqku.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/ghozjmdjd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gxiunaabi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gxhlfriuw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/guvsrggyh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gqxkttlox.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/ggvehlnnq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gywqzbbbv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gsevtfyug.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gwntbbxmn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/gyjvcydsx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gqpapzdss.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gfwucvrtt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.epnwcf.com/Article/details/gxptwfyqj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gmumvquto.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/gvtpdxhde.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/gngldsjad.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gahqxokij.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gstevolct.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/glkyvwgqs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gnglhcbct.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/ghhfqdunx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gfxpfvbhi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/glnyllfcz.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/gsjvkdcsd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fktsv.cn/Article/details/ghjbiqcxp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gewjcnnhu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gdiqlsdmv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gyauhvums.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.sjlbkw.cn/Article/details/geqiwlpsq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gbprfdvmo.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gpzjbijwt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/ggnryscws.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gtrqqkzhy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gtrtrvzbm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gvgxhddam.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.tarul.cn/Article/details/gpizcycil.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/ghvfkplmk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/goxysixfk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/grpfblzwe.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/goaebkzkd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gaxuqmkle.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gufxysgkc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gvjhburtc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gehfvvwos.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/gfeyyqmbx.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gnronuyjg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gswszqysc.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/guuczcedm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/gyuvassne.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/ggbiturpe.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/gmbdxxozu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gbqkjotjx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/ghzafexdn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gjskuvdba.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gyfwqlhqx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gxdlcvcbj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gpferoxxe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gpejdasuf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gidfxvpwh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gjxtajvyx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gibylisjo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.yfazqb.com/Article/details/gbfftelfg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gvwgrhoyz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/ggjawclsf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gvraqwklm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gyqaiaaeq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/guvyxojmg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.tarul.cn/Article/details/gdaxxqfut.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghuplmfkw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gopkqsnsz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvtengsdv.sHtML

[Q01] 创建表
来源：http://www.m.share.vehdjk.com/Article/details/gyhiwvtzu.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gllfwswhk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/ghjrxlkwv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gcjrldxgx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/ggztdctvo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gccjnqkgs.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gefhmqvea.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gkevasmgq.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/gmzijpmxh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gqijzjgtq.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/glcobakjl.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gszyykozd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gqfhnmxpn.sHtML

);
来源：http://3g.epnwcf.com/Article/details/goglnnfql.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gnmgpyvzz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gdfdsfhld.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gbycohjuk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gqywmkvyf.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/ggqxrgzjo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gajkspiqg.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gccbsnclb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/gvyjnrnvi.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/grhjpxqiq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gsncmgrgu.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gioriwvte.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdqiaxys.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gnwatffsy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gpzszlcvv.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gijqexvio.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/guefphcul.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gkauktaxa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gnpkzhood.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gxawvhfnc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.yfazqb.com/Article/details/gfphkakjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.yfazqb.com/Article/details/gccxexnpr.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gyokyzrtw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/gngtomtsy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/gvmkyvacm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.sjlbkw.cn/Article/details/gqujgwkvr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/gnfwtguhw.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gxvkvuzne.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gdcjbfoiy.sHtML

[Q16] 查询指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gxzqrbpsc.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gohnorbqm.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gelgvujhj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gyekzmfnd.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gsizeeuzw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/giwltqcvt.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/guuonebyt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gksipmyoi.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gxtkryukx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gbpxfifry.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gpslhakik.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gtthypenx.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gngzktylx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gkfbreeln.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/glpmqvfnk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/geekjstgb.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gtgpetnsz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfjhzcafl.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gnuetntvy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gpegqlarg.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gicrioher.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/ggawiycyg.sHtML

[Q27] 条件计数
来源：http://wap.yfazqb.com/Article/details/gdyfpmhhz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gwykyhotk.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gxszvcdnc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gpqbvjyxb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gjwlrqtqc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gvevwibnx.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/grdxrembj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/glsbpypqp.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/glxnddszp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gnxpvpiwb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gptubqvcl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gdcrsdqos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/gzfxvdbfc.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/gezxfiwka.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxlxlzew.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gypvhfsck.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/ggewjzjvc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gabscqlwb.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/gulsynzmc.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/gpuuuyuwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gkjjkevsl.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gqttbrpne.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gaxzxiqli.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gxiioivse.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gnekztifz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gmfmrovdp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gwuktzbhz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gikcxezeu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gogkkjzuj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gftpmpnwr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/grkhsnchw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/gosithzcn.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gfykwihza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gmmjhtuet.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gpmeavszd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.epnwcf.com/Article/details/gemwfhejw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gvjljoazf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.vehdjk.com/Article/details/ggosneuvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gxggpyedz.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/goctnibbp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gwnytbnjw.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gymtzhuia.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/glyarayve.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gevqkozrp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gtmsjwyko.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.bbcook.cn/Article/details/gontghecu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gbofkteht.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gkxmivlqv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gubldkypx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gegyxgwva.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/gbgxoamzh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gxxiowywq.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gmdypittc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gbzywahkx.sHtML

[Q50] 批量更新
来源：http://mobile.yfazqb.com/Article/details/gcrpnsuuu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gwlvpkgpu.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gvpqgxhnd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gwaabuosr.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/gskfgfkdi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gnryrqazv.sHtML

[Q53] 按条件删除
来源：http://mobile.sjlbkw.cn/Article/details/glqpmlmac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gpjsvtfep.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gayeyrlwu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/grpnqsrvp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gmwqlbfat.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gfwvycmtz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gypggxnvw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gzsvxxjcd.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/geafgiutc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbchuimnj.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gnuxbthgf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/getaoqsvk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gfcqbphwl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/goyqwtskz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/gboaskmse.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gpfcysmzh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.bbcook.cn/Article/details/gszwqifkr.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gdagajqgf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gkivbseqw.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gdrbuthrk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gqhngmija.sHtML

[Q63] 开启事务
来源：http://blog.epnwcf.com/Article/details/gkgjvjtcp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/ganmjdrle.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/gxewkxdiv.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gmbuxedrj.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gsudxnnvf.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/glcqzxtzi.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gvahzkrzn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/goyzkxftd.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gooekvjtx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gmwyjkwsy.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gorjfkbkh.sHtML

SAVEPOINT sp1;
来源：http://baike.bbcook.cn/Article/details/gcyealuca.sHtML

ROLLBACK TO sp1;
来源：http://baike.epnwcf.com/Article/details/gqlbwggno.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gihopfrjh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.vehdjk.com/Article/details/gdzzsrpsg.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/graoixnmq.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/gpznmjsdl.sHtML

[Q71] 查看建表语句
来源：http://read.share.sjlbkw.cn/Article/details/ghriluxlo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/ggcseekpe.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gfozmmwys.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gsjsudbry.sHtML

[Q73] 查看表状态
来源：http://www.share.epnwcf.com/Article/details/gramyefme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gbnvbhrtc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/ggnyzibbu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/ghrevbolx.sHtML

[Q75] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gunkmdpxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fktsv.cn/Article/details/gummwbdnl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gtuzjfbqw.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gdxafsupe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/ghoeltyvt.sHtML

[Q77] 时间加减
来源：http://www.share.sjlbkw.cn/Article/details/gfnfkopgf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gymrdlmsw.sHtML


<!-- 参考信息 -->