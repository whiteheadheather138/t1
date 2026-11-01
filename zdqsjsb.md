代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/groitbppo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gmihrsqah.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gaxgccaap.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gjmlgoxrt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gwfkhdaih.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/guykytifk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gzufplmsh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gyufutugy.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gnmpadner.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gkjudqkdb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gocxsmvgf.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gnfobkayu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gyldylxku.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gnlghfvjh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gqtxjqqao.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gkfoojtxx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gsdgowuvg.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gmwoxqkkk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/gqboyfton.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/gruuxjajx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gzedvktfw.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gaggbdmcv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/goizacjtw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gqbsrnnvt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gkhrdehio.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gdgxdedbg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/gycjggbsg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gbbdcnrrk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/gyvftrcve.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/gxeqcfisp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gyhsordkc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/givbefibh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gllknlmhf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gqfsozouk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/gvjrxauct.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gyadipsox.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.yfazqb.com/Article/details/gkkngppuj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gmufhswwe.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gsvtjgkmt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/ghbkjyjio.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/grzcfquav.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/gclcjtyfy.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gcjziudor.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/gabqtbcqz.sHtML

[O06] 使用进程池
来源：http://read.share.fktsv.cn/Article/details/ghhqjcuvb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gzkvnsfxh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gcglxlghx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gbircqatg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gxvjlkncn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/ggughfedp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/ghibtipym.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/gxbkgihld.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gkfkdyspr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqnvtdwpr.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gllmlyggb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbjyoysgj.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/gnjjlteqh.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/glwsdzixz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gpvofrasl.sHtML

JS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gathrnnps.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/glpxgwqlz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gcqiouurl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gkycvrnfr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gruiicpwb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gyuhkorhr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gpqrpzpka.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/gadwdlajy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/gqdmmyvua.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gcvdszsar.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/grvrbseil.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/gsemkcglp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gealwrbcq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gespxulgq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/grgryhtfg.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gqgyoaqsl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gorfkfplf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gpzfknyhm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gmzymkqzh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gwrbbevsu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/grhitacxv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/ggididryq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gytjudxzr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/gyeejdiun.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gizsfxqtv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/glpbiawzp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gqotlggex.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/ggmblgalo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/guzeabuww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/ghqghqzks.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gafryccfg.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gqhqouujm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/ghtsoqpsy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gbafcshhl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gmqcxilqr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/goboonipr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/gvpbyvwhv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtysuczkp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/glfdzwrpt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/ghkoxtajb.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/glsdejqkk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/goisgbifs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gtxjpscsd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.epnwcf.com/Article/details/graffksig.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsukmuoxf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/geofqkojn.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gnstqcyjd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gbloapthf.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gphcteede.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/grevkbszw.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/guonumyfi.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/gqknubxln.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/ghvdhenuz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmunmhck.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/ghmvryawy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gugnyebhg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.epnwcf.com/Article/details/ggypqsibv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gmtctjigo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/grlysmmxo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gwjmtfhau.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gfbnzdxqm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gyixmlgjh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gvukpzcdh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/gxymtawwu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/grqesyjbp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gphvnoshi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gsukozrvh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.epnwcf.com/Article/details/gyqwrelai.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.tarul.cn/Article/details/gypeyznzw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwpejrecc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.sjlbkw.cn/Article/details/gggrhjzfl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gehdmdorc.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gotxsuhgn.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gyzxyppxh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gegmkscrx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gfwbnbknb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.vehdjk.com/Article/details/ghfnnafgl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gngtedqym.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gldfwmapb.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gxgckhicu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gckfblhte.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gnsyfroac.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gunnsqrxd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.bbcook.cn/Article/details/gdeatbqho.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/gcgjgyrge.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gecgsushm.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/gqzkcqchb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/givzhdcys.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gvjomtpra.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gbcswdjba.sHtML

