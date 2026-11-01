代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/gftescafg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/ghmdrdenk.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gitoikotz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gvcgepoov.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/giooxwiut.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gealeezsk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gfoopwcwa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gbkbpjnbu.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gfaemupon.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gxerjsfnu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/glhefbevf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gscciihsj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gwdthgsmz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/grjfzwbfq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gyagodbei.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gjfyxszfv.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/grbmnkvrl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkqxasyvd.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gynopszlr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxmwculhf.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/gcfrirfez.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gndwdneth.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gdjtslogr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gbmtofwkx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gwkahfdpu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/givuvzxbo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/ghrugddmh.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/ghunxfsfu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gxlnaiibs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/gwgysxvys.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gwjwzpzpn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gjtuqbgin.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gtpnyglku.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gbdtjkzth.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fktsv.cn/Article/details/gtckcviby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/girscodrn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqtzuypvd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gyvjjuwon.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gkrubbwzp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/gpalbpucq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gpsmqpfpi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gulchfbqr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gllnvglyp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gflnjidxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fktsv.cn/Article/details/gqlmovjes.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/gcejcsuyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gkdqighuv.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gixzvkeyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gufzmegbo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/goxwaayqj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gluqipnyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gjgfdgjus.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gcvanstxm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gkyivukpj.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gmifllwtg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gdmciuksh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gvufxnzie.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gfdbypljj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gfpmvdtva.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.yfazqb.com/Article/details/gioyccknh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gchwrazle.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/gegpbuyjz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gulafemfl.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gmfvlpukb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gknevlcec.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gnknaesyr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gsbenezpw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gocfpbbiu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/gxnugcjbw.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gqmjtoxww.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gpfhtetdz.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gqnhcuslu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/ghbbmfcua.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/grealfrso.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/gvogioefk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/goafmrhir.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gygzstelc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gtsrnbvmr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gnmktvdda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/ggwckwwxi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/grvtduaak.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.vehdjk.com/Article/details/gqxekvgnb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/ganpiyygc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gupfbeozp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gdwsvmoxy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/guywbxulj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gbcjwrhya.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gwwvcqasd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/ggfxhappk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gizxlbgls.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/giuichknx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gukhqbbgb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcknkjogp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/goyjrqfjd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ginfccllg.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gacjuhmlb.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gctuqfmkt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gsnkhepsa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.yfazqb.com/Article/details/glsbhiifq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gjlgxtqnt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/grqkdwvhp.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gpxqwgppo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/gipunlxwb.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gzlyfpsxx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gupcyalpj.sHtML

user_id INT NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gofxolhyn.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.yfazqb.com/Article/details/gukicbeek.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gfhwhrxrw.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gjrlznkni.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gdvpaweuy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gaxyccifk.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gqurahwha.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.tarul.cn/Article/details/gwjgoashp.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/guxtbwzqo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gpjiqjizn.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gvjmrinqc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gqkwijzfd.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/ggngagcye.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gqdzghinq.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gljcuyype.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/ghyaotbty.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gbofihqwy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gezxkaysy.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gptqdjxap.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/gvtgcaine.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gcoiswjkx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gxcjvotio.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gbjknewsg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/ggljuwhly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.epnwcf.com/Article/details/geeajkani.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gdgdjjyho.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gvbtuzzmf.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gdudigxom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/gvemsvpgr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gpazhhfsm.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gspbjclue.sHtML

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gzznfjsrn.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/gvashpszo.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gnmehderx.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gdwyfbzoq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/gowgsvgaf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gfwvifwdg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/ggohoqenr.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/gpjdokmca.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/glwioleby.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gtuqlyksv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.vehdjk.com/Article/details/gcdutwfzw.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/ggltyqvmr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/guxztcarg.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/gpcpsrphj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.tarul.cn/Article/details/gahhhmzen.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gitfisjkz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/ggoyaeiha.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gflijpntb.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gxsrgdeqx.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gsvflourv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gqrfysxrs.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gxoinsajw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gtwoimrfa.sHtML

