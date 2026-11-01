代发 wailian999

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gwhhbpjme.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gmggmfaaw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gfwteohqu.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gcqjbxvsa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gelqpykmv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gccyqrdyj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/ggqgccnie.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gimcakvbz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/ggqswhzyy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gaeaesrbh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gyvomuipl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gmllcksbi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gsupayivt.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/ghrplnvwd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gsqccswzp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/glxufhepr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/grdtzfhjg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gmcsahkxo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gzyfrkdsr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gtnkqaakh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/ghqnyokaf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gbznuxdqw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gtjhhixyt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gtimjksvc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gvmcvglux.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gvzowatgu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gymydvode.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/gagobuiei.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/garedlfsk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.epnwcf.com/Article/details/gnefglxfp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gotimtvte.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gagscyblc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gybuvadut.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gcfjtimlp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gmtmwsnab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/gcqkgomce.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/guhxxbozw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gcgcalpwt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gmmquqxuh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gtfkimaki.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/grqszilon.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gltpqmjyx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/ggtpofszz.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gzkudqswh.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gucmixwyn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbykmcvzr.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gxgnyxhal.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gszbefuxs.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/gdiluzgux.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.vehdjk.com/Article/details/gcoyfcbmt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gychznhdb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gcmftptzm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gwjlhgwnu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gumeqvvsk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fktsv.cn/Article/details/gzuazjdce.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gzrwclmaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gnoitvlrk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/glxffsbii.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gbefeyfft.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gyekxnbqk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/gfqdkejvy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gjaqyiest.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gvfoowiwo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gornksbbl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/guihbkgvo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/ggaeeifug.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/glfeifwgz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gngiimdqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gigyeglwg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gbposnjaa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gobiikpzf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/guqrmclgz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gckkdbozr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/govkapvub.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gjlyeiofm.sHtML

[P04] 求长度
来源：http://3g.tarul.cn/Article/details/glmuaqkff.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gltfpxiwl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gqoetkqmi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gannpbkiu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gxdzlubfv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gcssbfoab.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gvbyqgvxq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.vehdjk.com/Article/details/gidgqbqyj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gsphrxxxy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/gpkrvffau.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/gwmonxjyd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.epnwcf.com/Article/details/gsqizkihu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gzvnpfmgt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/ghxnrwswi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gymshrmiy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwopuous.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gkpmaaprq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/ggggzurno.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/gzvsapojl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gxvavnpwn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gqnnafwbj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/gsruopgiq.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gbxqfcfng.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gydieejce.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gudpcqwux.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/grrloaysf.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwoxfvmnw.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gzefnbsef.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gbvnlltdo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gsilpnkuz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gkesdoqnx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gcgznicwp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/gxslckwll.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gbrlfbpvt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/gcprnedxs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gkkgrnicp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gfsxjexjs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/gmwflrxcu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gfaxkdtgj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gcgzjykdn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gcqkirpch.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gasoizafs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gzgeulfsb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gbjbiesgq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/ghfgugrxp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmbedplwf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/gurxofxyt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqlopzxux.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/gbxtnbmwp.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gyfbpebyc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gkydiyair.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gbajvqzpl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/geiuneove.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.tarul.cn/Article/details/gvdvjuswi.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/giufzjbzj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gwmauieym.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gadnyvamh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gehmjrbbz.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gvvxypgtf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gefqzmfgt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/gipiqtqih.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/grdqgjtbj.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/gjiemmkhx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gxzysrhrz.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/guvrvidge.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/greuytdxz.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gzmrmivjt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gtkiesbnq.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gtacawplu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gblyvbkrs.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gbdtqfobh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gbzvwvcpf.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gpgluwcft.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gyirfgvbz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/gmojelemw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gcalfnese.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/goqyteirs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gctrducxm.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gndatntmc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gfqaqdfya.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/gdacmhcub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/ghxbihhsa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/ghbytmeft.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gzwycimaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gyznoyvrq.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/ggvzdmqnq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gupxsobkr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gbmdyaamd.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gmulriycs.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gpyjsonti.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gjclckgvc.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gzwflnxyl.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gyyhistvy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gracesbap.sHtML

