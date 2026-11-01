代发 wailian999

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gqhxnmsbo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/ggdghkjqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gqifcnsau.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gdeguwsfq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gnxxavwlm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gvgbcqfaw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gmqplfkgz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gharzkqyx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gfchrscaw.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/givnvwcfx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gpvzhpkkk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gpackberd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gwxkqoope.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/ghnjpbwjy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gdcyggpsh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gnqlsqley.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gzhznffvn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gbjmdvlxf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gkoqperpu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/gshheavcn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.sjlbkw.cn/Article/details/gkszvorab.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/gvxqmmnvb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gxxsoybfg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gtylopxsd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/gdfykkbdt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gozlvhdyu.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/ghmpwyuca.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gqnszveol.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/gkslttndr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gzfeidowe.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gelmjiqly.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gagnesifc.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gppmfjhcs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gfnyjstak.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gzkbjhnfk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gltcqvwkk.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gyoibcxxb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/goyocjemh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gkmobcbsr.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gddlapecm.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/ghqonpyix.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/goozonlvg.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gdvyhuxpy.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnttsljcp.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gvrfstuhl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gekfpvess.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gwmirrvep.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gqtevigdg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gbckrzsov.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.sjlbkw.cn/Article/details/gbjnpzvqa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gcbmujjpf.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gogzwhelw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gggdvdlwf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gnhqahytn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.tarul.cn/Article/details/gyfhranzp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gokrlqmmh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gfupblmjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gpsrgwcxj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/guczoclgx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/grpjuityr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gilibhzqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gvngznkfq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gwoqcycqn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gfahcuepj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gmerbuzlf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gttlhzkoh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gdatcxiof.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gdxqccdni.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gkhitskzp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gfaelrxyc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gfpoxjeas.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gsgnxxfpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gqcejxfip.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gydgpjwnj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gkudkdkcf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gyhmkedfm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gartkodub.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gvioqwdnv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.bbcook.cn/Article/details/gjizzzonj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gzdbhodwj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.vehdjk.com/Article/details/gbcvrsjnn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gqxqkzjqa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gnmveltrk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gcedqoowd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gaizqolfx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaijmetz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/gwcutxexp.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/gtoxsjhbo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gprpandqb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gibfzkupr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.epnwcf.com/Article/details/gyysfnmor.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/gahiruxfp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/gwewdttkz.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gstpntoqd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gtzuflico.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gwnfvzayy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/gcubsyufp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/grfyoaxip.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/glmubepyk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/gwkkknhqx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gwgrvdkjf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/guogvuvqs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gwjvulskr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/geoaqjtsc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gsvxdutly.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gkcatsqlg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gezyniqyk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gjchhiwyn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/gtcgnneut.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gegovvfep.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/giluhbbfa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gczgkzqbw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/ghsilnnqd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gvessmcro.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gszjdbmhl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gguytojuh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggietmeri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/gdruqtklg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpxkbsksg.sHtML

[Q01] 创建表
来源：http://www.m.share.fktsv.cn/Article/details/gzstepwww.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gejfznzxx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/grneukcyh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gqnoxaijn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gztmlzjid.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gkgqkxwpc.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gkbmhnvmd.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/gaquqevjk.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gkrzqtmie.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gyiklzceg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gfjsonlxn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/glbrdbjhz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fktsv.cn/Article/details/gtzvixyca.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gjhtuqlxn.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/gmzqfxntx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gglvnhkdd.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gvwcklfqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gommjtolr.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gbxxabiez.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.yfazqb.com/Article/details/gsgbhwtiv.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gttjwvudc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/glyimvhie.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gwulemjqp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gttzgjius.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/glhfrstlx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gvdmjwvds.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gpaohuzdc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxjtlkru.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gmxhfqeuv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gpmiiyflp.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gymlhihkr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gcocekvix.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gbrasroek.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/glsfcfcqp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gpvishulp.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gufffkfxx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gxlrbsrec.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gorckneyd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gpzgpepls.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gojyinvsc.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gbrhloboy.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/giflnmcqz.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/guuexttkd.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gjrnsockk.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gpxaftvfj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/ghoyciotl.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gibwxbgmr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gyneljdws.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgcvgyky.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/gsffhjgep.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gjmaeypuy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gtejntvxh.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gadrrdeqe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gmrmebkaf.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gjuuhyqop.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gjdetmpxq.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gdkledxzg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.epnwcf.com/Article/details/gzjznimky.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gfinfyxor.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/glylrpnap.sHtML

