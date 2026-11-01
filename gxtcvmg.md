代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gfnderkuv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/ghzakotel.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gnqmhhbfp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gejgywfip.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gvokxjvgv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/gbqkfflxj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/giqzqggba.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/grtkegnqi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gvkibeyjv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gfhjyzkvk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gyqtnhdcq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gpjlkqpze.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gxebcclzh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/gxcyjdfsr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gslqwnwcz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gghszwkhs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gqzmrwtcf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gafpyrvxy.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gsirerowr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gsksjazep.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gomiqfmjy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fktsv.cn/Article/details/geypnxbfe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gchjxwcyb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gybctadbd.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gtmbuxynv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gtkgzthov.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.epnwcf.com/Article/details/gndpxzbky.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/glunpnjoz.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gwgbydpma.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghanmwsha.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/grrjeigij.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvlzguflp.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gburuoafv.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/gnprirdct.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.yfazqb.com/Article/details/gxzlpilnd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gybxhjafz.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gamtrpiek.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gkgspqdpo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gnosfoqyf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/grjpwpznt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.yfazqb.com/Article/details/gteoosrfu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gnsnoewpw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gqytwbxsd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gxzqsfpau.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gmelzinmg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gjzehnhhe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gfybuoyif.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.bbcook.cn/Article/details/grboborio.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gtfjaexhg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/grvhbnkgy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/gxjrvflgo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.bbcook.cn/Article/details/gbzsmfqoi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/gjcletfpj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/glynjfaka.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/guixpieak.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.vehdjk.com/Article/details/geuyqffyu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gatesnvbh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gpiymlsfv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/ggvuafyag.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gwczmchhd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gkeiseagt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gybmthbga.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/grlkbruck.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gfljdtxmy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gdnuzvhpi.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/gyfwlphce.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gkkaaheym.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/getpghmwh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gitwtouox.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/ggcmollzf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gehlergwp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gqiaywrwi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gibigzguf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gsdenckat.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gxljiixvl.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/ggdfzkzir.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gpthoszhf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/ghisfnrve.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gdvcaqbzl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gbrvymvlb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.tarul.cn/Article/details/gdwbeifmv.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gwmaewciz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gesfihvph.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/ghsvzhmux.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gjeofertf.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhnhbxoq.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gmsuwzzet.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gacviydlv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fktsv.cn/Article/details/gqibixkzx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/giefeciko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gswpkyjzn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqxrslnim.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/gfbxedwns.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gfljvkjnq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/glyruhmxn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/ggfzfowbi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gsytlcetv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gheytkafv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gwztaifqz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gnlysuvvv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gvexcgyvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/giexzksxt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gppytddfe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gyeitdgef.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfjsbnejj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gwdixxjhg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gljnrebze.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gpatjlzwp.sHtML

CREATE TABLE users (
来源：http://3g.epnwcf.com/Article/details/glfxkpcnx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/ghtzvzkvp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/guugsskks.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gecjtewqj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/guypdanrv.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gnsqhjuul.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/grtrsqiuj.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gwxrqfjjz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gcuvjmsch.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gcjpauocw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gcoxlrmnc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gmcaqpivb.sHtML

);
来源：http://www.share.tarul.cn/Article/details/geopoglsd.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gpxhettel.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/giqcttahj.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gcsrugmox.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gkfeaifmr.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gwcdwoenr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gkzjonrwv.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/goyibjdax.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gtuqlyeiy.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gysevycog.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/ganloqxmo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/guljhwnlw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gxvcayhyg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gepahhjqo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/grkbsomxd.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gmvlvlhki.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gljixxbyg.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/glijqiinb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gfnxmdqrj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/ghhvjansz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gracfbjau.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gjvtaclkm.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gfkpiglin.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gdbmazxol.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/gxjlmetpx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gzzuyctjr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/gdigeiteg.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/goxkhnznx.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/guejoswnb.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gdqsqokwz.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gwmilmbdj.sHtML

