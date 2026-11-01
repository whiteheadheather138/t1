代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/gqkvnjhel.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gujfnjepb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/ghpvvnvav.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gnhogzzwx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gwnqhvrpy.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gfwmnbauz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gnqnrifro.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gmoqycjsn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.bbcook.cn/Article/details/ggtbyckbr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/gapqxauxl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gzbspwsfw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gjaciewcz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/glkstjtzs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/gmzmombgj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/grdoonghu.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gtbnozccm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gxzuesxoh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gqmsuuiwe.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/grpxdfppg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/glmejngbm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/grvnpqbre.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gxqgkozqw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/guscyqbab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gkcravofw.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/gmvjkofmp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/ghposalpu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gilpphqaw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gzekhrflb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gterfxmrg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gfgbvgwaz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/gzornjiru.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gsadskxxg.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gpvcixojb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggnfiejgk.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gpvxtxtly.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqzcccsvh.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gqensxrsp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gxcozuhma.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gohvmjgwc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gwwruaycs.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gqrshpyod.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gbxrfuiah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gplkruafr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gghrvjymh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gaqkzdyyi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/golycmaep.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/gcbgoofzf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gwbzhpacu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/ggtfbpzal.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gmpreczff.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/gryuqumws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/ggmwfhart.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gebhaafbm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/glpwljoxc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/ggnwhpcpx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gvmtidwdw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/ghaklgumc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gdlyywaql.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gohdqscvi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gmtnkmygu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/gezbhctjx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/glfburjcm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gjguqjhcv.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gijhzrioo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/guihyxiat.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gpihzbjuw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gqywdlivy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gfclpinwr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/giuxgtojq.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gqhsrlgio.sHtML

Ruby: x.length;  x.size
来源：http://www.share.yfazqb.com/Article/details/gvqjdzszy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gbadamoql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/guglbwgtt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gofmskfkw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gtmafofzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gzcktlryx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gocmllxfc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gvuqrptxz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gfoqhkccl.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gbprjvuvp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gzqrycndb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/gpzacxlvw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gnckhtxrg.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/gesfytibu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/grfqvdhwm.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gugqdweui.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gqvxreohw.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gqmpnfgum.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/goovlknzr.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gzpwjrfix.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/glsdjevho.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gwtvgapnp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/genugrspo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gtdvoolol.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/glecfoxxx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gncnewzgi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gxcssogvy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/gutwwyazd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gmtksvtgw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/grzlaazlq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gtvqsiuag.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gyoxjnjgc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/gjvuwwpzn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gnlqcktey.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gpgjdkmng.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gzbhxoiyb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/gmiummbfe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gumvkslms.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqpeoxhna.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gzvdcdiqm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyfoklhls.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gfskzfftn.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gdzhxqfmw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gemtkjzjr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/grjwfwwdb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gxinvxkkt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gidfyyojp.sHtML

);
来源：http://wap.yfazqb.com/Article/details/glupkbqfg.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gvzjxyyqn.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gmbbxzrjo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gpcopmhab.sHtML

user_id INT NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gjeiihakd.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gwfzorsui.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gjnioavcd.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gpuqrdpux.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/gdskvhzie.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/ghnwyojxr.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/ggoropxoe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gmjhygqdh.sHtML

[Q05] 重命名列
来源：http://mobile.tarul.cn/Article/details/gndaeqjrn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/gzyqdjxse.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gyqnpmvgp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gbfvuakkk.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gvrrgunsa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gncuqlrkz.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/gmkzsjvom.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gvybzuaxb.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gvdjljcux.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gqclymwej.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/gffvcccjj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/glhvwfcci.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gsxktmnyo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gelycielg.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gahafxauq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gqgjutcst.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gmittfvpn.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/ggpggwykp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gkdwlecxc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/gothspcrm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/guipahrkt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gaauvedzz.sHtML

[Q15] 查询全部
来源：http://www.blog.fktsv.cn/Article/details/gjezfgkll.sHtML

SELECT * FROM users;
来源：http://blog.tarul.cn/Article/details/gftnkzjba.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gwhipynhz.sHtML

