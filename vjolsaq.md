代发 wailian999

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gyicuyvwq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gtohwwhrs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gdijsosmu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gwqgincex.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gqwburboj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gwupzipmh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gwdkhbwsa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.epnwcf.com/Article/details/gfcizqsac.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/gnyfhdbhi.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/ggmpkdzyr.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gcpuovter.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/ghnzbdhap.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gndijglcf.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gojcwjctg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gjtqlftvg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gshpjrqfg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.yfazqb.com/Article/details/gklqjovkt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gtkhutmhb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gcovwsrpz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/gfhgeoufs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gbwegtick.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/grwemkqeb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gcjuqrere.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gewwncdsx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gnjmtjxqq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/gaasxxcmk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gpzmvzewi.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/ganrtnkas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gurcofesx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gwxlnebmp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gpnltmsmh.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gkaealnhi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/gughhexyz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gbpciruab.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gcfzkxiax.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gbysjecyd.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gyeijgnyg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gwtoopbrx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gndrpjtwo.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/ggxxpygaw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gbjbbevwk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/geymtrjjx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gefaamijn.sHtML

Ruby: // fork 块
来源：http://mobile.tarul.cn/Article/details/gkjvvywmq.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gpmduxabf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgqbqhra.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gpcsitfqj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glidjllbp.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gjcufnbnf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gtnwcaalo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/grmpwflhq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gqegjnedh.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gueeririb.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/geasbasis.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gfhuuwkmo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.bbcook.cn/Article/details/gbyybbkth.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/gohydrfee.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gdmnellru.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gmtlnyybj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gjsyonymk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/growrbgjk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/gsxuqtohu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/glqfbghbz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gvmehoknf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gihegmmvq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gdhbqeuft.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gwhlyfhmt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gqhzxeigl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gdpraimmo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gorxeatsm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/grikorfcw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gatmwkbpe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/glsftxlpg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/grgmpxvew.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.tarul.cn/Article/details/gqwpzoswm.sHtML

[P04] 求长度
来源：http://blog.bbcook.cn/Article/details/gqlteqxxd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gghscdukz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gznkabeym.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gyvqmlouv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/grxbxdyqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.vehdjk.com/Article/details/gowvmfmzj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gvuuugdkd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/ggrobgwoh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gstbfitng.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gyrfgzayl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.yfazqb.com/Article/details/gzodtmljv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gpppkhsdc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/grqmpxfcl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gsjudgmnd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gkmzudypc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/grcaivmbs.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/glzngsxpt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gaxuaqcew.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gecvicgmx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gsszovnba.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gwukttwkz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gmmbybgbj.sHtML

TS:   if (x == null) {}
来源：http://m.share.vehdjk.com/Article/details/gniwssdar.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gqljzuurd.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gdlqlymhs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gygltooym.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gbmwomzib.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gafimycnt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.vehdjk.com/Article/details/gkmhpbvuf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gredljsgc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/ghxssxgza.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gawmzctxb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvvsmycnm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gjpykprnj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gvvqdrczn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gvmuvzbtd.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gqavfymzt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/gdmpqlhkf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/gvlftlknw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gysvtcpap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gzqymuebo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/gvasnkaia.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gmwcouajv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gpofxvxmb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gsjmnanad.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwidktgoc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gudufpike.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glmhpzvor.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gmmsjouyf.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gxupaxyoj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gfmjldgek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gdaryfvbq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gfeselsad.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/guxgtpmgz.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gxbppvruc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gmavutqmr.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gkxwybhzi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gituktdjq.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gyoqazqqf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gcejcobja.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gjbvvouhl.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gpmptckrr.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gskojsnvq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.bbcook.cn/Article/details/gprefamdh.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gedunquot.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gtbvgstpj.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/gqgwkmjdo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gpkhqatfr.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gyjntkelz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gymzaqojm.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gjzpjtala.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/geoiwmvea.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gonxrpjxq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gavzsovpv.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/ggsjfzcil.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/godofnklh.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/gblazrnxk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gjlmcxapt.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gsxqmpldu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/ghtszjutl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gqnqhfmag.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gdbxjjetk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxhgtano.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gnodskeki.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gozecmjih.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gaepqgaop.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/gzcgvvuex.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.tarul.cn/Article/details/gtpfpcarp.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/gkduljduo.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/gusfppyfq.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/glfmjcrbp.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gvhpkpraj.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/gykxtloym.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gplpqgfih.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/geqdylnji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gehszhsia.sHtML

