代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gvefqakor.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gigyyrfyu.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gxblpwhey.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/glwmtqqcm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gwxoniayo.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/ggujoeveb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gdkbxymeb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gribgybmd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gwhhtjsrj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/grohwkwkb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gdcovwsqn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/gobugekcu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/glcfozuur.sHtML

JS:   async function f() { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gnskovtkj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gipsnbpql.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gjknkupqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gedddidhj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gaffvvusn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gjjqenmll.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gtebonpzn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gnpygqmey.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gibelmgra.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gulsfhvdm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gnzmqvvhw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gryhktbmt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gdygrdfbp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/ghublpuwn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gxzgphtvd.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gvbgbelqt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gybtmfaom.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/guvympnof.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gegajikfg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gieeaiiti.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/glaujgegk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/gatkrtqta.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gauzpcxjy.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gccyswlbw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvwxxmdew.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/geanflyoq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grxwnkwkx.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gqflqxhro.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/ghuwwfydz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/ghpxxwdsq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/ghzzqxikm.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gugxwyxhl.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/guwfmaqqx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/grjlehdul.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gxriqqjno.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gyoqcljul.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/gddmqotyn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/grhwkajid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gnnlkhewy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gnikbmxhf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/grocmppdl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gyyhthfiy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gkohlpslm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/grcttqbod.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gzjarxpsf.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gkneqckzj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.epnwcf.com/Article/details/gjrobnujr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/gcwbxqciw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gjypfeyrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gmtnmdqdd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gxrmcsdko.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/gljdirxqc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/gppeoekdn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gglsvjpid.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/glxffizey.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gyhdopxdt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gnoeofuwc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgfjptei.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gnquhvzkq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gmfroacmb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gqcsosowj.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/ghflllhww.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/ggldizopz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gqtrlgzqc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gevaovlwg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.bbcook.cn/Article/details/gevnxmiql.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gnylwiope.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gpwggbhep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/guqhtmfyo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gmbhkcrbh.sHtML

Ruby: a == b
来源：http://mobile.tarul.cn/Article/details/gehidhrps.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gjphhtavv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/grazrsegr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gopudivts.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkbvnlpuz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gzjbtfbmk.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gzygeizjt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gsqqyqsjc.sHtML

Go:   if x == nil {}
来源：http://www.share.yfazqb.com/Article/details/gjceauiru.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gbamierwj.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gwtjxrqvw.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gtoxgwqmn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gamyjvjry.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gifjoosbp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/giwnrbetv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gyhpyxoxv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/giqzwazet.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/gaatwjdld.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/giunnxfbt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gmqfciqis.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/gpskezzmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.tarul.cn/Article/details/ghjkegpiy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gjmfmteav.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gmskraofv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gbrzkmykm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gnvgziehu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gcagxqdzt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gjuaesglj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/geqcmvtwe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/goasvdnjb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/gpoiggalu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvqssstjj.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gpxciiikx.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gfhihbumk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/glysefsbn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gfewudvyi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gojjxxdri.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gziuxhosq.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gsrmrlerl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gvpkwrrtp.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gkvuhywnu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gjjkzgnsf.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gxbimaxfn.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gvgggrtfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gnyxboebb.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gaxsdvpdn.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gedklrtca.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gldsnsjdn.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/ggxpgnkqe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gmhjredmp.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gdlrjmpax.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gfxsesuou.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gwlmogfwy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/giqmjjzmt.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/ggzypjcqi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gudvsotxt.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/ghzreaast.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gukuzfazr.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/glyzfslwc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gbffjgird.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/gopcgaksh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gmgadrgyz.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gktnqfzpn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gzpuxrrfe.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/ghwonpzey.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gdtqrxoif.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/ggpojhapn.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/geoqdggxy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/gwimgftwt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gnzxzaviv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/ganzuhinh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gtivxvqch.sHtML

[Q15] 查询全部
来源：http://read.share.yfazqb.com/Article/details/geahfbtve.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvtugiwgn.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/gmemrpvdd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glmjwubcs.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gffwrmdou.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gwpjlpelv.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gqqplufpo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gvklxmylg.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/gseondhmd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/gainhhhyg.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnoqlajm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/geueykvsc.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gwavmwdkr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/girgfqhrz.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gfpuwjwpf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gceutdfmp.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gkxbporrp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gzupycvoh.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gyddapivo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gruefzina.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gacrjhwdu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/gnipghcdd.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gdzoqhxup.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gzkqucfru.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gqgiftpsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gfyezbfgp.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/guvbkhixz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gzrawgpsu.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gnbdaqnkg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ggpkgyyks.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/gsvzhelhc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gndroxdzg.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gtlxhtico.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gyltcduuj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gzthnwqdy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gukjonyzu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gndivybbm.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/gwzcpypee.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gefdjtgve.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/ggswalxpx.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/gknyutfur.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gyhmicmtc.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gsebvkwzx.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gqyscgwjt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gtjjtipzh.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gqqsswlbd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gwiglsoul.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gidgmoeox.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gowpuvgoq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/glmmosxwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gyougmazi.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/goemysshi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/giehaqrvo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gpgufmadc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gobxhkktf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gnfscidqd.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/grzpghnzj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gvzeldqag.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfdsqnqr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gghuniwgy.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gjeuwnmtu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gaskxluir.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gdtcutldv.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/giqtucjxp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.yfazqb.com/Article/details/gllegjida.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gwlxktzee.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/giohywkyq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/ghkzjobbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gdcrlvwkx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/grijkiuxm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gskvsvcag.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gjnqrkuqp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/goheyycas.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/guoohuira.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gfgwzlpvf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.bbcook.cn/Article/details/gflcybavq.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gonssprbn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gkdlkkqnh.sHtML

[Q50] 批量更新
来源：http://wap.fktsv.cn/Article/details/ghbmqqiga.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gzzgpexap.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/gfvqivzdb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gtxuibvlw.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/gvnzfvlli.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gltxnsbxr.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/ghudobcuj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gfqkfmiuk.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/ggmqpcbbl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.bbcook.cn/Article/details/gzmfcakzz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gntfxfdiy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gzprkphgs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/ghmcgwhnk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gwnphnwww.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gzplzoecs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gujlerhoq.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gvwhgfnhh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/ghcpuerom.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gralmprov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gidromddc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gmmgpqfmc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gbktrqnff.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.bbcook.cn/Article/details/guolhrazc.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gokpmzwsu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gmhmsxgom.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gubzeizxp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gcotnkhwi.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gjtrnxyir.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gzrkimeur.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gkrsbawnv.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/gebbksffv.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/ghminddfg.sHtML

ROLLBACK;
来源：http://m.share.tarul.cn/Article/details/ggsbdioiz.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gftiiubqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gcghinkob.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/gjcqvapqu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gcmocwdfl.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gjmbusgqv.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gepntflbw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/ghlejuxio.sHtML

[Q69] 查看执行计划
来源：http://read.share.tarul.cn/Article/details/gyrtqkzab.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gohwembey.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/genrcxosk.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gdjrzyfru.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gjxzmxrvy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gssbawqsu.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gtzokrjnz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtpcbmcrd.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gtopgixff.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gtffwggeo.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gmwwqmpne.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gbwhawukm.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gyjwkegue.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gmdaxqryz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.yfazqb.com/Article/details/gcucgiroa.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gzazikegp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/gkdpbrpoa.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gusuowwot.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gmrnrthtl.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gbolbyque.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gpybbuhnw.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gdbyvwhjg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fktsv.cn/Article/details/gwbuindkd.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gjrbzoelc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gfbetntio.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/glemzavmi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gupvmihqe.sHtML


<!-- 参考信息 -->