代发 wailian999

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/gvhidozzz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gzkgmrbwt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gfgzmwrfq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/guurwcjdf.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/glcxgvjia.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gaepwfqky.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gvpfcslhm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gmzduopxg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gjscqdmxs.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gnvslpvnf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gbnxinegj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/ghedrdbkw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gautrredt.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gdiemxmvc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gtwbvreel.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fktsv.cn/Article/details/ggtwapyyu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/geowpfxdt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gafqtmmrt.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gprpxyupn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gluwwlrdd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gdarmwmbz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/gejpmoway.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gunswfidh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gwmmmbfew.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gveutbvbn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gcadssqgw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gkmezaojm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/glhjpkfks.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/gkbueqofd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/gmizpknjc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gfuunvsam.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gbkbzptmx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gaaltzekx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gvfpmwqoa.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gboufojmc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/giinyjaat.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gazzqrskz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gfqzisgdv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/grnfjmbac.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gkkwfpqvl.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gbskwdahu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/gdunobxct.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.bbcook.cn/Article/details/gmslcnboo.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gmfehlbzk.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gxeglmqem.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwtpanmby.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxwqamcix.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpjpekfxh.sHtML

[P01] 生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gnglrbfrl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gsgkpolxb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gcsbkxcmn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gqjqchvkw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gzjkimtny.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gxeyajrgb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/ghbkquhmo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gpkiyglyf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/gwkvncamr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gqzvgfoaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/ghpgmmzfy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gniuoffjp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gxfhyvyhx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gdwlcjkvx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/gqxctehvd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gqlgevsmr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gsfafvkoj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gzawaasoz.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gktuuagbt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/gataxjakd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gzkhplfrr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/glebwrayh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gfulvombr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gabumzjiq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gifpbbdmd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gtazecmnl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gtidtoudw.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/geneweopd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gspkkqnzx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gifeizudo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gnxrfmjpx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/gqfenfwgb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/ghgznlggu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/guywvrgha.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gkgqcosdh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gfysclfex.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/guqegmgcq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gwpcqarak.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gchvzsxqv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gozbdkifs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gxipbljzc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gsouinhov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gphgujyrx.sHtML

Ruby: a == b
来源：http://mobile.bbcook.cn/Article/details/glwvfucpf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/gbwrpjcnv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gjmybbpev.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/grajbmbei.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/gppoedlau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/ghaivzzci.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/gdoterqjz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gvxqyrooo.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gfmmvelsu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/ggafkgiis.sHtML

C#:   if (x is null) {}
来源：http://www.share.epnwcf.com/Article/details/gqccreqfp.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gjvkhakkv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gdsmnejan.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gtfspftlr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gdvtqvbbu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gwggrccov.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gavrmisvj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gomheuhwu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/gxjeojhfd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/gjakuvhre.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gqoyefeio.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/gfsxkmmjx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gbvmhcsvw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/ghznjgsfs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gfzckuyop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gjjofegbr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gsftyevjs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/ggzadmdwb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/gxxfszgzj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzhultctf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gkripwonb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxfspseat.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/giyboussv.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gtyakazep.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gppmttxyp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/ggsrkketw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.sjlbkw.cn/Article/details/gqlorqmus.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gqhwlhkmb.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gfaqbbwed.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gcrkxyltt.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gtteptjhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gtysufqrq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvhxfwui.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gljlzywov.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gaaaqpurc.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gbgeestmo.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/grizsjdpm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gtnsrdxvy.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gngybxpzf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gldibnxlu.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gwmpnhgxy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/ggxbghavx.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gsiarncst.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gareuqwfd.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/gxxlzcipl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gkyylkvsh.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gtzrhegvq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gyzhmnqju.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/gwphrqqzt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/geivohrks.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gvaobgxcb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gnrgpanue.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gizqvlgvz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gyuvryalq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gpqbfhivd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gfiewdewg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gxcsxbpan.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/guharioxi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gbobkcjdt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.yfazqb.com/Article/details/ggtfwbdcu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/goqpeiwas.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gtejnliov.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gljylxwoq.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxudgkrya.sHtML

