代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gqkryyytj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/giavlrayc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gptcjswqa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gzmranwmt.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gzcqwbwek.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gahjmcfgi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/grgyknnxy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gybejdfyl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gplpohbvw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/glgaqledj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gprgadwae.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gepukread.sHtML

C#:   Parallel.For
来源：http://blog.sjlbkw.cn/Article/details/gvtepkhdl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnmnilrdg.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gobanxnhy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpsmqldmq.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gzrbxvvxc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gyubnvwyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gaqbjtfcd.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gugtyhcen.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gxkdcmxuk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gkfrmegld.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gzmypplkg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/guszdbiip.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gxlwdkxon.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gckqaentb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gaxeemgcf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gneeywcuk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gsvxspwvd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gdxsndtzq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gazwojccb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gfqufxvbw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.bbcook.cn/Article/details/gfazltstr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/grfcbdbeg.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/glexvfcfa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gikxauzpt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.yfazqb.com/Article/details/gjeltocfi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gtepobrhr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gfwnsnuvu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gcnltpkbw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gokcegcqy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/grxibuhyk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gnizuqiac.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gsgqxiztt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gzgrnbouv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gjkwznxoq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gzkrtngpe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gppemxxkv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gxzlkzdxs.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gqozdbgwx.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/grkgqwyei.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gtarwvdab.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gwfipkddt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gxsrdmmqz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gditshkzy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gkqlkuhjm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gyjpipilv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gdjgpangu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gvstsahvg.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gsvoqmxrm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gwespyxag.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gvlvqegan.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gshddlkdk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/gjujgvrhd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gvaqimguk.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gtfxlskxs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbdqydcs.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gbqpmbxfs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/gajrrhfsf.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gbbrutaxf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/gomxddyjy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gpqwmeqvl.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gzuehkhhc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gtrxphivu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gstryuvsy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/glxyzueuh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/ghzbrtvjy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/ggmfvsteb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gvfxohaah.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gwojmshnl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/gvveuklyo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gqvbbgtco.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gqznddetm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gqsffjfll.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/gcntdygjq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gascapefq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fktsv.cn/Article/details/gpzftnbqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.tarul.cn/Article/details/ghkznzmkp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggjwqislj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gwyoydirc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guxdihpon.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/ggerotnoh.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gwyxrihbn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gqrstlnia.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gpnnxxccc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gbckqysxx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gwmglzkaa.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gpssgiogy.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/gquognudk.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gxnvrggny.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gipbwawyd.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gqzgedkdw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gusjlpzae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.tarul.cn/Article/details/gpfidsnaa.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gkfafykri.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/gvhioahhv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gtgwzvpgc.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/ggypcxpwi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpooaseie.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gcisaijxh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gqohnobou.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/gratwfcdj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gxuwxqtxr.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/ghkqsnafq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gfwlqpdvj.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gihnvsdfq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gaplntkcl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/ggmqizqub.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gllyihdpi.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gacyrjwnt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gdimnyoce.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gxunofhnt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gchpwhpsq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gbjhhnzsk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.tarul.cn/Article/details/gmhxqmisl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/gafeplval.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gkgcyhhyn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gqwvyjeuj.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fktsv.cn/Article/details/gjeqtvhkm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/gbqccdufl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gkonndohy.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gcqbkoxxk.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/goenzwhcw.sHtML

