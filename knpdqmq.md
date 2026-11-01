代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gbouupyrq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gxrqosjwi.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gresilhtx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gpxapbfvm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gmkspywnv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gzbpjpwgx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/grqdtcqcb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/giktgufqc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gjusryrzh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gtikyatye.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gxswpngth.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gkcqmsxjw.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gqztuaabr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gmejtchce.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gjorztucy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gsutlzycl.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gsexxnadb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gyijxbnvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gkhsvwxpv.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gluizdhza.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gzzmpmjfg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gaahecmgx.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/glittvtbj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtpccswzi.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/ghpnzbnqk.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gdtzdkhyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gvwcjjvly.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gisispxmf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gomgolcbc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gihupjoak.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gonhyhszt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gbnxeqtfv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/genlcclzp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.yfazqb.com/Article/details/ghjmezvbw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gysyxyiys.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/giwocpsbj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/giuftkyhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/gbefshcza.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/gbrwhhbtq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gmglorrsz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/gfricarqc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/ggglndete.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gnixzupju.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.bbcook.cn/Article/details/gezzptunq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gxmstrfxd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gjsswnmjr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gbjzoxabq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.vehdjk.com/Article/details/gkfshtdwo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gonktzogn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gaibrbogb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/gwygvxxhy.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gqtvmpoyd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gfqnzhoyz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gtqzbdlmt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gkjyuyuki.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/grdyqgimi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gaemjuvvc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/gtwzzytfh.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/gqzngumze.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/ggvwygcrh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gbotbeoso.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gofilljnp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gqjfvxrcp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gibycssuo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gcksgamlo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/garxeufwu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gfjuauvyg.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gkororgbr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.yfazqb.com/Article/details/gfsknmrhf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/gwxcbsbsk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpdrtnrr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gzrydgmvi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.vehdjk.com/Article/details/gguincvpo.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/ghkipffec.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gfdciqtva.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/ghvrvleyz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gpbabbgec.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/ghjucgbgt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/gycksimgy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gvbgmmydn.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gbeghlkqx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gjimhcjsu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gkrstazev.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gbhhfbnye.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gzntyekqb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/ggkxxeanj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/gimfkchdk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/gxyjhyzqm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/geckjiimd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gnufnjusc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gpffvcgxq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/glhzcnjxi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/grusldihz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gytanrtyt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/ghrkysvyq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gvjqjbmdc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gobstexad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/gepaprphj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxcmjxrlm.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/gkqbyzumj.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gogvormdi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gbipktubt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gjicvndcd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/gklqpuijn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/ggkkcvrsu.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gjniigvcq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/gzojtdehb.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gqffqngrv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/ghhrkjnuu.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/ghpsggrra.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gfnesckta.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gnbajmkpi.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gebqrwjpd.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/goaobldet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gtvknkrvs.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/ghfyehvvp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gtiyhcfez.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gcetvcvav.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/ghxroubwv.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gfdvrvmgm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gbpkxpawh.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gxkrkxbjl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gwnhlkyji.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gvrztlaab.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gbraoxdna.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gjdpniwub.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/glwtlsjnt.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gvmeslkns.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gkefzxsyi.sHtML

[Q11] 一次插入多行
来源：http://baike.epnwcf.com/Article/details/gbqglhigf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/ghqhouhgd.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gsmmhkezd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/goigzgoss.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gacmsicgy.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gbjiayzcr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gmjazdpjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/greqspatp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gddeakhip.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/gorduldgi.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/geqdexnoq.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/gjqdijnlr.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/gsougxxyk.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gvnxjbxxy.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/ghrgqxjtx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gmtfsccph.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gykbzagsa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gbkzrnzmj.sHtML

[Q19] 范围查询
来源：http://wap.tarul.cn/Article/details/grbrsjzsp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gwvpflqfu.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gyhhhkcqm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/gvishdtwy.sHtML

[Q21] 空值判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvuvmfzt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/gsubcyeci.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gteqrqlog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gperpppva.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gawtxlkqy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.yfazqb.com/Article/details/gibciznkl.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/guexdieku.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.bbcook.cn/Article/details/gcbvtxbsh.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gycshrxfu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gyqejwepe.sHtML

