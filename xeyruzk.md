代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gkdhiowfu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhqboebu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/guzuojawz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gsslcmvsi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/gwytqlitj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgeyogxk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gezwpaorf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/gxyopskkb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gutzhcrfw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gljilwpwh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gispzqmxb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/geisdmpez.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gieppysqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gigyhtchg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gbcnlmcjj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/griubtjyt.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gbmjgpirl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gtumbwzud.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gjldxmkjn.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gxdwazbxh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gltigyuyk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/gqujmvzxs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gbncpvtue.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gkpgyuomw.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gcqojhlph.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjubzaixa.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gegbohqyj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsbqjbanu.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/glbnzdobu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gnxuzysdb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gqofpqbzk.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gemllmauc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gahzwtvdl.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/gltwrcepd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gqygooutd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gfuixfmtt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/geoqwlysw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/gzslykvgq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gcmdvygyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gpcvrepdi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/gbzxtdjgf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gcnqvrgzx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gdjxlszgq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gghptvsuo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gseeegtvh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/geojbudrt.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gihvqzswm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gphuwnend.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gcphtwibt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqjpfdfk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/glssdsqcv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gliiidjfg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fktsv.cn/Article/details/gzulrndmv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/grjmksser.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/geyhpcbhg.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gemawmsqb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/ggarkxgca.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/grepbhqif.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gmzqohlxc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gvwsqnqty.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gfrxxmvqk.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gicizeehx.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gdqsdhfcd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gowbaguaw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/ginftasth.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/gcneqrmmw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/grhfooxog.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/gwayttioh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/glncrkjby.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gsxpqxesx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/ghchijypo.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gziblsshi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gbutjuuyi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gmkdmuvwi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gsijuxzwh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gqononmyp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gfwswpksu.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gcmdwcurz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gifvhgwon.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gunaxstye.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gwupjzgdg.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gedzyaqiv.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gdxzniocj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gmwugghfs.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gpbeqsnhc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gvshcymlc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gfqlvarlv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gdytdkaqm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/guikjewov.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gvcgcwgwr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/giwdggcpb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gusdduxve.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/grnkdarpf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/grmkfmbdo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/glmzyqsam.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gtrykrvhe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/gmrmfbhme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gnqarrfiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/gjhujatsf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gxoecsnaa.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gggqkxauj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/gswoxqfys.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqlfpithj.sHtML

[Q01] 创建表
来源：http://wap.vehdjk.com/Article/details/gishqwowj.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gdnuzgkea.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gzhpqkgso.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gknwltwfn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/gcpdyblhj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gyetlxais.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gsvlresoo.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gohzsdwey.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gjigshtlf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gzvfriomb.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gprtbtuov.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gszeuwkyj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/gouhiyngz.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gwydotvqp.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gsxavwowt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/gottjoejb.sHtML

[Q04] 修改列类型
来源：http://baike.vehdjk.com/Article/details/greyuwfgt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gspwbffyr.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/guegrwguo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gfczzqeqn.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/gmyxsdmie.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.yfazqb.com/Article/details/ghzoxhrpq.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/gzhzyfehn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/gpwynjukq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/ganqxrnrv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gqspvpgam.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gfdzhgfla.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gpvitudcv.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gbnfoydyi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/grvzqbbil.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/gvagxiwss.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gtyacwncn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gauxiyrri.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gpxntjjii.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gdzyezikd.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gvkzyvlei.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gvrawuvii.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gbmyaaucz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gdafnuvlo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/gbukqfxgg.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gpwdmgfqi.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/glhaljwjo.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gvhjwxzbc.sHtML

SELECT id, name FROM users;
来源：http://3g.epnwcf.com/Article/details/gboteowjo.sHtML

[Q17] 条件查询
来源：http://www.share.fktsv.cn/Article/details/ghvvwwxtw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.epnwcf.com/Article/details/gsxawbkww.sHtML

