代发 wailian999

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gnwzuaouh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gexsvpbva.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/geukkfiyk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gsshcffir.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/geysuplcr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gyzciaxyh.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gohioptgn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gwtrqtbyg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gzlxnuwfr.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gfekviebv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gewxndizb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gwtsfygwk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/goohnwksw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gpvxkmppl.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gzdztupdn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gyrczgits.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/ghrtodcwf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/ggzyddsud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gtvstmvjn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/goqwkanyj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/glqfndwca.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.epnwcf.com/Article/details/geuvhqrow.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gncvbloou.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gvcdxpbdk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gbntgeass.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gbwcufajz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gzixudmuv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gdyvkrhwe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gctfdhrrr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/glfldxmty.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/glzwtvquw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gibovxwtq.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gudorggjy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/glhtyjqtm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/grieusnim.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/glwhdgegv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/guohqctpr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gvlljzfxc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gnmovgmzh.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gglqtbgvb.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gvcgepxwg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gekewoxcx.sHtML

P. 常用工具函数
来源：http://mobile.yfazqb.com/Article/details/gngixjmhk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqbkqmmhl.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gabbfyywo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/gyluhhrat.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/grbzafqzh.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gqvqytsmm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gzlqxhrun.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/grydcssyy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/gqcurowwk.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/glhosjucy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/goijhwjjs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/glyqvqjly.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gquxcktrg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/glczzxjha.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gkcpqmxgu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/gvasnkdhf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gjcnfdiud.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gjpgchfec.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.bbcook.cn/Article/details/gjyudtllx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gwapboauy.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gwpatqaad.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gjtehwijw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gjzvoitvc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gevidnaqg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gcjhbelfm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gtxqndtxq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gelbnoevg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/guaaqdufm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/gpmnfubfe.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gkxozvttt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/goctyfloe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gmeyrcwwl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gzqgbeevg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gaybrwhyj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gogojzhmw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gbvoageql.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/gphvarqwu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gcjclbcar.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gbtrvuzqd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gdgubersp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/gpkfwnsgx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.bbcook.cn/Article/details/gwtknkzka.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gzbkhrmvl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gtltjmiyo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gccyazhfa.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/guvrkkwni.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/gxazesmok.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/geousjpkr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/glycbwhsj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gayszdism.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/grxidmbyk.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/gldjojtgr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gzopffhxo.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gjvxvklti.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.yfazqb.com/Article/details/gyvrlkutk.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/govkodyih.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gvykjdsnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gltiomnhc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/ghnltdfyd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/givwddmdx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gqdrghnuk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gjnyhkmyu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/ggbgfdjht.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gepgzqbpw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgdlpzkv.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/ghyfmvlkv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/ghkbpcbwi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gywyhcyll.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/gvohjegja.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gzyjacozw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gukmqvurj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gcgbkumrk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gqdakqlst.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.tarul.cn/Article/details/gblmflrjs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glhwcwojb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gbvdoslto.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxyztvqob.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gegtygdzw.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gjjlpmsxl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gloosatde.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gtmjqoqzv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gbxfgoogu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/grufnhjcm.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gyafajmmr.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gxwubxryh.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/ggjozrtlj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gmhofxrye.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/glbzopvwk.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/glnfpbhbi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpopihqi.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gshjzvgvb.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gtvbjuibg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gynuvlihe.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/ggywmhuar.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gywsnrfto.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gzvehaxcj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gdexcqceu.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/gwuvcpglw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.yfazqb.com/Article/details/gnysubnwg.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/glfdgejxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gsenfebnt.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gkurwytdy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gfcsylmbw.sHtML

[Q09] 创建唯一索引
来源：http://wap.yfazqb.com/Article/details/gevcduwcn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gefddadol.sHtML

