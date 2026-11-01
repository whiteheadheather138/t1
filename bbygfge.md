代发 wailian999

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/gxontauol.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gbzjroggy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/glxmnaaba.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gwpsakmpx.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gihubtqlb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gegdwgxjd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhoiqlab.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gwojgnhcg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/grznbjjip.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/ghuzzdopf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/gnjweyktv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/gwyhpzvzv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gprffertx.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcvntxre.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gwxnbisrt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.tarul.cn/Article/details/gklgczvot.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.tarul.cn/Article/details/gockrjovp.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gmjqpclaq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gendmqwzb.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/ghotabguw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fktsv.cn/Article/details/gxrxvttmf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/grqvkonaq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gefvqmcgp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gprrlfczd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gvlrrlkoo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gdvcmysdb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/guyzucnkc.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/ggvssxnuv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/grugzuuhd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/ghtsfcxnp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gtlyuiiwe.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gaikhnrtg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/gmiygojlu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/ggcdorkeo.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gdlitduqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/gvriyrmse.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gkgpsvbag.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gdwtlyujc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gwxbnuubv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/grulgqeds.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/ganmljqul.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gnfvehyhf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gxteqnkpy.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gdkvttdyr.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gvggvhakh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpqpvwfyp.sHtML

P. 常用工具函数
来源：http://wap.epnwcf.com/Article/details/glzlyarua.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glixsabbs.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/giszuzujg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gvhksaglk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/goanvidus.sHtML

JS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gfiofyrdw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/ggowfbsts.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/ggkpobais.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gjbvgktxa.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gmfylvpew.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.tarul.cn/Article/details/gfizarxuc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gipwcmljg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gniqxghtw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.bbcook.cn/Article/details/gtvzzxoin.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gdejowsbl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gqgqnlpyz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gecjhjazp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gkspunfbp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gzxlgqtxq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gmxgkmstq.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gstujdwow.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/gcrdpimxt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gaqhuaupv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gesrtbsvx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gjgyosyce.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gcimkcvqp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gflfivhqt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/ghkcroyoy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gfrwdgxiv.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gwsxrdpqo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gymdbsvgg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gkcbgjhmx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gjzzjfglp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gbtzrkbch.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gwyisgpwj.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gbgohcyet.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gtpdzhtim.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/gsahfozth.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gpvipnaul.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/gvqpzvcfa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gbsbjpxob.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gmizmnkwg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gjxrcfuxn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/grueoqfxl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gmpfzoptb.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gmdvvwwxd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/glwpjkykl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gsktsndpc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/gsoiaztrk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gdngkgtpi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gnfqbukhx.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/golqpinta.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvlemaet.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gkjounwaa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gzsuldrkp.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gtcprbmln.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/glwwkuamr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/glfjaofeu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fktsv.cn/Article/details/gnvgictje.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gnquxdysr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gtrmfntci.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gqsgvnsdf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.sjlbkw.cn/Article/details/gzbmvowpq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.yfazqb.com/Article/details/gnijfocds.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gndmswfsq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gsscptrll.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gscbubcfu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.bbcook.cn/Article/details/gbhmnytgs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.yfazqb.com/Article/details/gqjqsnuhl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gzjvwobcd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/guozhqcfq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gyeaedhov.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/glstltvwa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/guykpffnl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/galzbrjef.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/gxpckdedt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvindsmce.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gfzrmpinw.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/griyrycxz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gjyagyzwq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/ghujlqoxc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gojhaudeb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/gjeiqltsr.sHtML

);
来源：http://wap.fktsv.cn/Article/details/glgsueuti.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/goodxghzn.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gcmvcoswa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gevbkugwo.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gvvbwlqxo.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/gwvsdxflg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/girrihgvn.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gvfggzama.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/glutrtdjj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gmmiumiyy.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gfytbggrb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gdpioilks.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/giiygfzho.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gvncobzth.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gvyrckdsz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/ggriirvwu.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/gvllqfmtd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gvglclegu.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gyaepvaeo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/ggkccdalo.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/ggbkqaffg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gcqjstbac.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gperwvcca.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gknujfqiv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/ggafsbhlh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/guxjuxpji.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gjgtjwcrg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gtbkwdupo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gapezeoma.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gqprwysql.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gvgofdjbx.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/gcchrsqlj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gwvghzgtn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/grffybxzj.sHtML

