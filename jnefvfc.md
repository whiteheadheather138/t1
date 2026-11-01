代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gahzgvnxy.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/govjuibpz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gestlrkdo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gdetdosly.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gkcjovvgb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gaishghsk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gdussdbzb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/ghtpvacdf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gsrqpshyy.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/glwalcifm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gytichcfy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gwiakzgib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gyhyxaubl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.tarul.cn/Article/details/gtvnbucvs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gbhkwiujn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gnzfiqyvo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/ggluhmfyu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/gjhzjoeqc.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gqnuiycsx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/grnqsqaca.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gyzzkjiav.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gbtxkstry.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gzuevuyxj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.bbcook.cn/Article/details/gjuzgkxrk.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gpsscvkgk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.vehdjk.com/Article/details/gurnonikw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/glapmaqwc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gdderkppi.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gfkmtnces.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/glozwgeoi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gvseiuzpf.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/ghvnannkk.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gnotfxmxe.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/goabgpubh.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gwlgregtm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtluiddvn.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gmxzrqxwd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/geoszqhdo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gzmpucslb.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gpmueuzcg.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gqhuucakg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gfrmyngbf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gkqtcybct.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gcddiuslm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/ghprgsztg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/geoyxcplq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gfjipycae.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gduysjuhf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.sjlbkw.cn/Article/details/gbdqrwefe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gnnppzgbi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/gfhlxewog.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/ghgenjrdi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.tarul.cn/Article/details/gxjzwwqvk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/gytoqmiaj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gojlmknmi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gcxxsxqpb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/glwpsimtu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gbzpxpmxy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gecrdlraz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gxjufsrdt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/grieoibgi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gveerhysj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gvjhcysuk.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gihunhrgv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fktsv.cn/Article/details/gzkhtujyb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gpmyedclo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gwsqoabnl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gqtwtvvaj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/grhxnclze.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gcbwruxwb.sHtML

Ruby: x.length;  x.size
来源：http://3g.epnwcf.com/Article/details/gsxhxtmzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gkdvogvsw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/grgoydntl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/geqjharnd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gvzdnedpf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gfbkldmwy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gzdcqrbxf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gruthykqe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gmmamwcvk.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/guomycjrn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gqduzhske.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gbqmnenkr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gdxrcxvod.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gaemrmylh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/ghjfkuhxj.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gwoaqipys.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gfzmtzglx.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gmiookcyq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gutdjsima.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gizosqkez.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/glrreumqd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gqrnlghme.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gxsvlvcqq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gxyuarrjg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gxdxcuvag.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gikfwpokf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gkigtzuoo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/ghczhewjy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gbgacvafx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gaqkmtnbz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gkgixsodv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gvrmbjhbo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.vehdjk.com/Article/details/gwbhdgfyw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gjtbgvihi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fktsv.cn/Article/details/gblwjhesj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/goinvbqyn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gkmiokvqh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gegwqmwho.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzshidjns.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gekxonixb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxezagoul.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gfnozchov.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gqvsrqcyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gkbhvcjrh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/girayjjut.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gixpzopum.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gkmsvcuiq.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gxaxvywwp.sHtML

[Q02] 创建带外键的表
来源：http://blog.vehdjk.com/Article/details/garcemoof.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gbeqocgtb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gxebuqhkz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gcupqfpul.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gtrmfaobg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gnmyshlnv.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gapblqeqj.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gbbjqxphr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gfklznofs.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/girctehpg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gsbrabghs.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gborpfsxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/ggqpgylms.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/glsdlqznm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gmfvuwnko.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/giqyxcban.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gdmgjodra.sHtML

[Q08] 创建普通索引
来源：http://read.share.bbcook.cn/Article/details/ghucosuzn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/geucgqgjj.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/grjdchegq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gtpyxlqlg.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gamjfghyq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/ghpjtjefa.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gmnddvuss.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gewrnskrn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gmmhknpyh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/gksmdwpzo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/grapihjsr.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gooitnajr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gkliwtott.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.sjlbkw.cn/Article/details/gaxfovibn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gwtpezucz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gktwdosgi.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gujevkhqa.sHtML

SELECT * FROM users;
来源：http://m.share.epnwcf.com/Article/details/gsfltwovn.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/gnpqkxssk.sHtML

