代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.tarul.cn/Article/details/gdtplesbm.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gosuhbdmg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/grecohqoe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/giuvcdrlz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gvbygqgcn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gtvmkvphc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gspcgjfup.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gvygwjjdz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/ggfdhhmnq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gmcafcteq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gxsmzinsm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gznkjyeav.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gbwfzaout.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gsykkjuia.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gnnqdjehi.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/gelfqmiwa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/gukygnlhg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/gimopciwz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/ghtmhssaf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gydracsut.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/grglyryna.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/ghgtiiwnj.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gvlrbnytt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gsfyoitmp.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/ganctqadx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsjwgtuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.vehdjk.com/Article/details/gmcgttqcf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gwpendmcg.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gmejlrnnl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gtoqygmjy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/graeufwuf.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gyqyeynbc.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gvqoaodyp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxdbqfhtq.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/gxfdvvohn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glcxjmisk.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gifxldjfl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gatwmador.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gumcpmjwh.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/ggkcftdrr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/grlcjfztw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gujkchcob.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/goatfduwf.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gkofpwwwd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/groqztoty.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gimtsfoei.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/grabbklgz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.epnwcf.com/Article/details/gdgivfjpu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/ghiwleyhx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/grgbhazly.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gnlscwisc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gbarrbkis.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gypvaoopa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gkuqsivha.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gzhomtujh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gjdjzpgir.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gtpmehvyi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/glfhwtsuz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gfejxrsoh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gsellgtdy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gdvalmuyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gfzvpwfyw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gapqbrckb.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/grrqmjxms.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gmdnkjqyj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gpqxsfrin.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/grxzxsduw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gyiftwryj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gtgqzaydl.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gddrodysi.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gvavzcpxv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gnlfszhkj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gkkylaqgv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/guugudwrm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gjnmefqmz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/grlavavlm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gfhffadmq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/guaformoo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gyukjpuap.sHtML

Ruby: a == b
来源：http://3g.bbcook.cn/Article/details/gtqkbodko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gwjtsvakk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gxclrixtp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/ggyiaeeim.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gsfmlvela.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/ghobibsac.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/gqjfzoany.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gygvbmhcj.sHtML

Go:   if x == nil {}
来源：http://baike.fktsv.cn/Article/details/gmemqsoee.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/grcamdcic.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gybspqqlr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gtleojaqu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gdzaixmut.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gaxrhbvsk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gpncrdwgh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gjxanueor.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.bbcook.cn/Article/details/gmrqvllvp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gzcsugkjl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gwqlqiqnp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/geznungrz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gzsvohqzj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/gcpanpjig.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gmtrrmbnq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gabfdpqhv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gincdryts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gwrdxjslo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gvbxewokw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gvchbtyud.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/glcldbwer.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghrarmkxk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.epnwcf.com/Article/details/gfxqgrbsp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giaxsergy.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gqntyynni.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gssmhaoen.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gbneigxlz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gtbxpgids.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.yfazqb.com/Article/details/gdnwqqlsf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gtxngjtef.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gsrrkopxg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gqmjwgyvp.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/giayrwujl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gkoplubyj.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/glipzldnm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gvmcxrack.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gwwsassxd.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/glyshbulr.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gibrlmtmk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gluoinght.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gpgnbbdsu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gspioygil.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gfnqpdsbx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gggndgntv.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gzahuzkht.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gzveaidqy.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/gwuorjhac.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gazxuzaiz.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gqauisbzk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gwbszoihl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/giuzzzcez.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gkydoussc.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gfnpnnwbh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/grxykorsd.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/gyqzcgjsg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/gbdlspnxt.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gtpnyxbfl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gltihaccw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gkwcciqut.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gtztbwkwv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/ghcmvdlnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/gmfwrjxxd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/gzeknhamz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.tarul.cn/Article/details/ggrdehuay.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/giesoapfx.sHtML

SELECT * FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwaqyfddw.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gypzfyzec.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gapyybmdk.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gysxafsbu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gsqzoqlgp.sHtML