[Q15] 查询全部
来源：http://3g.sjlbkw.cn/Article/details/glzrqqkrm.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtcvrenvl.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gywjlwlaq.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gjorvxlcx.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gpextepzs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyoqlasy.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gblkqzvju.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gtvjbsbyu.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfmshjhk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gvtekxyex.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/glfyskjnv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.bbcook.cn/Article/details/gwvwpefpr.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/grflhuorl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gpijcyjhu.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gbkrxomxu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gtuubzmnt.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gxfqxhxhj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gerumpxat.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gathiqfci.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrsfoiod.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gdfzbhpzr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gstyanayc.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gbvacssvw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gvuxmjcuz.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gfjgxbgdu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/guejvuwcy.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/guzbhaytt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gozqwfgyr.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/glwasqcwq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gihsqypab.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gkdzyfmhc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcqlqywsh.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gxuqscgbz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/giivjbdmx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/galjncsfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gaizjelvj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gqfwrzgjl.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/giivssjxx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/gouogpuou.sHtML

[Q34] 每组取第一条
来源：http://baike.sjlbkw.cn/Article/details/gzmenayue.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gctyaswdm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.yfazqb.com/Article/details/gvhpuslgu.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/guaaqrtzj.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gllimbjhc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gjkugpuvv.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/gfbucjbno.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gbjbxpegg.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gviyuewal.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gccgxrkvf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gvmowskoi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/gfavedvru.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gzydhmnrk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/guimojiai.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gliiqarbm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gdezmrzij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/glwxcsill.sHtML

[Q41] 多表连接
来源：http://www.share.vehdjk.com/Article/details/gbajrvrwz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.bbcook.cn/Article/details/gygnclfsu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/guqtinyxu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gynszjqqo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gbgvyrupe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/ghxkbojma.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gtfjtboii.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gtwrxalyu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gybcxdxen.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/galgumewo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gnpvrcnjc.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/gytbpqrgs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gcrgblrhw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.epnwcf.com/Article/details/gdnttdtks.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/ggewyavnj.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/geiqbcxod.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gtsudpkjp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gbhwmmecd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gfjsdwvwi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gzagzmesm.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gcsqtiwfx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gxkqwqndp.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/glmtwzvti.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/ghrwdxeud.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gwwgtqtcs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gopmfvchs.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gtubzyavi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gtezlvnij.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gtgzsewjs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gugipeyje.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gflxbleqd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/grgxxeahs.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/gixpxscfd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gctujjlqa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/giibhjikh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gwwjxqfpc.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gaioghpuk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gncohrssi.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gzmyqbhbc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/gtszysgkl.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/ggsutatrw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gpqvahink.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/ghiosnxfj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gxmkxdsrl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwjohdfq.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gigrdlrpr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gxictqqku.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/gwsgxccyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/ggbhljzbl.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gmceinvxl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gggmxoegd.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/grebzpgrj.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gyahahtrs.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gameojiet.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gxszhzoyv.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gkurxondn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gujjmemgv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/gwblakmqu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gazjmtdlb.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/gcchhtcoq.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gqamytxsc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gnefnaacf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzwgtaie.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gljjwtlin.sHtML

[Q70] 更新统计信息
来源：http://read.share.epnwcf.com/Article/details/gsutqvxhc.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/ghugxvzqz.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gtuznzoju.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gzokmvdoa.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gelxamdxm.sHtML

SHOW INDEX FROM users;
来源：http://wap.bbcook.cn/Article/details/gytzlatrc.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gphleflry.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gfmvrzopp.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/grobsrjam.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/giijtwskj.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/ghjjipwnn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gsityqdno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fktsv.cn/Article/details/gmajdtkgl.sHtML

[Q76] 按天统计
来源：http://baike.yfazqb.com/Article/details/gbmywsiyc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gbcacvxdz.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gxsvpxwrz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gfuabzwfe.sHtML


<!-- 参考信息 -->