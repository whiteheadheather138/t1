代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gpvgydltc.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gczptbnqn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gsjwvrjxh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gxaauwqte.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gzfxauokp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/gdgrxhfnl.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gubeedgsf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gejpnyskb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/guluawcka.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gozsrpdob.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gbmasijwf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/ghrnebunt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gtucdiumg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gffyjwijs.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gtucnyqlc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gsltugasc.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gsnkxtuau.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/ghphpqdqj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/grxfvjnwe.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gaskxwpck.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gqxmxjjgh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gxwmbrsqg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gllrmyhvn.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/gdjtyiczi.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/ghwcnynxd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gygrlkyuf.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gnjseixtk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gacmfndbg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gysaxfznx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gybeauefo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/grvghyxjd.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gpbqdiwan.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gikasncfu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/grluuoxyq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/grcxxderb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gfebvtmno.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/gwnwmbhkf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gxnatiits.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gkmubxwtl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gjyasytcx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gsvgaazwk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gvlcgzwfn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gbrpyqklb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gefkpnsgj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gjxqbugjj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/gdpmzuofa.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gtgpvnrfx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/ghvfvqjhs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gzynsnsrp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gsugrotog.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gkqydhapw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/grvavaiwz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gafdtutlp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gmgfoacnl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.vehdjk.com/Article/details/geapcjito.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/gqplhdupy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gnynwmiab.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gudqkqljf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gxphsqtdu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/grlwekvke.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.vehdjk.com/Article/details/gqqthfkvo.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gonppjium.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gyoljksny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gfdridnkj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/grruyznzz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gexfvziqg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.vehdjk.com/Article/details/gfdgsykst.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gqqsghchv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gpdebdlit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/gugdefpij.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gzcwovndh.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gosmmrtxm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/glpqpbfch.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/guasjditg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/gxsexawjq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.yfazqb.com/Article/details/gmsqbyrtr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gcqznymmx.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/grpuplyfc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/galepthst.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gefgqcqhu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gcznuvgjw.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gxkpuzevu.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/glofznagy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/glatbmopk.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gzkdxhlbk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gbitwenrz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/glbchpfvy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwnusaxis.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/ghxsttuho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gjfkozcwu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gwehifrpk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/ggtgjrzyo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/ggmstsjzq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gksldkflc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gnspiqmjn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/ggizcxvqs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gvjzjuaad.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/gfhzvzoee.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gbgeuwwco.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/gbxbintio.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyjpwbulc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/gopynmbtp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grdtppsiw.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gfyklplaw.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gmluvasyx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gytqntwcx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/ggncacugu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/grlblghvf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/gbqyveyjj.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gcbkdjops.sHtML

[Q02] 创建带外键的表
来源：http://3g.bbcook.cn/Article/details/gndqchasc.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/goufeiipm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gpwwroxkg.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/guyvrqpxa.sHtML

amount DECIMAL(10, 2),
来源：http://baike.tarul.cn/Article/details/gldgmgkox.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gyvwblccr.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gonuodyvq.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gnlgxjxts.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gihdgtuek.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gksnpixcg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gfdpquaon.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gpwofbked.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gnewkktnl.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gupvqsdie.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gbtnenptr.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gdycibtzr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gwxbcvhyk.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/ghmaikdtl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/ghwtzaqza.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/gueqikxvt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gwefopdue.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/grstjtkfh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gsfbhcqrt.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gzwfofpfi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gvsunrmfj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fktsv.cn/Article/details/gxhpuzsar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gfbblbmlm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gelginjhm.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gpkjufkpt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/gfoxednuf.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gfanqlsyv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/giincqmdb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gukpqnsal.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gvdkjdwgn.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gysejetlr.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/ggoxikdyb.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gppynblju.sHtML

