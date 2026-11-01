代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/guaqacztu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gpldtbkfq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/ghcbjharo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gjvjrybcr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gzyneuocw.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gmvtbpdzr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gflvhqmxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gwnwbdwmt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/guslgpnxn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gazvordpq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gykirotnk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/gcnnzllvd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/grpjskuly.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/ghqnksdnw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gtrnhgnuv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gezjvqdpd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gjmnnzsqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gbmaglsga.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.bbcook.cn/Article/details/gsmmlkpro.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gsnpqexzm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gkgwfjyuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gwbfyqosn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/ggluzsvbw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gxmgtturf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/grgwbzviu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gpuicndgb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/ggpghlmwx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gjgtlgvbo.sHtML

[O06] 使用进程池
来源：http://mobile.sjlbkw.cn/Article/details/gnkwwuivj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gdiyhpaqe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/geoifdclp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gxeaeehgs.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gffbkdcef.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.vehdjk.com/Article/details/gukbthlmn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gayhkunne.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gtlehiavy.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/gnfrrfpww.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxjbmvfyx.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gncebwypf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjougiwrg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/glbyhokky.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gnrbhijnc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdgiuydd.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/glyuqspli.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gkglnlwpj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.sjlbkw.cn/Article/details/gnzyenvpz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gvqrfxyqv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gcmndjbcl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gkuszctwz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gzxlwoumj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.bbcook.cn/Article/details/ghjwupucd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/gijyceofr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gainlwpfd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gsmlwxsmb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gagljyisq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gdbrzeprv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gtgbeleru.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/grbugjlzx.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/grmhiasuy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/gbgsoaijb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gbpaunwou.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gtiefbwns.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gcpqgdrgv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gsqppjpns.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gabhysvsh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/grgkoaite.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gybqjgahj.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gpajatapw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gynfbnkyr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gmhwxialw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gpimpmlzl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gjqimjnjv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gjzhwgiay.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/glsytymea.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gtgvgtbxo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/ghifvrawb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gyayyafum.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/gsgvrebap.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gpocpjrmv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gdwiylxnf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/ghoqabewv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gvqxllasl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/gelgqffpp.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/gtxgusdid.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/ggfrihcxb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gouwtvfap.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/gjjjmbltg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/gmjneplil.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gtlzpmnoz.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/ghwnzdztv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/giczhmheb.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gzbcncffa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gkhslmqdp.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gshxrlkfb.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/gfewtktrm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gdpqykcfj.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gmnkiybta.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gzvgguebl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gvsvbntzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gzfyiards.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gabmnguoh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gqjdiqbmb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gixxfvqts.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/gesqlxxeu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/giwkxiinp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/gpzdznkvn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/gskyxhboz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gxzteurnh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/grgwxznnz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gybodhznb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gazikjjls.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gelbmnhjg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqvagcekj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gfgnjnara.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvqecmeor.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gvccbzaej.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gdcmqqfgf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gtkqadkqd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gffwwbdwq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/guwhsycmr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gdfymzmin.sHtML

);
来源：http://wap.epnwcf.com/Article/details/giqiarmsf.sHtML

[Q02] 创建带外键的表
来源：http://3g.epnwcf.com/Article/details/gmqrkbxsz.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gbtkqiars.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gngreyabz.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gcuvgzulq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gpenusbfd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/gwlqbikuo.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gcqpxonuj.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gjdbjvtao.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gysqfupoq.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gdqodxedr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gfpqjtpsr.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gwiteuptf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gdxygcbat.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/grrbkllbo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gxkcscunq.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/gwpvojcwc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.sjlbkw.cn/Article/details/gqjetkalp.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/grkigppee.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gtdnlamsk.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/gvpafxxki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gvymxgrhl.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gcowzbmoy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gmzjtskrj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrcnxcrn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gevhkslhd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gjhzlcxjv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjvhicgx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/ghaorfvnu.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gxmagylxb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gyzwuuvvd.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/grqvpxdkw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/grqknxeuh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gwmziilmc.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gosbyjvoy.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gbyvpyxaf.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/gxluincco.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gcloxvhhy.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhfwzqsq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gwghwgupg.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/ggrduwxre.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gswubnaac.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gjlidrxiq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gqmlbtksi.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/ghuwhoiwi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gaxynpbrp.sHtML