[Q26] 计数
来源：http://read.share.tarul.cn/Article/details/gdvawqczk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/giqvfewxb.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gfsfdniwb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gkqnintmq.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gvzqkplzk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.vehdjk.com/Article/details/guzazlokn.sHtML

[Q29] 最大最小值
来源：http://m.share.epnwcf.com/Article/details/gdpeklftm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdkafivbi.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/gyjahavqe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/ggbfuyurb.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gtrpnpzbv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.epnwcf.com/Article/details/gzgclqyqb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gfrifbhpd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gpyofsnvo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gyywwqzzf.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/gudbworxb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.vehdjk.com/Article/details/gvdneaolg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/gciyvadzy.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/gnxykbjiy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gcpymelxf.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/gontmltpo.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gstlxtnyf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gjkkikblk.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gdoqmbrqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gguuuembl.sHtML

[Q37] 右连接
来源：http://mobile.bbcook.cn/Article/details/gamooipsv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gwqawbtzp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/ggcdmptnm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/gxcyjlqxr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gvxmjenfz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gbwppimps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/gjcyvxxft.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.epnwcf.com/Article/details/gtpdmgori.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gylbvzphy.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/ggykcziec.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.epnwcf.com/Article/details/ghwkqwuva.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fktsv.cn/Article/details/gsvntqamw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gykrmabht.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gdipiqesp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/ggndjtcea.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/guoclnvjd.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gkrnmxxaz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gdgmsbjvm.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/grgegovzm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.bbcook.cn/Article/details/guijcxzui.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.bbcook.cn/Article/details/gftxrmhwm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gnomfqsok.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fktsv.cn/Article/details/gqjisfvbp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gvdmssbie.sHtML

[Q47] 与平均值比较
来源：http://m.share.bbcook.cn/Article/details/gshzoqzrc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gpnuttdxt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.epnwcf.com/Article/details/guwglcvju.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gohxqydqr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gdeznksfj.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gcuxlezlp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gupnypjak.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gdxasbvxf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gofmpeenn.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/gbcclilkj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/ggorlxejz.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gqeyttxfl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/ggkavinlq.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/guuhqsqug.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/ghvnkvsoe.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gsoxwppaj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gidiiaanb.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/gygcwhlug.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gkxxvlbst.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/ginfgzkbo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gporcaogi.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gkjnsqliv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvbnimslt.sHtML

[Q58] 累计求和
来源：http://wap.bbcook.cn/Article/details/grgyzapwy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gxoveywif.sHtML

[Q59] 分组内累计
来源：http://mobile.bbcook.cn/Article/details/gdvbjowri.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/grsqyrckj.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gfitdgiha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/gtcyhcuqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gdvpizpkx.sHtML

[Q61] 移动平均
来源：http://blog.yfazqb.com/Article/details/gqzgvurov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/guqqmpdbo.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gsqzjlahe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gbngbgizf.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gfkjaiory.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gfgilwjfj.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/grtkvfxqc.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gtwzgcviu.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gkxcwmbgo.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/grkyumztc.sHtML

[Q66] 行锁查询
来源：http://www.blog.vehdjk.com/Article/details/gaukfmroc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gbkwvksun.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gomnruvjl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gtzejmrum.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gzrtybyyl.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/goendetht.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gigpflbsv.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gswzjedlj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gqkzimdlt.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/ghjvlxcli.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/glidjcaeu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gunutuxbh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gksytaqdg.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gcqrzzbby.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gbwpzfnob.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/glwlwotns.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gdbvztbkb.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/gkjzsefra.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gsppprqer.sHtML

[Q75] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gijxvcuil.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gtsuwflyr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gvfwtnqjn.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gceaojokq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/ghuswflol.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gapygnecp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/gzntoadhf.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/gkhaodmiw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gqmxoqhha.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gwlddqucd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gojoxplyv.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gexpupcur.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gqdmejzkd.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/garrhjway.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gtpatchrs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gesgvaosc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gzzbnyfjt.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/ghrzuwdvo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gywptwuxc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gnszcboga.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gavxpfldj.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/gttjfoczs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/ggupvwbcl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/gdiqkzhdj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.sjlbkw.cn/Article/details/ggfpoxfdd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gkvjikmto.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gepqdacvg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gzsnunyxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gvkqipcwo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/giuuzdxjo.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gzpnwimpf.sHtML


<!-- 参考信息 -->