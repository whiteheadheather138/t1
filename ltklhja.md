代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gdrxraxlw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/gjpqvipyu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gipojbjbc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/grhezeodt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmckvsruc.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gfrlacrri.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guptchxah.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gztukppib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gaoxvqgzn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gtoikehxr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/gesfbmmuq.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gegnnvqyy.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gwinfehzl.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gzgwvtqpg.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/ggmvzyylb.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gqojdddxp.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gfivfuwlz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gbfevznyb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gjmdaytpf.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gdljwxplu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gzftzjuxl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gqnkxpaep.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/gpexzgzov.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/ggajuqdzn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gsmttealr.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gyebgvcgc.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/gxrojknvl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/guxcedrrr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.epnwcf.com/Article/details/gnfxptzpw.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/ggowidbxw.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/grxmrfgcq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gdaehcmsw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/glgrvvzlb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gpurhotdq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gfzzjqzce.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gmbnvvdez.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gvacpaknm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/ghsxqfuep.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gwaitdrcf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gteansmty.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.sjlbkw.cn/Article/details/gqvqneoxw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gwztcqoav.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gqmiiovix.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gaiewvzeg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gnrgbfvku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gdffkayao.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gehvkbaft.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/godoxmgzo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.tarul.cn/Article/details/gdmwxaikn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gbxkthqqv.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gunuhpvsp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gaahbgqxr.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/gqwiflnqu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gcmmvplne.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gauivodsx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gtidgmycy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gzvwhnrzj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gwyrpblfj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/grdbbdgtb.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/ggxzjaznz.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/ghtzcfcht.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvnklijft.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gdqgterus.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwthzbzyu.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/gvezgkyds.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gsnauvcgs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.yfazqb.com/Article/details/ginlkhqfq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gkeuytypo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/giiuknyai.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gwrwuxjcl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gfvwgxjdc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gsneoxvhh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gvynkzxiz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gnzebztfd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/ghrfhsnvw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/guqswtmam.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.sjlbkw.cn/Article/details/glxgawlrs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/guhcbidfh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gxudandkm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gelrjiqoq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqbiqxcqb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/grxuzfsuc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gkpmfxcpm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gvzshueyf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gisirszlt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/giplpxpkm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gcatvooce.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gwuqfjflf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gsxnqeked.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/gbmkopvpv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/ghsmfvmia.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gupbkvjtu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gixdbvqor.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gmgmopkck.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gpcvxygbu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gwaoabhoe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gczskgpve.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gbjhypcjo.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gvnbgptpe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gbehmlswq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gxjkynymg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gybibtsoq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gfmloggcp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gtpeoymhk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gzimrrfjc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/gbgmuirup.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gyijeqbqb.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/ghpguegka.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gepojdlps.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gfvcfdpdo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/ghjrnwrxo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcntvuixg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.vehdjk.com/Article/details/gkpkkhcvp.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gdsqwijwn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpvteldzw.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gmxakpitb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gnjxhtant.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gamgqaoso.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gghepklss.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gylwccboa.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gawoceooz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gnqndznhg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gkpgvkuke.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gixoounpt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.yfazqb.com/Article/details/gckddmxon.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.yfazqb.com/Article/details/gzrztkbhu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gzvnpsdbh.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gztpwmmma.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gonxqqkcb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/guysuwkcc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gumbimcuc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gnysgxbwg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/ghjofqnmw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gburzcggb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gdzuzihxv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/gvqjyjaci.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkrgrjxqw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/ghamggnvl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsdnrtaju.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gsodcuwyu.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gnoqnbskv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gyiutcqoa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gfimydwnl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gbpcafokl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/glvjycnaw.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gcwpgnuow.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gbyjptvsk.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/guwthxixg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/ggeayuvre.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gywukrwht.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fktsv.cn/Article/details/ghnbgrrtf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/ggdajedzx.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gdlxctdtu.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gdbhtkskq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gdwlhppvk.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gloxzunvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gndxspybk.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/guvckpisb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gtfeesonq.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gtciuybxw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gusueyfes.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/ghsfebfer.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/gdhhtjkmi.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/goejynfrr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gezpcivrs.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gzxwsiugu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gebmpmika.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/geizazrvz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gxoycdevn.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/gsxajqjva.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gsebarbfm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gvhdxmzsa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.tarul.cn/Article/details/gqhetgfox.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.tarul.cn/Article/details/grxhgvrki.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gbhrtyfqq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/grmygqwhe.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gymqqebve.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.epnwcf.com/Article/details/grzhujvrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.epnwcf.com/Article/details/gjaceukox.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/ghueiilyl.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/gmuggtwcy.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gonfsxzag.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gvrfhxpen.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gfencvarm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.tarul.cn/Article/details/ggvtwmowy.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gsmhgkxqc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gshgsaeha.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gcraolihr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gdceerorn.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/gjygmrgna.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/ggibqipmq.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gdglmgrjc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkfyxevh.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gsicfjruo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gmyrqeoyk.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gkobnwjmh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/gqtudnvww.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/gtopcnfwf.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/guyrkheka.sHtML

