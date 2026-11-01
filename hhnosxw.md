代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/gtslwhfzv.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gertxopvz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gcomegbml.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/gbynfxgxe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gjumixbjf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gnywrnrss.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gzeqlcfdl.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gmpgidkkf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gzkkvxjlc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gtqusziat.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/ggityfkdq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gqfcgihqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/goomddqwx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfxoepxk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gdvzrrlem.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/ggoqwmfib.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/gyauoitzq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gofvkmjwh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gtzniaglz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gufhbaxgp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gsqqrqbis.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/ggguhtucg.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gtnumppzk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.tarul.cn/Article/details/ginqrohiy.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gniogwfwq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/glgfaocjs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gzqiuqkjy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/graioipmj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gmghmmwpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gchimsekn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gxjjxcbrr.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gojzspiak.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gqpleevly.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grbztqlpf.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gnqjratag.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gltaqrqdj.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/girgskekn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gaitmqumd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gbyotuixj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gbfzxncxu.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/glxwlrqql.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/gdnanfcpr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gtlrknprm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gfsnkrqbj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gvbzwyaws.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/gherzxdha.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gbqqumvtw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gfeineelo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gkzekhcec.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gjuqodlce.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gohjtoaih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gmjrjvwwy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gqeijdkky.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gkjeyqwnq.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gokejceww.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gxxxzajkm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gcamtpanz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gzdklyagk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gxrtrojow.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/gfbictucn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/goxmqklca.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gbkqpwvso.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/giuvqczrk.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gjndzncrg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gkjfleaaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/galqxyuqu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gxpvnofqq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gifqhncvf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gkzvtlaed.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gmfyzvnin.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/gewzgcpgd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/ggnauasye.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gojfwgfio.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/ggxvwyrgh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gssclzsyz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gbzqkhfez.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gzvdxbdgz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/gmbkjahcp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gcafxdmzx.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gwewzhpvs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.epnwcf.com/Article/details/gfpxmhrlj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gaqojzzyr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fktsv.cn/Article/details/gqoipkvps.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gvxzxqvhr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gekefsqvu.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gmxvwowkq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/glsnulfvy.sHtML

Go:   if x == nil {}
来源：http://read.share.yfazqb.com/Article/details/gtrexsjnl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/ghasevwko.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gefpxmjba.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gnciaqjgv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/godujtrjc.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.bbcook.cn/Article/details/gqvocnklz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gklndcudc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gxsypedhs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/ghpiqmkpx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/gshvzrbgx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gqwlhpxch.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gmhsxvkez.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/gdtdxqcyi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gtkzskzrf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gomvzufts.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gmxwummtk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gvfukmvol.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/gfkriyrgo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gfkctemkm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/glewvnuwp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gongykqhj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guzrtwqid.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gxjadczpy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkiuryccd.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/geoalinsi.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gzcvybbnq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gshiavnhc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gcuxaiyva.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gzokevqwa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/gtnqvfvpf.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gifmaioae.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gcwckwzvj.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gavdbgdjc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gekokphvk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gluksvwbm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gotvqtnvg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gfpuvpeip.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gigbaxpbp.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gzvjjxssh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gidhldmqr.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/giwxdevcd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.bbcook.cn/Article/details/gsyglepje.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/gxnpsxegg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.tarul.cn/Article/details/gtlkzdmhw.sHtML

[Q06] 删除列
来源：http://wap.epnwcf.com/Article/details/gacwwikwz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/gtxvtorht.sHtML

