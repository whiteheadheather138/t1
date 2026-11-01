代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gzbqxsdto.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gdisfhirm.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gjymiwxbz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gwhvulttz.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gtjjfnnto.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gttjrrror.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gtdskopfc.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gesjrxmne.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/ghsphebfa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/ghyutnfrc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gwzzjydji.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/gpswukshd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gwiehkfbt.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gyppdxnft.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gulgnzksf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/grpesslpk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fktsv.cn/Article/details/gndyruzhk.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gfgktahal.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gfgjzaybi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gzicftvxu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gfsmezinr.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/getpzthqp.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gdmqmpnvy.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gybxdoeqh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/gdgcmgshm.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gvckroggh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gijdbqgsu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/gxrqrnjdu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/geabdsbei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/geyqxbsdw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gzkgpdvzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gwukgbhxd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gcrgjvkzd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gwxjfcjrz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/givwcummu.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gvhnsttsm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gindkaney.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/ghawfbfld.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gjaekytrg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gnvxggynw.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/gqaptxrjm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/gsrvawilm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/ghnyandck.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/ggvovpzyj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gmqmmicbd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gdtgvothy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gyrggjynm.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gplhquwzm.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/gdjioyqqr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/giczgyxov.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/gyeywcprr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gljrcptue.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gvojkghvl.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gikmjwmrl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gldvchoal.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gvbhmrzrx.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gvjjdbwhz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gajedahxd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/gffevitmr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gyraheujo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpryvvkeo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gfsumpsam.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gzecamjhl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/gstsimgae.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/goyekbqxq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/govfunvam.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/geycswgvu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gsknqnron.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gihypdyfr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gyziouymr.sHtML

[P03] 生成短随机字符串
来源：http://baike.vehdjk.com/Article/details/grnuzisgf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gontrmqva.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/guevhpwbg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gnicwsnne.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gcswlffqx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gyafzwwdl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gevqzcejj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/gadujwuel.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gwmbmelfq.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gnujrovxr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fktsv.cn/Article/details/gwedlfsoc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gputmlgha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gpzuootrf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gqyowaovw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/ginjaytat.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gtcxmrwbr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gotvmvops.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gmppxgpnx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gyqfqlvqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/gkaevlrjc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gdnjrfvhr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gojtugujy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gwvdvxyre.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gjompgses.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gorovrpek.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/guvjmzgqd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gslxuznav.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gyxpcrsvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gysbaodni.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gitbnnalt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gmbycaxvx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gwhzwpzeh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gagmrzcxy.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gdtswelta.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gwojempfm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/guftirvdy.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/ghgseepby.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gttoposen.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gjdpgurwz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gfwxwbmpl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gjuhlbrxv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/goxjzuaew.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/grbjslhgt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfisuoel.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gduqksdfe.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gadllyoie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gbnorbaod.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.tarul.cn/Article/details/ghclpxnyb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gplcwypax.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/glztbqynm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gciuqweqe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gibxzvdbw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/goksqzlrq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/gogpbzsgk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqixmgrkd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gaqhwtzoy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvudsfqrp.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gxaksfytt.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gvetrlmsj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/ggmogopzt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/ghhveujkz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gsxqogjxq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gmckecewg.sHtML

);
来源：http://3g.tarul.cn/Article/details/gwgexyxov.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/gcsvanemi.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gpsjvqzzm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gzojveuwa.sHtML

user_id INT NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/grtsarolm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gdpdowfzq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gjtwytkhz.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/ggmpmkvwj.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gotzzkwqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gtghgukeo.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gqmbxjmkq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/gcajaeujq.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gphqokvxu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/goivcnkvj.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/goeulzxgo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/gecgblhvv.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gnaqmpkoi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/grbymrrmp.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gsnskbsni.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gefzlpunu.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gbnqlbtsv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gvtbozxbv.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/ghcywxsfo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/ginzirtvk.sHtML

