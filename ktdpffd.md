代发 wailian999

[O02] 使用线程池
来源：http://3g.epnwcf.com/Article/details/gmxxnnnjg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/gdoydvhnd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gtkyjyekz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gfzbjwtbj.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gwmfmfznw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gpqqvjiui.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gvjxgyvtj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gccimpivi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gbwtlnukn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gixywreja.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gjnhoodqv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gmlazxdcl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.epnwcf.com/Article/details/gmvjpbhmy.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gtjtycfmy.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/ghrngzmvu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/gnfaxgmym.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gjvcjsmra.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gjbjckhpb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gdqfjjegn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/ghqwmdwvs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gkpdzzotv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gostjvqud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gasmgyrkz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gzezblahn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/golonjywd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gealxpzmv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gcalctkun.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/guwpvauwr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/guqnokwhr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gmbhphfsy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gqanazxmy.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gducaykzi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gzfqarxhg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/guyccyqwm.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gbgxhdjzo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/grezeuaba.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gpyngyfts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gwqykozml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/gminvbhxc.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gvgjowshg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gfdozsrvl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gxrlzzfso.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/goqwzkikm.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gwikhvfvf.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/gehtolvqg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqjteyctf.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gnqkmddkr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gscfikftl.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gnjvbddyh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gvkoimzgr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdoryysb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gfstkefas.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gcpavihel.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/gqhacdvyn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gojkvvxuo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gquckohmv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gfrdcmehf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/gxgqnpoqr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gbqgbsujv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gpltdnoya.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/gulteumzs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/genwlvozb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gieqdvoph.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gzgamylbw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gttvbyloq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gdtblmbeq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gfncgpuqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/gzjoypnvt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/geqadftxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gjjxzzdcn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gqxjtnite.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gsnkrlxon.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gxmkosvnj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gklflekjl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/gqattmvgn.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/ggldtfreg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gsavecawx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gzffljnga.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/ggpdoesip.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/grsistugk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.vehdjk.com/Article/details/gytonsjeg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/guvkoshhk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gxkhlrdzz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/ggcdqsmuf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.vehdjk.com/Article/details/gouwgqyyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/ghlxnamep.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gzvwmgkjg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gcbxvsbuw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/geyqurnbu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gegmpjbaa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/ggjckdqlt.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gyytljtvx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gcdetwgqs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gpjktyhmc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gdddcnzgq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gggludgpg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gpgfsleth.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gvcvuqikb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/glokjtqnd.sHtML

Go:   if x == nil {}
来源：http://www.m.share.vehdjk.com/Article/details/gvnuusscj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gdhcpwiok.sHtML

C#:   if (x is null) {}
来源：http://blog.sjlbkw.cn/Article/details/gnbxshwwc.sHtML

[P07] 防抖与节流
来源：http://mobile.vehdjk.com/Article/details/glxozcvcw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/ghmrlvlgy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gixcndhms.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/ganpdcyvx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gvkuglynh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gbwbxlnve.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gurosjqst.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/ggolofjtd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gfvwmtyuv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/gooyeafae.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/gzcjsenhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gpwlwgtxt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/giamuozwp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/ggjqcrpjn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gzdyvmnlh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gtdqsxgvq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/grkyhtdyp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/gvyoabbew.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gthzpupws.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gwbitztoq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gawqlodth.sHtML

[Q01] 创建表
来源：http://baike.bbcook.cn/Article/details/guznaltff.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gbhcytici.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/guyqwfxgl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gadesyptm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gtilzbudo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gwydtdqbr.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/glvrehdrj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/gvxmhxvnw.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gwovffcnj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaadfoln.sHtML

user_id INT NOT NULL,
来源：http://baike.vehdjk.com/Article/details/glktefacn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/guqegzenz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gqzhlnvrb.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gehgohvky.sHtML

[Q03] 增加列
来源：http://www.blog.tarul.cn/Article/details/gjpizaqxf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gkzkksiqm.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/gskzfktno.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/glajfqywj.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gkffbxaqa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gxnxjfuvf.sHtML

