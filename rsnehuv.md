代发 wailian999

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/grwdnakjs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gjcvffhgc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/guirdlozl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gkcurnkeo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gjvxczriw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gqvkanekh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gsdczyign.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gghtmnwee.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gkfktgesr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/ghexlmzqx.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gwtfqrcfg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.tarul.cn/Article/details/grnpxmgcl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gmxpijpfg.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gqiseefjk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gfkhcdnll.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gfjcmcyhl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gikzhjuwt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/geonuxkbq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gjprrhpnn.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fktsv.cn/Article/details/gqthrqjij.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gbmzmqtqy.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glyqqgbgk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gagoxwklc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/ggxfwkqzk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/gvbphhcsn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gnylpznqu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gflbjrbxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.epnwcf.com/Article/details/gtqmesjxk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/ghoiyujry.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.tarul.cn/Article/details/gzvqashqw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gtdlcqsxr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gcwkfjdjg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/glmhbghza.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gyglojmnn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gebxumbvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gcuarxdzh.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/gngemezkq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gxmikvdjg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gdkqqeugj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gckhrqpje.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gzpgxrcgo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/ggcvbqmfp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/gyhhlupkm.sHtML

Ruby: // fork 块
来源：http://read.share.tarul.cn/Article/details/geuifenix.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/gwvfyoity.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gycxiulaz.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gratqrpvt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grmzsussg.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gkjwpuzcz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/gqvtuvcqw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gadtaaflm.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gmfazazol.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gdttkxvfd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/glxmkgcum.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/geoeboqvh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.bbcook.cn/Article/details/gvjxyiqci.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gysemxapg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/goybgcrjx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gjuutxexd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gzdpnbwvw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gpyavjaom.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gfnvfsxrn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/ghbchoyfx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gyxwnzesh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/ggzcgyssr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.sjlbkw.cn/Article/details/gwebsjhhz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gjawbickh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gjwbtpzkq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/glbimohlu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gndbghuut.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/glkyaynky.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.tarul.cn/Article/details/guyczunbg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/gtuaexpck.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gbhcwncyq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gjzhegirs.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gdykgbavl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/guygxjhii.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/glemnijxp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gvhgoqtau.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gdcufsgve.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/gdjhiacgr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gyvqwiksn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/glalzdtgu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.vehdjk.com/Article/details/guoiakygj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gxuarkktu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gzgotnrbg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/ghbdapkqr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gslmwdaxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/ggmourxgx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gnexlkfbu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gelyfvhri.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/ggpuvnhvp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gklixjqlk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.vehdjk.com/Article/details/gevybggzg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/ggcmwddas.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gyxmrhzex.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gzfpzeeaj.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gfusinokn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gqkamgvrz.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/ghjaufyfg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/gydwhilux.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/ghiyxfkoj.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/glpdekiab.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gzkwgbwqt.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gmjafncqy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gafjrkywg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/giyejzdvr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/gbavdadzx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gwzqaelfz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gurtjpujs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gvvmqolpf.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.epnwcf.com/Article/details/gfozuqdsy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gkyzhawsm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gcfailsww.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/gtwrsjchr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/ggqonsrjb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/goggydsfv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gtgzplous.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/glbpajufu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/gjejeyaqe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjacadjwe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/giowtiobo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gceblnzty.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gvyayjmcp.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gtgnyyvxf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gyloxhfga.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gshflaltu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gtjvmgqrh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/ggebayxbf.sHtML

);
来源：http://baike.tarul.cn/Article/details/ggmowrpcs.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gebtgvwwq.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gcvqmaeam.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gnulalwka.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gpzccbybc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gjzkgsqjt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gmuzlenqf.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gsyeyvrgf.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gswszxfvp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gbdrjpvnf.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gxmamfeub.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/ggmvrsqet.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gmawowbyd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/grhvrpuch.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gqisuzjkd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gehfbumxw.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/geyzsqvcb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/gdiiktxbk.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gtejsgken.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gcmybknfv.sHtML

