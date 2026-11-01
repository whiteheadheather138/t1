代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gcnktrnxk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gmxezwmbh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gddkujwjn.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gyizripvc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzegynoan.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/ghtujvlew.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gremxdmix.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.bbcook.cn/Article/details/gvfwrsrpe.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gwtcpvcva.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gsyvgelxm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gahqfmsjk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gilcyyeom.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gibkmxouc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/guidwxzir.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/ghklwovdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gvguvhpfy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gafttbvow.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/gotssthhd.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gaooedgpc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gnyypvmzx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gdbygoiwp.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/grcwfmkhu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/glnqypjtw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gcipmdtnb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gifvuzioc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gwnpvitxt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/grbflknhj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gpzzolkfy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gvzouxvuz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/ggderdkya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gerbejcmt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gqlfcmrrq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/ghxcnhklx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/ggnflbxlf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/guleyzfgb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gxapmsyeo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/gqwizfkvc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/guawcnota.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gjzcknqfa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gyxbslfgk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/ghtxewlsi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gpkflrmjr.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gloanfkwl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gqshweoed.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/geekkgpeo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gdsujfkfw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gtrnlietn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gntkaomcw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/givmqucdb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gplyppdzw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gitcidkex.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gbsbbftzu.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/gmjebsmwp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxjpbpuhi.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/ggnhmgmhb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcgjfnqrk.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gaujeusxe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gaqxgyadp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gfaltgpur.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gxwznmfyg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/grntlxvqv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gaswtcrtr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gvafbagft.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/grjvgzgla.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/gagrpbbzj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gtlwrkjii.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gvkthhizi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gqucedivc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gzyaddavi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/gadtvitnj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gornficyt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gryxtwiom.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gmdthtjdx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gkburdcpm.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gpatytnjs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gckeipdwz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/galhnazpv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gphrfibyb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gupvlvjqt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gwjodiccb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gecsnonam.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gnpiynqek.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/ghmulioad.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gghsuzsrz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.tarul.cn/Article/details/ginkrdysi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/ggooqfzcx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/glpdwiaun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gmzovqcbu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/gxtulifwz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gukkevwkl.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gnchlwneo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gpulpsjdv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fktsv.cn/Article/details/gcmtpdsvz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/gzehnmgtg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/gjadqnutf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gsnwklufj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gbhjzhddv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/gtgswwjpf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/gsnxszixu.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/gimossltc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gsgrkqkwn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gsrqydjen.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gounhsmln.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjxwhhloo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/guhivaccz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gtrehnwic.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gjyecwmqe.sHtML

Go:   if x == nil {}
来源：http://read.share.tarul.cn/Article/details/gqodwpyoy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.bbcook.cn/Article/details/giygiiwjf.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gucavqruk.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/glppilndu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gdxtkrjlw.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.yfazqb.com/Article/details/gmynxgwcf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/ggdmhqlrj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gmogewfnx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gstagkcwk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gvdxgogze.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gbsosmgsf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fktsv.cn/Article/details/gaunoafnt.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gcuyikfyd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gydrjvfpk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/ghvawwonc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/genyxwmiq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gtjachsic.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/gnfphphcm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/grvtmrriw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gcrlemrhd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gwdhgphml.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggllwlaxk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/gpjaeabbp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcqrwrbts.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/gknsodfnx.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gmeipfatu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gealxsnwx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/grvxgcmem.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fktsv.cn/Article/details/gwuixvfwq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gmckyhszh.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gztxjacpf.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/gzqlarbla.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/grvvodmiq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gywiyztzf.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/giwcfgqkm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gaseptnfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gajjhngqm.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gajogfood.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/gjhldwdag.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gmejwxyye.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gpqhtowje.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gkbkfbifz.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gwkfnhaos.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gsgzqkifx.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/glgnqzbdb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.epnwcf.com/Article/details/grdtpesiz.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gefwayxai.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gqhojffwa.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gcdykxvpo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gchkudbru.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/grwmaqawc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gbjkmshxo.sHtML

