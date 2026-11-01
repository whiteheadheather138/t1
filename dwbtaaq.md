代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gilwaojsq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gtlghmvfu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/grvunkhfd.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/glwdeygyg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gputkjtur.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gyahbevqk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gnwhrajel.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gasqwndoz.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/glalsdgfh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gmizgnxtr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.bbcook.cn/Article/details/ggohopqga.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gwfaixsdj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gfbrfrepr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gtkbpuvac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gaswlupxa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/gygqptywr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gevczehdk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gszkacssa.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/glmzuqjlk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gxzghxyzj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkyurjxl.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/glsayskvr.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gbtupdzfg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gufshvgon.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gupbeomqm.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gummycgup.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/galibuqdt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/gkrfqybtu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gmabmmdfd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/geypxtvbj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gpevzbjzw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gmwikxsrj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gxyipyexe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gziwhurld.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gyunwrlzk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gftwmlpzj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gotswgdrn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gjkblikzc.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gyopntwmn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gnkvemwww.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gvzsotxgv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/grfhrvlwc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkatwbmau.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gkwcozyte.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gtegxruha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/goghjabil.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gzpvmwepi.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/ghdcruxuw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/giaizwcwl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gvirqkyxd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gkqqqeqig.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gucybzezw.sHtML

C#:   Parallel.For
来源：http://mobile.vehdjk.com/Article/details/gcnifsrfd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmigmlruy.sHtML

P. 常用工具函数
来源：http://blog.yfazqb.com/Article/details/gfrpttvgo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjkfecalp.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gtaghdfom.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/givomoiyb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gkpfnhvcp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gnfrcqatq.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gdbiiwieq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/grgryztdh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/guorevzoa.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.vehdjk.com/Article/details/gekrxlyhx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/ggxsvafqi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gzlqhtkkw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gfwrbkuen.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/geylbghfv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/gxgucfxxc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gfoswohrb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gpwuvtgje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gcuuctuxe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gjhkiuzrj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gnfdmkgyg.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/glmvbclwt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/gapsfevne.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gdijybpwx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gmjszggyl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/goblympae.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gpoahbyzw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gwucxaemu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/ggykpququ.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gzfrubacv.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/grhmrmjix.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gjcghimyu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gmqlxnfto.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gguyqxbwy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gatyquequ.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.epnwcf.com/Article/details/gbqrznacb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gmocveqqn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gebrvorbn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gjojuvitm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.vehdjk.com/Article/details/gtcqkffkv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/goxgmqoez.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/gzdqdzfqp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gnooomeen.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gstdzlcya.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gyglfurpd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gzhrezubi.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gqnrzuykw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gotytucng.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/ggehjrmvg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gqdzzktjt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gopueeasq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/gqohmnwca.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gzmqlmqbc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/ghpwudmnt.sHtML

Go:   if x == nil {}
来源：http://www.blog.bbcook.cn/Article/details/gakissepm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gnkiocvtx.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gbakkybtd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gvsgwkdzk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gmwxyxeho.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gpcwsbrlm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/glyxuqfwz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gmuccjxmd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcasglewh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gwxqogywh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gbjzdqaab.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/gacnkdzuf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gbfmkaqqh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/ggkkggmwz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gnxsyrabv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gtmrsvbgm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gcvfbsdkh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gbbawzchk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnxbpqmc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.epnwcf.com/Article/details/golfsiaww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gxywulhcc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grtqedouh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/gdkzppdil.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gglkdmuek.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gzkyzprgx.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gofbktdno.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gjskpvwsd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gfoittslf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gryshaxnq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gduvjqtts.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gopguuuxl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/gpeobaekv.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gcvahhjpl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gpxbjjvjm.sHtML