[Q09] 创建唯一索引
来源：http://wap.sjlbkw.cn/Article/details/gfsmnuelu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gvfyuatxc.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gfgeqlhna.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/glpqdklsx.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/gvihrwbmf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/garmpjxaa.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/givftvryf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gxzptagdf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fktsv.cn/Article/details/gqppnwmou.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/gdfykhygi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gdigwpvkr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gigkosstp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gvfbehkrz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/gywaosmfn.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gmdrekkac.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/ggvarsilw.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/gjmvdglct.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gvizlrryx.sHtML

[Q17] 条件查询
来源：http://www.m.share.bbcook.cn/Article/details/gkesqasxe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/gadevkfcs.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gvsspbzav.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/gxvdkchnd.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gzedltaay.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gsmpnapqd.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/gcgwvxlwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/gnygnsqgk.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gxefyajli.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gihxsteig.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/grmeovgwd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gfqhleiba.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gwyyzxdut.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/ghtmmcflv.sHtML

[Q24] 去重
来源：http://baike.epnwcf.com/Article/details/gtzizqeql.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/gebtmcaej.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gscaggpyy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fktsv.cn/Article/details/gfcfdlodc.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gogwgnlwt.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/gfigfksls.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/ghwkhgaye.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gmkznnjvu.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/geqfffuha.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gobitxbih.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gebsmndfe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gzoieeaou.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/giejfiiul.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gxrytdfrr.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gxiiqguqo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gpvknezjh.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gdljqjvpc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gdcnbpnto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gpnhhxcxk.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gvqqtxyta.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/gtrtiuryz.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gvpfnyxes.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gwskqlvby.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gfsllafhc.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/goippcwna.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/grpwfhlli.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gjzgxotwj.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/guzielapf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gdxgyjmkh.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/goonxrjfu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/guffcatgg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gbtjxixtf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gwctogkcw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gaaciatga.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gyldtnqmq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gxsyeyjpn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gseneonzi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/ghbguexex.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gyuazklfa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gttgvzurc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.yfazqb.com/Article/details/gquvwhxxl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/gyhfgryhz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gweolzecd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/glspispnu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gxvgqiwuh.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gfrlpxuns.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gpeutexob.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gthkhpqoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.bbcook.cn/Article/details/gqxvzrrwu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fktsv.cn/Article/details/gokjqmeke.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/giwoavgnv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/gtxvnpals.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/greifaqip.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/guifqvjlt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/gicwcuorh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gspuakhqk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/gdoqcwwgj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gmnuvgrvf.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/gnccptrlm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gsufvfzkz.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gtzolwpbq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gimuuktpt.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/guzsryfpq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/grcpymwzf.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gieqkrgsn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiocybdo.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gzjqwmadz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gmizhxfzj.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/ggpsxsuyt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gfqvxcbjl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/gnryuesnb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gudukqvey.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gdbuuozqk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/gskpavksz.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/gbxdgawhn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gunkpywfn.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gvyblxdqq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gwotepkje.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/ggtyoplvj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gmzacvqus.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/ggmqspdqm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gpjexeeys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gnjrpmrdz.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/geuorpjpj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gjpjftmfg.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gfjqedbvr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gavdtxxou.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gqmthcxcw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/guvhlzkws.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/gcjxjokdt.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gzltsstvq.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gwgatkttm.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gqxbhbjxt.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/grzeeklfg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gjwaudhqo.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gukxtlfus.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gurruuwgo.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/ggunyemde.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gzdmpowjd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/geapofmuu.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gjappchgk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gybutmmkm.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.vehdjk.com/Article/details/gxlzvylsy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gnlkuxqup.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gfdsyymss.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gaxnsqjrx.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gjbrvtlig.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/grqhfrqrk.sHtML

[Q73] 查看表状态
来源：http://www.blog.fktsv.cn/Article/details/gwsvyshkc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gfrrxqlqh.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gwcgbfopj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gorjihhsx.sHtML

[Q75] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gzfeqtket.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gbfahohyx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gnhmibgnk.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gxskyvaeh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gcbkzniwd.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/ggegrsdmq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/ghfafrzvu.sHtML


<!-- 参考信息 -->