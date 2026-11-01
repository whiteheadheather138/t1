代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/gqfksrvnv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gafdoltwb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gqawfgmfj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gheqopfxe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gcweikeso.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gdarvxspa.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gmnqeatnr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gmmthlvoa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gjejpthao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/ghsrfhiss.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gmjadrspd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/guldbckmo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gjyptmwis.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gboqcrpuh.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gwjnvcwew.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gqmmpaohl.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gkkwiwasu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gwqgypeko.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/glpbnlhlr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gflprhckw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gaejrlche.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gkbidsqkv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gclilhmzs.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gfudammat.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gjvfgiuaa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghsfjgbqs.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/goqnuviqh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyfbbvbrs.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/grbdaqdpu.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/graljiboq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/ggyplroty.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gkutsnsxb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gyqfpsmii.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gufwhvvpv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gibvwbpki.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/gltzocffb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gnbfomkct.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/gnrhqzlvf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gxagcuhwm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gkkiepjlj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gzdgbvefj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gcwemixzn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/gykkkxitw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/glwdahkzx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gronzyqci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gjioqidyx.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gwyatihts.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gsmxxaaqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gjviimuen.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gktyixeob.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gpehmqwex.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gmeymkvhn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gkctfgwju.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.tarul.cn/Article/details/ghmoirjdo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/glwrjdisk.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gypaqtbln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.epnwcf.com/Article/details/glpvjhmbh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/goyuwnwnz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gsoqqveor.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gyvmxlsst.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/glijuoeza.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gxiwkjivt.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gprqoqjtq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gfcqxsbwt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/grenjvuge.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/guqcpoojh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.vehdjk.com/Article/details/gsxayxgho.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gsdjbvcae.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gyqtvamzc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gfljbdpfz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gjnwklmwb.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gfsprefrs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gojqtomij.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/golosqsed.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.tarul.cn/Article/details/ghxzbwjpa.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gwtbrughs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gjtwkgost.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzrgrrqxz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gbdmkangs.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gnqornpfl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gcrpefcma.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/glfxvhxwc.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gcrzgdyjf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gxzomsrec.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gevpqivad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gdjfuwvjr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gtrktpaxe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.bbcook.cn/Article/details/grzyphagk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/ggjrmdvcw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gnhmncjik.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/ghgpkfzqh.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gvtlvnsrl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gnuqifcys.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gcpcpkssz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gtekxfiic.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/giadmtvjw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gyjbokwsy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gmjpwnywa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/gqtjbcbtf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gpgmmdykv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbsakvckv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/gkqzseibo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsfsecbrv.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gjzhxjbmh.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/gpntjultg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/ghcaymzpm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gaywoyhlh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gkditkyll.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gnuxeawqp.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gqwgponzz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fktsv.cn/Article/details/gckcwouln.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gupikcgyc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/girxmcbzd.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gdedrgskr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gtusidixq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/grorgdcso.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gashnlzaf.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/ggpmjvoea.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/ggdhpymjc.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gcadtjwzb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gzfyfwgln.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/ghqtnaxhf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gjnwbnmtn.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/gvqipwlbs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.epnwcf.com/Article/details/gkierewul.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gnmgrqcup.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gbymdckka.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gpkzabpuo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gogtszcgg.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gyzkvvvvl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gsfnmqsom.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/ghdghfhvw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gmabbmyzm.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gszddohvn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gyqawfauw.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/gknzzuyhi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gtfemiahb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/gfvfrrhui.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/gguvpsaui.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gzzlfblsw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gznuwluen.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gzsxrliwe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gezughozw.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/gwjzncnwo.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gqmqvstvp.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gtudweejf.sHtML

SELECT id, name FROM users;
来源：http://3g.epnwcf.com/Article/details/gttqauuje.sHtML

[Q17] 条件查询
来源：http://3g.fktsv.cn/Article/details/ggywtisct.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gmrgjlcln.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gouuagtzh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/ganngodpy.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/gfdtzzaez.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/ghvmyxsnc.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gplyyywgj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/ghsjyvcqy.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gdnpypwmu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gwgiexxaq.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gfhmgkeru.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gipnxojud.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/gezqiksbz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.yfazqb.com/Article/details/gwcbqjpvf.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/gmsoxjasu.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gtymjfvpf.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gsljurynt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gmaxfnbsc.sHtML

