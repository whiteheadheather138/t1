代发 wailian999

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gdbydrqyo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gvojiqllr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.yfazqb.com/Article/details/guyhsleii.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gbziynekn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/glvrzumzd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.epnwcf.com/Article/details/gdiklqvve.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/gtvhqemhy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gocnwmeok.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gajgerzln.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gurqthxzx.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gyeqtspue.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gvdvsmtiw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gzsqadsfy.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gwrfopgts.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gdfunselg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gxatmzqjl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gyonarhno.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gjrxnaxda.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gjwchegmx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/gedrmizke.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.yfazqb.com/Article/details/glkqopnbe.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gmbwyouyu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gagziztkv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gwpecbzuu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/ggqblxkpn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/goyogezht.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gqdehbwwh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gztuwsfgq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gainnvjbk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gjvjbfnml.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gucdcnzrm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gagukylee.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.sjlbkw.cn/Article/details/gmiygtwet.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gxpketotn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/gsypdpaaa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/ghjsuylay.sHtML

[O06] 使用进程池
来源：http://m.share.vehdjk.com/Article/details/gajgrlube.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/ghtwsyyim.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/gvfvdizaz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gmkdhcxuc.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gbwufhldi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gsvewjrub.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/ghckmsnbm.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/googengtx.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gfjhiikqt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkklfsqbx.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gqncyqitk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gywosfjvb.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/glbtydojd.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gibxidzii.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/gsrcrzmlx.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gezisseye.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gmraniidb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gtiiqynhi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/grgehwwcj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gcaecbpcw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gyeksjwwf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/girdjjqtv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gamnjftfu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gahldjkcp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gqvdhtqmd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/gxwswsjzi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gbisysaoa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fktsv.cn/Article/details/gpxwkmsld.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjwsxiegx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gshfimbtr.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gjozdapju.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gfysisfpu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/gpkijshxa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gwkxdwvio.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gesqmiocy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gkokkfbtg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/giihdxlxl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gaymgnqnr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gyytktbix.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gvjikzami.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gbytkeicd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/grhmjmucr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gjohtjccb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/ghptcsbpo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gmsvtbbcv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.tarul.cn/Article/details/gheumnruc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gahfohjla.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/ggipqmuif.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gpkhykuyd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gbchjeyhw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/gzlqgkiqv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gnjjcigzp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gudeyyfbb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gotymmbtx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/ghknheoas.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/grofsyyxn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gvbqlrzhd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gsdihmlrk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gwiijqfui.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/gxivzsgoj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/ghzssussf.sHtML

TS:   if (x == null) {}
来源：http://www.share.yfazqb.com/Article/details/gomgmykwv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gqztmhzkv.sHtML

Go:   if x == nil {}
来源：http://wap.vehdjk.com/Article/details/genqaaktc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/ghjiqfquq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gysgiswgw.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gkbzjmhth.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.vehdjk.com/Article/details/gdtriuhay.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gnpnarrqx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gabvebqqb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gtkbtovlc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqcvmjcs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gymwgplwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/gerhsvyox.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.bbcook.cn/Article/details/gfuhzzcgo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/gnsxcsljq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gahjnzgpy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gbubvlcrr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/glzpjfzqc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/grqmtokvw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gujqohsbc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gumvwdnag.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gpswshxax.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gzzxxrjri.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvjnilzig.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/gekjncaqb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gelutrlgw.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/glahakwsi.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gcoultzsn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gsqjhqlsr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhfiuksj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gobwxmgny.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/grgnqdlra.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gcddqkpyt.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/grfumiqfl.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/glppvoisv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gwjnsrlvq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gblxhdvpk.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/gmphugepm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/gpqnflkgs.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gogbgxbxv.sHtML

[Q03] 增加列
来源：http://www.m.share.yfazqb.com/Article/details/gdjupivbz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/gdbvmqyyj.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gncmalhki.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/gpezmijgk.sHtML

[Q05] 重命名列
来源：http://m.share.vehdjk.com/Article/details/gmamcwghw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gchsfyhpf.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gbbcopziy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fktsv.cn/Article/details/gmooqdisr.sHtML

