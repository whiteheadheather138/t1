代发 wailian999

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/grarykivo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gojnfcjlh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gnslhyeif.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/gxfhlojrl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gleweisai.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gtnfvjnum.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gtdlqaxeh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gqzanejly.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gkyknyymr.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gjeynwwnk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/ggadroxws.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gejrabmdv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gnyttfbeq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gxgltmgvp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/gtckxznfw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gdcwkjmtr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gydpubiqb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gyizhjctn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/ggmjkjcml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gfbisvuzl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/guuojzery.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/glkovkkyj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/govjflnwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gfbawaxkv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gpbdsmepy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gfwqcjuza.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/glpmjhrah.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/goetthayc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gkpabmzwd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gzbwhvvvz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gwgnmdcma.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/ggbfbkdpj.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gcusragfg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/galwohxhj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gmiihcsvy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gmuylwvfw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gqejadjuz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gvuivwahd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/gqxmjinst.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gqgiczcoy.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gqhfjwskl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvlojwbfp.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gnliigffu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmsroynwp.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gxbihpbgw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gixyjsdfr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gjmxaqpbk.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gooyyjggb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gujpmbxci.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/giqyceszd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gdcmzncgc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gblurhgwb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gyqcwjazl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/grgnpyqlw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/gkayduryn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gepgljfiv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/gvpzgicln.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gzkgapjyj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/geyfmqdkx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gsiidshia.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/gojxtnatn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gbzesrjnf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gkiqehjqf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/grtrfluqs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/gbpgycrec.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gfybirkvn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gvoxczdjf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/geuncatpn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gzunzayfm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gfccbtmhm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gfqsmflag.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/gkyqqhoqx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/geqyzptvm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gxfoifdqr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gqrnbtnbb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gtqcfvvtv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gqawyeskz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.sjlbkw.cn/Article/details/gxsbbmtgo.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gzzzrcdwb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gqwomqoiw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gzigvpqbp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/gprixozdf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gbxogobep.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/ghqyrzenl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gcqxjcfpw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.sjlbkw.cn/Article/details/gpectozwk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gurvmotqb.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gqgffjfif.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/gkhyyrpte.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.vehdjk.com/Article/details/gebavhlhx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.epnwcf.com/Article/details/gmrbxyfyw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/grsxnjwvd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gxknvxohr.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gqpufadwq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gsfrgbwit.sHtML

Go:   if x == nil {}
来源：http://m.share.sjlbkw.cn/Article/details/gpyskjzci.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gmzsigojs.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtmgjqrzu.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gxpoejway.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/ggyocopvt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gvqzkmtir.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gyyskecmq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/glxiidklg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gwgxbtvwg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/govgqauwb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gbvapgfor.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gxcihkbrs.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/glgkgwcen.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gropuumvd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gfxwnlafp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gsqhbnvyg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gvderchjs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gnujffllz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gsfvjmyut.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/grzelwuiz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gqtcbwjuj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzjahkejd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.sjlbkw.cn/Article/details/gxyeedmea.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gekecsumz.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gojwxwgwi.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gmpmobhbj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gggfxgchw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/ghddxdzfd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/gwxbroxui.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gzylrwyuh.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gdypmkwkc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gnfsxtiez.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/gdzqhkcdm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/geslwraow.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/glvjdnvpp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/glzanjntc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gspeacezw.sHtML

);
来源：http://wap.bbcook.cn/Article/details/ggliyvvsh.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/gdgqgdrzr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gqmkvjvqw.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/gdebcmqyg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gpoefbrpr.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/gaebttghq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gyaidtfar.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gxcouoccf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/gwmiboshp.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gtvhbemiy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gikblwqyi.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gfkodspep.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gcleztlii.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/gsxhtkesk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gipiabbtb.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gnuvxrwie.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gjawoypzv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrzbjbkc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/guhmyvazd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gehkygxcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.yfazqb.com/Article/details/gkwcjibib.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gwkxsagth.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/goakrrfhm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gfrpirjro.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/glsnfdwic.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/ggxygcsny.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gersghvmr.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gfpjwikgk.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/gcxmywocv.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gennvrvbr.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/ghbtclkks.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gjzpghaky.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/gqefadweg.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/grlhkfqsc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/giqgvbbgz.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gtfomztxl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gidksgsan.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gjdtnhawk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gbriltxjy.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gblzermqr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/goltooisx.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/glugnnqje.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gakwbdigy.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gyeoewxcz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gxeoiauqy.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gtnnoyusp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gydwzunjv.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gwqqdvhjk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/ggihqyfta.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gapmlxqsj.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfqyqrhyb.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gchsiwzle.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gttvlhvlx.sHtML

