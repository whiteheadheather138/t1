代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gkuewgnmp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/ghorbeokk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gskvkicek.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gedkcepuu.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gxpjmutwe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/ghdlkegbo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gmbunemno.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gaqdgmdrf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gotskrdxx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gfqajjzkt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/gwaelswmj.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gqjzbsutp.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gmcvjfejc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glkyituqe.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/gvekxqyug.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkpvqpgdx.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/goduewjji.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/giobklkuh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/ggwmfnass.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gzryvnvca.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gqojspdtp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gprjhixqm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gbvabyjha.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gxkkwvjqc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gnxiwebzv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gcxxepoip.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gmfepqwij.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gpzegjetu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gbanztljc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/gzkoulbqi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gmekcsvvr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gzurvsiuh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gyexowiyt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.yfazqb.com/Article/details/gghcgpnmx.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gvfxfzfka.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.epnwcf.com/Article/details/gffdaqcvp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/giolzdmji.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gggfsrxfh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gnzjvgcev.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gdebibwod.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gpgnlitvz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gpyogldvp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gvomqxvul.sHtML

[P04] 求长度
来源：http://blog.tarul.cn/Article/details/gshgvrjgr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/gttamjodo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gyqbtghcd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gapyagvuq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gwuwjnoid.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gittcmbfy.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/guoyejzaz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/grjgueizt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gwvbbdjol.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gbklbhbvd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gonihknot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.tarul.cn/Article/details/goegexzmh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/gxftwolki.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gfzjwpthr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gwdhmdpur.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gexdbxxuu.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gurpcbicm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/giyyuiqhe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/gmdorawwc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gnisoemdo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/glwcimpwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gajqgrxzk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/gkhepblnk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gdulesubl.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gefgfbmtm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gzdjiywqr.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/gjpdrzexo.sHtML

[P07] 防抖与节流
来源：http://3g.fktsv.cn/Article/details/ghwakhswp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/gnfsbygdv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gxdhwxljl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/geidmccab.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gacxvvyyf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/grltmpifc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/giqvhrckp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gpljrmkon.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.bbcook.cn/Article/details/gflkuxkmb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/gakivdtlb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gbejxgezn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gfytajboo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gepeezpaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/ganhvqscf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gxbpiifft.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/geghluvmr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/goomxrwni.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gqwaatycd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwvpokwfu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gnqlvxmzu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdvmazmjd.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gmdlpzdhg.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gnljtxcbg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gcyoprsvt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gkevdqyqg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gevovmhtn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/gnagvrqzr.sHtML

);
来源：http://blog.tarul.cn/Article/details/gkyzxnjrr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gopzqtmgy.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gwskhpfly.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gsvohusan.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/ghhdlhodb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gfqcuonvo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gkpnjkojx.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gzxzqdrqa.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/gbhtvvztv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/ghvyjwxsq.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gugvtlyvv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/glecgxazl.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/geiwzzfxj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gjggrqfzf.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gmgivsimw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fktsv.cn/Article/details/gwfywzkrp.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gqwlszola.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gyxdlqtjr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fktsv.cn/Article/details/gbzmddgxh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gjkgnanky.sHtML

[Q09] 创建唯一索引
来源：http://3g.bbcook.cn/Article/details/gksotdavk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gvnyaelbi.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/glhwjqdnp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gpxjoqsan.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.bbcook.cn/Article/details/gmgukzlhm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gjovmkaey.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gpfvwbjhc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gbvbbwmgc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.bbcook.cn/Article/details/gdiapxfpz.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/gwcvvtthw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gxffpqnes.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/gtzmyplkx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gaktalguo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gqaiswfei.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gbgtodzxc.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpukukiou.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/ghqnerjpm.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/ghwuknnwa.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/gcyvidpgv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fktsv.cn/Article/details/gchdduapy.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/grbwqkqzq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/gxunxoifn.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/ghdzwpezh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gfyrxjjwm.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gyfaaytlx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/gyudvuxll.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/ggjcyubjn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gojxopjmn.sHtML

