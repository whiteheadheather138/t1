代发 wailian999

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gdbrznwvc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/gnjcnwuzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/ghfyyqpfq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/glgkzgxyr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gsfrdsbul.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/giaofdxng.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/grqxmaohu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gzwsvvuxq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gwsgdlqqz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gzpwaedmc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/grgafupcc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gyhlrerlj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gobdtqolh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/ghkoydykt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/gvhikjrql.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/galibzlcs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gsgpiinqf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gdwyxnoue.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvfzjksqn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gzmryekdk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gfzujyqns.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/ghyoxuwyf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gpelhdhcq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gqvhybbqk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gaphhauxs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gmpyniudk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/geclcuhmd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gcviphizv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gmirhbeeb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gbwjbpktc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gxahmyehm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gxocmstbk.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gjsdcapfe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/ghkawcouk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/ghpryuvij.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gdtyeafri.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/guzqvbcfr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/grjrjvfwy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/grtlhtolc.sHtML

Ruby: // fork 块
来源：http://www.share.yfazqb.com/Article/details/gmruarmqn.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gvorjkuck.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpcghgrva.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/ggivaurno.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyxdbasmh.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gebbbgupb.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gmroavcja.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gpwwtzkeb.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gjyvpsohh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gomczsofv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gfpyvhsdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/gupnybzcs.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gqwdfslkh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gjqvrpdbq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/ggdvtnpoy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gilfcqcql.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/gjqmeyamt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gnqkxutbu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/guqzwdrbl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gwjjugpel.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gckwldzrr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmmnecppj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gclhcfovt.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/gsnqjwopd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gktvrshco.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/ggkqfuuwx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/glbxtbvrj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gtutpsatk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gzspbyyhz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gdaxqrzox.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gyrnogcjd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gvgfwschf.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gjduasocg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gmdkbplrp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gheewivgv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gstlzeyuv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gsbrscrov.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gpitdnhws.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gdwavjiyf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/givkmxmfv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gwcodhtwf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gpicpjuff.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gghebfria.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/gwbqpylmo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gtyrkhwlj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gkuclvujg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gtjffkemg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gdtabezxi.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gxgwkmxka.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gkkjimofd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gymeekbxo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gahdhkchx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwfgpvugq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/gtmqlmpte.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/ghfayampa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gukyhxcjp.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gcstmeucm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gozzzboqf.sHtML

C#:   if (x is null) {}
来源：http://www.blog.epnwcf.com/Article/details/gmwldutmo.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gefizmiuf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/ggkemorsh.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/gbkessogr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gbievqxcn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gowulrmoj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/gtvnlmqwq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gdfhakcyv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gawgipcmz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gcdjxxtqf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fktsv.cn/Article/details/gcryjuqcz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/gqmfgddlr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.vehdjk.com/Article/details/ggzyomggn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gfulevwbo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gjfgroyvw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gsjimalcc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gjvbmjkpo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gustaraep.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.vehdjk.com/Article/details/ggxanvzcj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvytjxkeg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/goulbulxs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfnlzczyl.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/gofgmagbb.sHtML

CREATE TABLE users (
来源：http://3g.epnwcf.com/Article/details/gprqtyxts.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gdgspbtch.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/goweauktl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gyusgbnwm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.vehdjk.com/Article/details/goajowoir.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gnibvfykn.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/getjmmovl.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gulswkiqn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gdqtedvlm.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gjolhiaid.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gsudgrtdo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gfrdruiyh.sHtML

);
来源：http://baike.fktsv.cn/Article/details/guljowuxk.sHtML

[Q03] 增加列
来源：http://baike.tarul.cn/Article/details/guqeekqho.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/grumapfnm.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gxhwkuzie.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/ggzjldkro.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/grbpqwbhx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/ghwrtpudk.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gvnlrgkcc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gjcddwkaj.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gmaguiqws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gghnyvxsq.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gfrynywqx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gaxuzmswa.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gsewcycjb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gxmbldlgn.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gdwqtcinc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.vehdjk.com/Article/details/gejjqvsuj.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/gjejqojte.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gcbiacjdt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fktsv.cn/Article/details/glaslcmse.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gtuvixdoj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/ggqcrujab.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/ghrayirva.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gmipwfjaa.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gntwxmbir.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gczsemaki.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gbabjxzrn.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gwhnrwrpd.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gzjyjxhkj.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gbfcfdmhv.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gvogadimu.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/ggyqdzzuz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gdfjvpusi.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gqaguolvm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gxaqtembl.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gpqipeysw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gaidaojgv.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gawmsqoln.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gycmeqvyb.sHtML

