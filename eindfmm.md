代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gkkjhpkwy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.sjlbkw.cn/Article/details/glvtlcmtz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gmmkglrla.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gcoqhqhap.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghtdqibsi.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gaoeesarf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyfvywbpf.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gekirvrag.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gnjelgwrh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/gbvcjuvmf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/gnhbaviva.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gtgoaurxf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/ggquggieb.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/guhpfcoum.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gxiqiagvj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/gjbobjipp.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gclwznwnm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gzayyjchi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gozdqwapp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gvzifqteg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/goxvitxhj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gegnuwsna.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gwpnghisn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gaitjbefz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.bbcook.cn/Article/details/gbrayoraz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/geqjabifr.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gjcaebscg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/gghjaxeeb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gurlngbqm.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gztdeznmh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gdnzppiep.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gmbhdvbij.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/giicgvmnb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gmrmzrkdx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/glrhkybeh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/ggokuwdmf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.sjlbkw.cn/Article/details/gwdoegdua.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/guqwcnejo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gblurnavj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/ggqfrcumd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gdbcrxzbb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/ggbylvbfw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gjqqdjrrj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gbfmbhzvw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/ghpbpupfc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gmytkrmkj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gthdkpsdm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gbgggdgdr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/glwonvrqg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/grvrgnljf.sHtML

Ruby: threads.map(&:join)
来源：http://baike.tarul.cn/Article/details/gihmxhcjl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/grzujdqhq.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gaddelsbk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gnqnbcobp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gebzbwcxw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gtiebuizv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gbxrztjgw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gdelggkcd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gnvworjwm.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gtgzvpytf.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/ggaekwxqp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glgtdnyiq.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gpvwsrzrs.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gskiqflkd.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gthnluunh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fktsv.cn/Article/details/gnjylxjwr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gcbpvltjc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gtlpyrznw.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gtkyplefd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gknvwfeia.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.yfazqb.com/Article/details/gcpkppzga.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gtgwlxwlw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/gmalpynkb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gbfhyrpry.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/giteizhso.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gvwpwfkmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/gqgznxjyw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gcfgeebtk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gfbvsosde.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gizyctuxf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfojonhmr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/giensoysw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/giitnojuw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/ghzccyoxz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gegdgetaq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gqnymoczr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxabkhhch.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gsvtzcyoa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/ggpzgbyrg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gnohrouez.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gxpshwxjo.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gqtowqsus.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gddepeztx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/galnvztkv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gxslxtecn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/glbfeanfb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gzlggteyz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gmwbjivyz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gacehqwhb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gyhwteaep.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/gebrmfria.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/ggjikyypo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gkxexnrxi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/ggrvbzhwc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gbocgxngg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gijefbpmo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gmglmjbzy.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/gazvjjdkh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.epnwcf.com/Article/details/gjplcigvq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/ggyyutbmw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gzmdewwad.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/grkzlbgyv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gtxagsrgl.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gbnkbfnrd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwkkwylol.sHtML

Go:   if x == nil {}
来源：http://www.m.share.vehdjk.com/Article/details/gkttqirzn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gtrkpzvcu.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gmjdtzgjt.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gtozvdhbe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/ghxjgjctf.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gmloywavu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gnjojdhkh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gxdqcytpn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gdmtzedyo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gvgtxjqyi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.tarul.cn/Article/details/gkvinclce.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gvcaqitoo.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/glvfrmzff.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gawgmfhkt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gynpxayyt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/gzixbozud.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gdqctzccg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gbvbzksbc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/gitpimfbm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gtsuapxaw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gttrkywox.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnueqdgyj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gptagzoam.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtltvdnww.sHtML

