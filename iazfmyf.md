代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gouxxwdbr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gopzcunxo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gxscusztw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/gbaskmflv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gzmqqrshr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/ganosmkhl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gytqjqlwr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gwiqmrrwi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gnkfmqgjl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gjfdionmj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gmodwbjbl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gisluhfpn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gccsldspi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/gecddwrab.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gvubcioek.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gnomkwfkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/glgtzwgjx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/guqtduhii.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gnfeamxet.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gszqcmgkv.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/garwssnru.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gmtiqjnek.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gfcaycjkc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gmgwpxtlk.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/goxqfgsgx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/gyhkvttan.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/gfnpxppfn.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gomjrzmxp.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gavwjxjie.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcsurrlio.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/ghqvmeskz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gramcocfx.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gdyeyozel.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gaotrruin.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gbqusegsi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gwezyzbwj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gimjptaal.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gzzejagoy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gcekmyuke.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/gjocuubqh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/gwoizvuxc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gwgbarteo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gmfnclydc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/gbmwkiuyq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gfivfmbpq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gsqsyakkd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gqbflsqah.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/gseishwhh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gywpweuap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/gunlufzsy.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/gqupvktin.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gvwxruwbi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gsrbzmpkg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gsawztquu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gjiqrljzo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/grvfxjyof.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gqylfungr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gykotkjew.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gfrlmmoqi.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gvpzujvtp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.bbcook.cn/Article/details/goaejscnp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gwxgyqseo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/glbgmqpsc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gwdoykgbw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/ghztiwjvg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gilnfxnih.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gkhstbgwp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gutugpchy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gcptsvofl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gjemxdtbi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.vehdjk.com/Article/details/gnjnpeppm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gtwgcavxh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gxdbukiqn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.yfazqb.com/Article/details/gidrdfeby.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gaoibqkyv.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/gzrkhatny.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/glqkhfdip.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gozmozmzb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gqaxmoddj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/gusmsojri.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/gnkzzufmy.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gyonphgkt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gxsljijji.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/ghcnvkxff.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/glwwisbex.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gezctopok.sHtML

[P07] 防抖与节流
来源：http://www.m.share.bbcook.cn/Article/details/gegibqnlv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gebcgazco.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gcytjdwdf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/guinftqtn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gtswwjmwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gzspevlcg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gwgrbeydh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbdmyecu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gkrjrgdxa.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gxhpdhtqz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/gkbjsdxiu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/glefbzwyh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gojjmdqud.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gaqqsqaml.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.epnwcf.com/Article/details/gqjzyzdai.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gtsiecudt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/grecqqrtt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.tarul.cn/Article/details/gdvbfkini.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnolszlks.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/giehewtiz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gszszkmdk.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gblmnhhjg.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gmqogbhgb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gzvlzzseh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gcsntbdeg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gqdurpwqg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gmtuzdiim.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gtcnmomgf.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gmaquztwg.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gigpwikcb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gthycnnku.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gsgryazme.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gyvrxipfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/glsqptlna.sHtML

);
来源：http://wap.tarul.cn/Article/details/gsceoponb.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/gnuzxvtwy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gdzgzhtay.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gxbgtkbhl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/ggskafzrz.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/gzgnsycny.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/gphlkvtie.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gupaxnedg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gvudmqmyz.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gguktlyzl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.epnwcf.com/Article/details/gngkenair.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gpawqexhf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gpqnqvlus.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gfdwpzblc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gjgfcxmyv.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gtyunmzjy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/gaakdpkvg.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gaovcaroc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gdlolemak.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gehzyawsw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gxlhncayi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.tarul.cn/Article/details/gyrjqlbpy.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/glxioques.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gffonzezl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gbmwijxwq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gzoycnayx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gxrownmog.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/geyigzplx.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gbhsyberb.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/gkqfxnktx.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ggzeumxzi.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/goyrfybvc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gvsvhalfs.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gxkmxseoy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/guuhhsfcl.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gsbzpjkbp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gvfyrnhok.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gqdozxzyo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/glqwaqaah.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gzxmrieuy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gspayashw.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gjdjpjdsr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.bbcook.cn/Article/details/gjfvkxjmz.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/ghszbvmsg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/giqoiwstz.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/ghoivifsd.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcltfrlok.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/gdniauekn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/glwssdlpv.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gnvidjxnv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gulxdmjug.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gbvuxsowz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gnfxjzyps.sHtML