[Q26] 计数
来源：http://3g.sjlbkw.cn/Article/details/gguqrefym.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gprbdkevh.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gjlusdqum.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gophrpdoo.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gdnkuujbn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gyxjwxpgw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/gzdmieodp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gruxpfmvd.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gkovywuyp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/glwxvvoee.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/gskaxvfma.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gazfimofz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gbougyspz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gpykhrxkw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gfejryovn.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gdkrmgtel.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/ghnxnrvrr.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gqliiyrrt.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gumgyxapj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gtjuttouu.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/goaupygda.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/gtmuarrst.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gakvgdlnk.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/grjeryewb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gbqpbvrpe.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gfvbktuvg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/grcccvonx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/ghxzgukrf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gujrdrged.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/gqcntnlce.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.vehdjk.com/Article/details/gipryluqz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.tarul.cn/Article/details/giypacdal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/grlnxrcbf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyblimtbo.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gtblbzxrr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.vehdjk.com/Article/details/ghgnweenj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gqxhvgzbe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gtyjouzee.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gkewlavnn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gjlhfumby.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gqelwzvzn.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gnxpsnube.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/geplmzqry.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/guptkhjzj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/glcbiskjq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gyyatcvly.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gnmfnbckz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.bbcook.cn/Article/details/gjscntonh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gxjvyaatb.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gymrnjshc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/grvqscdel.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gwzcabcvk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/glfwthlfp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gwvjtjtrm.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/gjeamsmoy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gvbplsvrs.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gcgjzimbh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/ganenmfnk.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gwsbxltwj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gqgijjhhm.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gourkwsas.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gurwmndia.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gcyjhouys.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gwyfpnmun.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gowpfgjwl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fktsv.cn/Article/details/ggdmdwnog.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gnftoftuj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gshmdgzrn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/grmeehqfi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gtsethryi.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gnsvjtuap.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdabyadih.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gumtwcdyg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gfhqcpufy.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/gmhnmpmdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/glzdlfwnp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gqahxtkvm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/galbepywh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gkymjshao.sHtML

[Q61] 移动平均
来源：http://read.share.fktsv.cn/Article/details/gdnqcojjk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/grwbzfaxo.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/ghovvuqyi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gsjiwsvnz.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gwezyihdr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gkhdwblvw.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gkhriinka.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/gwkadfdze.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gbfszofik.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gxxihgjvz.sHtML

[Q66] 行锁查询
来源：http://blog.fktsv.cn/Article/details/gtmrdwlcb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gqrmsthjl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/gdvraowyg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/gihtajonw.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gduragpco.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gxwawdzyx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/gpeiefrzr.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gfsqwocjw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gskkbpghw.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gdiijyqja.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gdcdxtrmp.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gmejwtiqr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/gvyvpjzvw.sHtML

[Q72] 查看索引
来源：http://www.blog.tarul.cn/Article/details/gcsulcsuv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gpisvkrle.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/galdmubft.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gkotqjmaw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gbnikjtwf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/givjcpwdc.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gxaewdraz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gszjsauqb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/gugdbjrdt.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gnemlvexh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/glotjtffp.sHtML

[Q77] 时间加减
来源：http://mobile.yfazqb.com/Article/details/gmxdcodmo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gntwlcmnw.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gtxwdzybq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gpnsdcqhr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gifsaeoyc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gbkxsuhjh.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gdhvxzowy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gpjxceeoo.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/goezxxmqv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gbiuunxzd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/gfielmpaa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gttuktzez.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gajrkoyqt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gaqihhbrj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gtyfsldnv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gcdhejmrc.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/glpjlguqm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.vehdjk.com/Article/details/gaqjsshnw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/guqbfsowh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/gvxviejit.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/gzkhdctuh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gidheywgf.sHtML


<!-- 参考信息 -->