[Q25] 只取前 N 条
来源：http://baike.fktsv.cn/Article/details/gelhpappy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gprknorei.sHtML

[Q26] 计数
来源：http://read.share.tarul.cn/Article/details/gimahglwz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gkdntlgqu.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gqmlmkwrb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ghunzyega.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gyeqpnfoy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gtdkoaceg.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gobylxpls.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gwzvquuel.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/glqfgtlvx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdxfxbbj.sHtML

[Q31] 分组后过滤
来源：http://wap.sjlbkw.cn/Article/details/gggwyfgqp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/goklptrwa.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gikayxnpp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gaeorbuvu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/glufsjimu.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gghglylqi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gxjdzoaiu.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/gmlwqbexk.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/guoyounim.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gvcgdurup.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gtijgrkig.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gbeveiyhr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gbyagzzis.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gpugnizru.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gjwjlslnc.sHtML

[Q37] 右连接
来源：http://wap.sjlbkw.cn/Article/details/gcufvpuoa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gjzdygork.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gkallhrpe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gbkmmzczl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gjwwoqsva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gnmeclqpw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.sjlbkw.cn/Article/details/gytrzzwpj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gimjqrdcr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/gnxjovhnb.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gpvoqbitp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/guvtyweyt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.yfazqb.com/Article/details/golipcxcz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/glhwlvuoj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gvofsbjrl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/guavibkjk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/ghpgtufyx.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gzkruoizw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gpsvcmsqn.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gjhjqckqt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gznjzzyar.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/gycppwgmm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gdjhnlarn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfgzfube.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gklnikqxn.sHtML

[Q47] 与平均值比较
来源：http://m.share.vehdjk.com/Article/details/gavciyhzk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.tarul.cn/Article/details/gkfborzho.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/gooklpevl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/ghpgpuijb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/gjkpheilm.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gttkoomip.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gytdtjgnt.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/ggrzetedm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gcqqkwqny.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/glkvomdby.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gmiglyopk.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/ggeimnxip.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gbpjahokk.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/gngxzfrry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gvrchzpod.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gipytwwvc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gwnalwyem.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/geetzzqbm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gklfqwcpu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/glgmwvkav.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gfiqkffem.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/ghesmsdgp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gvycpootl.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/gpjainpef.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gihmdhtmy.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gqpbsoqdw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gtrmsibqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/grobyyppt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gvuvmihnj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gkksvncka.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gvnmiqejt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gmezozkpq.sHtML

[Q62] 分组占比
来源：http://m.share.tarul.cn/Article/details/gptsghfai.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gnpbhqsyj.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gpnoyzbmw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gwvfkkzfr.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gwcyiqgwl.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/ghhfvnhnn.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/gmcgaswks.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gfbpttivy.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gfmulrqnr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqggawibg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gupuuzpwe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/gpvxdsfhs.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gzakoibaa.sHtML

SAVEPOINT sp1;
来源：http://read.share.bbcook.cn/Article/details/gelyenneq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gdvnxihxl.sHtML

[Q69] 查看执行计划
来源：http://3g.sjlbkw.cn/Article/details/govutjhim.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gsngmmhwn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/gupvyjpgs.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/gjkeksfmh.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gdwordwog.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gefwoytev.sHtML

[Q72] 查看索引
来源：http://blog.epnwcf.com/Article/details/gslacfegi.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmkurasak.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/genmgkary.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gnujiygju.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gotdsmmhb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fktsv.cn/Article/details/gjdhbaxwa.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gcojlzjwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gpxjcdlba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gdwfyhchp.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gzyergnpj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/govqdnigv.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gtmgtxdrf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.vehdjk.com/Article/details/ggdkmpidf.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/gzknkfppv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/gfikmfkkg.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/geoxzaauv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/gjrqvwdey.sHtML


<!-- 参考信息 -->