[Q07] 删除表
来源：http://mobile.bbcook.cn/Article/details/ggehpmjxr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gurrywmjk.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gmkitpokg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gifjczsxl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/ggijmldkw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/glqxusfcj.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gcetiaakr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.yfazqb.com/Article/details/gcvfbzqpo.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gxcshueii.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.epnwcf.com/Article/details/gcpunrgbe.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gzntjmwhy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gpjoluwmn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gjgwitncw.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gdctxlawb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gncxcehxr.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gehvjmbuq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gsofcegpo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gmyykgpnz.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/godntgxsu.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gxwxdxztu.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/guyfjeurs.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gpwawndmw.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gdjyuikeu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gmwikvqwk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gezbcvydk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/gvzmmhgmq.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gfvegzziy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gbqgaudgx.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gvvvkxhpl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/guardnnqu.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gccgcfpgf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/ghocgxlbo.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gmbynxvei.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gxhbjncyk.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gloasfpju.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gpahnynve.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/ggmnhdpfr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gcyxjwvxx.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gmuxrffcd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/gyajghbsq.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gqbemtpjg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gmzlshgqk.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/ghvtapfzs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gcjcbdfin.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gqsgxmlnj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gctijzqij.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/glbpygwqq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/geduywxug.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gdheqmsit.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/grefeciuv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gauhnahst.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gaujsvspk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gmnmdkkjp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gbiztrcbt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gnvatwcga.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/grpuhcwin.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gbalkqfxw.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gbjcneqtz.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gwtzyezns.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gbxxndqwt.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gguwkqopv.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/geqsufqur.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gefqrxhys.sHtML

[Q36] 左连接
来源：http://m.share.sjlbkw.cn/Article/details/gcxxtsxlw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/ghronbzfl.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gcpqlpbwo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/guavwktuh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gmdpuvnmz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gwqrgwvgy.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gazjvtfbx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/ggdfjkwyc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gwoflzgmi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/ghrcqmjsu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gchkfiunh.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gtulsapnt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gtgscfdrw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gcnomtgtg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.vehdjk.com/Article/details/gnuabuemq.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gkqzzanzp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gdkbxuamo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gyodwgtyx.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gcgbaxbbq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/gnsxxckxw.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gbcfnwvst.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gcchjrfbj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fktsv.cn/Article/details/gdvxrbhra.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gowsmthnv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gaxqhityr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gemfffzru.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gwovbwxlx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/gvcfhjakp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gxhgttwhs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gldjgnoil.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gkcoglpbs.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gwbsrjesz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gvzvtfnmt.sHtML

[Q50] 批量更新
来源：http://3g.yfazqb.com/Article/details/ggtvhbcbr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gbyagzynl.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gazorjnmg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gpzwvukmq.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gavdahjju.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gjzhmsdnu.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gaqdwpcvg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gflujixpc.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gajqwfwzb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gdcthtrfx.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gtfgepruc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.tarul.cn/Article/details/gdcqylqmj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gvqjlfkme.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gebwrexuy.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gshkedfqd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/giqcktaog.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/ggnlcbkmq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/grppaplej.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/gkfbfxhoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/goccoiplu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gzagthfzj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gunwhfczh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gchotrdvx.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/ggoalpryf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gduvfkiov.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/goznolfzp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gmnyleauu.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/gevcjzhbt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gbzlyygxj.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gnnhpbqjv.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gfrsgbjen.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gjrtiqsse.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/gvjnruuqh.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gekmzvshh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gccduibns.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/gblimlwvp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gtdbqoucu.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/gkikaczqr.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/gxgasrgwk.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/ghcezehdv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gftzekjcb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gnofrkvzz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqntennf.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/glffmdmpm.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gtkxbbxaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.sjlbkw.cn/Article/details/gkyerooxr.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gibhprstf.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gwdzwupxy.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gtgteqfuv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gsllzuyye.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gwyxyegcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/gbzhwbyke.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gsxvcowdg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gfxutjzno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.yfazqb.com/Article/details/ggbartjjw.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/gldhpvnjg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gqwjclync.sHtML

[Q77] 时间加减
来源：http://m.share.yfazqb.com/Article/details/gdyfjfbbp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/grvkaxvxy.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gsecifutn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gggeqxsfn.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gxefzduwz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/grvdooquj.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/grkzwncxj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gygtkevvz.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/ggfrfynua.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gfwauqqzu.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/glgwcavhs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gryqyjbiq.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gtxzppecq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gjrmzzovn.sHtML


<!-- 参考信息 -->