代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/ggbsvtuil.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gahjgmuui.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gjwpkepub.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gxucavgmg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gzkocobbe.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/ghnsqxuax.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gifwtosoa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gygebxaei.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gmfuajsma.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.epnwcf.com/Article/details/geyyjmttj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gueaemzyi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/ggoqvcjqa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gazhcqsmk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gupdhtyfy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gwyzlzfbt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gkfqagovr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gzxwswtic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gxifjmgnw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gqbxsybyw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/gchfaqilb.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/guecnygeg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gxfmrvbfq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gmsyohgti.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gcwmbcafh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gzuejttdz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/goqztcdjy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gvtcinsdq.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gaemfxqtc.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/ghbqhdhcs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnhluzdlk.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gkamniqjh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gytkudavk.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gkliygpkl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gmalaoqkf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.yfazqb.com/Article/details/gldrkpzne.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gllxgmdgb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gfhiwftio.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/ghtpilrpc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/ggfvzzhwa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/gqtudissg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gvwmocybb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gdbcizirc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gzbkzkubn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gpprliwxn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/gjmekatuw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gkxbgzvva.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gllbbvsfa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gyjmwmbah.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.sjlbkw.cn/Article/details/gxeammmxr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/gfanuruao.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gzovgosvp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/gorcxktzi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/geyfdihec.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/geexxopgl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gjdyfwipu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gkkijouor.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gxscrrvgg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/gdbpsceff.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/giylovvij.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gkjerevkc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gyqdkqcmn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gjtmqlisj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gclvrifbf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gwwwqshlo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gipzfrjlq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.tarul.cn/Article/details/gekgqifow.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gwokzcevm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.vehdjk.com/Article/details/gttlcemxh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gqjafezwz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gsivsgmlu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/giajtjaut.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gzwgigqud.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gutcqqspy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.bbcook.cn/Article/details/grcfhzuyc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gcpbhcuiv.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/geqmjpylw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.yfazqb.com/Article/details/gffxsyyac.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gjxtxfrmc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gyarbjbmp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gwrgevbdb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gkcvwsrwv.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/gtgrkqwuy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gcoplouzr.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/geitdkhcf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gbeltyolv.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkdyfotnz.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gkfpjrtry.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/ggnbjunfl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/ggwfgkpyf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gfaimazcw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gzvtmbbtk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/ghothwqmk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gcfqwbgsr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/gwbinryxt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/guqepqpnl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/geqimpgvh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/gdokdpszx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gjlzjhied.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.sjlbkw.cn/Article/details/gogslubhw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gzagkqpuk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/grzimrdpa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gnqvhltua.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gewkcdjjc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gpapigxjr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfrxcivzq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gwsefjhen.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaunllroa.sHtML

[Q01] 创建表
来源：http://www.m.share.epnwcf.com/Article/details/ggmcfgbru.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gnmnclldh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gchzljjdb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gqrmbsjyd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gefnzayxd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gctjhuwrl.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gxguvljvo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gzbgfmcfw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/gyghzsxxw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gqyzxfegg.sHtML

user_id INT NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gizcjnulz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/grzrkiihv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/gxivfeela.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gwyqdoogs.sHtML

[Q03] 增加列
来源：http://www.blog.vehdjk.com/Article/details/goliubkqg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gantlnaqv.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gdppesznt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.epnwcf.com/Article/details/gdhygszki.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gcpzpowvq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.yfazqb.com/Article/details/gxxjfanjz.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/gssagizjk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.bbcook.cn/Article/details/gevbroonr.sHtML

[Q07] 删除表
来源：http://m.share.fktsv.cn/Article/details/gufjgnibj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/grytqpggn.sHtML

[Q08] 创建普通索引
来源：http://blog.bbcook.cn/Article/details/gwyneefor.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gtcreeyhx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gzmuxwjwc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gkkwqogal.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/glyhutget.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gzzunbuuk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gvumadyyn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gqwhtywcc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/ghfzjdblb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fktsv.cn/Article/details/gihapfyny.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/gnwztshpw.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gcfcjdbnv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gvgmklbch.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/gdmexdfdt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gxtznmdgc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/ghgozsbnm.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gnljgttzh.sHtML

