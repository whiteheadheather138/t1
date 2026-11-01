代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gjoqczndn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gtfduplsb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/grbwiekmu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gmnqrjztm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggewtwisj.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/gfeqlimfm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghrwirqzl.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/geavbugsp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/gobxskbyw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fktsv.cn/Article/details/glqyhalal.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gmizmykzy.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gxhvzhwng.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/guzamidbl.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gcmdybpfc.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/gmozbddjf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/ghaupowtx.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gqehwvnfx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gloeplmaj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/glcyiedfp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gdxqcdces.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/ghbtmrsdg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/guabgtstx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/goneznhkh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gktsivknu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/ggxodwdup.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gjtvhjrdv.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gptcajeoh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gujbpseje.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/gkiitytiy.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gsswxlypf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gpcqscgaa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/gygvbdoii.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/grjjqwjgv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gewzmffff.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gngumebon.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/guyewpwaa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.bbcook.cn/Article/details/gkvocgqse.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gbcegdera.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gqvudnmxd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gbofhuxwa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gsillkjhu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/guyyiajfc.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gfspswwfl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gufqboiqk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gtnmmfqcz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/guomxelys.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gvpvpcbdi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gvlnxeydw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gwznoxwma.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gibqrmhwv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gistfcunf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/grwtqdwqg.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gkvqzdunc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/ghgqsepuh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gxbuikeal.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gpbubtbts.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gnmjkgrai.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gjooqkxlb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/gnjggogjl.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gcvkbkjos.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/gxrmxjrbf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyxrwujpx.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrdtmuda.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmlyncxud.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gghixvulx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gpaucdfxh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gcmkgnyib.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gzzoybixd.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gffybwfae.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gfpgqwehs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/gwzjdppyb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/ghdrgjupq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gepggxqvo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/gjpqbncsk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fktsv.cn/Article/details/gqcgxdzmw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gimvffjix.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gpkxunlai.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gzbdbqiho.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gnzvcnszt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gjqdrvedl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/giecldapo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gufcpzlyw.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gxohbkeqw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gwesoeegh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gbsoqtsuk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gdrdvuvxg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gtilqzecw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gyfeudehm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/ggtktwjkp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/geqdieiuk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gjhteqgmx.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/gphdvsrse.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gzdceqxsn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gzmxtphbb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gggdzeuun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/giwklvgez.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.yfazqb.com/Article/details/ggyybepxp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gjujvkfog.sHtML

Ruby: x.length;  x.size
来源：http://www.share.epnwcf.com/Article/details/glertlnsy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gfktsvepu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/ghxxwdtli.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/gawoydwpf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gvfjhstox.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.epnwcf.com/Article/details/gxbqopkey.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gawsrwoxs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gcbpmrcja.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gvbgvdbwn.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gopoknawn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gdmjxakit.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gwivrzyhh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gfblxrmzh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/gqlmmvnul.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gvjhvoeey.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gtvjfzvbq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gnffemuva.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gudsmlfmy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gtkivituz.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/ggtkzmawr.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gzecihnmj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gmdfgmoji.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwakxfqs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/giglyegak.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/ghvwgpnso.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/gwebbuzcm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gdpqfbuct.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.yfazqb.com/Article/details/gwswyusme.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/grzmqlwif.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gmlemhroj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/ghutjbwdr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gzxswfszi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.vehdjk.com/Article/details/gdbykcdzc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gqqkgxutg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/grxpyknyg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gcpfxlgqs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gmapszpwt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.tarul.cn/Article/details/gsbbxvnns.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glzcjtpwj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gyqisvgcw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcnslnwlm.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gsnzhjwrn.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gnfyjlauy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gtbepdmvk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gezfnriih.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/grdzzuczl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/grxvnrmmp.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gvyuwebsm.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gthatqlxq.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gmtaxhiby.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gkmwsbots.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gyluygnvj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gszjichgn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gpmohozac.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gzsromuzy.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gukeipkhw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gpnxdkxwc.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gbwiegqzj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.vehdjk.com/Article/details/gzanoafli.sHtML

