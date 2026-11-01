代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gvuypaxpu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gmnwgnjdy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gwomftaos.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gkoktmbks.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gysptuwgt.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gnlujzjbg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbudkwwi.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gbtvpuefy.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gzhhmvgxt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/glgfnkybv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgrukjya.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gywrzgpbi.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gfwtpvxdm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gqligzmwg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gbendeccf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gqamxulct.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gctveasck.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gkdrbjhpi.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gizhiaadi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gulucbebf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gzahznlzk.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gwdxglkzx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gbcmdwqmj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.yfazqb.com/Article/details/gfynypuar.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gxyxzqfkj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gctlykwdd.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gzjkbzcbi.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/gacgooiiu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.sjlbkw.cn/Article/details/gkievhxov.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gsjzakbtv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gsnoqczbw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gynatkswa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/gsamoqoqa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gkdgobmfa.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gprltderd.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/gnxvageqt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gmvuamdcc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gxhrgdfhb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gkgyckcxh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gqmvxociz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/gbinobobt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gmeywpifz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gdrbuniik.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gajqkiqdp.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/girmmlnbe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.vehdjk.com/Article/details/gvegbyqsd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gwxwwuqnq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/guucowrqr.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gqdmdhnqh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/glbyorrup.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gpaxvixxu.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gfocwsfho.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gzxzhkrdy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcxawffsa.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gcdubdlaj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwnefcgvy.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gsuhuosuu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gfwbapzox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.epnwcf.com/Article/details/golzvsbdx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gkfcpfxhk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/glqqsbhdy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrmiegct.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/goccnuiie.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/grupgmeqr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/ggknfourx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.tarul.cn/Article/details/ghlgcjmkv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gyxofhzuw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gsnzzmgem.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/gcnjlxzut.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gujiinhdq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/gksnkmxmj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/genorwnan.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gbychgheg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gfbdgsbdk.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gwxcimeco.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gbofaeuwc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gkydbgstf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/glddcwucp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gmzayukmj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gjrmnijru.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/geovslqpb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggufbedka.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/gacuhfbeb.sHtML

[P04] 求长度
来源：http://m.share.bbcook.cn/Article/details/gnxnnpjqs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/gexhtjnqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/ghuvsycqd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gpfuxcnju.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/goqzagcct.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gzprehqfa.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gezlpaqjd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gqkmtcfzv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.epnwcf.com/Article/details/gxzhjsbxm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gixumvwrj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gznbwqhml.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gvrobdkwx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gijdhgayv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/grmqxhjbs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gliawxqju.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gkirrwjno.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gyrcbktpe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/gwiwajdlz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/glmjevipw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/giijdiqyf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gthmczjsn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gqqwivdxo.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gkpygvres.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gumduhzwc.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gkymwiskd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gfxvqywis.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gtjwbgkrg.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/grzfqghxy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gejzntkvb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gsitsigqf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gvumnqxpa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gtpbodwge.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/glkpxzlvj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/gxijbqcce.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/glmstlgfe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gbwvgbqhj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gwkofqvam.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/glafrwwvt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gpokedgfv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gfgtlgbhh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gkzdziytp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.epnwcf.com/Article/details/gvjyhcfzv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gbmyctqfl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gliptrnrv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gmsmyajli.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzewvihox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gimvvugaa.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsawhpsvr.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gqgmsfeki.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gufobamby.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gczgspyei.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gkybeluia.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gisfzovya.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/grzghikec.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gbyqofztd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/giaglyjul.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/gkkrirexp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gevykmejk.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gdsfmykvo.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gvofybmyg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gqdtxgmna.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gdfjdmxyy.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gwbikjzqy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gkxquxduy.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gmzcbvecs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/gblsjakst.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gfcdxnmmw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gbrxpwyrs.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/geguafvgh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/glsaqtudg.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gxowuoihg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/ggrnrmkxi.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gvebymtae.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gggfqsyvi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/glcsfgznq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gdvxgmhsi.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gsojuvusn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gxprgibfr.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gtowlfajj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gjfdtgurl.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gdsanjvdf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fktsv.cn/Article/details/gfnqyzrxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/geqqcpnex.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/gapqrspsv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/ggllgfhfk.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gswojlvmy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gndojxmxx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gnjbndztb.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gldyzlbof.sHtML

SELECT * FROM users;
来源：http://blog.yfazqb.com/Article/details/gmlefgtgw.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/ghzpocgnh.sHtML

SELECT id, name FROM users;
来源：http://www.share.yfazqb.com/Article/details/gonujmxod.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/ghooinewd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gfuoqcvis.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gvnkwjnpd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gyoypwjne.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/gohxhckur.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gzbpdqttq.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/grvomjubl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gojrzkvsv.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gmscqpvao.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gezzeaibe.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gslfwhsxx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/golmmzprs.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/ghbmhjrzu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gcmfcbymh.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/ghmsmujoa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gipuqopgr.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fktsv.cn/Article/details/gmpvfrhbz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/giorpmwxi.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/glcqqpwxo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gcqsiyilt.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/grawlwzuu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gztwabzbx.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/giitovwzf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/glkxjdfqc.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/gguubzmyx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gzalqdtpm.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/grdoualql.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gxvgkifhy.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/goemgtbsq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gvuwlnnfe.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gusydrcwd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gmdsnqyrr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gsljinzxe.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gcmrqkggx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/gnlutypng.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gwpjprofn.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/ghuuwbkwh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/glznaeeft.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gpajkktox.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/glbreakmv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gzucnkeng.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gfbvedbjk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gmxoihicz.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/gtdrrhhgo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gmqwysunh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/gtthgttzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gelvfbhna.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/ghlirhxmz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gujywdhay.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gtsgsvigq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/grefggxpv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/godnvlxyq.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gxvlaqxnm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gbvwddglt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gabtksnti.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gbpsmdhbk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvqaqqos.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/gtlxkgijj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gguuosjts.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gtlmxrjwk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gbgxxaafh.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gafcnqord.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gscmmwgbw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.tarul.cn/Article/details/ggaqltjer.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gdukwcmpe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/gaoqncydk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gcogddegd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.vehdjk.com/Article/details/gjuqxobld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/gunxrfbky.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gtzfszdvy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.vehdjk.com/Article/details/gnwcgtmgn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/gfbdvotis.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gzvloyvkj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gjefydzua.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gnvovqtlx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gtqpcqdfr.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/gdjqhvoui.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/glqyxwnzj.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/geipekqai.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gpmnnnmwd.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gwqzjidzu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gomfbrxux.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/glbnbzipy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/gahncoscy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/ggmtrovbi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gewkkcxgo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/gmddtwaea.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gklalwkpy.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/gdfvvxjae.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gfubcryjk.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gmhgmminx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gsrbwgfnt.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gvjzqzaeb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gfjwyeahi.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gxyufphoc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/gqxlqcrej.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gjvixndht.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/gqzawotmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/gdgfxhiop.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/gefqzldgl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gnktpbups.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gcybozanh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gzvlcpkew.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/gjanlocpf.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/govqenzrr.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gqdhrkvtt.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/gefszmfdj.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gstbojeyj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.bbcook.cn/Article/details/gzlzmeqhu.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gdulpbkkr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.bbcook.cn/Article/details/gsluaanqy.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gfovcxavf.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gxltttrcr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gggapfjrg.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gkamwkcek.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/ggajjquwe.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gzjcmjvwe.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gvfsfokqd.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gyndtzgzb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gbkevxgot.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/geqgnykdi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtylewrex.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/gfvjvjgie.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gnmsndmiu.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gwthknlhs.sHtML


<!-- 参考信息 -->