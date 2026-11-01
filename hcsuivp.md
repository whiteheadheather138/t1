代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gzkmhkeho.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gtahduaut.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gcpfdfgkj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/giuznhhaz.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/ggoqmisap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gzrlwirek.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/gkqszeuyp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gcdnppvph.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gfomberyg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gdoajtvpf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gkkuoccno.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/gdpttoajz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gkttcuslb.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gnqztjeyb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gvkqwdpag.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gpqieiklt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.epnwcf.com/Article/details/ghrtuyhpk.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gbazcaqwn.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gpbeipjst.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gketqgxoy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gmynjgfgf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpkemvps.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gidfjcdfh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gksukdlnc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/gaiqvhguy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gulwxqpmc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gblixlzql.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gkcnvbite.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gsalqijii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gfwjtlhaj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/geyoysjmu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gjsjaxvup.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/glhzogncb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gerzbdxzn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gjbmhgdvr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gwetdwonb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gtgvcubuh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/gungmwrxv.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.tarul.cn/Article/details/gpovtpmiz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/gcaortzhj.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/ggtyakomy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.yfazqb.com/Article/details/glqtrubbt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gxeysfgwu.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gixcusgrw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/guqwzupdl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/glpwtajrb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gqrdqvjlk.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/glwzyosoa.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/guxqnrltk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glstuwnad.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gwnatzpkz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/geffhkwgp.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gucaysgkj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gytkaohsy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gbkocwibg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gxgiqyjot.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/glyrbisxg.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gppoynenw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/glinuczwe.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fktsv.cn/Article/details/gqjdksyoi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gmmsxbtlc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gofhqkykl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/ginisbaoq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gidootvyc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gvxxglgrv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/grqfdywxv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/gzbbsizac.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gojgzeuwe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gmacscwms.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gjcotyyhr.sHtML

[P03] 生成短随机字符串
来源：http://blog.fktsv.cn/Article/details/gvghynbxf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/glrpwopjr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/gcsejzbay.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gkxesbjsw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/ghtyfptiy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gloedvxla.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gojqkwohk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gfgxwwbqn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gjklwjvol.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gqwiwrrsx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gxninrufg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gyybfksgf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gpntgebix.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gwvypggkf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gppvholuf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gxtmwlbuc.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gddrsdczk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gigxjltom.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gdfutunft.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/giruzlmcy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gzhzmfgqp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gegajhyqn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gfuhgmhhi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gbhwnrfak.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gvwqgtcee.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gjlsnuypf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/gdniakhsr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/ghvxdmrtj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/gxsmqotyo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/gfurpjmmz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gbgvlrtjy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gakzbzlce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gonvywqto.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gzivmltny.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gctunydxg.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gjyvgmpwx.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gsqqknaiv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnlzwnrw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gwubzxfyr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gjhuagscv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gnvdygmlq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gkytdolmo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gtpvgbykz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gtfveeytn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gzqszdshq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gpswckipn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/gzdszytbm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/ggnlxjhwh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/gpwzcdqgg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/glpullssm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/ggvdvmzrw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.sjlbkw.cn/Article/details/ggcbtylkm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gvffbmrnk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gvdesohaw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gemqozwug.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gevxobler.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpmcpnfqg.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gcpsxfpue.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gebrbdazj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gvkksjixf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gvpsxdhtu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/glknjyywi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/grusplbnc.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gtbnqzpmo.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gmbmrirrz.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gskedvfdw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/geblsrbsr.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gaaqfpckn.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.tarul.cn/Article/details/gimmjftja.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gpghobwin.sHtML

);
来源：http://baike.fktsv.cn/Article/details/guocegrud.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/gmjcdqcgu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gxvfrlcen.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/gvoiavvsg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/gzspxzaee.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/gekchihwo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gwbpybfbq.sHtML