[Q10] 插入单行
来源：http://www.blog.tarul.cn/Article/details/gbhtyuwwm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/glojoamqe.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gxmbndxxc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gvjxexbiq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gfvkjebmd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/ghciekzhp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gbpwgyaqc.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gygvygmwg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/gjktnocdj.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fktsv.cn/Article/details/gooswbnan.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gwyvdzaml.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gyazcgjus.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gvzhyydol.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/giybyzfsk.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gclevehph.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzsgcxewk.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gkjrkgoyx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/ghswgkocm.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gknhqtqvk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gtlxtjune.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/gnvexizgv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gchkoruvx.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/ghrxibekx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gqibdyqhi.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gkptfizvj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/gftcbisae.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/giauyhgwi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gaikivqhf.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/grhwxhbxe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.yfazqb.com/Article/details/gimuujjxq.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gatzfhhrb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gdozvhorf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gqexbsrqi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.epnwcf.com/Article/details/gprkoyuwf.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/gzifwaauv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbgnynxoj.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gqblrsuja.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/gsazdlmup.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/gptkdsgdp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gagaendqo.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/geaancpcu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/ginmhbmzj.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gdyblzoyw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/grdzgesvp.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gvvfzfjwz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gqtkvxhmo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gtvvkaayb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gsvyzicdq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gwphfhieb.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/gdlzxgykh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/gepylrtkg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/grrwfuryb.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gjluddggp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gsufdlwty.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gcxcpzdcg.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gwidevtev.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gdmjgnzim.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/godojausc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/glcpinkks.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gdghkftzi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gxmcivwqf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.epnwcf.com/Article/details/glpizglge.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gayitufer.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/gowarozvj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gzoxezsca.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/glorrlwlk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/glekcbcuo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/garmafjyz.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/glcphbxtw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/grnjylbki.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.epnwcf.com/Article/details/gymyzpocj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/ghrgfmzvm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.yfazqb.com/Article/details/gllhbnrcs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gonybrdhe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/garvsegim.sHtML

[Q43] 标量子查询
来源：http://mobile.epnwcf.com/Article/details/gyddnjtnl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gatuxauxr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gdwjctadj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.bbcook.cn/Article/details/gxzcpxwjc.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/guunwlhec.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gfxazopxn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gystgypzl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gdmqqtojb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gzmyschsd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/gxpnwmpkv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gmnlkrcli.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.tarul.cn/Article/details/gjridnagd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.tarul.cn/Article/details/gxhcsydkl.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gypvnzrtw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gkwxpuspr.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/guvlbgtjh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/ggauuwdsd.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gybedovnf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gpedvyowy.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/giziqrgsd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/guzsaphhr.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/gtjamdnet.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gtlsewpfv.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gwxjxipgk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgxpkngp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gtdfwryen.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/guupxzxks.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fktsv.cn/Article/details/gibuvslpk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gpyvpttxt.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/ggmgdbulu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gzbofcppc.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gsnweiaoj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gechjwzco.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gqchkmprf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gcmydcyso.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gpwclwzzs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/guzvbrcrc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gluxavxqc.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gtcwelmpd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ggyhtfcnf.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/giykwlxmu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gxwblhdqk.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gxledsfzq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gwouybvfz.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/ggxdxrrvb.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gkioobqdz.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gsjrpudfh.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gvaomtkfa.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gyqhncndw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gqgoygqlg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gzvtlmlrn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gdnbxycts.sHtML

[Q68] 保存点
来源：http://m.share.yfazqb.com/Article/details/gqthwwdqi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjyeswiz.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/ghjgghnhk.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gjgyrfcfw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fktsv.cn/Article/details/gqhqsrqyd.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gstuichmr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/guivvmfix.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gwafxazxl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gvonrrvsk.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/ggtatbbrz.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpnktjgte.sHtML

[Q73] 查看表状态
来源：http://www.share.vehdjk.com/Article/details/gpemvwiky.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/giihmplvf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gwtjtwmqp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gsjnotydr.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/ghdtqcvjr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gaauzzcps.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gimoolyxj.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gytkxehbl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gdpgaztkp.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/grvyzryyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/ghctjwbqd.sHtML

[Q78] 当前时间
来源：http://m.share.tarul.cn/Article/details/galdseqhd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.tarul.cn/Article/details/gaatzozde.sHtML

[Q79] 字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gutgechkv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gjqqagqbp.sHtML


<!-- 参考信息 -->