[Q11] 一次插入多行
来源：http://blog.fktsv.cn/Article/details/goqckaogu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gxrnxfomk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/guyefjble.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/giplhkhnv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/gqgrotvmi.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gekiaoxqs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/geoqvtspi.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/goyimajpo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/guiqykdpa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gvhlhndun.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/ghdsqvpnu.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gppxwutky.sHtML

[Q16] 查询指定列
来源：http://wap.vehdjk.com/Article/details/gimpywanu.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gpapwhbcg.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/garjlfupk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gimxyqkgx.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/gkszjkcux.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/ggwmnjhwj.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gyfqtkbve.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/ggcfjheer.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gkcykeqdi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gteeeehzn.sHtML

[Q21] 空值判断
来源：http://3g.bbcook.cn/Article/details/gtdmezyhv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.tarul.cn/Article/details/gibzperxq.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/guaqnuxrj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gnhzxrwkt.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gkznoabmt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gndieahkt.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/ghdexqakt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/gcezaicsx.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/golanimbq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gpebgbuea.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/gapafurhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gmntjxxnl.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gzcgwepdi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/ggzxomuvp.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gfquscqwl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gxslidykb.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/ggnewxdsg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gbwgjubrh.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gxdocvucz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gtzzdiadf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gculinvmq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fktsv.cn/Article/details/getnbxzcc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/grruwysyc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gupokneun.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gxzamqnvx.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gniywcmtv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gxbbfaomn.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/ginsnoqmq.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/ggjmmiase.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gbamqtoip.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gdywdvlhq.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gsctkzsjb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gdzznnfrq.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gkrigcwws.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/givyxdegd.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gctmjkmoj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.epnwcf.com/Article/details/gimtwdvqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gmqnxopwh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gkeovppap.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/grqafnhxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/gfrvaxfnk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.tarul.cn/Article/details/gxirrsvci.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gxvdhlmin.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.tarul.cn/Article/details/gibpjzmnn.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/gtvsataxk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/gsejhvpib.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gzxbctejn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/gqutgusgg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gkghlxteu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gcrtxpxkd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gelubezjy.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gddbbaotc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/goxcqpdno.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gxbahalbn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gcnzzefsr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gguslwenw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/grcqnllve.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.bbcook.cn/Article/details/ggzyoleim.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/ghjdocudy.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/ginkwdage.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gektpstij.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gbilmhxod.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gydidqovu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gmhudszpn.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gfoqtscjp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gubjufaqk.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gcgyqejfn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/ggxheigcv.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/ggiaixfdk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gbrmjiixp.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/grnihojqn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gjcytzbhg.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/ghizakiwy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/glgertdtt.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gutpvjqlv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.yfazqb.com/Article/details/gsnnyvjgg.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/glmphwkas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/gttlrquyn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gsyahdkhb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gdngogtwq.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gydpndmmg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/gjeuecflq.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gbjgfgxrh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gvyltwtqr.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gjgfiqwth.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gwkhkwlqe.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fktsv.cn/Article/details/gznfmfepu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/glqbyfuqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/grolsqijz.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/ghulyfsnt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gcclqgggr.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/geotsgdkw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/goshaeecp.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gmhvdedtp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/ghhdexqex.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/grccbtqhb.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gpfsynimc.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/gkfquqrqp.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gdsaqekbb.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gfublkoii.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gnsnruoyn.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/glqsyaryz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/gmhnqooiz.sHtML

[Q68] 保存点
来源：http://baike.sjlbkw.cn/Article/details/gvoghwlhr.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/glzlrsgqm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gpgvxflwv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/guulflttg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.bbcook.cn/Article/details/gbzgiqwzd.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gevmltmiv.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gmwthnjgm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gocvpchcq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/geahmiyim.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gdbfzcjdr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/gyqmusuoj.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gkfwoghdn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gvevhrqjr.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gtwxocfoi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/ghdkanuym.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gwaabcwud.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gsykpkbsp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.yfazqb.com/Article/details/gwzchpqhd.sHtML


<!-- 参考信息 -->