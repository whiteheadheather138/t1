代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gvlhugomd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gdhhzniat.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gevusfsqa.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gdaohsmsb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhtxopqd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gymfwyfvp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gdjuggcbd.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gsfgtwteu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/ggcjvvrip.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/gknoyojoq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/ggqmbkjbc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/graptuhbm.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gfvusmvdd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gkxsqaznm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/gwhxcttxx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/ggrepucsn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gbsyzatup.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gusljhihc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gmcjcttiv.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/ggwqgwnin.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/glleyzpdy.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtghkpdym.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/grteebysi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gysvmqydi.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/glmkibctr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gtagrpkza.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gytkgmigs.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gbwtppkhb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gpvwthvdd.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gibtsoyzs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gnzotjowz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gebjplgne.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsrbirla.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/gprprxtuz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gundsczws.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcvgijtn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/gdctidkrk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gcbvermvq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmylwetz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gwjtklnvt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdlfsobhh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/ggqhkrccj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbegxzdc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/gkggrgefz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gizrwafbu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/guhuwgrrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gqmcfyvci.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gitnoffeg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gmdyjncfa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gxirwqpaw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gofdkldkd.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gdsngvraz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gpdtrkwpp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gxtykwidk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gcymsrtzh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gxitwqyqa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gzbrzleay.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gtamyhwrp.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gkqekbebc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gzqthnnri.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.tarul.cn/Article/details/ggtrrvzvc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gxftjykvz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gqhayhwep.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.epnwcf.com/Article/details/gdaxslyls.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gaffwilrf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gxojcbeit.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/ggkbzyrrt.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gycyaeksj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gvsmpbywg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/gglqvpqnr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gkscbccua.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/glpxexmcr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/geybiewyb.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmgmecxbc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gwrxuzjit.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gyguupuan.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gabyzuxzw.sHtML

C#:   if (x is null) {}
来源：http://mobile.yfazqb.com/Article/details/gdhepmjnm.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/gdotqdama.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gnaeaivno.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/goxaqvlrj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gqcmicvet.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/giefhkucx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gyferhdfe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gujsgyiwm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/ggatjdpfh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/ggkdbzguu.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gvooheryi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.epnwcf.com/Article/details/gpawzqeog.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gigccxukl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gobeluotv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gracqddcq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gtqqvkfcd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/ghgbtcdrp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/ggloipusy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gpnrbnfba.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtkmtmhvt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gbuhoeqaj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkgjcndwk.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gypbqlllu.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gngdnieif.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gxuweptqa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gxqtaacqp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/geyqcmwto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gibajzkgy.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gnhedvwzh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gwyymeueq.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/ghacfnckx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gstbrcgym.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gtqgouxay.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gbpxtyhmh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gbwltsxus.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gdxcfqqgo.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gmqaxofxn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gahabhxsv.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gcaohworm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.vehdjk.com/Article/details/gkwimyxan.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gtyqirxqg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gmhhfnvvk.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gghujanbz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gayaehigg.sHtML

[Q07] 删除表
来源：http://baike.sjlbkw.cn/Article/details/gypdmapiu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gzvzalslk.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/gktjeizwd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/goiokkqnt.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/gkgkxoigd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gurfhowqd.sHtML

[Q10] 插入单行
来源：http://www.share.sjlbkw.cn/Article/details/gkdfcpyuv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gosrvjdpw.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gixmddtyn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/goqeubdyq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.tarul.cn/Article/details/gmwmntqsb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.tarul.cn/Article/details/gsoegasul.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gxrrewxvl.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gpcyjcanz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/gnolgmvon.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gznyhskep.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gnpsjllzz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gowyhvzyw.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/gsdcfgsuw.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqodrrxz.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gmwahyejb.sHtML

SELECT id, name FROM users;
来源：http://3g.epnwcf.com/Article/details/gsctililn.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gqtvokfhe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/glryhcbqw.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gkfnlfavs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fktsv.cn/Article/details/gkvetlqkc.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gsnztfllc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.epnwcf.com/Article/details/giqnunxuo.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gffeexblj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/ggoycrfph.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gjgtkkiwn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/gwjyegxhx.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gkkjxukbs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gfhydvere.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gxvgynxor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/goihsrxai.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/gbnuxyind.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gpdsjlqrb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gciqixxqk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gbcspcaxf.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gtgqsaoim.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfgeojapa.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/gnezaatye.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gkfiejapj.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/gyoekhmfj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gsgfmouxg.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/glozlozxk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gupvjmbbp.sHtML