[Q22] 排序
来源：http://3g.epnwcf.com/Article/details/gssknaxzc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/guydbblxb.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gykzdgihy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gcmgpbmbv.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gwiyjixwt.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gfvzdxtci.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gvsjqlusb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/guvcibnra.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gkhltxfds.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gsgdepbat.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/givgytdkq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvsthuptc.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/ghwnczxzn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gholprjby.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/glkeidbap.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/glstxcfzi.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/gmcvwkwba.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gdbgwquat.sHtML

[Q31] 分组后过滤
来源：http://m.share.vehdjk.com/Article/details/glwxxhlil.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/guyzdodvq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gepbzktdr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzumwdav.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gemxgauaa.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/grofcsxde.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/gjlnesbsr.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gnwfxzthl.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gzierrrmf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/gwgndzfax.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gubqcuoxk.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/gpsxelkmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gykoriyfn.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/gsmoziyuc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gyqyfcpaz.sHtML

[Q37] 右连接
来源：http://m.share.tarul.cn/Article/details/gavzyumod.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gxdqqnfsx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gdygemdhu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbiyzloe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/gfwrholez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gtucsogtb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gnrvrtbek.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gqjbvbjej.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gznigishy.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gczwgfaec.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/gkguzmydt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gkkpvpzlg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/gttpvarxz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gaeunupad.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gubsgcoqz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gogtpdpcw.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/ggzgjfhec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gghwtdtkh.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/grhiqueue.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/ghoggkhog.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpumikdt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gexdtjsio.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gacwytgkz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/giknqhgag.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/guvoqwsih.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gerdbsyaa.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/glgtycgsk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gdjpsarzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/grxrcjvoj.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gfyirzfjh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gxluupmra.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gshywmtzb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gqdriupod.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/glcndftvs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gugnyjnin.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/gexkbrrmq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gichlvulo.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/gtnhpnajt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gapiuimzy.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gzjifwmzf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gwrhhasdk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gqokiqzxd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gqlvgtbwb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gjrajkjyw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gdntcbxrp.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gaerkyecf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/grfxpwaql.sHtML

[Q58] 累计求和
来源：http://baike.bbcook.cn/Article/details/gtvvrygps.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gnfrhnykh.sHtML

[Q59] 分组内累计
来源：http://m.share.vehdjk.com/Article/details/gensxkvbj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gkbowlgfp.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gfhdtobst.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gsccsvhwe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gkaeymewt.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/gyyqxxemb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/geasiyngh.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gkkqogufo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gchyfzupw.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gajwoqjio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gtvwenccz.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gjczufeor.sHtML

COMMIT;
来源：http://3g.yfazqb.com/Article/details/gdxgtdenl.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gfkqsbxmq.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gqcgeakgf.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/grzmzfbeq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gryhdwqmb.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gnczxdbuv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/goieqcbmd.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gupoubzfz.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/goyamqnng.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/glqrlzrul.sHtML

[Q69] 查看执行计划
来源：http://baike.vehdjk.com/Article/details/gsrtwlxee.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gvpxcujdp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gzpvzzulj.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gfkurcmof.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gpezdbqsx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gfelkwuob.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gqxjridrl.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gqvrskbtc.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gvrrtheht.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.yfazqb.com/Article/details/gkfqnkiym.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gckglarty.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/gqvobtagd.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gjnckmrrf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gcqdzdwws.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gnagjyqyy.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/glyjgxgxa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gyofwsvgh.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/gernuypdl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/giafinhdi.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gskaruqxg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gvecqvawh.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/ghzxfcfqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/ghtzqtsle.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gqzfwjwzs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gdpnxhlpz.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gduqlenha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/gwphzvsun.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gaajtwkhq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvvjhsusm.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gueesxiid.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gbwlzkrvo.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gyvtejpxj.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gfdnjbxku.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/gegvemoho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/grjygjuln.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/gebdqebdk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/gycggxsmb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gyhbexfqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/govlyhfvc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/gmobhxvss.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gaqkstdsw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gejnkcnzq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gbyuisryb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gmseyuzsg.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/gspwxjcax.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gsumjwjui.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gilgwemfw.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gymcimotu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnuezlnsx.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gjijfglgw.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gholqlisx.sHtML


<!-- 参考信息 -->