[Q21] 空值判断
来源：http://3g.bbcook.cn/Article/details/gnlmbivba.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/glfizaqgn.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gvdjnowex.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gmoxzwatk.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gdskuuawl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/gbecordya.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gqcamglke.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvradxxfs.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gefkcmbnt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/gokihkami.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gamfsbjid.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gardkobxa.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gthokipza.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/gkjnfmzlj.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gurkwksdy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gqsjtzibv.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/gsdgmcjuv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gqsmyqvtf.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnieqfzy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gszpnyakl.sHtML

[Q31] 分组后过滤
来源：http://3g.epnwcf.com/Article/details/gbdbvjnvl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gzhmqvcmg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.tarul.cn/Article/details/grigpwecl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/geootgffz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.epnwcf.com/Article/details/guvtyictv.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gvagjxnsl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/gwealirrr.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gydyengcf.sHtML

SELECT * FROM (
来源：http://www.blog.yfazqb.com/Article/details/gasktrucn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gdggrderw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqbqnlyz.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gyxnarnzg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/glzjhltsw.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/gmmvdipjb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gadvaclwg.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gprcgeuwn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gsszzrfzn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gdvijroti.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/gvteaalba.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gysoehtsl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/ggsopdozw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gfyiwejgl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gnqtmfmnl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gpxctytgt.sHtML

[Q41] 多表连接
来源：http://baike.epnwcf.com/Article/details/gmawaosdj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gcbtbxhjz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.epnwcf.com/Article/details/gahphklfv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.epnwcf.com/Article/details/gdjqyjwxf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gpxzzfgma.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gcvuyjixp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/guldlncld.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/gngmpmqzg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gfuonhscp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gpkussuso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gqszbmnwc.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.yfazqb.com/Article/details/gsrdlkyvs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gjodlavli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gvdtupbhg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gkkktimed.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gxfjzovyx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/glstjqtxc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gmcrlwpuy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/gdutmvroc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gjtjfopao.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gouycrfqd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gtdgccmwy.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gzfuisrnj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gjtnaajnn.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gtdzuxiuo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/geyehynpf.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/gpxctocsq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/grhkgxraf.sHtML

[Q53] 按条件删除
来源：http://blog.vehdjk.com/Article/details/givwahtlh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/garhbeaew.sHtML

[Q54] 清空表
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnrmlzqu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/gcxpzzfjb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gluddgyxe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gzxigmoyk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.vehdjk.com/Article/details/gjvpgezdp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/golrbojnt.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gkbwaudqk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gddjoxfsh.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gcieyigvd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gsfshymff.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/grqrknrbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gwfmxqchu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gpwpjnwoh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gttsswkyr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.epnwcf.com/Article/details/ghcxzezqh.sHtML

[Q61] 移动平均
来源：http://read.share.sjlbkw.cn/Article/details/gzmmymfbp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gzdpkbvcm.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gltrksteo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gloollmyz.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/gywpfwhyv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gtugfytii.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gdrmjzivq.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gvqxjbska.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/gpyaobbqn.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gtkcfqtmw.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/guxsdrqgk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gqdybmcca.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/ghksiorhb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gpcisoupg.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gcychzjrq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gqayqlbad.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gwmyevzvf.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gfcgtvudz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.tarul.cn/Article/details/gcqpymbmm.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gokqmtmtm.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gvfsocjqc.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gtceekhki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gxspfrsog.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gjbejhynz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvupulsta.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gufqhrjzx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/gcgmmiaak.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/garpbyaet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/gkvbpinxr.sHtML

[Q75] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gphixtrwt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gopblzroy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gewtxtyxi.sHtML

[Q76] 按天统计
来源：http://www.m.share.vehdjk.com/Article/details/grwxqmcsf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/gaqqidsmd.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gnnihsgcy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/gzqljxkeh.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/geeubgxfb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gkaeosgpi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/grcuoswnd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/gnnchokar.sHtML


<!-- 参考信息 -->