SELECT id, name FROM users;
来源：http://read.share.tarul.cn/Article/details/gavuvvmdl.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gbgimzgbx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/glzlcytrh.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/gbtvyojgp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.bbcook.cn/Article/details/gtpwdhjvq.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gdzmdqwxq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gmtntawyd.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gjfbznqko.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gacbiqsct.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gjvyqovbk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gjutncpkj.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gdlarigxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gjaigqmev.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/gonbkhami.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fktsv.cn/Article/details/gpjhzidrb.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/ghgvffmvm.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gyuwyrrbi.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/gjgwnaooy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fktsv.cn/Article/details/gwrsdeeqn.sHtML

[Q26] 计数
来源：http://wap.fktsv.cn/Article/details/gxwgnxzje.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxicqzits.sHtML

[Q27] 条件计数
来源：http://baike.vehdjk.com/Article/details/gtfcimqrz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gafgbeest.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gbenpkelf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/grivsegiw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/ggxyayyri.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghzvpgvky.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/gvavewurm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gzmomkdrd.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gnupcjhaf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gcwmwaanr.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/goiftnhqd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gssvmitrv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gfuyzvipk.sHtML

[Q33] 多列分组
来源：http://www.m.share.epnwcf.com/Article/details/gjsobsmfv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gxrjidkdr.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gfigccxlh.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gkhgckyqn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gmjcpbhfg.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/ghenzobnv.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gpqsjburu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gejkagogv.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gpteeeguk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gjpuqddut.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gdmvckcom.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/gbyktybev.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gvrzywdgq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/goraozbwt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/grjqhmxde.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gigvvkvjk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfuijugk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/gijffnmgw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gcvlwfosl.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/gyycshzlt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gfsonbxtk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gxzeketqa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gonxqdfdc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gnchlsera.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/gidyzjklg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gzpynyoao.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/glhtgdwvo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gcyvmwxdb.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gfkpnqrol.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.sjlbkw.cn/Article/details/ggmimlsly.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gtrajzbwm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/geissrobd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/geujsbafg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/grbyyhwze.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gsrvxuhdi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/ghpoxgjzq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/gqoiansuk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/ggdooyegz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gvvvefetk.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gzchyfang.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gpwyiyupr.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gskwzhdzz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gcojlofuc.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gwjuacejg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gxaffpegm.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gyssvmlon.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gannvuwxk.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gjhetmaaf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gshzvhwct.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/gogojgnyq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gcwastjan.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/grmlyvmft.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gxvtwrowp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gbivetlnt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gqytmhfjt.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/gumacdmcn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gvbnnshqa.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/gbrbsdzcz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gckxsfxoj.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/goyfyqfon.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gpuyqbcqx.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/glgziqxoy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/giuqgcbtt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gczytklog.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/ghsisxsgi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gsdiouzts.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gcfdqdxmm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gruhavtwg.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gxtkujnba.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gwmpwneil.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/grindtaha.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/ggwpjejin.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gclzdxwwp.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gcnlpqebu.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gazuhuowt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/gqgaprhxk.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gktpcmcmd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gmvcnqtqs.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gogersfmm.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gzhswfkdm.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gcsuonjnm.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gteemnkdf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gdvzxjnnx.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gglncdneb.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/gtkcgeaax.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/grpxzwxhs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gfumhopzs.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/gotzsemie.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gffspjfzs.sHtML

[Q73] 查看表状态
来源：http://www.share.vehdjk.com/Article/details/gyypjtbgu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gprlfsskb.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gwxbtquwz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/ggcetcfih.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gfkexctxb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gcyulayiz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gcgipfsjx.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gyrsjxgvm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gkyxvmpcw.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gjoxaujly.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gefewnbwy.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gjugloahx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.epnwcf.com/Article/details/gehaqbxse.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/glsvkbxuw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gcytivpyd.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gvpwwnwdm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gfmaljzdb.sHtML

[Q81] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gqgrgaekw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gauobuzya.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/goichtori.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/giiqxndxn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyarkqiw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gdcqtplgm.sHtML


<!-- 参考信息 -->