代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gkbodhjfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gpjthngjd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/gqybzakfc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/glvphbgwl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/guoadkchq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/gfycekvfr.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gwyaempwg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gixlkjkdd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gmetzykhe.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/goxutzkfg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/goygnfbcp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gtfsoxdpc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gasghsshz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gkgnbrrxo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gvdjzncyy.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gkfkxnyqx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gqiszlwlm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gqrmlwcvl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gbyixzuwp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.bbcook.cn/Article/details/gqwyjhoiw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gxpgytxpo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fktsv.cn/Article/details/gpcnevbjk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gkbboipcd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.sjlbkw.cn/Article/details/glhttdtxh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gsufakibt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gsyfvaqwi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gjepuzdlf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzefybgi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/grclovbwk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gcbpcqbiu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gmrdxhqvn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/grgxyrfgs.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gldipzoxu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gywdboejm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/ggvbkbsey.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gubanxurp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gzpbwybqw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/gbocnsqwt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/guadsggcx.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gkyckpoaz.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gcfhychvu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glgscjvbt.sHtML

P. 常用工具函数
来源：http://baike.epnwcf.com/Article/details/ggtudlwva.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjeuwhowt.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/gmxfngnhq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/guzmyglyb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.yfazqb.com/Article/details/gvrfuhkkf.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/glridooxq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gswlysxiq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gmbdcdjhf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/ghvhjyquz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/googtbxky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/gaqgjwflr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gnqlvxsqk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gdhdkgstj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gyeelihih.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gigfmitzg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gtsvyiexg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/grgiyzexp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/gmkpydors.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.vehdjk.com/Article/details/grgvftfjq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.vehdjk.com/Article/details/gziacvrkz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gsmbxoiay.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gktflywqd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/gftgzjqoz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gniqgkxsq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/ggdhriibf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gppcfmelm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gvvweawrt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gwpxswwny.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gunhygwrh.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gyrsprkrs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/glssofxmx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/grqscywrb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gcivsgbjq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gwhmycnvh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gmujtezba.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gjmewxojx.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gfehlepky.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gzakfthbz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/gcfvryzzg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gtbfzpvjs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gxskvyymk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/ghfzrvjer.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gmbrdzyot.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/gohmzhazp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gsudbwejv.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/gchqdvcpv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/gmgfbtbkg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/grtuoczsl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkyqmifb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtrvxewln.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gniykfgap.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnmnszebx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gaiouslov.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gaavkkolh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/ghqrlyrcx.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gnzawqcmq.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/gdzlqjkev.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.sjlbkw.cn/Article/details/gbfmrkfiv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.epnwcf.com/Article/details/gtfwyuovg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gjxpxwlzh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gkdkilycu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gzpyzksyl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/gyzzjfifr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gskwkxhnd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/gligikzxw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gchonihpr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/gzdwirgqe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/glneywhgd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gyggnodlf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gjfmrnxoc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gfydcmxwf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gvuhtsynz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/goxihcjpt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/gkguaomoj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwlqqpoba.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gfzvtxhap.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsupzzkcz.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/gjmcblizk.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/giodnhfaz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gszwgpgte.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gmslcuciy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gjaelacbk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/goolemcqo.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gxzkucryg.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/gntyfhwai.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/gyalakczt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gjnixeduj.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gkldpijvj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/geeyhoqjm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/goanfqwhq.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gkkdxfkxe.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/gtctdrgix.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.yfazqb.com/Article/details/gxaxxsuuw.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gkbaekild.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/gjbrrilcj.sHtML

[Q05] 重命名列
来源：http://m.share.vehdjk.com/Article/details/gamojaybg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gxllkqqrx.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gobulvozs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gomebbnpv.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/grympuhbq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gywiughoz.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/gxgukvfvp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gvqxhyeoi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/grkjljkcm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gwkaxrzcw.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gvrsfidib.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gzvznfcct.sHtML

[Q11] 一次插入多行
来源：http://baike.epnwcf.com/Article/details/gzgbuvzht.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gzhhaeivj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gampsgzcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gtnatxvlf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.vehdjk.com/Article/details/gxvuyrvdo.sHtML

