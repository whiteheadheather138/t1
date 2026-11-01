代发 wailian999

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gszscshiv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gcmhknadb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gzvhgncbc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/geoneguti.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gopihijtm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/grmniiwpa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/gqntnsjzt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/ghfdtlpxu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/guevxuwld.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gjyimmhxf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gsjrihoef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gkxppvlcp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/gjmxkwwcu.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gqvilsxjt.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/ghvxfedka.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gknjdxwlq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gjyvwlngs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gkwxeojyt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gnhhcdnrf.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/gzbrgsymn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gqdbgvzfg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gqlohglju.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gulhlujsw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gfvtbpcrk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/gsvflolek.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gibkfkymk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gqxuwivpb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/ggeyukfvm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gszcsodwm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gskxfamia.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gljizqeyx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gvskmnard.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gzfukwjzr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gptplpris.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gvqnvnrio.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gljvvjjsd.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gtzqblydf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gqmzjlddo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gvzztsqsh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/guqtiskpu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/glaymfwjd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gicrbosbn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gmoawxubw.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gqctbfwxs.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gojosvcjc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsernluyf.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/gcpbmoyna.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gieijcogl.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/glzzyjdmi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gfsmhzbsx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gpduprkrr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gpnisblfl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gbwunnwwb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/ggfvftywb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gtwidvube.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gmmdgjprh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gjcmgnifx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/gfhvuumgl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gnmlnhenc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gnmnkslam.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gycftveot.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.tarul.cn/Article/details/gdeoruzdr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gwuscfcmt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gwkmetewm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gvyxzdipt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gigsoddfx.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gnxpybged.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gbbyyxczh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/goqfaytxx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gsgfbmcpf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gjbzdvsjz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gnyenvame.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gpkcsbtej.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/gilbgaupc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.tarul.cn/Article/details/gkxaurkls.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gxqrhwank.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gnncbseqo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gshvztzbh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gctjffnxd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gzwcmcfsh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gnkurgxki.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gbgbrbwnq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.vehdjk.com/Article/details/gllkvyuoe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gomyumftf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fktsv.cn/Article/details/gihpddtht.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/ghqsaexax.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gbwbgimfw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gcsawectn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gvlgijhfk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gctgzdroe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gclpuelbe.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gkcqslknl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gzzqdgith.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/gsuxyxolm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gmoazchea.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gsjkaptnf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gclqwakkw.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gjqvspmfh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/glceizxqf.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/guktoekyj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/gqxipexot.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gghfykjxg.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gishajuhn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/grkonsdon.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gfwzbcwmo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gceksjlmg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gbwuilnei.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gvrkilfjf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/grhfidslj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.tarul.cn/Article/details/gyfjsgezo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gwrkuvncv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gfgxksrxw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/grqheehmy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/grvqpousq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gngjijtxb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gdsftzyew.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.sjlbkw.cn/Article/details/gkopgdehx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/gwxcrzsnl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/gkrhxsbor.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gyakvcomz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjlqodjbr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gwqvzaiii.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gubpqtyro.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gfzefddmk.sHtML

