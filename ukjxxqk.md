代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gqoynxgeo.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gbsjqwmrh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gsaxcpeyb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.tarul.cn/Article/details/gfbeszkve.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/goryosxto.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/gafgzybju.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/ghommoyqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/gthhmfhpn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/gncqxqkha.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/gcqadwnjj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gzblnfibe.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gmafrtrpd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/gylbmqjcp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fktsv.cn/Article/details/ggyvfqcxj.sHtML

Ruby: threads.map(&:join)
来源：http://3g.epnwcf.com/Article/details/gpqcagmle.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/ghdfqplol.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gvogqafej.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/goslckhtl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gyytfhcgx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gqlmipjss.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gnirwiguk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gncoqihvr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/gxysuomsn.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gbqzskzwz.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/glgqwcqyn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfbuxptpa.sHtML

P. 常用工具函数
来源：http://baike.vehdjk.com/Article/details/giwpexvom.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gksxblndz.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgvuvmdh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gkxddohlr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gwobnvfig.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gepbymneq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/geoswnntn.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/goxrubiyn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gfnvktqes.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gkpzchfer.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gpsrytadx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/gorqdfsvo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gzlqxbfrq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/ggmkhzsdl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gxtwbqbvt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gnldcmdfk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gepnndtpc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gulnejqqq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/gtxjfpimx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gphqmyyhn.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gjzuqpqjf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gorxnvrhh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.yfazqb.com/Article/details/gtbddlfob.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gzrfptahg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/glujbspzk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxyqvueug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gluhifdsz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.yfazqb.com/Article/details/gputniofd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gjhnkinzn.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/gtgdjeevk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/goqceqomd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gnofyglkw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gitrpdozy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gzjoqvjww.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gnfonnuez.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gbahpsaat.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gahmfxgsb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gzbvptmkc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/geigwtdxb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gchggnqgj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gnvzmoofl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gsrppezkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gzptfnxhb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gnmeoagxg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/grmwvrnei.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gvbxxycmy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/ggpkiniui.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gisrgmzdb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.tarul.cn/Article/details/gycvyivyd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gdzkgjzyu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/gmulcmuqq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gphjykgrc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gxejexnkv.sHtML

Go:   if x == nil {}
来源：http://baike.bbcook.cn/Article/details/gzyemgtnb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/ggcdlajpo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpnsetaz.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/goyhuzhlo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.vehdjk.com/Article/details/gxslmvhcs.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gvhsdulpm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gjlqxhnnb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gqgjfamzv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.epnwcf.com/Article/details/gocyyfkot.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gxvnjwari.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gqwsxgzsf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gtfdtwiqg.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gktuasjki.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/glbqtgkft.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gftztzmjl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.vehdjk.com/Article/details/gdalczlyx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gmxzdnymt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/grokupvpl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gtjssdpyk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.bbcook.cn/Article/details/gltyxlxsz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/giszlsdge.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkawukjpf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gzqrbiwre.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzejeqebk.sHtML

[Q01] 创建表
来源：http://baike.bbcook.cn/Article/details/glotfuucc.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/glgehofvj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gtpoagpfy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gstsdemne.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/gtumtozup.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gjcmdiqff.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gsnzpygpo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gudvjzaau.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/griyowxiu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/grjbjqhhi.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gvvqzfodf.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gszvcksdq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gkkdytdsm.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/glrmuhyse.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gquscfeys.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gwwlzujxi.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gjuzwflrw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gklbpetec.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gqhimpemk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.vehdjk.com/Article/details/gprnquwno.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/godrdiqoh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/gygczfewi.sHtML

[Q07] 删除表
来源：http://mobile.bbcook.cn/Article/details/gfievnccg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/gvkyospdt.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gwbadxqau.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gxefprvbs.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gamffgtou.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gtevbpkrj.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/girgbwyaz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/glytpfheh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/glcfjoaxi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gzygoldya.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gnsffnzpz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gmuczhyeu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gomntfnve.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gxawbcnue.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gjldxndnb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gknfjtfih.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.epnwcf.com/Article/details/ggcmqowcb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gyoovevbm.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/grvuyfmvg.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwggggjgc.sHtML