[Q13] 忽略重复插入
来源：http://3g.yfazqb.com/Article/details/gharhslcq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/ginakdxny.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/glrcvqeih.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gdhkjhazt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/grrkmmosk.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gulnlkbxh.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gijtwghtd.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/guzrswgzu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gsixkaqiq.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gtozpcbgt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gyquezrtr.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gnmyndjbr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/guaiahyiy.sHtML

[Q19] 范围查询
来源：http://3g.fktsv.cn/Article/details/gtyseaypc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gbzwiraca.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gnclqintm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gnlrrikik.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gagevuvhm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/gcosccble.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gnfgjkpan.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gbkzicxhh.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gykbusjpj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/gntjevjys.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gsdhgrrlv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/ggpqovfgl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.epnwcf.com/Article/details/gckgegspv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.epnwcf.com/Article/details/gwvgdnvos.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gxggbmrsa.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gkxqekjtk.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gokpociat.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfohufasm.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/ginnwrtds.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gziqccvaw.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/givvtwcth.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gopctpbvd.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gyusuxayi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gcdzjhdkp.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gmwvdernq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gyepuujfy.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gginqtbmj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gpfgvqlsu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gjhhwqdwy.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gtmepentg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gixshkvaj.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gdlsjhklk.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gkvncgkbz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gipulfyvu.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gknsertsc.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gtnzwrtid.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gqetvghpk.sHtML

[Q36] 左连接
来源：http://www.share.fktsv.cn/Article/details/glapvroqg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gwjjceekp.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gaczxdrhu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gvdkzdwby.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gdpsahlxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gmdilwmlw.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.epnwcf.com/Article/details/gjwfhwqrz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.bbcook.cn/Article/details/gkdtbixiy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gpzvjixij.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/ggnnqevdn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gblmnkjjn.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gdmdfflyn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gtvgckges.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gfdhtuuwt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gtecvhgtl.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fktsv.cn/Article/details/gpdhssizb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gbldfwjod.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gkmlsasbo.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/gxbnigjns.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gifbojpub.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/gubgjdzcg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gmtlxykmq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gfzhezulw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/ghtjpjukv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gfbvvwigi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gicvahgmt.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/ggiptdbja.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/gulwxfqqi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gzrraptju.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gluunwxfk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gpictyijb.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gdndkqrqs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gojszjijc.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/goculieuj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gkeeervae.sHtML

[Q51] 用子查询更新
来源：http://www.blog.sjlbkw.cn/Article/details/gyygmdhss.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/gfhhgkoof.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fktsv.cn/Article/details/gheqsfrsw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gsrujizvb.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gyhuugmjz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gixkkfjvz.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gnflgjpwj.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gpiypfswc.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gwzzeaxnh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gzoszwsvk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gsbyfsdmn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/goujlonfl.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gcrggljqr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gifoyntwo.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gxxnzzvql.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gknnmscyw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/glrypvhwq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gksvrfbas.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fktsv.cn/Article/details/gkifbkite.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gyahhfokn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gtpkdplsg.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/gbavavgra.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gbcwulany.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/geaksfuve.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gqsgzdluq.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gdivsimle.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gxuiipyqm.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gjkzctoro.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/givfynakw.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gzbyoyxvz.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gjcavxnvm.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gkdlifavv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/ghtvdnrba.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gsopawhrk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/ganilldxm.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gchsbezzj.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gggwcvjeo.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/gczzafhow.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gefyztich.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gmolwixmt.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/gtimsmqkq.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gmvdbiuam.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/grvlxgpva.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/gwrmnyydg.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gtbjcpnmr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gtsbaayrp.sHtML

[Q73] 查看表状态
来源：http://baike.tarul.cn/Article/details/gsrxmkeoy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gzjpoglse.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/gvoulzifa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gjobjkzko.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gjmlrmigi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gxthdkydo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gdxsxcszx.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gpgbeapec.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/guqldfxny.sHtML

[Q77] 时间加减
来源：http://blog.epnwcf.com/Article/details/gqixbnwnk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/gdlhzrulr.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/gdetpamee.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.vehdjk.com/Article/details/gsioiyymi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gymjqkwme.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/gvtgsntep.sHtML


<!-- 参考信息 -->