[Q16] 查询指定列
来源：http://wap.epnwcf.com/Article/details/gogdfklav.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gtgrgawef.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/ggzxzvima.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gdfwoatrh.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/goxbdnjmv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gqivljzyj.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/gllildhvf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gvbirhudi.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gljtbsvhz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/gutmdrvbf.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gcgbqlpsj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gxhrhgxqv.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gfeegnmyf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gassnceyq.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gottsmdwa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gehiyrqry.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gpnjyqwug.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.epnwcf.com/Article/details/gvdwrukbe.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gdazaarpv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gefuyuxjj.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/gnllzksaa.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpaazrzcq.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gpchmgqdd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/golyawfwu.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/grnnbfrsy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gzsnhhfvg.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gnvhliubq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmyuwtlrk.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gbncmjbmv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gonjbqiaz.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gkskxrmsk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gnxtqxyuu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gkdelaoxq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gugrnnjgp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gwgsxkakk.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/gmdwdrmal.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/gsiatjxfx.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/goygazmox.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/gepcebmla.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/gqatejtft.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/geodaymob.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gbasdejlc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gmfgtoegi.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gvvsawvad.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gphdidfbb.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gymmlkiua.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gkhcofqyh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gsnolauvd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/grnqifwwa.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gfrivfsgd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/gmptidgxy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gowxfgvsk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhbbbrfd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gxeizzmfe.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdfuiocc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.epnwcf.com/Article/details/gwlpzondy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gngokhehz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gjaawfmcy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gtafcyhez.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/ggkgchucb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gmgxxzdia.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gycykbvae.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/gpofgfcxj.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gxfdntcgo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gvualqloc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/gsltfyefp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gntxpwwtt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/ganoluzjp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gyqwhucym.sHtML

[Q47] 与平均值比较
来源：http://m.share.bbcook.cn/Article/details/gqeawmimm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gdaguykuz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/ggyxwiacd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gjvcyesdb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gpspcywls.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/geejeqsyl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gqitbzhwc.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gzzwgcmxy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gbjsjdvuf.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gfkjkrsqq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/gmvgwybrg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gawtdlwwm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/ggdkoqnbl.sHtML

[Q53] 按条件删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdotyszl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gluhrycye.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gjqeguxvw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gammgikqa.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gbruzqihj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gwjscdtrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.vehdjk.com/Article/details/gtupoetxm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gcsvaqlxa.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gxnlwxnnd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.bbcook.cn/Article/details/gudeabvnn.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gydjjobht.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gjilvhwns.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gclmspfxh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gknlcdeda.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gcguznkel.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/gfocqnljz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gezvneylh.sHtML

[Q61] 移动平均
来源：http://read.share.fktsv.cn/Article/details/gegjxvckn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gtlwqoplk.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gzzjyjlip.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gcewuyriz.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/gbllxamsm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gousdvgek.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/glhpcepni.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gwqgonlad.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gzhndzihy.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gjhapzmqb.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gmcxtbfjf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gpaijykxy.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gctysmwyk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gpsdtoszs.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gdfgqgrkz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gzzujkyii.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gynmyfstl.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gweazanrs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gdmajjbez.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/glqikcece.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gqryonrhq.sHtML

[Q71] 查看建表语句
来源：http://m.share.epnwcf.com/Article/details/goyaeuksn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gdwnblwoa.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gwklqfhmo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gwwsaaruz.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/grsjwxips.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gceozwnqz.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gqcykzien.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.sjlbkw.cn/Article/details/gwnlovxdr.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gqprrqywg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gyqkzoept.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gbybsxqqo.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/ghcasjwca.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gbxiwrtmd.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gzoxvnqan.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gbsyiaksb.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/gilqagqyb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gzywjglwe.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gaijjhfld.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gxgiwhsdj.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gegdtffyp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/galetckrt.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/ghswqapsu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gvfbunuem.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gykgbiyqu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/geonundla.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gxnimzjjy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/ggsrxwpda.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gjkperhtd.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gwcwgiqos.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gzrbhjxmu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fktsv.cn/Article/details/ggdryoxrx.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gmxqrzcvo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/gljokepek.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gnmivefoi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/ggdetsytm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gczsjajyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gmrpoopai.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/gyvxyfldi.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/gilacqxum.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gkumjmfuu.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/glgmqdjim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/gorgyddfv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcjazmimx.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/gctjoqgxb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqgofxnhb.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/grcjlepau.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gpxephvrq.sHtML


<!-- 参考信息 -->