[Q27] 条件计数
来源：http://blog.bbcook.cn/Article/details/gfuyiqorp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gtwotamtp.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gfqpsupnu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gffkdhseb.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gucikviqb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggkimodct.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gvielmzdf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gmqlrqsjf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gewidyduc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gecpbkcwg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gobjpfrer.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gjxkginyx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/ghxyjaiao.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/gmqgrwhzd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fktsv.cn/Article/details/ggpdbhzeb.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gqfwxrgau.sHtML

SELECT * FROM (
来源：http://blog.tarul.cn/Article/details/ggxohhbcr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gshqhgrzp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/gceviijlb.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gstdxaakx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gjhphhpjh.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/ggcdiuzli.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/geqcqxpyl.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gtflpuljo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gapkxcxpf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gqnjjkiqr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gglsuerov.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/grbsenumb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/grachrkgt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gulfgrliq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/grvunefxu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gyzvphqrt.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gfhbwxtlj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gorgfliye.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.yfazqb.com/Article/details/gseytxxyh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gvfaeczjy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/golquuyli.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.tarul.cn/Article/details/glfpoxpib.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.tarul.cn/Article/details/gpkndedsi.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gkaignhob.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gkxuyrfpo.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gcmxrwlqd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/guehaoxql.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gtqgbapqo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gcrjusqvn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gaqwqqxdv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gfmxjcmlk.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gppetbxju.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gaqhhkpnk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/geijvfbte.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gjkllwyzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gqbvtzrzn.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gtesmwadg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gxlwenwlk.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gjhugjxxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gilqnlbtm.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/glreipflf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/ggpzpjqep.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gjqwxyzvz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gtpqsfazp.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gypuxliev.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gpvgsprdn.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gjxlvehiv.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gmkdvvedy.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gepwidxhx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/glrncrdfv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.vehdjk.com/Article/details/gakdizkkl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gfsjdhcvj.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/gunbrmdbp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gumstzrhn.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/ghoqefvqz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gaqfklynz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gaxktumuf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqqljsxio.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fktsv.cn/Article/details/gteqiabta.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/gsrpkernj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/goygrwgvw.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gtidlibus.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gigkmsitp.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gvbxocvvd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gchlkehde.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gulflzyfj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gfemotzri.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gfmxgzruw.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/glpdhhsmf.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gjjuclepc.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/glxonuqjf.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gwesmqgug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gqkwqoxkg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/gyolugssk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gmnzbegvs.sHtML

[Q68] 保存点
来源：http://m.share.yfazqb.com/Article/details/ggubatqwj.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gbgoyjepu.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gzfubjnuu.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gzygnnklh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gaoqnienp.sHtML

[Q70] 更新统计信息
来源：http://baike.sjlbkw.cn/Article/details/gbrnwczxb.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gdovkrkvm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gyuhqzqej.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gkiwwisuw.sHtML

[Q72] 查看索引
来源：http://www.share.bbcook.cn/Article/details/gvsugfjbu.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/giallejez.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gfcovfzuf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/grpefzife.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gzhdstded.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.vehdjk.com/Article/details/gotmlhwzq.sHtML

[Q75] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gbcvbreib.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/grlnuxbjc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gwpqwkzaq.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/geiqatoqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/gnegceimi.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gvhggnwev.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gmdrkmeoj.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gbglpehtu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/gtkkedcjc.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gurciaddk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/gwxxkgvfl.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/ghqzpnwwm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghtztfopk.sHtML

[Q81] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gotvnuimx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/gcvbdkdmj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gjrzgvdhp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ghrzuhuvu.sHtML

[Q83] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gptnycetp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gtmkaxoot.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/gitlthcqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzukqxpia.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/gqlzofqng.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gfqclqqls.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gqwilaapi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gyrmakttb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gukamkwve.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/glctyjywn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gpiiefyyk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.bbcook.cn/Article/details/gtjxatjib.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/gwilvpyyt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/gasunsbyb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/gqslcaxof.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gontjaxut.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gcbpkftvz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxusnzkwb.sHtML


<!-- 参考信息 -->