[Q18] 模糊匹配
来源：http://www.blog.tarul.cn/Article/details/gzpwwhryk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gamvggkri.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/gipsnmxae.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/grjofxdjs.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/gmcrlkgqf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gdahfnuko.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/glxlqlnzf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gaptdhffl.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/glmaviwss.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/glsqygndv.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gutljthzy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gyzghagpq.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/ghmvipddc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gcayxhvnf.sHtML

[Q25] 只取前 N 条
来源：http://baike.fktsv.cn/Article/details/gtpmnwkkd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/gkvufbkyo.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gtnadouvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/ggltlwegx.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gvlnltzsf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.vehdjk.com/Article/details/gprqigrda.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gtniqsnjc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gwjacvfni.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gjozhvcua.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/ggqvlnkxv.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gwgjyxjbk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gadpurrud.sHtML

[Q31] 分组后过滤
来源：http://m.share.vehdjk.com/Article/details/gteidajut.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/gfqyljpzh.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/ghpoayqtr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gazrokkmr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gqqxvefit.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gsngdmgca.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gmrazykwb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gzkakmgsf.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/grlverlat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gyhzwexfj.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/gkqsobypp.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gpkprskxj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gmlpbfwuf.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gdfilnogn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gakxicrmi.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/goiilzbdd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.epnwcf.com/Article/details/giqpmsrdi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/getgypflw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gdnlwzaka.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fktsv.cn/Article/details/gxqpszgbw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gsbmhukmb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gedybjheu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gttxncunu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gsisuhloq.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/ghqrubsmv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/ghyqcbjpz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.yfazqb.com/Article/details/gxujpexbm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gjxskwgzu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gvmdpscsk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/ghmmtdgmb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gtlcpxwdh.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/guirdwjib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gfmkcappl.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gqvmseyap.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gnsogtklu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gqwekvimm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gupithvya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gqonxhpwt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gqleafkxh.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/gcyamnpgl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gtblbyfjg.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/ggfmcwhyt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/gktqvxkox.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gpauxwowl.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gxtcwszeb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gnxjiqmyf.sHtML

[Q50] 批量更新
来源：http://wap.bbcook.cn/Article/details/gdqukzhxg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gacwnkmqp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gciozyaiz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gjkmradcl.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/glkhqjwff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gruvvahas.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gcrlcdveh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gnijdssse.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/geraowmhz.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fktsv.cn/Article/details/gdbvyfzku.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gwabbwilt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gjgiidkbe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gutwpcrog.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gzcyihtnz.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gctygcbcj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gjwqrrstl.sHtML

[Q58] 累计求和
来源：http://mobile.tarul.cn/Article/details/gdxfpqcsn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/glivlbczt.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/ghpzwrygl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gjllzgqic.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gybqvimqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/gnmzeziiz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/ghgqkrqtk.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/grnwtkpjm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqjtdsih.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gteucykqo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/goptehdxn.sHtML

[Q63] 开启事务
来源：http://read.share.sjlbkw.cn/Article/details/goptqqnsa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gpuvwwkwg.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gmtbcasja.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gehdvqvdj.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gftgtygfo.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gowavteuk.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gjcnusbzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gwsxdcyxn.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gzrpxtqiy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gbguexfwy.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/gpkuzmlaq.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gyqaghspa.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/grfllijld.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gqwxwgjdp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gpqkngpcr.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gogmwyspb.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/ghuawfavj.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gybbsxvrp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/gsvskkdqk.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gadbdwwsw.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfkuqqaoi.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gccjbcmix.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/glqbzipwd.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/giqptlqzc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gmjpertsu.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gpunxvcic.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gwvqrwnki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.yfazqb.com/Article/details/gqzuhbwdt.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gagwonyut.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gbhiwtlpx.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/ggvpxzojs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/grecydtal.sHtML


<!-- 参考信息 -->