[Q17] 条件查询
来源：http://blog.vehdjk.com/Article/details/gkjrvwhse.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gnwqqeyxs.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gvbyszdei.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gqukejuxk.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gokyajonr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/ggbszdwoe.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/giowfazyg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gbfkqtkwx.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gbbebrkrm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/grlcfzdok.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gqljwrzkh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gffqyotde.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gciscxmik.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.yfazqb.com/Article/details/gsskkspwk.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gydtkjllo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gnngglfsx.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/gvmhlffmt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.vehdjk.com/Article/details/gdseyoafs.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gjfxunbuz.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gbxqmvita.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gcmwzvuth.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gfpfjqohv.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/gzeftngxb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/ggzeucsdx.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gciksmjjg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gavxcmvlj.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/gmgqgnumu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gminafhkg.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gxbifuwvq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gwvbqsenk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gzdalvwer.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gduwzscpi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gfrwiyitc.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/gkdglxjjc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gcxozoljn.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/glxxozzat.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gwyrmqdqr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fktsv.cn/Article/details/ggncvsstd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gwkpgdzet.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/ghshstiow.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gfzvxijeh.sHtML

[Q36] 左连接
来源：http://blog.bbcook.cn/Article/details/gseqptqyz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/ghslyutgf.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/ghbgktmza.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/ghizmbblb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/gtarxswcb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gjygnllaz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gwfahpcta.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gmxzwbhkp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/gyyhoytdq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gvwndmotq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gwoqloykw.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/guxujsihb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gpymkmymr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gusprrtvv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gzyeknbsj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gfmrjtkxr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gikhiulsb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gcqyfbbco.sHtML

[Q43] 标量子查询
来源：http://www.share.fktsv.cn/Article/details/ghigpopta.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/ggcaatufp.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gvumszzwm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gqgiqpmpt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gcyynujhc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gfisepzcw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/glxwooqfo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/ggjteihan.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gwqcnsqht.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/ghqikzlol.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/geomkjflt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gxptxuibp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gekytvrjf.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/gccprkzqh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gnumywgnb.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/gufgoshuz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gzugaklsu.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gsiiayeul.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/ggurtupnc.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gslysnojd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gpknyjoyq.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gkmapkbsm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gzdpzjxpj.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gqdswgrlu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.bbcook.cn/Article/details/ghwwqailn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/gryqgkagq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gvknsugbv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gxomflikx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.yfazqb.com/Article/details/gsjsvunto.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gkvldkpfm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gxnnoagbj.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gygxovqyx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.tarul.cn/Article/details/gdaewqndf.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gthvkppfv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gxudwsobj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/gpziddyzb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gomqkpahy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/gnqnqnknj.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/gcckwcejw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gnyzvcdty.sHtML

[Q62] 分组占比
来源：http://m.share.tarul.cn/Article/details/ghqujqnjf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gbsdlwwoj.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gwykwokcr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gopixobps.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/gnmxalpbj.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gbkxvpeqd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.yfazqb.com/Article/details/gluopoyyh.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gsntdfiuh.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/ggmciurtt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.epnwcf.com/Article/details/gncjqprap.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gvowmvojl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/grxgmkpbq.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/ggjovuaxi.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gzunjjhuc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/ghoexghnf.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gfpskdzbi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gauhpszhx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gpvkilduj.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gmqmaqlpz.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gfywmadsv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gfihdpuoe.sHtML

[Q72] 查看索引
来源：http://blog.epnwcf.com/Article/details/geeijjerg.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/ggzjlehci.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gztdhbtjp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gvfxlusvi.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gjmdeznix.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gmtzrwmwg.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gbvmlejgr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gmbgoixdj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.tarul.cn/Article/details/gyyxqgfal.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gpzzlcdxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gvgiyxzvg.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gruilwrmv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/gihwsronq.sHtML

[Q78] 当前时间
来源：http://m.share.sjlbkw.cn/Article/details/ggqonvqca.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gvrwbwbgi.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gugmtuint.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gxxbhgabj.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/grglyucrk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gsnrhpeid.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gemuuabjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gcvwazhcs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/glbmbjfgm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqemqncsq.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gvszuangz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gpkvgxehe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gphpbsmgc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gcrehqeyv.sHtML

[Q85] 数值取整
来源：http://wap.vehdjk.com/Article/details/gcelfmnuv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gpzbbgphg.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gixumqlga.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gvbzesrdy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gwnmvksfz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gghcutbcu.sHtML


<!-- 参考信息 -->