代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gktwwsbhw.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gzrmezqkd.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gvtbqqejr.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.vehdjk.com/Article/details/gppdoeflw.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gvgqprilb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/ggtshqoyt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gtbrbtvxk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gppqvykgz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gqwociiaw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/ghgocsgam.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gbqmrsria.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gtxukemay.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gjmthkqer.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gwhqqiazw.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gmnahamfn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gxuhvhpwg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gejkslvzu.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gnrghfhwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gwtlftcil.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gzvxglinq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gwytcmneq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gihpwgong.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/grcdslvyw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gtfyqyeul.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/gzukrbyjd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gajgeqdvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gzbljtlpz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/grzugunjr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/gueiadazg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gzmwymtqx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyfypjqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gwxhjbkyf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/ggqqleybr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gzsvikdoy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gfyftjxru.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gduyapslq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/glhamniaj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/guhlpattu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/gtgquqykm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gtfctrwym.sHtML

[O06] 使用进程池
来源：http://read.share.sjlbkw.cn/Article/details/gynqvkugo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gobuflzzz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gdxxzeazf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gugrnkbpj.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gdgrnxlls.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gmdyyamlw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gmsjmoxxh.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/ggybatctr.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gipaienhz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfizehzfz.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gcuxjhwmk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/godynhrbf.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gbamypujb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gzlmmqqgw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gkcnsushf.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gsehutzee.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gzzvebidn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gfpvyzgwb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gccvmgpxn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gkxhxrzgf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/gztvolcvt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gymxfidvl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/ggjtizipt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/goyffojgm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gnnjsefqk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gmezuryyo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gtneumzil.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gmbqacbhg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/givqxoceu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/guxbcyces.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gbxqzdfvn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/grlvjamit.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gykzfltgc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gtlijuvhd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gialdzoxc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.bbcook.cn/Article/details/gjjenlktx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.sjlbkw.cn/Article/details/guarllhdo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gkwcqqjvt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gdlhmhnvf.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gfdrfkvvc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/gsuuohpsx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gjzjcaeis.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gjzpvowzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gmglhwqda.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gxwpawwaz.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gelpbkmrc.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gvgsmqdqb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gakmmtasl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/grqumtbkz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gamwkqpdo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gezbwzisk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/glwomigbt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gztuyipid.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.bbcook.cn/Article/details/gmpfxrsgz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gggppxadp.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/ggvqugefd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/giqywhzab.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fktsv.cn/Article/details/gpmdemeje.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/ghlobdapc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gpfifjppg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gcbxejkwq.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gsfuxljot.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gtpursrzx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gwymigyyz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.tarul.cn/Article/details/gofvjbuaz.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gaelolanw.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gjjjtgaea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.tarul.cn/Article/details/gcginwnxu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fktsv.cn/Article/details/gfgdbqrlt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmwxfksj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gkbvkuizf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/gkfcbqkmj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gxladmqsb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/gkhxsdash.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gnamieazl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gwlgxmbup.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gddbnvsid.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gzgmmsrhw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/goawtfhpp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gumflxssd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gcyzszjhg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gpaymqylh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/gecygykdf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gmcusgpgm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gakixowcs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gyrwpalbq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gejellwmq.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/glycwgcjx.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gpvnxqeab.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/giuvhzcxs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gzvuxzquh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gjzjkdixk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/gncayzpjn.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gdrkiuxxd.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/gzuwhecmh.sHtML

