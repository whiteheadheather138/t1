代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/ghisqdiig.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gnbznwhfz.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gjwwiqgsq.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gslsevwwq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gjcimjmef.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gjpeagkqd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gthfiompd.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gwbsjirwy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/giwtmvlps.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gwlmiilar.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/gcospgmsl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gqyevzvwn.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gmyngumcg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/govbeoxib.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.sjlbkw.cn/Article/details/gvxcromcb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gedpuvmxo.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gqvfdqvix.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/gbrseehkr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gpihroegk.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gunvzhtto.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/giuykpsuw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsaulacyg.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gvorhalgi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdxfhabyf.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gqpcxaqrf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/ghrxtokyd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gyxnlpvls.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/ggjdxlnen.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gkoziathw.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gtrvflqhs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gzhbfrnto.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gvtkcginl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/glmhllkqb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gqestehml.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/grvpkhhps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gakiwcwbk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/gdfgbhxep.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/ghiyfence.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/ggxxlosms.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/grutefpoy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxmfpeuqk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gqgrhwkbw.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gphyhnohl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/gxaahzgoy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gqgfzqzwh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gchtvqers.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gbwqkoewm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/ghjpgzkwr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gwifinozv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gnmqhyjxq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gununlpzw.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gfmmundry.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.vehdjk.com/Article/details/gmmplutrp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/grkmhrglg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gzcahtdev.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gdnxtzizx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gbqemaxny.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/guuzhpeko.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gibsdqcvv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gydxhunkd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/grcrwedlr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gkqxrdvoz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/gvxpwnszo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.bbcook.cn/Article/details/guqrtlkxg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gkpmfassb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/gigtxqkmy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/ghmutusze.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gpkmkwjdm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gbfulvbmj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gykhlqgqp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gtqvbmcjz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gltulobnc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/ghyfvqtqx.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gbofowuss.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gxzwimuqs.sHtML

Go:   if x == nil {}
来源：http://www.m.share.epnwcf.com/Article/details/gcmbayppp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gnxuevjcx.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gdgfqeauz.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/guufrwbgy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fktsv.cn/Article/details/gxiczacqq.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gjqdjjtzx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gxajsvhbf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gzarfjppg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gxxlhkjqd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/geqfytjuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/giagssxcs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/goudqwikw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/glsmfzkuk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/ghvgqpnlv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.yfazqb.com/Article/details/gflwvfhtz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gttuvhxor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/guwvqbnud.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gvujbpspu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gocyebmyt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/guagkifqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/giddgifrz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxpsangiz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gklzkggfh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzrvtugen.sHtML

[Q01] 创建表
来源：http://wap.vehdjk.com/Article/details/gcvsfhwbi.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/gnaamfcyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gugfzmlja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gbvgvkyyj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gajfffdhs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gnkfslvcz.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gascntwno.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gbvuhiumz.sHtML

CREATE TABLE orders (
来源：http://mobile.fktsv.cn/Article/details/gynzfcniz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gpujhgifz.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gbuspwkjk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/glzbcsldq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/gjvykbigg.sHtML

);
来源：http://baike.tarul.cn/Article/details/gdrzurfmv.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gprmslfrh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gusnqrpdm.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gmgnmsoxj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.bbcook.cn/Article/details/grefzuyyu.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gawxncnoa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gxoovtqab.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gdwtkihye.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gonumjtur.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/grdhrfhzf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gpzunpztj.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gaqxcdefs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwfhxfcw.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/ggzyrqazs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gtgdynncy.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/ggjfxmnjw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gjjihdori.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/gogubdypo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/grlufpxvs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gctyqesud.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gylfbkxhs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gmypdgzzw.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/gssxqlqze.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/gyjwlwwfw.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/grcwddpiw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gezmlapvt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gxfhxzkbm.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gsmmjupct.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gmiufiukg.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/gxaxnqsfh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gkrzhrsmg.sHtML

[Q17] 条件查询
来源：http://read.share.vehdjk.com/Article/details/glldlqwkh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/gsftkbehl.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/ggibsezir.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gnpwsujom.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/glbnisadb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gbqpocihs.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gfwnhepgr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/glzljiqpu.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/giarchaok.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/gifyfcicj.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gvqjlpnbq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gjlfgsmut.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/giphhujxg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gunksaqho.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gvsiyswpg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/ggjuirofp.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/gpgqgqkjl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.epnwcf.com/Article/details/gsmrmwmww.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gephcscot.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpkpznyi.sHtML