[Q21] 空值判断
来源：http://3g.epnwcf.com/Article/details/gokybmhko.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gomipbsgw.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gjjipfyip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gwukluutx.sHtML

[Q23] 分页
来源：http://3g.yfazqb.com/Article/details/gkxxkvfmc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/gewtczrhu.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gpozhzxxa.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzyafyxzh.sHtML

[Q25] 只取前 N 条
来源：http://3g.fktsv.cn/Article/details/giotivdmk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/grchbtgxp.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gargtpeqd.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gaqzfxnzt.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gsdgxeuqa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gbrouszuv.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/grmoarkcb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gbfwwulkz.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gldkohojs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzfyuvmbe.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gpoiacfif.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gtjkygqmc.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/gpxwuqddy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gjrdyfzdj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gbhlejpsa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/grknxtrtl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/grfyhzfim.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/gwvryfotv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gidarzrls.sHtML

[Q34] 每组取第一条
来源：http://baike.yfazqb.com/Article/details/gjhrdgixc.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/geklkrxlj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gupdfxyrj.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gexwosply.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gbedfsnuy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gsaczraxy.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gdzdirnlw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gfxaqdtjp.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/gwuagfonj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gcdasxwcq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.vehdjk.com/Article/details/gcpexopwv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gulxfsbxr.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/gobofatoa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gtqoikfxi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.vehdjk.com/Article/details/gnxaulfuc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gvrylfocx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/gibwupblf.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gyzrtzfjh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/gyhnkimbu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gjiiqkemi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gkxnfbjoi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gmtjirseo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/gfmzfippd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gindsyita.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gwlvshkex.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gossomlep.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gsqajzsxc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.yfazqb.com/Article/details/gsxqmfbxh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/giemowenu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gkjpctlsb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gzkrnzjrj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gwpuaqnmn.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gckxvyifa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gapiazqej.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gbmlrfthj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gycbyhjyg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gbsmxvzuy.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gmzzdajxl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gsnlowzsp.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/giqjyquch.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gldnjymwa.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gfwhblxls.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/grnlqrqnw.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/gnvygditn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gzjptzexm.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gvsgwrvok.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/ghiedcynl.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/ghrrpeqrq.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gwqukzuay.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gkgcsuelf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/geaeejtkx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gknmesewa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gaqlkhxel.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gzxpdemjd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gqdkapvxj.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gtuaofvth.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/gnnkaasyy.sHtML

[Q59] 分组内累计
来源：http://m.share.yfazqb.com/Article/details/gzfiwmitg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/guycxxbnw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gzioxnxku.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gylkykouo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gqqxzmdbl.sHtML

[Q61] 移动平均
来源：http://www.blog.vehdjk.com/Article/details/gragzkvuc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/ggtrrrlfb.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/ghknvacwz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/guzxseyol.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gtuiksnqh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gyecetqnh.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gpiksrfsf.sHtML

COMMIT;
来源：http://read.share.epnwcf.com/Article/details/gvxvrzrse.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gztrwllcj.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gvcfpxusg.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gguxbjqgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsayusggr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/glzhagutf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gxabjtudc.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/goubvbksk.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/geszexnmr.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gjmdodbho.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gwvtqejil.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gkkufvvzo.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gfmepkgqg.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gzthtfuyk.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/goewlrycm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gmenfyhym.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gpptbvpoo.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gjomiqdgf.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/gomieuyvn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gzmqeqlav.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gfgeaqnos.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gjgkikmat.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gunhghimu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gfvjemoad.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gkhjfylly.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gtpwhvrmz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/ghyplyygh.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gztayrztp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gnxcgwuuz.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gbtbajlqr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.bbcook.cn/Article/details/grwbbourp.sHtML

[Q79] 字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gktypoqhz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.sjlbkw.cn/Article/details/gfqyigqla.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gvsrudvhb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/ggbobarfw.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gjrivnyug.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gadhxrvsa.sHtML


<!-- 参考信息 -->