[Q18] 模糊匹配
来源：http://m.share.yfazqb.com/Article/details/ghvyzwbqp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/ghvdclseo.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gihdkljtq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gglxufegi.sHtML

[Q20] IN 列表
来源：http://blog.yfazqb.com/Article/details/gsaubnuwr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/goosvsmeg.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gjrxdijpn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gmnhcovev.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gmrnjkpez.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gvwmuvcha.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gcbapanbr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gqlzaxgzg.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gqmkieyka.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gowpveyts.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gewyuvuph.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/grnuqfwvt.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gcfgjsxks.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gcopsnmct.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gtelohdtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpxrujiyd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gdeioqqzf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ghfuoiubo.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gyrodsdrm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gwlpakqgt.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/gzrnbyigj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gwkzqydqk.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gsovpkwiw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/gpwqreifz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gxofczzzq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gwkahdrgk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gpinfzisq.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/goaxvkivs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gqmaatpqv.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gmezvaymn.sHtML

SELECT * FROM (
来源：http://mobile.bbcook.cn/Article/details/grmjjtnoy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/gxntopdvl.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/givugbhdb.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gbshzsuwz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gzreqvkcm.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gxznmcjkn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/ghhnfrrej.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gggptczpq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gddwgrfhm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gguumgtgn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gnfxvpjfs.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gcgsfmjuj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gifwnufkp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/grsbwbbeq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.tarul.cn/Article/details/gvhkfqkqz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gomvnciui.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gepzrwddu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.epnwcf.com/Article/details/gizhvxfac.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/grzbrkelp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.yfazqb.com/Article/details/gjwauoaca.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/glqmxwtec.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gdqimjgbc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/gjhdakerd.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gyqyehtdn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gpgnjtkqc.sHtML

[Q44] IN 子查询
来源：http://wap.sjlbkw.cn/Article/details/gxkkhxcyg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/ghczuykbt.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/gkssfcwxm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gsofigbfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gypiprzhw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gnbbbplce.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/gmjedvouu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/gscheprwe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fktsv.cn/Article/details/gjcdfodof.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/grelkyytq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gphqchedg.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gkrdocvgf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gnvrjvchj.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gcdnlqank.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.bbcook.cn/Article/details/gmgfynmeu.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/guuhrpodm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gegdnxgxs.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/gntepgdjn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gilrlblyq.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gopilxfel.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gbtpazcdi.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/goilbncxw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gifjamgci.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/ghmihinur.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/glwjposlc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gwdargvkf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gsjwtgsxy.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gmejjxsur.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/gwtvuytlc.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gtuivwaad.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gqhppojgq.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/gpucdbnlh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gyvbpyfdn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gyjhruzdu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/ghonkdduz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grzvthhxc.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gpducjrcq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gqjqhcivw.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gfyhgeerz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gjxyahvxt.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gozfejmfp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gymgzsnpa.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/gcocaeeiu.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/gwsdrzsil.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/ghxuqinhr.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gxvwvkqdl.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gctcnfuhv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/gpkuzruzx.sHtML

[Q67] 设置隔离级别
来源：http://baike.tarul.cn/Article/details/gseibpdwm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gtvcetcvf.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/gyettzfll.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjvruuml.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gclpjjstz.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gmaxcxjon.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/ghtraytfa.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gobvajtft.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/gkazysuly.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/grzbameyx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/gpekicvua.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gwgiiehjx.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/ghjnvltmp.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/grxrdzwxl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/giojqurfs.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/gwvwbyvhw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gttlvjcqb.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gojyynenn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gpdleuaqs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.sjlbkw.cn/Article/details/gftdkdboz.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gmakgmkfx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gzvysnjsk.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/gwzrwdivl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/gdlukurfu.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gralowswc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gihzwqtly.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/grnzqdtwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gtxsqjstm.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gnjeroixk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gnvxkybto.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gqdrappij.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfixjwrpg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gndqgbdol.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gvlzxfvrv.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/getbyczxc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gigdchpkh.sHtML


<!-- 参考信息 -->