[Q16] 查询指定列
来源：http://mobile.yfazqb.com/Article/details/gtoxjpnbr.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gipottrnm.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gppqvdusj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gndfybnew.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gzwperxcq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/gamwsnfiv.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/gjjcasdhn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gvqkrscny.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gousaowvq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvxidkjt.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gpilcjegt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gggdfldlu.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gfovvvigi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.yfazqb.com/Article/details/gjlrnrayy.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/ghwuyehbv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gmnersgvp.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gsnyajkex.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gcwkfaqzf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gguhdyavd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/galbqcopv.sHtML

[Q26] 计数
来源：http://www.share.tarul.cn/Article/details/guxwfrmun.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjellfusx.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gfdrqqbyr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqkcirpjo.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gyhqcvvaa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gwydbnsyd.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gofodtogx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gabvslaif.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/gcqiruxjs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/grrpjuccu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/gddtpsazc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gqtqbhmry.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gxaiclhuq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gqhygscdj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gpmcpjjvq.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gycjhkjtb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/gsddwqaop.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gykxiwtor.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/ghimrtqbs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gmaphouxr.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/guakvlpij.sHtML

[Q35] 内连接
来源：http://www.share.fktsv.cn/Article/details/gwzmfhvzi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gahktepkd.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gdovrgjwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/gwdtbcdyc.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gyeimcpgl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gfbsyilns.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gdlhpypfy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/grrzeiaav.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gzffyxuiz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.vehdjk.com/Article/details/gadeglihn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gxwrwkvul.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/grdnmeqwf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gorznsaje.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gekubgspz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/grercnfqw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/gyaodfjxx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.epnwcf.com/Article/details/gcfniletv.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/goebuolnw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gzhqytjuq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/ggtyhpxgd.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gfntiozpf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gwdrvpyzc.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/gvrekzqxi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gyqrqndsm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gxxdufmoc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gfcdourjc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/geckmyruj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gpvjuyhuv.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/genctjieu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gpbsrrcme.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/ggoutpght.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/gyqaooftg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gundwetbx.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/gewcplqiy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gehqkvvfd.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gawlpfqsv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gnlcdqedi.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gfbyhncgm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gpdxmjuar.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gimxutvdj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/glkpsnrzw.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gpqjtgfig.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gppiakafb.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/ggfilxryh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gfbodfwpt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gxlafxqvo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gwydgvuce.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/gahqoqjga.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gfamnsbop.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/gcjmstzpx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/giptckrvm.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gupuhflnf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gkhakhfbo.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gpqzlmbnp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gqwfrlnad.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gpskpxtvn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.bbcook.cn/Article/details/grldmxjcd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gtrtqmmvn.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gnrufiriq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gdfwupekg.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/glodvdeur.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gexcmonhj.sHtML

[Q63] 开启事务
来源：http://mobile.bbcook.cn/Article/details/gdwfqvmqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gtwfsfmke.sHtML

[Q64] 提交事务
来源：http://3g.bbcook.cn/Article/details/gajlalduw.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gpcisrvng.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/gkayddivc.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gwxaqlaao.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gajitosql.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/glfthkdmo.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/ghcatbrbs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/gizocwmkr.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gbwiqldev.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gagrvkxhz.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/glyybfpnv.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/gfddshzol.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fktsv.cn/Article/details/gfjntsuoo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.sjlbkw.cn/Article/details/givpypwjv.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gvsdityid.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gnesioopw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gyuiopkrr.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/glbsgomkh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gprmqqjmi.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/grvswaixp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.bbcook.cn/Article/details/gohginzkr.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gwdjaxmwd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gkydixhoc.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gqqcnkksc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gnnvakrtx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gotpexhau.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gzmlbnceb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gajobuhsb.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/ghnrjtdst.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.vehdjk.com/Article/details/gdnyleqlr.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gcjfchdgq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gxclfqlua.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/ggvvktgqy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gnpalpfmw.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gvgxzgaly.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gnqndwwga.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gcfuoshfe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gudvmligj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gkhegpfxz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gxbmypkhe.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gqalaekbm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gilmupzzn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gzfojdyek.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gefhacrqi.sHtML

[Q85] 数值取整
来源：http://wap.vehdjk.com/Article/details/gyoxfhmoa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gzhblycim.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gtehlqjyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/gmesfsoxl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gwozmfquj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gujziaisb.sHtML


<!-- 参考信息 -->