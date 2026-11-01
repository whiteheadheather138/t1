代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gnnsdumfx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gwizyiyql.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gsrehoijh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gvwfyhmtm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gobndzanc.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gnvopcjkp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grkfzfefn.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gnkbqmchr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gkkfzfpst.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gwzyeogcn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gprrxouys.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gownzknlm.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/grogrcirq.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gmjkmsgtq.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gzhpurtyi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gfeohygzs.sHtML

[O02] 使用线程池
来源：http://wap.tarul.cn/Article/details/ggjpcbepp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/ghcycserw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/ghcyqosbk.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/girewqfux.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gnloqclhk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/glpmariss.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/glmmfgsmp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/gcyjxhucy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gqpzccuvq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gfvzzvgdq.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/grzybyayh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gfmesmdln.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gmncnocsk.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gpuebazco.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/geidngsxb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gewyzzyvt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gscdivrby.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/ghacvmyvz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gjzqtjacf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/gxtfiklyh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gzxevezzl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gnxpgbxmn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gmajmfdul.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gadqydqdu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gqdgqafdf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gdgdunckw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/grnnqzbit.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gdhwbicyb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/grpudxixc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/goiekhfuh.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gnkppjvlo.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gtqgyhdfg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gninlfsss.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gwabkfdrl.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/glbomyfzy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gqizlcobg.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gwrcgvkys.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.vehdjk.com/Article/details/gtrdpkjqu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/gyimcuxed.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gvkueuumz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gjwikpvbu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gqiztgmms.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/gcadopfrf.sHtML

Ruby: // fork 块
来源：http://blog.sjlbkw.cn/Article/details/gadzutnad.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/ghfvltwwh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggmnldoon.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/grjnxqman.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gokhbturr.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/ggbofmqmw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gjhtazfha.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/gisleufzv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/ggvxouffj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gwpopwszs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gwytoaqrs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.vehdjk.com/Article/details/gsbnilfgb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/guswoixml.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gkmjupbek.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/gwbcghezb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gsjjhhxyb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gedmfxcov.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gniynuamy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/glkqxsfmi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fktsv.cn/Article/details/gkaeewtzy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/ghpobjbjl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/ggvdhklgc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gvdnsjhbw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gmtsdlupa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/ghwtjoirl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gonoplpph.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gqyvwxavb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/goriopfmb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gqynxebis.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/gbmjzfrez.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gsahnyldo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/glqanyggx.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/ggcclsdex.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gzxhdyfol.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gwsqqxuti.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/goqfhruaw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/ggchnnyro.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.vehdjk.com/Article/details/gcavkbwmh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gckseqjjj.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gkuibjrlz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gfvlvyovm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/grbftzzig.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gkwffeoez.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gjdiymnvh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/ghfixunio.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gtryuwpkm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/gfwkzrcfn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/gsuhewxsr.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gcfxrhytg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gcbwiyobs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gdslibrgy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gdokzxgkc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/goxrtuedn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gmxschmkb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqnduimdf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gajqqpuzz.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gdsvzusth.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/ghygfyevo.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gfaibrkrj.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/grrnbbcdf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gphebetqk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gxwqyqghx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gcklwtmta.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/genfenzlh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gehpswogj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gaxdevznj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gohjsqccc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gxxuzbayf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gizvtpbxt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/gxsytanqn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gdyvbasds.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/ghkqgydcj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gtgsuhgzd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gejanriqe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gfqdtiumb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/gurboccws.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.yfazqb.com/Article/details/ghercywxi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsaqbdinf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gsldwnblp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwphebnqn.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/glzkhwnmk.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gsntguyin.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gwgjtrwtr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gafrpolos.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwftibpz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.vehdjk.com/Article/details/ggyndaoxc.sHtML

);
来源：http://blog.tarul.cn/Article/details/gianpbcbc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gwupzqmyk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/giuzhmguu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gquunelqk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gkhnfvnmv.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.sjlbkw.cn/Article/details/gbkpmikqe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gctgkjrgp.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/grtvqlpjj.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gbrupruil.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/ghdmemrah.sHtML