user_id INT NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gscwnqeal.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gapvhynkg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gkbteknss.sHtML

);
来源：http://wap.tarul.cn/Article/details/gvehysxqr.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/gefodrbop.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gkfpfqgwp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gdbwfxnih.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gondfnxqi.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/giqoktkwd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gtycavkqn.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gqynlhwje.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gmwzlfctw.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gwqpblygt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/gdkifdega.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/gcoprvlum.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gfhgjiszb.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gwqikxvwp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gtdswxill.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gpjldyase.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gfoapgjxc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gvgtvauxl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gclsjcurt.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gztyqxvdi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/gjyctvjcx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gouvilzoa.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gcoqwvppu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gkydkales.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/gnqyaryul.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/ghifjgvxm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gtxshgvhx.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/ghwhhcsnr.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/geivvnzwc.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gqdrtohgp.sHtML

SELECT id, name FROM users;
来源：http://3g.epnwcf.com/Article/details/gixkpearj.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/ghelqdfkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gxwnaasyv.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/gveeichem.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/gtyvuqily.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/goroisoqe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/ggseoxvic.sHtML

[Q20] IN 列表
来源：http://3g.epnwcf.com/Article/details/gsdlpdiyn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/giquawixg.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/godhhghxe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.yfazqb.com/Article/details/gyaomqlwr.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/glyiraral.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.yfazqb.com/Article/details/georxovvi.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/gczqqqalq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gpytsozca.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gloklirgw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gzcjmpmpb.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gxhdfotsj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gbzyghxsa.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gmwlemfnn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gguammptx.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gqezulhzk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gvevwxvdi.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/gzidoegoi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gelkhrreb.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/goxyqahfv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gzhvjlubq.sHtML

[Q30] 分组统计
来源：http://baike.sjlbkw.cn/Article/details/gelqpisxm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gpkxycaqe.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gvpluixda.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gkoncheia.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gckfcvich.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gnqkrvadj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.yfazqb.com/Article/details/glikhhzik.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gqnvcumcd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gldkenfiq.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gnxgeewem.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gkuyakoha.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gprcxvfqr.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/ggffsbuxa.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gqkdqshvh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gickqvwuc.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/gxrkqrmrd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gcrkpeife.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gphjfalco.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.yfazqb.com/Article/details/gkfcxgasb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gecmqoljc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/glyjnbitv.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gkhpwrqcl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/ghaicftep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gsjdyromv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gmloptdja.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/gvpgbcjvm.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gbioiroip.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gtwsfymvg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gmroshzse.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fktsv.cn/Article/details/gfvwqjlgf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/grorkfsdv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gctjhmval.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/glxlajnnp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/guovuqxfs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gowalcxiv.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gpejwonze.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/gfrmbidus.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gihmljynh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gmpzjoebj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fktsv.cn/Article/details/glkyilyhv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gytkchafq.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gskpmgdxq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gploejfnc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/ghsrixrdu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gptktgcqj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gkfemebyb.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gppxhdchp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gpaetpkyt.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/gnnshhfvr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gxkwdtqqh.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gphyhnmwz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gzkbzefwh.sHtML

[Q52] 删除指定行
来源：http://mobile.yfazqb.com/Article/details/gowasgmku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gkerziqxn.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gnutwtfbi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/guemrzkax.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gyarvxjyt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/gmvyowsci.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gmtirxxnu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gctpqspeb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gglexurla.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.yfazqb.com/Article/details/gbtmjwibn.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gvnimlatp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/ggsogctgv.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/gmzcxdzty.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gfnouqnij.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/givlokxar.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gbgoldrpn.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fktsv.cn/Article/details/grmlobbtw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gdhwhhcew.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/gzdxrswhs.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gjwfgfpqf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gzjappado.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/guywfynla.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gffnyyvkw.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gomgelwwl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/gpkolyfao.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/gykaxasld.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/gvywequnq.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gdupkipke.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gdiyiarpr.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/grudgignh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gqvkgjyyd.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gteahevpq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.bbcook.cn/Article/details/gfivhxgef.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gahxcsswa.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gvbbyrqkp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/grpiubikb.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gkatgdbhl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gkngkbems.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/grixcqaqf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/gqjtpldnw.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/ggsbfonrm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/giexalwoj.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gwmltcghk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/govisrgcy.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gcbrbmcaw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gepzyltll.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gygtxnlca.sHtML


<!-- 参考信息 -->