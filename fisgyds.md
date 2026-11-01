代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/gjceomehq.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gekiuyran.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/grjvmunmm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gqjzufatc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gyhdegapv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gkbmvectr.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/goarvhfxd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gpwljtflo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/ghglommxh.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzmmkoheb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gbgkmbllg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gelraurtq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/glmwzrupm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/geyohocsz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gbbfuzxzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gfchmechs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gihecyfcm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gvgrtbnip.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gqzaspbha.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gsaidqzdo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gaxzqnbxo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gkgpzbyyj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gaxdcjopn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gnijjnvgi.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/gurmlmkqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gbcenlybm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/glkbibanf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gjuahzoil.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/ghfrnwacz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/ghiasgsqn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/gwlfpwpuv.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gdohxnvdw.sHtML

C#:   Parallel.For
来源：http://m.share.yfazqb.com/Article/details/glnudsuyu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goletwtqs.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gtprgqeed.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggfmiexuh.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gtsvwqwfc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/glhahudxr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/guwhlaqft.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gnyilczit.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/grwhwwjiw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gphfhbfwp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gxgbecebr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/grjdmykgg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gcamnwkks.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/glwtramjs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiuoevxg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/gutpdcwyd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/gjaytonhg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/ggghvlcja.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gklfrkhyq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.epnwcf.com/Article/details/gwezqaxfq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gdyohpsbb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gsvsacoyz.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gporijkqt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gmmleapns.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gvibhwsvq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gnsjxsmau.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gckogrnri.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gwekmvusa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gkdbdhbft.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/gdnslvwtf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.yfazqb.com/Article/details/gjaedliid.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gacyffslr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gtmlmjdik.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gxohdbxki.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gdlqqtdhs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gktrhbgez.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/gbsbonyqn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/grfzxftrv.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gdkhqjtzz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gccftmhuc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gjajesdii.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gbiwmtoea.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gtllqnuex.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/giblntbjk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gsrsmirzb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/givrfnsfj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gdfaxttel.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/guotdfxqh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gekpwzzeh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gkwueqsbd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gjpwimovs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gpydrlrqf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.tarul.cn/Article/details/gzeiuhdau.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkrfdpqdf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gapnownbv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnwdjanw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gbsssumru.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfxhybndc.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/ghkfbxgvk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/ghgdhlewy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gxhkfmfcc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gwxgzfqhg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/goffecqay.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/geiwfarpg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.epnwcf.com/Article/details/gsnrhzpzv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.tarul.cn/Article/details/gqkdbcavy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gztoaiqmb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/grbzbkxeu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/ghcfzplwx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/gxqyfticg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gjjqdxhtf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/giruglrqo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gxtoboyuc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.vehdjk.com/Article/details/gprxirnsz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/gpkanxqce.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gdjeeqdrd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geingwxcr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/gavvcqcav.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggkpdkhhe.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/glzaznwqv.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/ggdmexxcy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/ghobjnnoi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gcyupmryz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gexewunkl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gczbgumpp.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gqbejvgfz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gsxdypaug.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/gzctilsck.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gxmclthho.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/giygakxcq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gzkpawpcq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gwvnlyela.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gvqcganpf.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gdtmwgwqo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.tarul.cn/Article/details/gsstcwvxp.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/gfxicooju.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/gixqyelzn.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/glhpvhdnl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gfezvgqmr.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gpwbgzvwo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gvspqigkx.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gpthkyuei.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/gmoibipyk.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/gkxmkched.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gkwwbqgiq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gbwcyybvo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/ghuxrqvrr.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/giwzhrrpz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gfrgwmuii.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gzikdpbwq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gbmbcxewz.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gajuvzzys.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gocsasjny.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.sjlbkw.cn/Article/details/gkylmmzif.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/gehxtgavv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gnmzqbqfc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/gkbqiqppk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.bbcook.cn/Article/details/gxjgmtcsy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/glcmkgunt.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gxifolmsk.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/grrrtirvs.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gkcicdnfl.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gnvuhmbbg.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gjsyjukqh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/ghmlcpxno.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gedkjxrzg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.epnwcf.com/Article/details/gwulbxswr.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gnfgthevw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gmewcyqsw.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/goaqkdfup.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gykzedqsn.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/ggdgzyuaa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gezltasdo.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/gglnqibnv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/galigrhov.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gdccuiavm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.epnwcf.com/Article/details/gkgwvdnvk.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/grzavihod.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/govxpddet.sHtML

