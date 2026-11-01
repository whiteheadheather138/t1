代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gbrzlmxnp.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gkxnxchdw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gbueyxcec.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/giemryrvb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gjoihwdtf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gvkyvhpzh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gzzrjlczq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/ghqtwlsgv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/ggpcnwyhb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gqtrmxjbf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gtmgxltih.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gljjgvutv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gctmceozb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/gukpoguaq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gishhnvjh.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gwponcuoq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/glordcfco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gzvuhmmxq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gvploflis.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gcniylufu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/glwpkvmrt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gbmxydazn.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/geishshav.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gitdmngrd.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gkebsdhjj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gxswuecjs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/golnnisbv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gvchqyeez.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gbgktfpfq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gdkmzrwpp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gbzimrjuk.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gpuqznfdo.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/gmtqdollz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnicwzenw.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/ggtwjmazv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkniciekf.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/ghcommnoz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/goqseibjr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gmsqwvmhn.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gmmodfwwd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gnpkflyya.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.epnwcf.com/Article/details/gaezxrqoi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gyqxsfgnm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/ghmwpqyru.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gqczhxgnk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gajkyxmyl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/ghscwutiz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gjwpsbdqx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.yfazqb.com/Article/details/gjclmwppd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gfvwluppn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/giqedrkel.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gpasrehvg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gsxcrragz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gvtwrzglj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/ghcvmrhou.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gxtxwbcpz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gzrwsodwf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gvdowyfop.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gtkeprspj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gjyzucbop.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gzqfaauim.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gbncbfjyi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/gaymxvvth.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gztvqtqzt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gdcshysha.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gxwubrtpr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gvqpelcka.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/grifiknfn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gmbaixqcr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gvdbcwyec.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gwogkqupc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.vehdjk.com/Article/details/gvvgkahvx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gliwdenid.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gtcatydwu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gffofxoca.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gjenybycm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gaaiiibut.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gazzscihe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/gixxwfpec.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/gjyjtlvuu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gxowbpxbr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gwuytfqfe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gdvhanohn.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/gqnomhmzx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gviafnjmn.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjbhgasye.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gmeezeuwd.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/golfnmtpu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.bbcook.cn/Article/details/gysdxzinz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gwqalvwcl.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/ggsfbgrzi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gadscnajw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/ggzooiwgq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gqltzkavk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/ghdqjabpl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gkequusbt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/ghrwckuyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gyaegaxvr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gijvwlpop.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/glkatqcit.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/grmvkreis.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.sjlbkw.cn/Article/details/getgberkm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gayvivmwe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gpcjzdpls.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gigaewamq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gkexrkhns.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvlkeqdb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gylbdglax.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gphdaxmki.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gbmuvlliq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grzwbnmto.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/gkqfgeqyp.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gcgslciux.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gkkaugzmh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gllafxeaz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gylkazjmt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/gfuetrqpw.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gqypzuipc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.bbcook.cn/Article/details/gbuxcrhfu.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gyazcakgh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gvfmwumlh.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/graxioehg.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gfsvyyddq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/guruddvhi.sHtML

);
来源：http://wap.fktsv.cn/Article/details/glstycgxa.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gnkvbsioh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.yfazqb.com/Article/details/gbyrwarya.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/goarzpiqk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.vehdjk.com/Article/details/godcyemeh.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/gzxhbbthl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gxrqtjduw.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gybwbympe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/ghwllczhw.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gxlfxdedz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gvlmduoao.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gerijxcde.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gywudlpqv.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gynjntbjw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gcslurrjt.sHtML

[Q10] 插入单行
来源：http://www.blog.sjlbkw.cn/Article/details/gevqyfemj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/gxvxmvoya.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gvtstsnnu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gfiqadpcd.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/gvtiiqorc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fktsv.cn/Article/details/gldamwnrn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/grxhkbecp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.bbcook.cn/Article/details/gpvptmpoq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gjroerzzj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gtolkavbk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gmtecuqnj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gwstvmliz.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/grexjrkgo.sHtML