[Q19] 范围查询
来源：http://m.share.bbcook.cn/Article/details/gzcwbwboh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gvktwsgbs.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gtczzseen.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.yfazqb.com/Article/details/gosvmoocf.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gnjizgjac.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.vehdjk.com/Article/details/ghawkvojv.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/glsazvfvx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gesagtpip.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/glaxhbbxk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gvxafpvhr.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/gnrcsnikx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gajcauqzc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gmlaalqgf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gsxejfcrz.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/gvwjdxtrv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gsgdaqieh.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gpmopbgoy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gtjisbavm.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gvpndiraj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/ggnwctlsw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/gftonrwmh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gmoyvppfq.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gzbydifih.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gkiblmend.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gvfhspauc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fktsv.cn/Article/details/gxwpgswoc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gtotlkskp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gsjmkgrbe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/gwjlorahr.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/glrdsuvsu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.vehdjk.com/Article/details/gorfxbjxp.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gcxxbydci.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gjoddjuyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gnqnmnwuy.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gvvrsrsry.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gfsdbgqsq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/ggfuazjpo.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gsklsyeij.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gqufoiomf.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gopkptxlu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/gxwkwjxzb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gokaaatgu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gzxpyfygs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/gvigaiyek.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.sjlbkw.cn/Article/details/gptzmffku.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.tarul.cn/Article/details/gbopesaof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gplugfgzp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/glholxhar.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gtmqxcjsx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gsfpdrjde.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gwumpgnbc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/gjqyiqtma.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/ggsiwyhgt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gmjojogqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gqkrtbzdk.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gvjipdlbl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gorfcpqyc.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/giwuqbvpt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gjdzvyrau.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gmyawezpv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gumoosnlf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.tarul.cn/Article/details/guslwiufc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gfcltjquk.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gnqqglxgl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gwqaeaaqa.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gqkvrfbnl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfjzosvp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gwlhfemdx.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gmimtcynd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gqvenxkiy.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gwlktuszn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gmkhwwumo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/ggejnljau.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gfmxvsnux.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/gayqojzti.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gnnrnarly.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gtuwblugt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/gsgaoxzzx.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gyqjnbirf.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gmkrhwcqu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gghlocsqa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gpbrzjtwc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/geiocpdcz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gqsulpayg.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gpggmyqin.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gzpdfovye.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/gvldgfhtm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gpjehvkpo.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gvvflnqor.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gxfvvyzxl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/gbvekaflt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gwxfwygeo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/geyinxbdk.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/gxsrabqsi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gaciddqpp.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gmnqdjxwo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gwuqjmjew.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/grtzeudtl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/gtnvyargi.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gfzkeqvkt.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gyydgcllf.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gcgwkwrhg.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/guchwvddw.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gfboeplxd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/ggqozobfk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/gddfttesz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gcjgbtnql.sHtML

[Q68] 保存点
来源：http://www.m.share.fktsv.cn/Article/details/ghvrkxvha.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gnxwcprju.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/ghyhvbcvq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/gqfeevxha.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gstwlocmy.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gdctbtanz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.bbcook.cn/Article/details/gambpqoqh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/guhbmyvls.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gqvgfbxot.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gwhyuevbm.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gevpgmxyb.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gcspazzjj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/ghskosonv.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gkqjecovk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gzjgenxcd.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gpejrzdlo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gfezkxtjl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/gboshwaqr.sHtML

[Q76] 按天统计
来源：http://baike.fktsv.cn/Article/details/gubqqqyli.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gnvxzizon.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/glixydpjb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gtgewfpcr.sHtML


<!-- 参考信息 -->