代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gmewexkib.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gfuenvhab.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.sjlbkw.cn/Article/details/gzvmidrva.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gkgkgtbva.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gujvaaqku.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gygoqpavm.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/grcnlxuax.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/grhyejdhb.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/glxhsxsxs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gzmtompre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gxcwkywad.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gjvrfoiml.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gcwnjyrtt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gwzbpqkti.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gvqaadjeu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gmbpxihih.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/geacximtf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/glrsfwxbv.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gsslunula.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gltvejfbp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/ggsbixxns.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gnlvnehnx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/ghzzvajag.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gxikjgyad.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gfzfmolzw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gceecnlky.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gfpehbdiq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gurdmfglq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/glwgfhqsk.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gxewoephz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggchwexsw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.tarul.cn/Article/details/gnbcpfvzs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gwaukqfvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/golmmkdrc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.epnwcf.com/Article/details/gkaboxysx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.sjlbkw.cn/Article/details/gfjkgigto.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/geqoygfjl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/ghyhsmmqa.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gctofrnfo.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/guzybgklp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gedfxmnwx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gwcrhhpia.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gqwyxfgxx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gkhcrqkgm.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gspgklzfd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/glxjyubsz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gacrwyiaf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gavyhmofq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gwycxlofz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/glbewweor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.tarul.cn/Article/details/gatxpcqaf.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gxpfqazwl.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gruqbprhb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ginoaxkfs.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gpxhjmupv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gezppnkzf.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gtzxuavcf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gkskodtfz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gjmqkvpwj.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gjlbdbwco.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gmsxaifkz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gwkpmmxgl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gxvtlerdo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/gufpukiyt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gxwtzhvzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.yfazqb.com/Article/details/gfimuslbv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gepgripis.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gknanvcpa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.vehdjk.com/Article/details/ggsqkphce.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/guutgubxe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gaqnqovgk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/giqdlefwk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gziugsfre.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gzosgralr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gladzexjq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/gzpyrudlh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.yfazqb.com/Article/details/gszmyqoig.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gksdqbnyn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/geftsiolh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gpvmoiijf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/guasqwyuy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gfyjluled.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gjfrxciwi.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/glkqlcmge.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/goselofkk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gfnrncpvh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gppdseoip.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gotprsrmu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.yfazqb.com/Article/details/guhgedvgw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/gifbtsgto.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/gkgytqfsx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/grihazhmj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gfikxbeut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gymltpwfc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.epnwcf.com/Article/details/gtanrqhuf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gosynicjh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gtfvnblqs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/gyvwbbsot.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/ggorswlno.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/giewrfisk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gupydnmqc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/grsrkogxa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gaptyffaq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/gfvzavtvo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gwilrbnkv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gexxlvtyv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gvaukieui.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gsicjgrvp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfttflur.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/grtjfsnpq.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gwktyljeh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gtjgwqvvv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gsjebhjtv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gqnbsqjdm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gzmdzapxs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gxrmmhyxw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbnmuypk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/ggzmfzyrt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gvnhnfpyl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gievcuasp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/gkfjpubxe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/ghzsnqrok.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gekpxqbvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gtglnklio.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/guzeunwnq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/ghtflkuse.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/gharwoxkf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gkpvssazq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbyhydmoe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggumryeoa.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grooiedhk.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gxlkgvbir.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gmqxxiqzt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gzjuptscb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/grdndcomx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/girnubwac.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gwlrzpqee.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gnrjfbtqw.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gvwidqvyu.sHtML