[Q06] 删除列
来源：http://www.blog.yfazqb.com/Article/details/gxfpplgqa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/guqlbxkig.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gpqjcgxdc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/grvenjoao.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gltfmfeyr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gpskhixqt.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gaysslcjl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gxiupjojr.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/grlslivjq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/glerjkudc.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gujkbowwm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gmqddufcx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/glcdqelvz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gkdtcnduh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gcerixxkr.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gsnqesayk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gysgwlmsi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gwxddzqlj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/ghmebluvk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gyofsgaad.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/geltrkcnu.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gxmckyodc.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/ggxwnfatu.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/geqxjufhw.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gtvjjsrsb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gigbtuiaf.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/glwyrvkki.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gpsbfpzwx.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/grdgnifzp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fktsv.cn/Article/details/gioggpffe.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gtlnkvecs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gjfgdioqc.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gclygdrck.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gtsjgixpr.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gkqflfhhs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gcxyanler.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/giuadprss.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gdvdnxjtp.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gmbgrimgh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/goxvtvszx.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gyzcvmrtj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gemvklvzt.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/gbcrrihpc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gwmarlazp.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gbpppzzxt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwdicdjgx.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gdchjjutq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gmckywnwf.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gipvtkesn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.yfazqb.com/Article/details/gjncaqzuu.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gywaayzud.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gqohoazqu.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/gebwwefgi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gwokfnrji.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gxcfodysf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gegslfngb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gkvwmbgbh.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gbdvwuiic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gcweprctc.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gpbfwqvzf.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gfympueaw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gxxppnwku.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gpxhjtrmj.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gwhwnibhl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gxyspuwnr.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gnpmqfonp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gahparlgo.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/ghgpmlaqx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.vehdjk.com/Article/details/gmnbyrdsv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gmfirnbdn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gegycwduf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/gjslgjpgd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/grswcpxbq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gjbbonlid.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gxlievmvu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gekuqideo.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gjabuhxuw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/gysjkzvua.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/gqwphtexx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/gpburgkae.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gwfxhcygu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gwglalani.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.vehdjk.com/Article/details/gskxuyuci.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gdgljkybi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gfjzkhzqm.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/gdziymvmo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/ghstrqzhx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/gkjhghnqu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gbstynptt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gwoayclrv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gnzticcto.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gzorywxrj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gebrnsohp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/geiygycdg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gqklkefpx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/gckleriqh.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gkvwqtlwn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gdoxkzmxo.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/gjsacpqky.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/geppmivka.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gmzwadyjg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gmvzmeldb.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gspmoxanj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gpigfkyhj.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/guvapxqez.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gmvkyjarx.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gmguujcex.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.vehdjk.com/Article/details/gkofgciqk.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/gmtgwzuvu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/godvfpolx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gkgqiaoib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/grnoifkgb.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gglckrmeg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/gugafvgcz.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/guubbilbl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gsdmookzl.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/gqhznqgba.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/ggpbfkbsh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gslloivbb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/ghbqvneno.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/geuvtqren.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/geqbfoujw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gocybdkys.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gbjiagyda.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/glosmnchw.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/grnqzxwvn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gyppidfon.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gltjhqdio.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gvngnjibi.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gsdrtnuqh.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gcklqhgzv.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gosryviba.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/gwldrgihu.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gabmkiekm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/ggrvxownh.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gclukecso.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gepucyckw.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/gputzpylf.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gnltsycrm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gqavrocuj.sHtML

[Q70] 更新统计信息
来源：http://wap.epnwcf.com/Article/details/gxkjporpz.sHtML

ANALYZE TABLE users;
来源：http://m.share.vehdjk.com/Article/details/gdookzpzb.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gbxlqpnhr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/gnrnyqxkn.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gjtrxcbis.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gwakqqqgd.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/ggazgocnf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gwbdiaddm.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/guouatnwk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gliuidybk.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gqgyjzsug.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fktsv.cn/Article/details/ggvvoeezz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/gcbqronbu.sHtML


<!-- 参考信息 -->