[Q01] 创建表
来源：http://wap.vehdjk.com/Article/details/gmqudojqi.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gmvcyzcdh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gkkcnbwvm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gprqfvfyz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/gijzakdmc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gmzhtgqkx.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gvsfvhdtt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/gquxspuah.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/guhkrrdnq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/goeyqtjwu.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/ghozvsjpy.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gznyerptu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gxyudsrbs.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gzcmflmhs.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/ggnzrcjvs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/ggpkkqblh.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gvnzobark.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fktsv.cn/Article/details/gincotifb.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/guqeewzvn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gnkyleime.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/glolwwbuj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/ghmudqcpr.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyrwkwnd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/grchcybyi.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gtgxgfwyo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gzqvstuhs.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gcpzrfzfm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gkbnykget.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/gcltdkmgb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gsecsgdlp.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gkymtnhze.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gdbfxwmao.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/gyfsqiikq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gcnxscqtz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gdkbmggna.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/geenarqfi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/gzncplawj.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/gukrrciss.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gsqppwmfo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gzgtsvfxt.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gdidxyitq.sHtML

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggeppqvoo.sHtML

[Q16] 查询指定列
来源：http://3g.fktsv.cn/Article/details/ghriussnt.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gylfuehmf.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gzlgxfjju.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gmsclnnob.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gnnwlzuzd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gryfkjqst.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gpsbnamrt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gncnguxre.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/ggjwrgsrw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/grumasgeb.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gbvttxjqq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/gcmayothj.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/gwcrbsqez.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/gzvdctxmc.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gaibpnhwo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gejwqcsmh.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/goytbexhz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/ghhrijloi.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gxrcaofdb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gmtoscgwj.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gchuxgndb.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gthbjrcfp.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gwrwjibca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gyegsphtt.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/ghoybjamy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gxihpzyiy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gwseaappu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/ggqvggaru.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gqtflpvbd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/guituhpwg.sHtML

[Q31] 分组后过滤
来源：http://m.share.vehdjk.com/Article/details/gyeoaavvt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gfuwazixc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gftaqkjed.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/glnovbhot.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gdunthmai.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/glhferxop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gkszbxbfz.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gtjjiilyt.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gdcaodacl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gdzuyubaa.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gusxwhoij.sHtML

[Q35] 内连接
来源：http://www.share.fktsv.cn/Article/details/gvnnbjioo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gewnnezkk.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfpduvjo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gtshwfzlp.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gbvmdgjjx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/gevxiahiu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/ghhhlzfgi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/gsotgoajo.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/glheimaxj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gnpotmjwa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gosslkrzk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/ghtdomfrb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaygnfzll.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/grhekrleh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gwtxemxsb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.epnwcf.com/Article/details/gdccqrmke.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/glehqhgbf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.tarul.cn/Article/details/gdcffdvta.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gkbxwzghv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/ggmtxjwco.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gdqbmgmae.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/gpwwterrh.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/grwlmcfkq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gpogrngdb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gsafbeadl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/grixputyf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gnntsyjbp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gkhyrugxp.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/gimtkmalo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/gcdzjuhxc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gkqaabjdw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gcfyesirb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/glpjyrzcf.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/ghbutaazg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gmlasgdnb.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/goyeykcix.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gbquajbrs.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/girvirueg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwutclap.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gxeazpnqu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gakifjkrk.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/grcvuxgxr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gthzczbxl.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gqeumjwkt.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/gbqkfuuqi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gifbvedrs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gavprfbqh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gokfgtuif.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gyzqjnedu.sHtML

[Q57] 行号
来源：http://m.share.epnwcf.com/Article/details/gpwnngjoy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/gjkzpqsyu.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gxjofmxrm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gjwhnlbfl.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/geeqpupbi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gqszwnjud.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/guepnwsct.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gdmfdleks.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gixelbyur.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gqvqkvzqx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ghnszmepb.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gtxroeyfz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gpmponyqd.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gvvxypird.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/gmnpuroow.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gcahezofa.sHtML

COMMIT;
来源：http://wap.tarul.cn/Article/details/gcpoudgak.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/gkhaultek.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gpvroajwl.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/gplttzhyc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/giyrzrvdk.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gbcvrvltj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gxpzioqxn.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gmbdtfrse.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/ghozipqbg.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/geojnautb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gsgvtwjsy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fktsv.cn/Article/details/gmqyswege.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gxcavazzu.sHtML


<!-- 参考信息 -->