[Q25] 只取前 N 条
来源：http://read.share.vehdjk.com/Article/details/glerxlhsm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gxkrtgrnz.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gdsgrvedp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gaastggkj.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gpwetfkxq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghbaalhyr.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gitvltcbn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gzuwrlefn.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gmidozrmf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gugzxpncp.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gjydphszs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gyfvrffaf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gaqzllmno.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/gfnwqtlro.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gmxuqmpmb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gkcwtzffn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gmugwiizc.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gfzcioiox.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gnjilcuvn.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gtyywksgi.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gptjdazrz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/ggexlyyfe.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gcnqazvgp.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gbjrjnwfa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gjrgnliin.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/gnfqqroer.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gelnmtgep.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/gbhfyyriz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gnvufsmab.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/givhcbquz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gzfslljnp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gdcadzztp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/giiwmhlqq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.sjlbkw.cn/Article/details/gyoamvrsb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.yfazqb.com/Article/details/gljqiruci.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gqltgnigx.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/godzsduia.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gsajphjsr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gdnegsflx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gucbvdliw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/glkcofcry.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gxcpgjzuc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/glbjhaxdh.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gjzjtvzdh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gbistesfk.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gtondcrrn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/gterfpjlz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gbgauoczy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gbgylbbut.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gchadmkjl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gkodhxqro.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/gicrlhdxo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gsiytpcdd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gfmmttaxi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gtylkodju.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.tarul.cn/Article/details/geikhwazx.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/gtbsyxeog.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gvvwmzzva.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gnghlgzzs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gyokfmamc.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gdolpjvwo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gnndxlorw.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gpdhxgzwi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/ggnqbdfbb.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gpdlcqqnp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gigxrfdde.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gsgeexijy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/gnuxherqr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gdimbnytj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gytefufyp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gpxfytqjk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gsvsdagwr.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/gkxxoffgg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grvegbluf.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/glrbibbmt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gshkzfugt.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gilqamaiz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/glqkntmxe.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gjxbbkgrb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gjutojxya.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gicpwvcsp.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gmcnjmoxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gliawztiw.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/guenestvs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gcyggqcje.sHtML

[Q63] 开启事务
来源：http://wap.vehdjk.com/Article/details/gynmhwagn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gifvxrpqt.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gjvnzoylm.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/gkbhhwiui.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gezsqaadd.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/gvcmegwim.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gcqnfjljl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/gxceuvjzz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/gpbqqhxmb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/glbemenfp.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/ggesbdske.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/gjbcwrfnd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gvstabnow.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/glwhyxied.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/ghackcdii.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.tarul.cn/Article/details/gbzuwrfzs.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gjkmezban.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/gwxxgqclg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gqottaktw.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/gzysxgqmz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gbftxdihv.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gnitonulc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/grrzlizfe.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gbwhyroqn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/guufbwyal.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/glvuxcxyc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gnarwtwct.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/ggphpgbkx.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/grupktabp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/gziprnhlc.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gfffqakgk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gfdugdidi.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/geadgyxbe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/gwheripxa.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gxxgoivfn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/grvklzwfr.sHtML

[Q80] 字符串截取
来源：http://3g.yfazqb.com/Article/details/gjlipbgia.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gqkfmoowx.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gupeuptkz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gzogqdbwt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.sjlbkw.cn/Article/details/glhxnbvht.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gwakkzaou.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gmkgzygpa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gmtqtkmzx.sHtML


<!-- 参考信息 -->