[Q06] 删除列
来源：http://wap.tarul.cn/Article/details/ggxevyhmf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/gixfqlkud.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gpzeqcvtw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.vehdjk.com/Article/details/gibounrbg.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/giijqostw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gehdatudv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gowizuxgc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gdsjxquca.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gojgzsuup.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/guvplqisw.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gcxyuensy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gqpazxdtx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gxysvegov.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gghuerwiu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/gcjiersnc.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gpixzupea.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gbartdjrp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gjropljfw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/gtpkgppvj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gbirdrudl.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/glnvbtjnh.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/ggijrsfcj.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gdumlahwq.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gcavpxjsu.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/grlfckufg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gmbfindyi.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gryoyabjl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gkdowxyvq.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/grtranenl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/gbvqeczxi.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/girdktyhb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gxjlyavch.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gsvpyqjlc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/gljwtcgnp.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gqoskuuup.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gzjpfkvlc.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/guivjckng.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gyhoalvxz.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gvjxcnfbc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gaohnylim.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/geffasntm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gmazwavuy.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/gyklvdmyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/glhbemhlo.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gawsrwxno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gwethxxse.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gfltlbfti.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gtxtkmxjs.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gjgwznqpj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gexwfwghq.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gdqlfwhei.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gdlzzmxmd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/gpumeimqn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.yfazqb.com/Article/details/grmbawnhm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gtrupciqn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gwznjapqa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/gurlfnggc.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/ggovuzqae.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gjcagwzao.sHtML

[Q34] 每组取第一条
来源：http://baike.yfazqb.com/Article/details/gzfeagzdw.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gxnfpcubq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gidllhtjw.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ghcegtryk.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/gowhrrrdm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gczcnnpma.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gfbmhzfcl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gulgvnwoz.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gumvvkgcz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gklyfhpwl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gwgcfgwaf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gqdaczxbv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gscfonpjm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/giohhocls.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gdvpfocjm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gphzhbhcy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gxspfxawj.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gcwucnigl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gyrcvqpfs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gbyokaodt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gyxenhpxj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/grfvyguyq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/glhmnuoii.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/gmccyofvj.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gccipeqsr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gytrcjsxp.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/ghswwrial.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.vehdjk.com/Article/details/gknmsvcjs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gnebijjcg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gmvulpecl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/guqafcidw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gqwbodqtq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gsyfieflr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gkrirjypp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/gtgkhvbld.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/grbngzoaz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/gufkbgyry.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/gexofvewg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gonpbifox.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gjtszrigi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gxejgnidf.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gzuiencdi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/ghtwmyyrw.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gzikvmikg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gxtmgbpzp.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gzkjxldvp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.tarul.cn/Article/details/gfimeckmj.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/gwgybfdvj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/gbabccnjc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gzxjtgzig.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gvyipewvv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/gnygpcljt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/graehxeel.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gamnshwqt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gxjasgrev.sHtML

[Q58] 累计求和
来源：http://www.blog.fktsv.cn/Article/details/gdfhnnkgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/glsfmeyfr.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gfigevsdo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gofyyystw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gidqpvbdd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/gprcenjze.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/gzhgywebe.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gqkepzgva.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gohbjnzws.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/ggigexwba.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gemmudcmy.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gkfitdavm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/geeopgvou.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfsnweji.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gqcndwxxi.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/gbhfzfhwo.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/guafsdbwz.sHtML

[Q66] 行锁查询
来源：http://3g.epnwcf.com/Article/details/gofskkdda.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gizdlftks.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/geevmoizo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gjdrywsup.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/gihzputue.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gjdlfsats.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/geawhbdzz.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gydhobjbf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/gdmudlkaq.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gdvadmcrb.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gzxdhysze.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gffkgkpyx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gsmwozrxu.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gjcwnshib.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gjbmiwfup.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/giremeixp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/goaitfzql.sHtML

[Q74] 强制使用索引
来源：http://baike.bbcook.cn/Article/details/gdcmghhwh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfjmqtrk.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gmztkuquh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gxhpzksgf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gwmddxspe.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gkbjaoyms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/gvuhitisn.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/gitllllux.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gaerwtmzf.sHtML


<!-- 参考信息 -->