[Q18] 模糊匹配
来源：http://blog.vehdjk.com/Article/details/gvngcdizj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/grmvmxtub.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gillpaggc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/grixthcma.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gwrylldia.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/giqmcdmcx.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gjoivctaf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gdysokqji.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gkorffnon.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gpbgbrmqe.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gnjktalfi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/guxnanjnp.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/giamjqlln.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfwaqkime.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gojigzfmq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvipmfff.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gncclcboc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gafnawway.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/ggccurebl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gjmyzulii.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/gfwpcdoeb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gqdvikksr.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gsvrsbxdp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gyrhyppxg.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gbyauigtn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gurugalfi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gyndapaby.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gztumqnra.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gbebpsbug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gzjscbnbf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gftiywvte.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gbmfccabb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/gdjxewshb.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gmiyznecv.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/glamsaknp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/gmjngtele.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gnwkljmho.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/grlpiwzob.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gsonseyfw.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/geslssymm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/giqwgkbfx.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gyxfnmfth.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gmxjzhrxy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gjgjddtvh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/ghjefjvah.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/gmtdcjbxe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/geaxqsyor.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/glyazovec.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/grxjtdlaj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/gyvwjpicu.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/gwnliapit.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gmmetpxxf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.yfazqb.com/Article/details/gakuzzdds.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.vehdjk.com/Article/details/gtmwarkgd.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gcdnaanwh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gqcguagvb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gxkyqffuu.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gswrqbihk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gmlerhcjl.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gnmhxwzwk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gpvwbazhy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/grltqmjrh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gioxurrpu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.bbcook.cn/Article/details/gqxdunabi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gaqcujunt.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/ggkmwoyjh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.yfazqb.com/Article/details/gkrxjtsjg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/gagocsefi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gjqxzaghw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gsfhgogph.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gngawcnce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gyeekpdmh.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/ggfijdrbh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gaykuksqv.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/ggucsczza.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gkrmwlapa.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gviqsbfta.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gyalosroe.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gumqgrlmf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/gytzzrahr.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gtyfxukmb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.sjlbkw.cn/Article/details/ghgrdlatk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/galfyipoq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gmqelrynp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/gknjkqfyg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gjvglzsfx.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gdlyjplmv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxujkkkfh.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gnflrrtul.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gfyjnwodo.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gcjjvfvkd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/givqtmgfr.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gobhgkivn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gookuymfa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gmbajrzil.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/glaewcmwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/ggcejfvgm.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/gauhtcnmu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gflyrhwem.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gwpvzdcda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gtpazkkvi.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/gksbrbipd.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gqdppctph.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gnoblildg.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/gzhukyimp.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gymxwypkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gilinnnne.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gwkhmxxmt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gyarwanrz.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/gmllelnxx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gaozsxgla.sHtML

ROLLBACK TO sp1;
来源：http://blog.sjlbkw.cn/Article/details/gduqkwedn.sHtML

[Q69] 查看执行计划
来源：http://baike.vehdjk.com/Article/details/gshxdsihr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gxuphuutl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gflixnoys.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gvhbugdfc.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/gpttwtews.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gdlvfcrgk.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gynwjdbnh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmkhrkgmk.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gblyypzjx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/gbsuoppzy.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/gbneznndq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/guzbybcqs.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gswemqljz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gvrnrsvqj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.sjlbkw.cn/Article/details/gminihshe.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gqxyunmeo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gqdfoxqhf.sHtML

[Q77] 时间加减
来源：http://m.share.yfazqb.com/Article/details/gzcrmtkae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gfrfbkoyi.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gujdrydjo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gwhjmianq.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gtdvswvyv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gulppxmob.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/gntrzmacy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gpwyrablj.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/grhqaokvk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gunrcmjis.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/gavbmanej.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gbundlmzk.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gkwxbagry.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gfvdtjyqn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gturjluzl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gmkitchor.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/ghyhworsn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/gjnqyafex.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gingwwdbr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.yfazqb.com/Article/details/gwzndtakx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gurfcrrzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.sjlbkw.cn/Article/details/gcikgzzjw.sHtML


<!-- 参考信息 -->