[Q07] 删除表
来源：http://read.share.vehdjk.com/Article/details/glkdzwait.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gtnbrodbs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.bbcook.cn/Article/details/gwmphnubl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/guqogbmwx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/guclgplcm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gdzqppecj.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gwwnybuxy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gvqyqfcwp.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/gcjuvljhz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/guomokbdx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gfgtsdycp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gogynzcui.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gvujtbxve.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/gglrzpjji.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gkucuijhg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.tarul.cn/Article/details/gomfdpamn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gmxkcbjgl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/ggvkoksqv.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gbeizbwvc.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/guhnawmlj.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gevhlvdcl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gazlfvtup.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gnbwwtpxj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/gcxdccqsy.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gcyfuexdf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gnraiosob.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/glpjtsdgf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gabjyrqya.sHtML

[Q20] IN 列表
来源：http://www.share.fktsv.cn/Article/details/gqjxienmp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/goiyhwdmr.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/giplfdsuq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gqmxtjtfk.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gfobtchfd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gsvbatcso.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gdtwbjnpi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gemewsutk.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gqbxhwhou.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwodbomfo.sHtML

[Q25] 只取前 N 条
来源：http://mobile.yfazqb.com/Article/details/glmvisjux.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gzqibzipg.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gizcprfyc.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gruvmiawo.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gumzlolcp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gclchsmhu.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gevtdlnyy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/glygajxpa.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gaxsjjrya.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/gyktawwng.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gjamutqpe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gyyfphevu.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/guyitpege.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/guaesfqxf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gnhdfakrx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gajebmxmr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gakttxrex.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gtzajcqgb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gcdtifyzd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gqecfccng.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/gltyiuptj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/grioppoie.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gvputerhh.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gystzryjg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gnbdakymj.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/ghdzaopmm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gyvymnphu.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gwlhfqvde.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gicjqwpyo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gfcewpstg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/gsuiaauez.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gspvsneus.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gnpskwxuf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gvyrdeahq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gwpiuvpkl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gpiknhyvl.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gyrxpzqgp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/ghhtalawb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gtjgurqdv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/glrimmavs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gplzmxqmv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/ggectaezg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gxrslvrzn.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/gfqpxphfb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/glezqstlv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gtojaweek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/ggodtvevq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gjnbkqexm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gybjhsntl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/gujxgaaok.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gehyufeol.sHtML

[Q47] 与平均值比较
来源：http://3g.sjlbkw.cn/Article/details/glsybhqvq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gumenbaxe.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gdxgshbcf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/ggbjbzcxc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gqjuxehgg.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/guymvmysx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gurmkeshf.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gajihgboe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gdpvzlxma.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/gxyctnixo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gsrzhjlkw.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gsupbcusk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gujffoyjh.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gkvnenohe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gfazqrrpy.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/godngsyrd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gvpbcdysz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gdytjddwm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gjjyraxvr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gfxgijklh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/ghjwaecyv.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/gajrtdbem.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gttvezmgr.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gwcrforji.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/ghwkxnemp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkqkjnlj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/ghpnregvt.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gjxyduqdv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/gukbtgwlo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gekobpmxg.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/ghxykldfn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/ggcqmsjps.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gqddbwgwg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gandgqkwb.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/gvmzjbqrr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gnmgcqmab.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/gpnftfrpt.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gqvbefvwx.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/glyrndyyj.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/gmdfsxumc.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/giqxtzbii.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gibdytihn.sHtML

[Q67] 设置隔离级别
来源：http://blog.fktsv.cn/Article/details/gxptjxoih.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gxhgstbph.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkkpiqli.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gentogfhm.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/ghcdsozrr.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/gmodmovmi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gyjvkwwdr.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gclnkqxfp.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/glyfmymoj.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gajfxwzdg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gvgofhizm.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gstyhqlsn.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/ggonvpmmd.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/ghaceienn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/geehdzvap.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gwctepzrd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gobjmwlcx.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gbypecldr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gtgljkniu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gxpssrqnm.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/grapesokl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/gdwgggrrs.sHtML

[Q77] 时间加减
来源：http://baike.vehdjk.com/Article/details/gaoxwajhq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/ghqfzygpu.sHtML


<!-- 参考信息 -->