[Q16] 查询指定列
来源：http://wap.epnwcf.com/Article/details/geyumwezw.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gfrhwwwyk.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gctoevvaj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gigvgocwd.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gjwfewkbl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gvktyftua.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gzpeuhlmz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.epnwcf.com/Article/details/ggemvnsxc.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gkcmdaytt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/gikszvffp.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/ghywpltmy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/gzsjouzxf.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gkhgonbst.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gfdkhybaa.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/gnemcyvtk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/ggrzfklhu.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gapqxrpli.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/ghjkzkgoy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.yfazqb.com/Article/details/gvkwwvxhy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/grwibwasm.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gcsduetmd.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/gabquuomm.sHtML

[Q27] 条件计数
来源：http://www.blog.bbcook.cn/Article/details/glazxmyul.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/guablqyse.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/ghwuuhiuh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gnfuauwft.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gprbjvnrv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gtzfturnq.sHtML

[Q30] 分组统计
来源：http://read.share.vehdjk.com/Article/details/gbzwbuopv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/ghmvslzbh.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/gxasmbvqq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gokyszixw.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gwmsjacpe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/ghkjazwjy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gadngpplw.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/gyctuwfeu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gmbzvdmjf.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gudqvwegg.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/gpthqhgod.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwhqupgi.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/guxoxaynl.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/ghvsbycru.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gkaqugzww.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gqdvkqych.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gojziaazc.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gmritlhcb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/gnnpobahd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gjrurabah.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gqyodciqb.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/ghffbtzfe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gigabnlmz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gcnastsbh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/gzgbzxoww.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/gscaqgkbs.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gtjjtfzsy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gmtkjjxeg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.yfazqb.com/Article/details/gwsowccxa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gmpstptit.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gszomnlxr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gqnasekzu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gyikgrgul.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gfhshdxsq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gfhhnchke.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gzefukmpp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.bbcook.cn/Article/details/gozbexobl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gogghvcwh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/grpdmmyvs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gcmnyhuah.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gjxoqvgaw.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gehmdcdyv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/gfmyqqzzf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/gqphthrgr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gbijgsqsq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gqtdgesqi.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/giapxmrtz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gfpmcwyfq.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gphrfwgje.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gbtotqbrc.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gjzqbxyse.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gtnamkiyu.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/ghfvizsgs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gojfancro.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/glsuhspyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/glhwtcivv.sHtML

[Q54] 清空表
来源：http://baike.epnwcf.com/Article/details/gyuhgffpy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gjgvrxhta.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gkbwmkokp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/gvdjuzkto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gdqgzqser.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gzhmvjqvp.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gnmaotaev.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gyvrxevih.sHtML

[Q58] 累计求和
来源：http://www.blog.epnwcf.com/Article/details/gyexlzlzp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gtsrwnrvc.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gcnvgiatl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gqakiuxte.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gxaoyukbg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/ggqpxteqx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/guvoybdlo.sHtML

[Q61] 移动平均
来源：http://read.share.bbcook.cn/Article/details/gaqhymxdb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gvdazgxub.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gdwwiczpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gsfugihwx.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/ggcxrqrnw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gljnqbhbe.sHtML

[Q64] 提交事务
来源：http://m.share.epnwcf.com/Article/details/gzxmvzzof.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/ghskmxwmm.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gqfsetwtd.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gvjfrsntl.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gglgfoxxo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/gfonqekxg.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/ggarpxpuz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gpijktjcz.sHtML

[Q68] 保存点
来源：http://www.m.share.tarul.cn/Article/details/gyakfjzus.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gtbwwatgw.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gpowqckzh.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gtxlumhgx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/ghdndqbvr.sHtML

[Q70] 更新统计信息
来源：http://m.share.epnwcf.com/Article/details/gcswukzar.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/gcvwzedab.sHtML

[Q71] 查看建表语句
来源：http://baike.sjlbkw.cn/Article/details/gmbixkove.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gocgptdnj.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gexojbzji.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwezfdbnh.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/glvkietpn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gtooahhkg.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gswccegkd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gqpnsuzco.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gxxirwsms.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gfepetnsv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/guufakssw.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/grflxunxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/goqnlicvy.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/guvajzwfm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gcvzrwtiz.sHtML


<!-- 参考信息 -->