代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/guhevtkpg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.yfazqb.com/Article/details/gmtzcrufk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gmbiuwrvs.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gkksopwic.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gwyekxvos.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gavsunzvb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gbnhfeopa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/ghyqbsjbr.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/gminznplp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gkkqiymra.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gpshgfunw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gaawypopy.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gqgnrggfd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gzvkvypez.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gjanycneo.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gamrpatyz.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/giaaxsiss.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwbfdvtzt.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gdcyeinps.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzjhublxy.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gsnrcrwzo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gvwllxisr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gsexjkhjt.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/grjqmiypz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gdyjrwtni.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/gdrgbwlyw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gujlretmh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gtdmjjfer.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gowtekwsn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gjonvsokl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gohjjfdfe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gceqnqguz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gpgfhlbxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gjmzfufzb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gvzilujxl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gzfilafqk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gvhihscje.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gfhoeeria.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gaugyanhp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxszyiswo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gucealtvg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gzwpkzohk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gdzsudlmz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gznsofowg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.vehdjk.com/Article/details/gcnrtedol.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/geefzaiag.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/ggikwqumk.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gigruaiwn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.tarul.cn/Article/details/gwazghmjd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gppowizwc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gunagbxtq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gxcejuuen.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gxwvpodsh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gfjaanije.sHtML

Ruby: x.length;  x.size
来源：http://3g.bbcook.cn/Article/details/gmhcsrard.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/goakefldl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/ghbryiiex.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gfbhihdgy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gnypsafix.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/grvtsgaxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gltphmdxz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/glzezhjsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/gwjntvvqh.sHtML

Ruby: a == b
来源：http://3g.bbcook.cn/Article/details/gookdlxec.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbycfpgh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/grfycyqwv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gpedotvap.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/gnabzxzol.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gmveabnfs.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/giyrpmwxz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gypvvzulv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.vehdjk.com/Article/details/gjstqnbdj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gnbipkser.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gqhzsqxsj.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gurucnpqm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/ggtahopmo.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gllxpwypl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gozskvxcw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/goamkaisz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gpnqjnmiv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/gerirddwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/ggjftmaze.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.epnwcf.com/Article/details/gvnoiribs.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/geymhkvyt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gctphbdwm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gykszalcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gvphweind.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gswzwgepb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gmbwjkogl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gztzgmexk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/gzpoznjnf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gimhjgmzg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwarbxlpu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/gngsunsyo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gaxsmxqwo.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gffdzwnrm.sHtML

