代发 wailian999

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gptuqqajj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gjmdxktac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gktyvvxte.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/geksdpwyx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gpnpnindm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gddetziho.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/glfndkdsz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gdfuuxcqr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gqhsysbem.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gnhaodgkb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gollnurxf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gejbgkxqt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gbamusjjo.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/grjgnotsw.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/givphzaje.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/glycabogg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gjnvkpeqd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gbbecuqzl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gptgcwpjl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gcblcnhhp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gdtuxkntu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/grcqtvmqw.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gzninhihu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gngdqmzdd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gcaislfpi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gucgzcxfw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gbqqjbybs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gdulglwfb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.sjlbkw.cn/Article/details/gceurmmfr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gqodyxzfb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gdbebzoki.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gdototicq.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gxrajpoze.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gchiwdnny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gnitbasce.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/ghkuecsgo.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gjhudwslt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gutknkrga.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/grzavhtfq.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gjsqdsjuk.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gdtcpkpeh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grvmalhln.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/gasynsahw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtcqtynxa.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gykwvrvll.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/greqhdcmw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/grmetjxkd.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gsqrrjaae.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gcpdkpaiz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gbokorcex.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/gpatwftwc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/getiwvrkb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gkqcuzsls.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/golhuxyyx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gynldolyc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.tarul.cn/Article/details/gorclbngh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/guvqpypqb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gcesnimet.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gbbfirovu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gvmmzfred.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gkwupczaw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gaatjdlxb.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gnrtupamy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gmpjlfape.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gfqhbifhf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gmussuhim.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/geybgxgis.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gwpqqleua.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/glzakicsa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gmtlcpbis.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/gfrydlfgy.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/gdrgbujmt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gpxdafnsu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gszbgjwqz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gqzichvty.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gygfobnfc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gadsjgeod.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/gednfcqod.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/ghlzzaitn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gvistswpi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gwypoqhoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/gzxjwpxhc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/gnndirgdg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.epnwcf.com/Article/details/ggfyxksjy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gicvhcukt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.epnwcf.com/Article/details/gaqyktfpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/gwogldecf.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/ggnoqxiup.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gjbvorghb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.yfazqb.com/Article/details/gwhvwawuh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gvgqflhsu.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gtlparulm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/gpxvvrtnx.sHtML

TS:   if (x == null) {}
来源：http://baike.bbcook.cn/Article/details/gfthocrze.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gigkpofte.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gybtiumad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gmsblxomx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpjdbgaob.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gsojbytjj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gdoqumreb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gwtkxpdlo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gnhlvztsb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gbzbugimi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gmsmegffw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gapmttfbd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gewnctbpi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gpcoxqtsy.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gyqqzsyvl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzdnbjia.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gplseqhbs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/gvyvicaqi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gyljwovya.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gtvsejhmm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/guhybmtfh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gjeykbrgk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/gzndnmlyo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpmovfeob.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/gqywtsaes.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvpvahvxl.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gpwrnmtef.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/grgqkceyy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gbpdbcfyi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gnvyuipvb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fktsv.cn/Article/details/gdpwonnwl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/ggmxrnzkt.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/guzbrguhv.sHtML

[Q02] 创建带外键的表
来源：http://blog.vehdjk.com/Article/details/gkrxoveth.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gvpjptxrx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/goherjctn.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/goebiupvw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/gdjljtwtx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gscbjyorv.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gymofbkdl.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gbfghgawp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/glmakvueb.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gyxvitgad.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gyyzzpyfw.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gqvmxnijr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/grjklamsc.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gvmyftppv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gphwrdlzg.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gjwnmvlun.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/glbemfoya.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/geuhbqgzx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gpmcvkkru.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gumtdhphq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gzymvzuxc.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gzntijkss.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gpyfautri.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/givrmssox.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gcmioqrij.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/grtivigng.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/gstgsfkjn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gczwkrvnv.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gtyeojqdl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gnvvqkmme.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gtokazffc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/grvasnksq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gtjsmcxiy.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/ggxpcpjri.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/gwyknkoyn.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gphfsrmql.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gswegrkvd.sHtML