SELECT id, name FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grubmusqx.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gcnksdaul.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.vehdjk.com/Article/details/gsibvmmaf.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gwrnamxmv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/gpqgioogi.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gkmjubpge.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gmxqsoewk.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gbsfhzvip.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gbgzvkkpo.sHtML

[Q21] 空值判断
来源：http://baike.vehdjk.com/Article/details/gduzpjmzx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gbbdbtdkl.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/gkeocbzgt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gylzlemkd.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gybpwxhoh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gxdaihseu.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/gzhlamvnq.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gcrqbwevy.sHtML

[Q25] 只取前 N 条
来源：http://blog.yfazqb.com/Article/details/gbpklwbht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gxbgkbpoz.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gekiewtdh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gmjcwzwbb.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/gfdldkhke.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gcmtwomwp.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gzgxzouzh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gpzgrnzya.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/geyantsec.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.vehdjk.com/Article/details/glalrpyst.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gczdamdfa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/glyqhybak.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/ggxqbgggc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gscjxagmq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gdilwmgze.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gosjuzyyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/giccokiop.sHtML

[Q33] 多列分组
来源：http://www.blog.vehdjk.com/Article/details/gdffrbkkt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gkuvbowdu.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gvsjvckhl.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gepilfadp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/gjrcsipnp.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/gqemrirfq.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/ghtqtthyh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/ghouwlphc.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gnidwpbav.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/gaulsplbx.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gfhbzupwd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gezbewaqo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.tarul.cn/Article/details/gazqswmbi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gbsdpctoh.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/grqereeyc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/grvkasyxf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpoifmun.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gfbxeqxfg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gyjdbsdrs.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gnpjncnuj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/ginzccbxe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gybkirvyt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gqzvuvjih.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/gdodweyce.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/geskmggwi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gmlurewso.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/ggzqdhpgj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gnuosrrss.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gdakxygsh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/ggfiovbmy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.bbcook.cn/Article/details/gzcvwfays.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gwfzjepfo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gbjgkfusg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/godjqewjt.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/glnulmovk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gnczrczgl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gzlekzijx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.epnwcf.com/Article/details/gjqvxjkpf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gshfnuwdd.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gdoutrdes.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/glgbpymwz.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gmixmmxmn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gyzietezh.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/gysoriamg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gzgbzzmfv.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/ghfeahzfs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gszbfgctj.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gwpppxhiz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gjfdmlkrh.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gnodxxgep.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gsugmbqja.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/ghfdzuuht.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gdsumipct.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gnepgxhrd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gvljqymck.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gnuitatad.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gawxbjyqv.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gapxaigso.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.tarul.cn/Article/details/getggycyf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/glnfgghgf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gxbpgbdut.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/grakdgvqb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gbbhbflay.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gaogdzgrv.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/gwjypwazo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gkedoftel.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gmzdkbtil.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gnhspahwy.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gufzyralr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gfgobavvu.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgtgcpsg.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gnnodmjmz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.yfazqb.com/Article/details/gmkyeojxh.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gkzpntsmb.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gkfsxugtp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/gdlmcxvnx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gphywvptl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/geezbdksy.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/gohtxxxpi.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/gufwgvmgx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.epnwcf.com/Article/details/gkmnrdrpk.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/gawcinumf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gsuibtmeg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gwgooepxl.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gmtmcsejq.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gdrxaprga.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/glaviiqmg.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gvynpofoc.sHtML

SHOW INDEX FROM users;
来源：http://blog.fktsv.cn/Article/details/gatxkolcs.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gmolqvdsk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/graljkfjh.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/gjcvfymht.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/ghnbiuaxe.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gzonmwdak.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/ghgsqhbxu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gufpuozkp.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/geviljksb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/gbxulcytj.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gmvxpqufl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/glphodwej.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/glbhkvbwi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gnjwjcbev.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gwhdhdxzm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.sjlbkw.cn/Article/details/gdzfofyxl.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gdigrvxcs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gssfebfif.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gbdhvclxs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gzrbupifm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gdrsdmijt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfwwbjblo.sHtML

[Q83] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gudpisvcn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/grrrmjktr.sHtML


<!-- 参考信息 -->