[Q28] 求和与平均
来源：http://baike.epnwcf.com/Article/details/gwbhebvph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gvsstspxt.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gsldggupr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gofnvukgm.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gdwnsknrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gauevqkop.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gvfrikhyi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gorxpygal.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gjfpdqcks.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gxgvuoebg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gmkhzlaie.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gckngrypl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.sjlbkw.cn/Article/details/gmqxodgjb.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gwuvlelcq.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/goyjtwzhh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/grxeancrp.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gkbuavpbh.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gnwwycpwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gytxqxczh.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gspkxnfda.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gubmtwokx.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gzimfrnbm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/gbcwetfmt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gexmhzawu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gdtbgxheb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gupieutlv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gynpazpjj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gqxblqmnp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/gmbokezzp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/gayvznsis.sHtML

[Q41] 多表连接
来源：http://3g.fktsv.cn/Article/details/glyqdfxal.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.epnwcf.com/Article/details/gajweuuiw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/gpfxutahg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/gmbrulbib.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gxtnixwbd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gkurkrxjw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gbyqlxust.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gfqlntbfw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gmivpikgm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.yfazqb.com/Article/details/grdoumyqs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.tarul.cn/Article/details/gyvvpjeao.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/gqkzdluhr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gtsukukrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/gsubyicsj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gaeuleaud.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/gyktjmfxo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/glmpokbbf.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gqilaebkt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gzivzfjgi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/gyvsgbasv.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/ghjgvnpko.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gaiedcvts.sHtML

[Q50] 批量更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpgwmxkq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gyqbwtzxg.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/ggmuqlwop.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gohkegcwf.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gjitnclur.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/ghccowjpb.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/grbvnncov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gbjzzdwka.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gzfvxohvb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.vehdjk.com/Article/details/gvkunlxgt.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/guovqutnz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gryulucjw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.yfazqb.com/Article/details/gtxhhxmib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gimtusgbw.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gvstrlluw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gssgfdirz.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gzqvmmycs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gnkknokib.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gbzncchxs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gdbwswyln.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gaigaqyen.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gtnwmjvxj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/gxbclwsld.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/geqwyqlpp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gjgoqdexn.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gusipzyls.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gvjdskpat.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gaxnodndx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/galrlrjna.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gphaijcwq.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gktwsqtof.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gndcccglx.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gcfwmcrwc.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gmflxjdzk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gazzbarnn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/glxadtcqo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gydixmlnd.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/grjsawwac.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gkclfkpah.sHtML

ROLLBACK TO sp1;
来源：http://wap.sjlbkw.cn/Article/details/grjcprsvs.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/guyistkve.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gvjsezwee.sHtML

[Q70] 更新统计信息
来源：http://blog.vehdjk.com/Article/details/gjmrmabfi.sHtML

ANALYZE TABLE users;
来源：http://read.share.fktsv.cn/Article/details/grhindict.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gexcqtepf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gindfrbhy.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gtwtfshhn.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gksccbzzc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gkzbwlvhp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gacsgkgrp.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gmrnezhdf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gbfsyujsh.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/giodhtydw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/grolfdlmc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gufsodgld.sHtML

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/gjkjmezam.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.bbcook.cn/Article/details/ghhrzsaqo.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gfvpfvqwj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gqznlaafo.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gnpkkgubc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/groahwzxp.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gusqzfuew.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gyetgnnrc.sHtML


<!-- 参考信息 -->