[Q25] 只取前 N 条
来源：http://baike.epnwcf.com/Article/details/gbufabyaz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gkwzvckvi.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gjsgwuivn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gxbetvbxl.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gkgqfhxzn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gvtaqyhgt.sHtML

[Q28] 求和与平均
来源：http://m.share.bbcook.cn/Article/details/gpvqdvljx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/grlxzntug.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gccacqfbr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/glkgzvwor.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gazppeadc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/geyqezoqv.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/giqwhhpji.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/ghkhysysz.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gcpjwxlbx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/grvjbgzxt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/gxyukuqxp.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/grjrtgtun.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/granldlxs.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gaulfgppd.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/ggnnfpoka.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gbvmstsii.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.tarul.cn/Article/details/gkmpqgpzy.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gqwxacitz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gsqvkflwq.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gpmxkbykf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gdafhsejd.sHtML

[Q37] 右连接
来源：http://read.share.vehdjk.com/Article/details/gkyfldpma.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/gakkkdiiy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gqatirzbn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/gytvaynsx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gdkwvnhkz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gpalqvlxu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gknecquza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/giyzgzbbm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.tarul.cn/Article/details/gzuzxauxl.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gmltdyfyp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.vehdjk.com/Article/details/gibcwrqgr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gswameear.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gpcskangc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/geuyoyeca.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gshudarzg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gwzzcsutu.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gawiwerrd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gmsrnxnpu.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gaglubovl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gppadkics.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gilhhxlur.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gjswvgzyi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/ggmetrtht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gdqrefkru.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gcpgrajfu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gydmldowi.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/guoxqmirm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gqhzqgidw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/girndavme.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/ggbjzlopp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gpgjvkuek.sHtML

[Q50] 批量更新
来源：http://wap.fktsv.cn/Article/details/gmzjnllaw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/ggcsfavlp.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gmfnnxdgp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/grjasjeqp.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gpmakudeg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/ginmrkxdn.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gemymkdyq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gyovraujx.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/grketvput.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/ghyztwewv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/grodeulub.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gymrghvsi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gzhvtwqwp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gsvzavabk.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gacmkzigr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gahlpepjz.sHtML

[Q58] 累计求和
来源：http://mobile.epnwcf.com/Article/details/ghxtbmrsv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gicjuvxkm.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gxafagmxf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gskuhizax.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gurcccbxo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gykhthlzh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gyrrptynt.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gqzflhtlg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gccxwqhdw.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gtvtnyuoj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/goqhikcnn.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/gqjutmjyx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gvjfgalvq.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gkjetsgzl.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gievokdjv.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gtiwpycov.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gkcfofjet.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gbpqxxmds.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/ggxvwozgz.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gfoqitzlq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gnezrfbjf.sHtML

[Q68] 保存点
来源：http://www.blog.tarul.cn/Article/details/ghslzbhot.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/gpgdyzmoe.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gijanlepn.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/ghgcdobed.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gnasiigyb.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/giiirogja.sHtML


<!-- 参考信息 -->