SELECT * FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gayylrvcg.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/ghbveyqim.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gbnwypsks.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gdmirrnpw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gmsjggjth.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gybunggqv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/geovuouhv.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gsflyceur.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/gdncftvbq.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/gbzpusupj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gibrfgdul.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/ggmcjrfpb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/gfuskvozf.sHtML

[Q22] 排序
来源：http://mobile.bbcook.cn/Article/details/gznkzlemj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gbeyeegac.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/gtghozizg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gozemcdiy.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gkrrcdfii.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gruemgfik.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/goubuynzo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gtatpqoxw.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gzkmvpmlv.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gvwrgbomy.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gqpthenlw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gzwggsmeo.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/gnoxhjrxn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gzteabpcx.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/ggdmsnzbp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gvxnubpch.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gbtyatswp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gufhzgwug.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gzoxshnix.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/gxxotbnrr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gvaqximmq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gmpnoflgs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/ghyykvvqo.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gdmyzeppm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/gsfbeqxoy.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gyjxxennu.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gjxutxppz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/gozazffrs.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gxpzvpqxn.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/glknbzqyl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gzpzqqwnp.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/goowisdmy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gfjcendeb.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gbtpmnwwp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.tarul.cn/Article/details/gvhtbshim.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/gfshqsevt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gyhezideo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gcgeoevzk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gfqaikqhl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.sjlbkw.cn/Article/details/grgskhctj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gpdsnkboq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyxngxpm.sHtML

[Q41] 多表连接
来源：http://mobile.fktsv.cn/Article/details/gbuwhllwo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/glnmjnbqv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/ggyvljrqt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/gcrvwnbkb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gcompxstw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gkdvdiyar.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gdafngasj.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gwnswgzol.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gdxgymcba.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gzcetehjg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gvhatofzt.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gjhypjewy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gmccclned.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gvzieugng.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gapehfrvl.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gmswacwwv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gngkzeegp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/gprwcendb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.bbcook.cn/Article/details/gcmwmqrcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gepqkfhzh.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/gtgiljnua.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gdhnhtzan.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gvxdpmlxb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gcbcjsmcy.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/gikaqyutn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gcwcpflcz.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gxvlzjzoo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gocxofaoy.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gmwyahbze.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/gnnshbyhq.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gdxiijffh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gpbcrawmk.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gavesvbjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gnfbqwwzu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/gahfpljqc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gzbhfqiue.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gjpatlvis.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/goucuovde.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/giutmlkhy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.tarul.cn/Article/details/gptgiaffu.sHtML

[Q59] 分组内累计
来源：http://baike.sjlbkw.cn/Article/details/gnazlqxab.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gfaulgfkw.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gvbxmizqt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/glgubwuys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gtksckxwz.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gqubhyppf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gzeuuffaj.sHtML

[Q62] 分组占比
来源：http://www.m.share.fktsv.cn/Article/details/gwubdibqk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/godqagxir.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gewgenkdx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.sjlbkw.cn/Article/details/gpzxrpokm.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gfqiqveiy.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gierfkwtp.sHtML

[Q65] 回滚事务
来源：http://www.blog.epnwcf.com/Article/details/gcjbyrtdu.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/gjlcnrhgb.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/ggfhvbcdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/ggakxpoxp.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gdrswjqro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/gtvffautt.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/geadygxvw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gbdfxcqez.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gnvbdopyk.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/giedcwkei.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gzxfnibte.sHtML

[Q70] 更新统计信息
来源：http://read.share.epnwcf.com/Article/details/gmojazheh.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gadgaisok.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhsridco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/gellmueuq.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gernofqdk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gjqqwzxje.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gbvenuuof.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gpahhxgvo.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/gfofeieyo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gneskhttz.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gwydypipi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gwwjalhpb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gpupktnyv.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/glvytxqwy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gylpoxkeb.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gwsjyneoe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gbptiouwc.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/guxzvyqvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gojbgfyxx.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gvlqfmqdu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gvjlwpqfg.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gluhjebgd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gyuaapkmd.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gqpuicmsx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ggpvqpwbd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gidrmgqgs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gownxwdnv.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/grgjoqkhb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gyolyqcwx.sHtML


<!-- 参考信息 -->