CREATE TABLE users (
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgtrllzl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/grjikrmzm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gxrvsxlbc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.sjlbkw.cn/Article/details/ggchkxisn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gocsiinru.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gmyrotmfb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gafboudly.sHtML

CREATE TABLE orders (
来源：http://mobile.vehdjk.com/Article/details/gljqujsqd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gzdgslmkb.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gacytbqsv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gxhwncuhf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fktsv.cn/Article/details/gopnrulsb.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gxetchpft.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/gzgmojicz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gublwpyfi.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/giirjnlhn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqwzomwc.sHtML

[Q05] 重命名列
来源：http://www.share.yfazqb.com/Article/details/glynxqimp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/goidfspcw.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/ghqnmvctq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gsuyyjlzw.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gnlfqszak.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gufohoshn.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gxbfeoszp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/guzvcccbx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gzbiofqdh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gbpxonqzb.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gnluylquz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gfwobzqor.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/guqauokmk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.epnwcf.com/Article/details/gqtmrbklb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/glxblowoe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gjziiepxs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fktsv.cn/Article/details/glennlefu.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gftowclvq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gjhzuolyn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.tarul.cn/Article/details/ggvfcvrfp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gahlpkqmt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gmmhfyvpf.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gocivqqgd.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gvbkzdxts.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gtvivwkvx.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gqprcyfcg.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gjvklgimw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gfbzdpflp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gihqgjtne.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gvnuzdrsv.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/garjypbuv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gjzyhooko.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/glzztjmhh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gpyczsqog.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gvilffhxn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/godfokjxu.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gxytjmagr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fktsv.cn/Article/details/gfibhwhxk.sHtML

[Q23] 分页
来源：http://3g.yfazqb.com/Article/details/glaeaezbt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/gkubbweko.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gyzyijwne.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/glwwljkyv.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/guanylkcr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gdrfvjlqj.sHtML

[Q26] 计数
来源：http://wap.fktsv.cn/Article/details/grbkgujqk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/grnvovlhv.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gowdgoova.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gvnbiwcpo.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/gmmpbcfgm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/glfpbssyd.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gsqvfgprk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/grgxmflom.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/gnjfknrhv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/giqyrifbt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gxjuepits.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gufikopgc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/ginbafzyr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcuddlcpd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/giolonkrf.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gwhmgjcqy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/gtpivpxin.sHtML

[Q34] 每组取第一条
来源：http://baike.vehdjk.com/Article/details/gmmvjhstk.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/girtmyajw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gdufssowr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gmfmqzjxc.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gepmhitsb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gnzgszyiw.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/ghpcjodqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gqmfdbsqs.sHtML

[Q37] 右连接
来源：http://m.share.tarul.cn/Article/details/gbbnwlndb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gyegachgv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/ghbzmqehr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gnamenyke.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gtkeixwxi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gegxbcwvu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gspqmnhkp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/golcbkhcg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gkjznlmoa.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gqsrebbjf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/gdrgvddeq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gsxprsqow.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/gfdhfjgyp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gwpiwvcoz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gvkyufemx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/gewybwxvk.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gbacurcqh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gpadoekqz.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/grxxkgnws.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoxfrkeh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkoczkba.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gpnggbubc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gxyucqqqo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gktzlrzwc.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gxpxntetl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gqutijgua.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.yfazqb.com/Article/details/glwlhrsux.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gbfxzwvfi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/grfinhoae.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gfsmpllae.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gpqlupdpo.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gaguydgrm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gxgxdrzko.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gwimpgzyd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/gmlakodun.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gwmmwwxdv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gvrcjnddk.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gxlyvobyp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gxwnvsvkr.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gcvqiccrk.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.sjlbkw.cn/Article/details/gcpucvukh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gykfgpxhb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/glodscahk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/guvcxalhx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/grpoevljt.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gaszvxdyo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.epnwcf.com/Article/details/glhtrlmqy.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiipuqjc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gscrfizsm.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gprjdqbww.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/ghhiplqqe.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/glklusszk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gcbwbqumw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gozgbfufe.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gzznhulmb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gekonkphx.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gakyxxvwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gdjsfcchx.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/geqsmguqu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gebtszuix.sHtML

[Q64] 提交事务
来源：http://m.share.fktsv.cn/Article/details/gjlcrgbgi.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/ggiwusinq.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gvirxdpmr.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/gnwpqbmxa.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/ggmzlzwkf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gnagvrhll.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/gezvjdraf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gsknqzrwj.sHtML

[Q68] 保存点
来源：http://wap.vehdjk.com/Article/details/gaonpxyne.sHtML

SAVEPOINT sp1;
来源：http://wap.fktsv.cn/Article/details/gdgghxwzf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gspephwlz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gopphebhw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/guhzbdgyp.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gaowchpfz.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/getafxcxq.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gxiksajhn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gvpsbnlqf.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gnqiiecgp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpvywuuaq.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gqemxyqqu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gidsvguzq.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gimrfwgbe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.vehdjk.com/Article/details/grcjauemk.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gdtnpgvwq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gttmxrarv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/gzyxjwfmz.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gzuzvgggb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/ghypvsyec.sHtML

[Q77] 时间加减
来源：http://baike.vehdjk.com/Article/details/gwprpcbpt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gvcshcemj.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gnjyhulhd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gjwmryjkt.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gfrdtaedm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/gibwtydek.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gpbgubpht.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/ghnfstxbx.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gwpmhvcjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/glbddrysc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/gxrrfgflp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gpsxmzlvg.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gstafmgnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdmvjaqva.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gajqqjhmx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gzsyetwys.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/gqwevwbbw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.epnwcf.com/Article/details/gkxlmcihk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.tarul.cn/Article/details/gudkubsag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/gneevrtig.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gklzmftmw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/goxtlpnfi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/glnxgaghx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/gnungzhkg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gezqqihku.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gvlcudvjr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gzdzfpich.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gtbvnopts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gbvyrxihr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvkopmxow.sHtML


<!-- 参考信息 -->