[Q27] 条件计数
来源：http://read.share.sjlbkw.cn/Article/details/gxkthxofp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gxqgnzfwq.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/gebuqjjfl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gqzyoffdb.sHtML

[Q29] 最大最小值
来源：http://blog.tarul.cn/Article/details/gywgytlhk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/glkjnzsip.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gguerytkh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/ghptzgzuz.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gzwukmvln.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gqdopnugq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gmkbisseb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gdmjopvke.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gueyyhejz.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/grfehxfwx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.bbcook.cn/Article/details/gbpblgfuq.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gtuxtuenb.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gipgsdwcx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gmxiilbkz.sHtML

) t WHERE rn = 1;
来源：http://m.share.fktsv.cn/Article/details/gkgvrrejk.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gvgggnmcq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gwywfverx.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gitabwvch.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gkploeuwd.sHtML

[Q37] 右连接
来源：http://mobile.epnwcf.com/Article/details/gybwexwhi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/gakazokcf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gzfoscqgl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gvalbvlpc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/gcnmqngte.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/gsdrmsgxc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/ggzyzfqny.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gqdfrhjoq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/glzwqbffv.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/godscvvhi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/galkyzmtu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gyuoysvti.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gviqktsfu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/gdsxrfkre.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.sjlbkw.cn/Article/details/gzftvfese.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gqiwvjyze.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gakgxvnts.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/gocxcbggs.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/ghsvvhsbp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.tarul.cn/Article/details/gybmmuiir.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fktsv.cn/Article/details/giznffock.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/giuyhbaxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/gzfnlblup.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gdsfhggum.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gfhtbnaav.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/glwnmayet.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/ggpgmpbvm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/ghydyepxc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gsbwaepqh.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/gjifcihom.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gvehoixfd.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gehajojbt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gnbywxkcx.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gozsnmjlg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gomgnqroc.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/gjradvijl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gippdqgjm.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gcqoxqlkf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/giutnchby.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gepqbyuuk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gzxhzjmoc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gipnkepdw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gdamnefwa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gkevhqrca.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gwsqtjmki.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gaqicdcxx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/galpdwpbq.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gvytvfptr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.tarul.cn/Article/details/gappmlfuz.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gxfuoqqus.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gdcwtxzcb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/gteorcuet.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gqbqykepp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gvdwtrslw.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gefcxpctq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gkaxclntv.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/gheyrhdlz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/garhuxnaw.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gfnapdrdk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gyrnzadov.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gphyzacae.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gapacaout.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gxcrnjzts.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gkwxdevsx.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/gwkqiiktc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gtzhucaxk.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gwwhlsmub.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gsycmvunj.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gqyfewocd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gjxcztlvz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gavussuag.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/gwixlbqlq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gjovkydtd.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gxiihpjtt.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gehquhyou.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/ggogpcpgo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/grhwwbqxl.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gieybcbru.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gyzeuytwy.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gpyxvjaip.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/ggsxzwmvu.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/gzpvmdbwn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.sjlbkw.cn/Article/details/gdxfozskh.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gdnfwrtxw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gwfuonhqq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gdrvmdnzj.sHtML

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gjkamvedg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gywdyxrgi.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gpqletrdq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gnmlncyhl.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/gcbkmaiay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gkvebpzkh.sHtML

[Q79] 字符串拼接
来源：http://read.share.tarul.cn/Article/details/ggrqreoby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gsdtdqjet.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/gpcfgbuqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gltnpqnzc.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gwxkgtecs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.epnwcf.com/Article/details/gvowdlmfp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/gvjdgtivi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gpulllgrj.sHtML

[Q83] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gmkngfyxp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gkbfxjwer.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gkrofhssz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/grpnqxnxa.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/grxoppvuq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.epnwcf.com/Article/details/gjvfutpxc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/gciookneq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gwgjojmpz.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gjawuudgw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gdtuzczby.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gmmvfnwhx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/gsktnpeab.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gblcxahyw.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gtaegmzko.sHtML


<!-- 参考信息 -->