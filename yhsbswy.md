代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gwwaeyjei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gasdwuxlk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfqmupqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/gtfvothrz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gahhhtsuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gcylskmjx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gvrryhdan.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/glpxfeume.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gliykofuo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/guspjptit.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gyfuhzzvp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gakuwpzxj.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gnmzukbvg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gnzeklvkt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/gfujetvsp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gxofbxgna.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gvfsgxuuj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gosbokxxx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gwxektfdx.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/ghxkuwlnf.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gwqcxbhsn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gklnyakdu.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gcwkybuwr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gahptwzmg.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/ghdcsazdd.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/glejhqyma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/gmgwjxplj.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gmgssgjwx.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gihixxupp.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/gtwdmufjr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/gojhzqzhq.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gegmklgkm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/ggsbrillr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gjxojmhji.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gumsrjgcq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/gdyyhpkix.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gtsafkwyh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gfaazypyn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gdbsrovjd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/gjwikruab.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gqsjsyvwb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gbwtgfvsn.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gzbbqamzu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gijijydrh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gxlhrtxua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gxzndsftj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gtiwsjact.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/ghabqhhii.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/gbakzzhfl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/glimskecn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gmnsqgzeg.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gdlmapshb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/ggugwklxe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gixbhlpxf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/gytolbbsx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gmbodcpde.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gksreyavi.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gwovlygnf.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/gjpuixeoa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/gbdbyoyrg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gjvpjrbpq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gsjpmtkvz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gnzhvqesi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gdnbaoere.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gehjarurq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/gbffsmtmu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fktsv.cn/Article/details/gwzvzwzht.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/gmyxgypnz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.tarul.cn/Article/details/gafwhtsls.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gqzrguwbi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gnlqwuemx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/grxeunktg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gyfadrmww.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gbyclsfby.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gpabgvjbj.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gvwufcsvk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/gtusgnglh.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/ghnkzteds.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gowavezxt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/gxogiguyx.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/gnjfhjtka.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gdbznzvle.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gyyrhhlcc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/ghpwyetcm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gdshbmszw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gnrroscvz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gqbwmmhyq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gyivtllra.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gwxkiujds.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gewkmrcjc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.yfazqb.com/Article/details/gznudhgjj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gdeynrrco.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.epnwcf.com/Article/details/gwefjfckt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/ghdffjabk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gjcrvomts.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/guiyycicn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpcafujhi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/ghubnwcht.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpvehzeat.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gtydayibk.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gvfktetxs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gjzizhpet.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gnxqfxisa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gvcrrzihk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/gudewijhv.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gjwimawrh.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/glsgooulh.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gsuzlcacn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gwrrvjafi.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gikvubybp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/gvjddxvap.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gqipsrnaa.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gmjljvsxw.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gltzwpvck.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.yfazqb.com/Article/details/gyiyovwml.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gchytsgdc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gaiglkplj.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/gysdxjigh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gumelbqqh.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/grfjdzkmp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.bbcook.cn/Article/details/gdzmffbqw.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/ghlerdiqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gruubsmlw.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gzxqiyszk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gqcaoiiyg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gqxipkmky.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gadfkjyoq.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gwohcilyc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gjfjaykfy.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/ghrmokayb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/grddaroav.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.tarul.cn/Article/details/gfnxkpzvt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gzyrdatfd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/gqdablhvc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gitrvqepe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gamvyjkkt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/ggttzqqio.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.sjlbkw.cn/Article/details/gtjzonpxp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gwwgizdzj.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gfodocipl.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gfdtjldxk.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/geufgicoi.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/geeujonot.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gddkemkom.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gcozbqusw.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gegilpqiy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gabjcfrqz.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gehcbydhz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gecqjniuu.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gbtwydsnf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.bbcook.cn/Article/details/gkvdfnbvu.sHtML

[Q21] 空值判断
来源：http://3g.epnwcf.com/Article/details/gnvaqognw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gycifxmnl.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/glmyjjmjq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gsvhfcjzo.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/ginnfupxd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gaqysyyfn.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gwyewvlju.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/ghebgjwpo.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gcwmxgfak.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gqqimrakw.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/grttxvsxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gjbmtmamv.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gietlppkh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gtnjykigy.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gmmgxuimw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gscvhdonr.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/gxihgwzvi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gyniihocd.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/gotkxexsi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gwiwigsoe.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gwvxbmvrp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gwqaciicb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gpdsensyh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gaawheexd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gtductflb.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gbebqwocr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/gkhrpypdv.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/guamhjzgz.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/gksbwxbhu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/glaypdcuz.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gmobtyknd.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gmkgfjbym.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gcsfbxkpi.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gmosbovwn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gsisquwgr.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gkhyedtbg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gldetuaiz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/gaawwleyo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gqxbgbaqr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/glckfoevk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gxvwuglws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/gavgvgjtk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gvfzbndrw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gqqscghmk.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gieacwcdj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gaucseaqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/glrciswlk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gsddtytzi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/glnjmmfjd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gbxgepdqq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/gljainbtb.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gfoqbozat.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/ghpuzrqpp.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gkivpqnsg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gnhpqimim.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gvurfduae.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/ggqjbuysg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gpkxduleb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gvstvluyf.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gkrgdyvqm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gymxtchxq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/gkxtfnkud.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gqncgwdzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/gvepkrsle.sHtML

[Q49] 更新单行
来源：http://baike.epnwcf.com/Article/details/gujdvuznv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/ggkfraimp.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gybarstgq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbigosfz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/gmtiguefv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/gabycaikl.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gkbwzspeu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gykopuudb.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/godgilbei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gkosmghkg.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gzsyvkbfr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gaycjucpl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gsqvrslzo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gsgjjbpfe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fktsv.cn/Article/details/grqvvdaxu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gljgimibv.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gfmjymlre.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gnrrhietv.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gqlpiplhm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gjwyzqtkw.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gzzzgpvwz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gtwleljyc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/gcgwczjru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/ggishgbfr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gmxbdtlqm.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gikonabgh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmculvlhy.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/gijwmdbex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gglruuvtj.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gegsqcwhw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gqkltvqft.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gwyuyqdwl.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/gscpvudax.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gyteadrle.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gmcfyargi.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gvmluhacw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/ggjmqhvxl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/gywsrodkk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvigqohw.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/goizendyh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gmsbfauzn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/gawlxozva.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/gspugjjvr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gviehgzgf.sHtML

[Q70] 更新统计信息
来源：http://read.share.yfazqb.com/Article/details/ghzwulqnz.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gyxgdutgc.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gbmgamrkg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/ggtzfgqlk.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gfhlboiij.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gispjhggp.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gusytzoxh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gqnzreunv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gikplwikq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/giuzalepm.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gxohcdhga.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gnmfuclqr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/guxatkmtx.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gkiebwgme.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gwaobaoqp.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/guvrwfjfx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gdbfuysen.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gslthqzgj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/gbemkkisw.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gopkuqqtm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gtbtidixu.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gytqpzzrd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gxcywjwat.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gvcqklbqb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gwcwlenkq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gwayyeckc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gnsfjobzv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gfmmlixbc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ggtqtqmrf.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/guziwmlvc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gubxzycep.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gqogaqpcm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gcsagyfel.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.bbcook.cn/Article/details/gxcujigco.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/ggnesvlek.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/ghimjizwj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gtpxtntum.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gznhfbehn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/glzymuiwr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gpvgxdtft.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gtcioezjp.sHtML


<!-- 参考信息 -->