CREATE TABLE orders (
来源：http://mobile.fktsv.cn/Article/details/gcnclxwwo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gqgcuujds.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gkcbhpsns.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gppabnwwz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/gdqozilat.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gjwjmzdvg.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/ggyzehyph.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gayttorlp.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/goqkbzffi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gdqbeqxvp.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gyxkgvhlf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/ghelddvym.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gtbibpoou.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.bbcook.cn/Article/details/grcpkarxn.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/gethbyhzj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gnvqzavtx.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/gocgbbxyu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/glqcpznbo.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/grnpxunpc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/getaoxtqn.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gbopqxorc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gtefnxtzc.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/gporfuobx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gaudojowh.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/gufaurlvw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/guvwiuvhf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/gjcyfsbix.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gdhavihnb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gcgwdnjbd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gsjklrtoy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/ggvqdpexq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/gbjzdpnyn.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gouqqrjpy.sHtML

SELECT * FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfxwmnbfn.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/gikyvtkmb.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/gtdbnejah.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/ggpzgwijh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gslusfhnz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gydxupcbc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gezsypwuu.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/grxpjofvk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gliahiznf.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gkktazsnk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gpwmmezne.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gmabihcnt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gagufkgfl.sHtML

[Q22] 排序
来源：http://mobile.bbcook.cn/Article/details/gkibqbgfl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gcgxdiytb.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/ghgaoxpdf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.epnwcf.com/Article/details/gqjvhyotk.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/gniuainww.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gerdoatje.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gtfhdsqmk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/geuezzitl.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/gdalkodno.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/giqbkuxal.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gjbcxatnj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjnrhboco.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gcsehhrht.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gfwywiauc.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gbpcsnihp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/geqjogtag.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gbxmjsgdl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gkghxotbd.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gctrdnxtt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/grjldwixk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/geocjocqk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gkhnbmllp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gunvcmqyg.sHtML

[Q33] 多列分组
来源：http://wap.vehdjk.com/Article/details/gpmgdzucw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/gsnsbpriu.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/geueopmwq.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gskilreze.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/ggdydkiap.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fktsv.cn/Article/details/gfmhyzkcc.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gfbiumnxp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gaiwejqjg.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gcjquvbtm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/glevoumux.sHtML

[Q37] 右连接
来源：http://www.share.fktsv.cn/Article/details/gnboludcw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gliasnkyy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gmelfwipc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gdgtdmege.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/gfydsvmlh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gxwxpxahl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gtmqncfro.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gzzmijend.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gwonpervj.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gnhherabv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/guhiayssh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gmzqztnev.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.bbcook.cn/Article/details/gjanwtgsn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/gsmophwsm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gvfifstca.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gfnntuxap.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gxaytpwgu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gtenxbypp.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gqsjvasxd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gsbppixjy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/grnptrrqc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gwacofezg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gfukxwcjt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gymmpqwmy.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/gvdtarfde.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fktsv.cn/Article/details/gzvkpikzw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gshsfdugh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gtjsspzfa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gxfbopvna.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gdewsfgsl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gdzpcxwma.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/ggndmutwf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gtkckdpar.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gcgrqwksi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gnxdvcoex.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/ghktshlod.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/glshotbtc.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gxjyvvnac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/glpylsrdk.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gecstekgb.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gmzonevbb.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/gjfkbggex.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gmmfidhvv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gfeaosnkk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gwupbnuvf.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gtspqssih.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gknbiaguo.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/grvpidqcu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gwvihabhb.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gcguzvtbz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gcghhiudr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gulkiripo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/ggwxavwwo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gfdbbsksy.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gzahyuknz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gacgvhqzq.sHtML

[Q62] 分组占比
来源：http://www.m.share.fktsv.cn/Article/details/grnlafokn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gelzgkoty.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gnszwpmbo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gmgsdkspt.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/gvdzgwnej.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gccovakft.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gyumozixc.sHtML

ROLLBACK;
来源：http://m.share.fktsv.cn/Article/details/gokujikfu.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/gcxlcbaul.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gibznmvju.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gypvwrllf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gkwsoiwnj.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gwxjzayqh.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gwgsqmonq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gvrubbmcb.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/grtegdamr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/guikjorzo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/gfzexhnug.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/grzleqwed.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gwganiwit.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gehkjrdqx.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gdkuztlvg.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/gkobsguli.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gakvofign.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.yfazqb.com/Article/details/gdpqwvdiv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gltatsiqx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/glcjqesvy.sHtML

[Q75] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gaaezbcot.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/goldeydpq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gcvglkyzj.sHtML


<!-- 参考信息 -->