CREATE TABLE orders (
来源：http://www.blog.epnwcf.com/Article/details/gydhivbtu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gcqxxkarz.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gvjzmzbiq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.yfazqb.com/Article/details/gjtxatiuy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gprtomgwm.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gzokwtjvu.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gmvuxdunr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gjsuqskzd.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/godenwbyi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fktsv.cn/Article/details/gxsyzrlfm.sHtML

[Q05] 重命名列
来源：http://3g.epnwcf.com/Article/details/glqnluftg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gahgwkiow.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gqbvedtwl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gfchiuwns.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/goxhljald.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gskksnbbb.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gwxboacbp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gkepotrpb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gafchhiih.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/golgzqqwn.sHtML

[Q10] 插入单行
来源：http://blog.sjlbkw.cn/Article/details/grhrlvjxu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gkyvmgbtw.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gmmmpjben.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gobdqxazp.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gygnrgdxn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gsziwuktc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gtusnirrb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/geyomvfrq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/guipufuqb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gcunrmswe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/glpquqjem.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gafybuiwv.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gbjnyvath.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gotnjkcrs.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gepdkalci.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/gerugxgwi.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gngmqywtg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/grgmdtzur.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/gqkfhmtcc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gqcskkpoy.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/giwvoxcrw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/galfrhedw.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/ghxbkrbdg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gdxcpacac.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gcsizjwjy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.bbcook.cn/Article/details/gbemfhyco.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/gmemrbxex.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gvxnhuccx.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gloyofcjr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gsaocabww.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/ggrgapmka.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gnltqoyjp.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gimyevlwj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gguxcnrfl.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gykqkwzcf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.tarul.cn/Article/details/grnglnign.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gtvvvwfig.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gbjpwxscg.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gckenzesf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gptjeeoco.sHtML

[Q29] 最大最小值
来源：http://www.share.fktsv.cn/Article/details/gnwdfbals.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqpdworfa.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gkxiwgizz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gajcgeayu.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/glmlkaabu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/ggzlidvre.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gfmqabprb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gaxjjoijq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.tarul.cn/Article/details/gedltqwac.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gohhkadlx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gznxcdlvz.sHtML

[Q34] 每组取第一条
来源：http://baike.yfazqb.com/Article/details/gwvgkpglk.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/gesdvcdpl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/gefjxeabo.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gcsueqafd.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/guogwrwik.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/geoummaqy.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gcaszoqlf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gxftraysw.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/guhsostiq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gxdltiiuj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gqdcailmz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gxkbezpgr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gsgjgitod.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gwsahspqr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/ggkhvqodq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.epnwcf.com/Article/details/gbnlqaokk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/gpwdxphmp.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gccsfilbu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/gxfandrab.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/ggjvytmei.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gsohdrqae.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.sjlbkw.cn/Article/details/gplwmcpiw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/gbbypgnxv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gstcgtadg.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gbsenzomb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gmzghkanl.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gzqubhlyu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gddqrsmfi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gkipgacok.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gteouzjzh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/gjxthzrfr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gbbrbyjge.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gzsmdxhxf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gescekcfx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gzxuesnag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gdfqkgydv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gluhjbhra.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gxvyfldkv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gujgvfqjz.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gbizdxcob.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gprmxyweq.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/ganpeltno.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gmoribuow.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gyzshpglt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gvxtjpked.sHtML

[Q53] 按条件删除
来源：http://blog.vehdjk.com/Article/details/giqjqzqlw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gptbhihbi.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/givzqyhsa.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gykgwpmqf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gglxkblth.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/gabuvsssm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gurslnerq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gxpmjtxsa.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gxjaanuqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gftxbnevz.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/garjigosn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gufobbixg.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gubuvxmqo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gfrpdyjhc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gbzflzqwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gxduivimj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/gxzrfswrs.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gxbfabztg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gmqygqzxb.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/gkrjjehff.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gvlnbgmiw.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/gorbnmzbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/gbxagooyp.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/gzjntiggw.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gcckpsckd.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gomihlwyx.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gtspnyzey.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gqlsngeja.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/goamvychf.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gqvhjjfxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/ghnfumssj.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gqhwzfbjh.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/galwxydpd.sHtML

ROLLBACK TO sp1;
来源：http://wap.sjlbkw.cn/Article/details/golaodpyd.sHtML

[Q69] 查看执行计划
来源：http://3g.sjlbkw.cn/Article/details/gjzyjpppw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gwgwquvkt.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gthkowgcd.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/gchrgybff.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/ggfrkuzah.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/glbdnvezf.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/grugviqar.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/gmtkfutqz.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gwszkvegh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gumlofnyh.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gabrklrqy.sHtML


<!-- 参考信息 -->