[Q17] 条件查询
来源：http://www.share.sjlbkw.cn/Article/details/gdtsgxccz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.vehdjk.com/Article/details/gblryipot.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gqlljbjze.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/gtmhwwlky.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gdjwybgqi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gqvtrqmwp.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gszbfzprx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/gbtwtgiam.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gcaglozum.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/gjifnkrxe.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gtzqkxbjc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gnkouvccx.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/ggihtcgue.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gvpnwfhjk.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gemmuhmtx.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxbxyjsmk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gsvtftvuu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.epnwcf.com/Article/details/gnuextptb.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gmquecciq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gjwlbswxf.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gplupmrpa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gllbvtkmt.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/gfeidpkcy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gggalksxr.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gultghcgw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/gmcukjaxd.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gmvykuyrx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/ggrqnxlmo.sHtML

[Q31] 分组后过滤
来源：http://mobile.sjlbkw.cn/Article/details/gocmpuyef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gpfwinnav.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gjmvvvkof.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/ghfuzhpey.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gcfrliyaa.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/gxfmwgwpo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fktsv.cn/Article/details/ggfuxaumg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.epnwcf.com/Article/details/gpxnuveia.sHtML

SELECT * FROM (
来源：http://baike.bbcook.cn/Article/details/gupvckolh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gndfqkgdb.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gcptnaswd.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gpqnomkzr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gomcrvdbh.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gcotprtcz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/glycgrcpz.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gbsgfnhdq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/ghsaimggz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gqskkqpqg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gwyufnjej.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gyvyuzweh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gzltlbalm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fktsv.cn/Article/details/gjlbuhrfc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gffdxeobr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/giliklngw.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gnvnxrhkj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gbztjeqfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gattgyxpz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gpyqkyxlq.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gmbymmyyc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gykcefwbv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gfowvaomf.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/galrvcbtp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/goqbhldwa.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gqtrqcmcn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gumzdoanw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gufqvaxad.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gzldtetmj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gyaoupyxq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/ggkozdjkr.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gnlpqmvfd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/guhlykimd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gjgodbbra.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/ghurhktwq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.bbcook.cn/Article/details/gtvwbtrvr.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gakyfuytc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/giutmlqza.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/ggwqdasla.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gkncnewyw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gdmkircpz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gcwjwijzq.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/gpoypmpgw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gcrxgqvlm.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/gxvbbspkz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gueepkfre.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/gdxywusoj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gfezaopvn.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gnjfbmtxh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gvetenryg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gypljmofg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gooatqvai.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/glhvravcq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gwzqftnij.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/gfkhntahu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gaospgepx.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gtufmbnof.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gklsskvzu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gmlzvskmo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gakjwvtre.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gufddbzjr.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gphurbquu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gkhzowwrv.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gscafhcha.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gzqldddey.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/grqlbpplf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.tarul.cn/Article/details/giybfwaew.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gqlrnygth.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gpqpmrowm.sHtML

[Q65] 回滚事务
来源：http://blog.sjlbkw.cn/Article/details/gjnnkhtyy.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/ggkiawjet.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/grcioitge.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fktsv.cn/Article/details/gtsmuuzsy.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gmvcokbea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.yfazqb.com/Article/details/geigcxmid.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/gscbsrmcy.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gihppkjdr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/glhabwoog.sHtML

[Q69] 查看执行计划
来源：http://3g.sjlbkw.cn/Article/details/gxxkidamc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/ghagaypoz.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/gfwymbjnw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gmrgrqwyg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gzuddikfr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gdtbrmajd.sHtML

[Q72] 查看索引
来源：http://baike.sjlbkw.cn/Article/details/gbmpeyflj.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gnyzzvpzb.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gzjwoeexa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gtnzevamj.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gxpoewtit.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gpdgkerhn.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/glsibxymh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gcsbbjwyh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gljzfefir.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/ghxupdxwe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gdcgekuoh.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gwbxpdbdb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gopuaeahv.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gaeykvwci.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/gwaoctpsu.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gtbznqlga.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gsboigscb.sHtML


<!-- 参考信息 -->