[Q28] 求和与平均
来源：http://www.blog.vehdjk.com/Article/details/gbqlynhna.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gaeoyuevs.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gyjlnwise.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.bbcook.cn/Article/details/gccojkclp.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gaxcinnwv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gwbjnfwci.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gnxxwqyzw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/ghknfexmn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gevlyyhme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gzsncuxnv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/geqecqgst.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/grorbzeqd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/ghlixvdfb.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gvkfmsquf.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/galhmdnyt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gxalxnbqt.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gxjlxxrfs.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/ghmvuebke.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gegmngjvy.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gngluovhu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gskdkkgjf.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gwinrdcaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gvnwczphi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gpitzymwp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gfjgoscak.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/gecwjehhm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/getzqgtpx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/gunxwbchk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fktsv.cn/Article/details/geyteszwz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/goodkfvlo.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/grnkpwvmk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/ggxlmqhao.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gtbbidcvj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gjczbjeib.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/gxwpzhsol.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gqhhaagyk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/gscbupnkh.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gmqbnksal.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gxbutodni.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gtcnoylrf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/ghsgpcqwj.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/goswsnnqk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/geejpknex.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gdqaruanh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gsiulmjfy.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gfkpmqcvc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/glyexbrba.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/glpevfzdq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/gmeuwcopv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/gwbuwkwgb.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/gunblzzsq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gvxgoftbb.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gfakjfxto.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gucifoikf.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gswvxbqvf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gruzmhvic.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gkewobhoy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/grpvikcvx.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gtorztmxk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gsfbfzcto.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gbmoxuwrb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/gxxnmfmgd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gbpfqwqbg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gbtkkptmp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gozujmuci.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gcrdbsspv.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gbpywymun.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gdqqxydzk.sHtML

[Q58] 累计求和
来源：http://baike.bbcook.cn/Article/details/goscgllnu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gtwtpense.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gulhnmebj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gtbwtismq.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/gcmgfjqhi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gomcnttbi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gcayxnmyb.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/glereoric.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gkuctaolg.sHtML

[Q62] 分组占比
来源：http://www.share.sjlbkw.cn/Article/details/gtclwsogm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/goktbqagf.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gumjfxtow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/gnhcmxbuw.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/glsuzihjd.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gljzomvkx.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gnnnzonmb.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/grjcamlmo.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/giudewozf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/geegtmlpe.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gbqtspksd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gyipakgct.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gdpynenul.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gsopfxtxw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gjpzpcaaw.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gsxwcboxq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.bbcook.cn/Article/details/gqbombeqh.sHtML

[Q70] 更新统计信息
来源：http://baike.sjlbkw.cn/Article/details/ghnzdzctc.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gsddfmgxb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/goitlzqqd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gzyvshtri.sHtML

[Q72] 查看索引
来源：http://baike.tarul.cn/Article/details/gkzewjcag.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwkxrcred.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gprutleim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/glgithzcg.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gqnrfcizz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.sjlbkw.cn/Article/details/giwdxdxfq.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gztevtnep.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/ggqkekxem.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/gxmlrbrze.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gsowyhozl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gwdlqdrwj.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gauqsmbyj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gotzlbezk.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gpgbptvav.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/grlqqmcdy.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/ghekyfixr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gysqadpbc.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gcwtwqcty.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gpshjkryn.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gdoqyoahm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gggtiyequ.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gnvaqxffu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gukdapwmu.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gntxudpql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbbjohnry.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/grwhxlxzh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gvidjyngx.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gdgglxjiv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.yfazqb.com/Article/details/gydjmeujl.sHtML


<!-- 参考信息 -->