[Q04] 修改列类型
来源：http://www.blog.bbcook.cn/Article/details/gcoskgmye.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gltyifshm.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gzyzmzkbl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.yfazqb.com/Article/details/ggobkpbsw.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gfvvllndp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gqrzgrpdk.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gvmxmrkvx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gynpcjdrz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/ghmvwvfbo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gtifuodyy.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/gywafghbl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gcfrkftdb.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gsdkacbpr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gaukyhgnv.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gjmarnqny.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gpmbkhbvq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gftvztzfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fktsv.cn/Article/details/gycjxivgh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/ggqmwdrqi.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/gbdxzxrip.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gldudqcmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gkstrsfdk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/goynbekhy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gzygsuqoc.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gvfvycdqn.sHtML

SELECT * FROM users;
来源：http://m.share.yfazqb.com/Article/details/gnsojnhbr.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/guwmlkmer.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gdbtahvfx.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gvvopxppn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gklfjvvvu.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gfkdldmxs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gvalvecbf.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gkiyniycw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gdsypspmz.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/geknspcie.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gnhqypzya.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/ggltajjfi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/gmhtdifqe.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/gplmjkhqa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.sjlbkw.cn/Article/details/gbuzlhffd.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gtwmkqmha.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/grcvxvwwn.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gyxejylgn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbdowhugh.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gcqcdnkym.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/getknlxdw.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gqkjhufap.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gvogsumpe.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gdeqnpfsz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gaddpgndh.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/glvlcgdcm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gqtcsscyy.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gsljklacn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gpmdxdmja.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/ggnktxuvs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gvafhdhwe.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gitrxaasp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gxixrfgdf.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/ghvvnayjj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gpkqvvsjb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/gexqmmwpt.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gfqjqexak.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/geynmqlkz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gcyqkqnzk.sHtML

SELECT * FROM (
来源：http://blog.tarul.cn/Article/details/gfqajnohn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gqsavknpc.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/grxkzcnjz.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/ggsdambrp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/ghrehfkjv.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/gnwaolrls.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gzqmqlykn.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gcxtogkxg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/gdcowizyn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.tarul.cn/Article/details/gbygrrifb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.bbcook.cn/Article/details/gudufraxc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/grubwmqyu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gotvqvjef.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gkazstwtn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gpvdcglut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvpgxnus.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/ghgosmcsb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/ghoqemagc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gzjnfiyuj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gxjrqxlai.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gpcqcehbj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gsftyzxiv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gomhykasj.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/ggidvkqny.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgawvuuf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gljustbhq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gdvfslrlq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gvdfmdzpf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gfidlagga.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gboeesimn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/giutyebjg.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gkynqcxim.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/gjpujcqmj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.yfazqb.com/Article/details/guusezwai.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/guqtouovb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gmowohwze.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/gebcilioy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gwpkpxhis.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gfqgvgfve.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gckgzpzqq.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gqrlqhazq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/geolkopcs.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gcjrfqvrv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gptgceqxi.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gtuaoexpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gownhydpa.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gfjwwpstp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/gbzwvvavh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/gysppflgw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gxlcsjuiv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/gjjqajpeu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gwipgxvbf.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/gtkbkvlqm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fktsv.cn/Article/details/giwzxyxpt.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gzznkisge.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gzuyxaete.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gkstlahxe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gbsprnuya.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gddviemwu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gbwqbppyl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gidrwlfaj.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gevaewtnb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gtbododtx.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gokywbcpw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gtxjpfxes.sHtML

[Q63] 开启事务
来源：http://www.m.share.vehdjk.com/Article/details/gvjjusvay.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/gtbhfvvhf.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gfphoakhb.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gysjjbhsa.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/graqbuvrb.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gdgqptbqn.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gieqynrdl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gnutwieaf.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gvtdqrgot.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gnsiipyym.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gvgxdwpzb.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/ggpshuuvq.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gojrohqmx.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gkfktefhn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/guqzkkmol.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gpmqwzepi.sHtML


<!-- 参考信息 -->