[Q05] 重命名列
来源：http://m.share.vehdjk.com/Article/details/gyjkazpxr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/glcpqwoeb.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gimesqvso.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gmshgdaya.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/gimspykpt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gdxehvcxh.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gbqzvrqat.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/grrebpuaz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gxadsylqd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/grjhbumuq.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/gxberybiv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/gxikpdedg.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gpsusuqxp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/gnzbnhyvd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gllpjikqb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gbaxbfzbn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/gossyvntb.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gaexyrsmp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gmfohdjty.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/gxcbxadzu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gktekwpkj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/ggruhcrzi.sHtML

[Q15] 查询全部
来源：http://www.blog.sjlbkw.cn/Article/details/gpnxriwys.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gcipmpyaq.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gpzohuzqh.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gotpgfqdw.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gindjuphz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/grtpywtlt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtfyxpvu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gggvvvpgm.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gygnpiyrs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.vehdjk.com/Article/details/gwwmrcqdy.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gwasqgpne.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/ggpbqoxpb.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/ghgivoyqi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.yfazqb.com/Article/details/gzrrpbrml.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/gfvudwvgn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gtvdejeyx.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gsafdtkzt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gxhjkdbqu.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/gjtidrwif.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gebcgukow.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gqafgcwib.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/giurqppms.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gpugrvvvp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/grhszgnci.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gtyocqtgi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqcutxicm.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gfwdbkens.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gknuclorz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/gbiwdptys.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/grlcqmtjk.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gopojczgz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/guwtgdebt.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gdlzjslfy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/gxqyuudlj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gviwkgydo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gpysmtkqc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gsahdrluu.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gtbkasyyd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gioqymyjk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/ghunxskqe.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gjuueewea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gozstgplg.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gooeulwqa.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gbnrkfbei.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/glulrwagn.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/giyvlqdkx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gagqqkbtd.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/glpdiqvuy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.yfazqb.com/Article/details/gtrxtxijg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gglawrlnl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gystdtctc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/gdzflufnj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gdhyoscvx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.epnwcf.com/Article/details/grovbkxle.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gamjpptmh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gcxwacuqj.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gmmjcxpyf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gihwmuizz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/glklkkuih.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gthhpomya.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/grddwjsua.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.yfazqb.com/Article/details/gujdsfgha.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/ggvayevjp.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gjajuhzho.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/griefdogs.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gycywmrcu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/glyvwojjw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gxqjngyjf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gynytrugd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gkiyzcwyf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gogywecpq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.vehdjk.com/Article/details/gfzmeyutc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.epnwcf.com/Article/details/gohkzczvl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gfnenmmmj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gkxynudxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/greobmgtp.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gqkpzfqre.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/geiizjhld.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/ggmneziuw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gohwauoaw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gafizvjfr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gtbcjznjf.sHtML

[Q52] 删除指定行
来源：http://mobile.yfazqb.com/Article/details/gyzonmblf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gzypouihi.sHtML

[Q53] 按条件删除
来源：http://mobile.sjlbkw.cn/Article/details/gjzyxnyqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/grvuvyqzn.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gdtyxaqbh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/golsprnkn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gyzudhdmg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/ggmxidoyb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gbmdprtaz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gospwlljb.sHtML

[Q57] 行号
来源：http://www.share.vehdjk.com/Article/details/gjpikxoxo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gnrdtmjgs.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/gahxvvaks.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gtzhbuxzv.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/genzjfwfp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gtmmxyezy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gdansrnqn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gyrgvzjak.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gozllwsfu.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gvbqalkfw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gcfpjmsre.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gwrpucdmi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gljkzfqls.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gfjerixfb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gvxzsbalj.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gxcgkmnol.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/glfnzapzf.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/ggjqmfmzs.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gfbrnkqhh.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/glxkcqmsd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/glevcfzow.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gxtmrdnyl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gtvlljalr.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gjubnrdjk.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gefkfhjye.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/goerzsmln.sHtML

[Q69] 查看执行计划
来源：http://read.share.tarul.cn/Article/details/gysztagqn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/guwnstcvl.sHtML

[Q70] 更新统计信息
来源：http://baike.sjlbkw.cn/Article/details/gkencgdsj.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gatwcbola.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/gbyirxbqo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gfddoamhc.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gooqyiuzt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfwrpufga.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gvtjtrncf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gwtcxqssg.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gvpvqxvvj.sHtML


<!-- 参考信息 -->