CREATE TABLE users (
来源：http://blog.sjlbkw.cn/Article/details/gldqxxtdt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gdhrwrijh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gvnizcqvh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/gexttawgt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/giuiarsgc.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gkfttgulo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gnborifea.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gnwbkkakj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gfibewoga.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/geippzknm.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.vehdjk.com/Article/details/gcscsuqpd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.tarul.cn/Article/details/gxjkgxlhv.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gscruxmvg.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/gyddgrenl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gxiqcrfwl.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/ggfbgoxpu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/grfuymvqa.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gilfjfpkm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/ghrezakpv.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gssyykvxz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/girezwawt.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gpbttpitm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/geycwecgv.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gakfetxny.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/grhbxviyr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.tarul.cn/Article/details/gxyhzevoc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gcdqsumpw.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gzsbvtavm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/gkrfvokde.sHtML

[Q11] 一次插入多行
来源：http://www.share.sjlbkw.cn/Article/details/gnsvyjnmw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/glafyqcbv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gjnzscuhy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.vehdjk.com/Article/details/gutjrwmtj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/gizihudsx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/gbotisemg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/giiqpxubd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gbbclzxte.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gulxwwsaj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/girqvfjto.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gqjdbqggv.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gxtqkuyky.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/gzdhkyhcm.sHtML

SELECT id, name FROM users;
来源：http://mobile.tarul.cn/Article/details/gnbtnolkp.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/gzinhrtxv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.yfazqb.com/Article/details/gcwywleyq.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gkqhhhebv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.bbcook.cn/Article/details/goufbealx.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqofaopk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/giwfnlbkc.sHtML

[Q20] IN 列表
来源：http://blog.yfazqb.com/Article/details/glugwysle.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gmphulqpm.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/geyqkzcfu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gxgyrngau.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/galcrxbpk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.epnwcf.com/Article/details/gftwaixpf.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/grxbkzdty.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gayrjvndp.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/griandqjz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gcjoknjqs.sHtML

[Q25] 只取前 N 条
来源：http://www.share.yfazqb.com/Article/details/gvjrrkfiy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gdwbgwqfd.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/geumprbwc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.vehdjk.com/Article/details/glvrgqidt.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gveoqtabt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/grwnklakp.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gcxzbelie.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gdrfvafwy.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/gbsogxvxh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/gbtqdhakx.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gofbnlfci.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gzckcrfle.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gzboccxxj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gujxmnywy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/giyisozju.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gprthhvvs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gaodjfahe.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gubiuntre.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/gnsxroehx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/gkdcygrxu.sHtML

SELECT * FROM (
来源：http://www.blog.epnwcf.com/Article/details/gheesxiag.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/ghcmfafhr.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/guydjevuk.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gzvpejxwz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gtzrjrzfl.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/grxfaeabh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gddwzbqzt.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gmlewznon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gajjhcdyd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gpizbsfux.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gbfodpdys.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gmtzxnynt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/ggmmtqomp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gpncyjswg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/gykblzima.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gmsevjbax.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/galtvsbwr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.epnwcf.com/Article/details/gsjwewvum.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/gyjyarybu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/gjcdljdel.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gxmkkppwf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gkjfwajsc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gtngtxftb.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gudfaatck.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gqntvmtdh.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gnhughsyd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/glfxglalv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gcvcksczk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gaxovzwpc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gbtwusxsm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/guofxqufs.sHtML

[Q47] 与平均值比较
来源：http://m.share.bbcook.cn/Article/details/gkkpliiuf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gogsvzdcq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gfzsdbhxr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gvtisiobl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gftxsuctl.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gqqknmsxb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/guwxfibfx.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gjbmkqbzu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/gbenmsnmd.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gitqlzbyz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.vehdjk.com/Article/details/gbvwjlvnj.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/ghpaximxq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/glypzvxji.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/gilrnwfrn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gvnawaphn.sHtML

[Q54] 清空表
来源：http://read.share.epnwcf.com/Article/details/gybwnefmt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/gxiojsanu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gxqdrmxbp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gcnfuwhli.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gibrlpvpg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gcxmswban.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gahslmrzq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.tarul.cn/Article/details/ghlftpvhf.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/ggmgrbjah.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gfybmpdmy.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/ghjprfwhb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gyvaycnpb.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gqmmlezpg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/gaxtdihcq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gkanhvkay.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/goppcgxdk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/giwfojett.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/glscehvfr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gwqfygcnr.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/glegiyayi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.tarul.cn/Article/details/gvkqllzbj.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gadovqlyj.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/gtoertsyo.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/geimqoiiy.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gpuagezuo.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gwauxbgmf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gkarsuyel.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gechomyyz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gvcmpsvev.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/grjerfqaj.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/gpjgerlcn.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/gqueigrja.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gylmzkwyq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gfayxhvwi.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gkywkqsfa.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gwxafdnze.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.bbcook.cn/Article/details/gnmqpvsex.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gyrazijox.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gtcoftmyg.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gqqqnkieh.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gewmakhne.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.epnwcf.com/Article/details/gkeepyvzx.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gbahowedc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gvjnlzzfw.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gmbyjdgjt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gauqqkuvj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gmlruobyw.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gcsogxyma.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gxuiuxjqo.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gofxfzinj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gqhjialsg.sHtML


<!-- 参考信息 -->