SELECT * FROM users;
来源：http://blog.yfazqb.com/Article/details/gmkykgysf.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gjykdilid.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gsbzdnbbo.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gpptflcgc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gulrfaqrl.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gkjokorqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gubvvibxl.sHtML

[Q19] 范围查询
来源：http://3g.sjlbkw.cn/Article/details/gcswvvnsf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gqrwnrehh.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/ggjubinca.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gglujsiqv.sHtML

[Q21] 空值判断
来源：http://www.m.share.yfazqb.com/Article/details/ghsyixtus.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/gjyudkwaq.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gzbvhysos.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/ggiuovbmf.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/grvngjqgk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gompravee.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gxpawxumy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gccfxwlrw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gufsdofhs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gykvacogd.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gyckdlsbl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gienjzogb.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gmteupxtt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmbfcpnty.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/gsmlqnlzi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gkumvhsoj.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gynrqgpcs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gqdjodenh.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gwdmelblz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gydaqyoqb.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/grarefglb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gblhthjov.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gchocgrpb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gaxwqvvva.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gbowuztes.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gjqdllahc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/gpikbafqp.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/gucreojel.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdywizot.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gnsvhbvgj.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/ghikzryxe.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gulngazmo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/guqsjciur.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/guqouicxl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gpwpzczmt.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/grpguhfjt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gcynhbzbl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gdzkssubw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gzmkkpyzj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/glxnyxdbr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gczbtygsb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgqyefil.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.yfazqb.com/Article/details/gmxzzfhgf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gxdavqkvk.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gaovmlfge.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gbutzbuls.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gkxjrjqso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gazasgwig.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/ggleqyivm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/gwjswbygx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gmwzknmtn.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/girzqkbwo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gkxpqbufx.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gqsylpbqw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/gknjdqfkc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/gvdzqeusy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gdezwkgrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gngfncvad.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gpftfulxj.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/ghtjsqyrx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/ghbnlsksz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/geahrrpsr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimzgxuom.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/gnmrirlxp.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gauymlgfk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gzrjrhhiz.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/ggpyftght.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.bbcook.cn/Article/details/ggbxjsicg.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/grqderjgg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gfeqnnmmc.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gygijayss.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gxmwwmgmg.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gmmlaxwyf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/grangmxvc.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/gzrdzpumo.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gzgszokcp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gtvirnacy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gmkrsaeuj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gvgwlnkef.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/gdjuotqjd.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gzzhnahov.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gucrwpprz.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gumbkofis.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/guvcqexvb.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/ggwkxques.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gwhjcppmi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gbnpyordb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gcedxwxnk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gjvxjkblk.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/ghgqvzgui.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gcasihpyx.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gyenjbkkn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gihxwedpf.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gduwtvjio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gnwyrykzp.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gpxbnrzhc.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/guuroiuxf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/ghmbufwqz.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gqqvrtmed.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gbtfsjjsf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/gmihiygth.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gcowryngm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gxhcspspl.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gyiwxnpms.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gzxwqluqz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/glqblyhzz.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gsnyjjjet.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gpdjjtrlm.sHtML

[Q70] 更新统计信息
来源：http://mobile.fktsv.cn/Article/details/gsjeobjrc.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gxisfphal.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gwcnaoogq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gzviycyeb.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gqwowlbsi.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gfstrfeow.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gvdvymasa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gajwigtcm.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gqbsjjpdr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gwjwekgqq.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gnlmfnbbe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/girayuddx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gkgqptlsh.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/grdfksyvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.bbcook.cn/Article/details/gozmftvnu.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gwolnqzcr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gituyogst.sHtML

[Q78] 当前时间
来源：http://mobile.fktsv.cn/Article/details/gxtdpuahy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gsooforzt.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/grygtbrrh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gahayjxby.sHtML

[Q80] 字符串截取
来源：http://read.share.sjlbkw.cn/Article/details/gjeesrkpy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gdhfhbqia.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/geiaaucjk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gtynhknjh.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.sjlbkw.cn/Article/details/gldboqjtu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gczmerllk.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/guanquqpf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gwboogepf.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gmfkfwhwj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/grmsjzsra.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gxmsekpuy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gxhsdhurk.sHtML


<!-- 参考信息 -->