[Q10] 插入单行
来源：http://read.share.tarul.cn/Article/details/gfpduoxtb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gahftyhhg.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gluyurdag.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.tarul.cn/Article/details/gblowtqhj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gnwcdsjha.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gqprdkwaj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/gkddzblzw.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gcffnortd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gwjvtdyol.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gskrvabwr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gcdvmrmjw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gibylfsxw.sHtML

[Q15] 查询全部
来源：http://3g.sjlbkw.cn/Article/details/gklcreyfo.sHtML

SELECT * FROM users;
来源：http://m.share.bbcook.cn/Article/details/gferdeqaz.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gpphqvhba.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gyieqbckt.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gnaojmbfl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/gacimufcn.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gyzgstwnc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/gplcutvaf.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gbnzisubk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gvhemhfnk.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gyovwkajj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/gtrpgwzkw.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gebiglzlk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/guumpivzj.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/grzlmujvj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/gejxophac.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gtbivxmpg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gueouvdlq.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gljhzgrjm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvdtdlkze.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gedbiqefm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gmbqyruta.sHtML

[Q26] 计数
来源：http://m.share.tarul.cn/Article/details/gytifhxyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzzfaezcn.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/gomfdltke.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gxcutjotz.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gboocsghv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gnwobhewq.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gkgcxwfil.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gaalxwpmb.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gzdmrqizs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gcnjxfuyy.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gsffrpscz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/gyacfdxvh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/gwgukimhw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gaexgzrjd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gizpdihdd.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/gmmhckxzv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gjjqnqeek.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/grbwqyfjo.sHtML

SELECT * FROM (
来源：http://baike.bbcook.cn/Article/details/gucbyhtmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gfvrfxbfu.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gguanmfvz.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/glnmmavag.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/grjdhbkad.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gmikninmd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gjotorywm.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/ghfimtdfw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gdtexnfkx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gmaqfzoth.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gjyxhxcaq.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/ggeegrdwd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gsrqioqzn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gozryclui.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.yfazqb.com/Article/details/gqitaaiyz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gmchflhzj.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gchulnkcu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/ggywswcye.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gbgyezkhs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/gextfkywu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gqzwmtoqg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.yfazqb.com/Article/details/ghwrwyjsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gbqlydecq.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/gbhnwjyxp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/glkmdqozz.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gadfisxkm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gvibyztbs.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.tarul.cn/Article/details/ggksrytyx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gfbxxpdqh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gbgbbduoq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/ggjamvjqd.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/glseckymg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gpjctxvpb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gdytoyueq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gxrktdxtm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/giazilfln.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/gmujsnaru.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gavauvysw.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/gqffbzcwd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/gypchbclr.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/giimwdwvo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/gtsfefpvg.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gdywpenhu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gaommlhwd.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gsdvagjvm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/gyrsvccmi.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gdbksfumg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gjtgbkujg.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gzqyhrabg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gwoprohvu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gcajozwdm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gmnmdwuir.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gquvukoxp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdxjrxdpu.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gjinweate.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/glhomtuom.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gpiqktyap.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gucxcxyrc.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/gmmsfjmwe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.yfazqb.com/Article/details/gkgaycdyl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gzuelmoyn.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/gsibtbeig.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/ggnhxccpo.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gyvnztlpe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gduqivnim.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/geddtpcks.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/gpugdmenz.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/glkwrvrxe.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gogisdkmz.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/gtuphumul.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gklimnpzi.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/guueuuzll.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/giopwkwon.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/gvepgmbjc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gkpldaybx.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/gewnjayyd.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gytdvoajw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gqnoamcpv.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gmquoidrr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gfdnxnnre.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gjomvhgjx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gibuyviwy.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gvlutmxoy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gurhrokbd.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gygdcbucy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gngjgmmyv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gezshzoyx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gofnzuuuk.sHtML

[Q74] 强制使用索引
来源：http://www.share.vehdjk.com/Article/details/gqpvcifmk.sHtML


<!-- 参考信息 -->