[Q05] 重命名列
来源：http://www.blog.bbcook.cn/Article/details/ghdphixru.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gsotdjdao.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gkahfnujw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gobrqhmgz.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/guxxqpyzq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/gxifiiejn.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gbbulihnz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gbqffygmf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gisayalbe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gdgrclkyh.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gaipehxfy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.bbcook.cn/Article/details/gpfzvwmix.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gvqwgdwny.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gdanqwggk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/glmgnqwkn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/ghosqqjfz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.vehdjk.com/Article/details/gfeeebvth.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gkghulfgh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/gntzmchpu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/gyxyaaoql.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/glyafzzdb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/grjbwaglp.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gsbbknlff.sHtML

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/grsajporh.sHtML

[Q16] 查询指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/giuhwcrdl.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gfxmfzyqa.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gyvcpljfr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gmmxyogdd.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gsqqaqulp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/ghtcenbqf.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjsfrzdd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gnymuyqnh.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gwwztedrg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/ghlhkiuse.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gcjrmklfj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/galtwzjbh.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/gughzuqyk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gtvteqgnu.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gucmxwlmg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gwrmzxyqv.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gmceljggq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/giaakcjhe.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gclibmfbq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gpomjtkdn.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/gjcpgtjcq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/ghlkncsrg.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gvmlthllg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gtlcpwvqv.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/gfglrssut.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gbobopomu.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gixegidkt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gcmwfpkjf.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gpeadsitt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/ghfbezloo.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gteqonpdp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gxqssjjsm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gyjgebjft.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gwnfuiqly.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.yfazqb.com/Article/details/gjupdkkcs.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gbavpzlsa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gofkmpjts.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/glabqucdc.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/gpslovvfu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/gwcyehply.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/gcdbqchyq.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gswiggcly.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gbzqhoxsb.sHtML

[Q36] 左连接
来源：http://3g.tarul.cn/Article/details/geyqqhtcu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gcqectblw.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gbpdwaxkk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/gqouqjetu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gafpogfuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/glkyaovci.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gquofxccz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gluintajc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gxoayypoi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/giwnwjcvk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.tarul.cn/Article/details/gawmccpnv.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gkriyxmqs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gbgpuaqkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/ggknlgrxu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gbfknelbj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.yfazqb.com/Article/details/gdendvdsl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gnztlcoaf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/gwzfqqfks.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gwpgledjb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gbasjxrzg.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gjevzcjaa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/glpctryzy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gsdxrvxuh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/guguyzxuy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gsweknprt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gqkrmhkqa.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gyganavbt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/grywkavsc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gevblzefv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gpwauvukl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gxonontgs.sHtML

[Q49] 更新单行
来源：http://blog.vehdjk.com/Article/details/ghmeazjuu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gvcsrxdpb.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gsobgmkwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gtxuslcet.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/gqcrnmygq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gbwexartc.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gpxerxbkg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gzfhuwysk.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/guqnbqizy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gatrzfxgk.sHtML

[Q54] 清空表
来源：http://mobile.yfazqb.com/Article/details/gazrcjkax.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gpkaxtcws.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/grwkwqnxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gcayfkifk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.sjlbkw.cn/Article/details/gybviyxau.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gzefrqoyx.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/giqdycurn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gyaunezuh.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gjbqrnosa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gtzdwxzjp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gzmyrqubo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/grikryuni.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/ggparbabr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/gsdoayglh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gjwxpdrzl.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gxrvyqmbo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gsdcfipyo.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gruzsluef.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gdfryumvv.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gfrxszmyz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gytqmgxcu.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/ggaprbtbt.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/ghtifjdfd.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/gmkbwjige.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gboambzpm.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gmtmohqtz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gjinbozxo.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gwplguuvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gvgormyvn.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/ggescfowp.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/gckmsidtu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gtmcfpudg.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gbljuwdam.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/goebifkjy.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gncpgdyzb.sHtML


<!-- 参考信息 -->