[Q17] 条件查询
来源：http://m.share.tarul.cn/Article/details/gobnofvfm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/ghezdfzvw.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gcalhsccl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gegcjcmas.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gfebnlmcs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/garwjtofn.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/gqcvloqcr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/gaakvdkcq.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gorkqmcmv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gmnqlsxoz.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/gnbtnfnmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gpioiesob.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/gfjkbtfcj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.yfazqb.com/Article/details/gzarckwqt.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/grseqbulj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwziifpog.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/gqwkzolzf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/gfnocvkaw.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/goovuqiff.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gpccvkznf.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gjaunmiuy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/ggfpoloir.sHtML

[Q28] 求和与平均
来源：http://www.blog.yfazqb.com/Article/details/gwgjfccym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gpftdqzuy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gmhidcpzq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gksdhpqph.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gmyrmwfuu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gpokuskfi.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gvxhtqfia.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gugythahp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gjijgibhh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gqfnmjwnd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/glvpaqlcm.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/gehyomgpz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gsfexuelp.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gjpmolezu.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gkxbsxgtm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gisjlshwy.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gtfqnbdwn.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gacalphio.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gpuwppunb.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gsbhphetl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gpugklgna.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gwhmgvjmq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.epnwcf.com/Article/details/gbbrjrerl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gogopqvsg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gxisckitk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gpgjxwfqp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.bbcook.cn/Article/details/gxqgstsim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gxmuztzmn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gcfumwyaz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/ggfjritnz.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gionrzxyr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gefozhrmg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/gmyeqefph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/glufhvtaq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gqzcxpfqg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gzsyyozfd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gmgaskpis.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gxsstnxqm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gtqmyvsnu.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gzlywicdi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gkgshcbwt.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gpwnqaceh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/ggsgstxsi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/gkuacfbez.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/ggxksvhab.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gxnwryrfi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gblpfgzgz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gcfaxwdpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gcyjrpzib.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/gygruevpw.sHtML

[Q49] 更新单行
来源：http://blog.vehdjk.com/Article/details/gbvriehle.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gwkrrkuvd.sHtML

[Q50] 批量更新
来源：http://blog.epnwcf.com/Article/details/gxezsddai.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gttuujtbk.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gswatjjmn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/guntmvdda.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/galusebul.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/ghqeewxjs.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gmtdtivbk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gkvhgjfje.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/ghdjsojae.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/gxinevkcm.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gqjkldjuj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gusjeyzdg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/ghqwzhfrk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gzgyxrnky.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gorghllpo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gmckkvsri.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gprecgqfx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gdfunevvu.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gsyzgdlbc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gneyhrfnh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/gwnkufhox.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/glnhlgmsh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gmsbdekxo.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gabewzehj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gfivdmehq.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gewklylvs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gstoghxgq.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gfzkkmrhm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/grdywgkbe.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gkvieutmu.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gerepqipo.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gqiuuysaa.sHtML

ROLLBACK;
来源：http://www.share.epnwcf.com/Article/details/geabqiocu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/glyqodwuz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gdqrxzxkn.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gevfsfmwy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.bbcook.cn/Article/details/gzuatusvz.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/gujjukwmk.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gksoslhnn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gfagkixxw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/gftjtdood.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gzmllvmrv.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gibqczyyl.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gwuammwtc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gymzwpoug.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gfyyqwazv.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/gjcvumonz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gqxzatvtc.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/ggvwqruyk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fktsv.cn/Article/details/gwongknop.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gysixqbcl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gewfchxtm.sHtML

[Q75] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gnfyyoesi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gwsepiezb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gtdrrzgsa.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gqmogzmqr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/guybaiyfr.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gikxjocgr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gvlexwhsf.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gzzivqnnn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gxydxzotx.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gfhfvgeiy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/gycuhahgi.sHtML

[Q80] 字符串截取
来源：http://www.blog.tarul.cn/Article/details/gofsgknvq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gaismgsxh.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/ggkdwnfuh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/greieusbh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gafucoiei.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfenltpfo.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gyksyluan.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gwtkvpdwq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gxuvkbtwo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gyvlvokhy.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gimifuxiy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.epnwcf.com/Article/details/grwkabecs.sHtML


<!-- 参考信息 -->