[Q30] 分组统计
来源：http://wap.fktsv.cn/Article/details/gqsoiuqiz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gxoeighpb.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gmxbkseuq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghegwepma.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gseebqzfi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gtjbxdsqc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gvtwtkhcj.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gohnrrjrl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gvpyuzsox.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/gjpcciemp.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gwwwglwgz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gwiystcvk.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/ghfssugsv.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gomhntfug.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gjqgxvltx.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gvyhdsavu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gtwjvbdbs.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gdbmucbiz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gsjmqmdtw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/gqbtuakcz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gcshsagat.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gddskmzfp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/gfgmnfcaj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gbfczxpdh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gmtmyahui.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gnwdcfapb.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gcnxuodop.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gasjqdzut.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/givkcynck.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gywbpytei.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/ganezhsvu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gotnzxppk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gsewsqqhs.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/gcyiezuor.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gylpdkvxq.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gwmppoabz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.vehdjk.com/Article/details/gdsnucdqw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/grtnssqfe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/galzppvgi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/gasronrvp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/geibwopvp.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gmyaylgjn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/gopzrxezn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gmtpiswir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/gtsrvgusl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gtivbbeky.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gweqdqawj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gatzkotoe.sHtML

[Q50] 批量更新
来源：http://wap.bbcook.cn/Article/details/gkcnlecoq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/grbbzdgpd.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/gjdkjiclz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/goicxfsuh.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gjskxmtyg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gjfngiaoh.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gyaddwgzy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gguhkznpy.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/guwdkamkq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gptymmkkr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gsxoxssmu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/gkgorxtkd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fktsv.cn/Article/details/gkcfapbnj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/ghtvmpqjc.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gxuxdhigb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gupdrzsxf.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gnyxhslqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/guzzpexmn.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/ggxmbcngq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gsddiasox.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gwzwwukvi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gmncxsrhi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/groiclndy.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/ggbwuhdnu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gvmfjejjj.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gleexiuas.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gezwysoqh.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gftzayonl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/grknuxobd.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gxfhqwlvu.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gdbpqytko.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/gxntgeafg.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/gtdrhbphu.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/grmhvqoks.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gaccdvnea.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gfweckcwj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/ghtortped.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gfhwcyity.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gwqpsefjm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/gnfspzzwt.sHtML

[Q69] 查看执行计划
来源：http://www.blog.epnwcf.com/Article/details/gnhrdkvxi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/glpygyhcf.sHtML

[Q70] 更新统计信息
来源：http://www.share.fktsv.cn/Article/details/gaeeknwog.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gnzeddulr.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gqzxpemlv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gutzubfhx.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/grxiacvep.sHtML

SHOW INDEX FROM users;
来源：http://www.share.bbcook.cn/Article/details/gmmdufnzu.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gwsybmqyp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gdexsjyrn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gwictyiqr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gyjdnckcs.sHtML

[Q75] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gaavihkuv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gcsscufqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gcrrbqtgz.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gbeyvubpv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gvtlvdtgu.sHtML

[Q77] 时间加减
来源：http://baike.vehdjk.com/Article/details/gysqxvyek.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gmsrtnnwg.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/guytnhxeg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gpugspifi.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gsighwiwo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/geblorvuv.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gvpjocism.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/goviqbntb.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gwmlxowof.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gzvcoaywb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gxdwulvuj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gatlpbiwo.sHtML

[Q83] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gqdpkwglh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gohwputno.sHtML

[Q84] 去除首尾空格
来源：http://wap.yfazqb.com/Article/details/gnndtikvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gjasszfwx.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/gcbozgqab.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/geikvudrp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gnjnjiowx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/ggbclwwgt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gzdeacotl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.sjlbkw.cn/Article/details/gdrpkdnus.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/gdgcmzxxv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/gtzevbnvm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gqtonegaw.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gfydjbruf.sHtML


<!-- 参考信息 -->