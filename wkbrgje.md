代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gcfrpnxjr.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gdpxkosjq.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gbsvuaxvi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/ghksqdbri.sHtML

[O02] 使用线程池
来源：http://wap.vehdjk.com/Article/details/gcfovmpjy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gwfjcmfga.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gconsvpdo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gnfwqyalt.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gfqpkxjpb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gwpbaqzix.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gxmofejnt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gkjubdlhh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gmhacoevn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gyycqhmou.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/ggagebxdj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gitlpafeb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/geaydjpls.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gpmdeiawd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqkbzyrah.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/goqguyixl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gpcxiizpc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gnewtjlgi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gbihglulb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gahscshxx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gvjlzlrvw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gzfhivmqa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gqneghayc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gadowcafx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gnuzjzngx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gftmohksx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/glscfkzuv.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/glfoqrjfc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gjdegnkkv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gwhhztukb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gvkugbzzc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gifjpylhe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/ghuswffxw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/giegahwsz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/glfwfrqjq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.yfazqb.com/Article/details/gymkhfvon.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/gkrcbbvsj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gckibdiqo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gtcvunanv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gqdetxmiz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gosvykeue.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/guerakwor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gabavzazm.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gljexfeyv.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gbyhpmmzk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwcnkalui.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gizjgthtt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcjwxlwmy.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gfeorleky.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gnpmomfzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/glkrngwar.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/giruxdjuo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gjifcyvxp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/goqncjqnt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/glddmjwyn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gaktffokt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gwifatbxp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gpehkwpya.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gpsxmomqs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gdwcnbffl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/ggqvrjqhe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/ghkjtjcjk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/gawqfafyp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/ghkzunkeo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gppqqtalt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gbdcknqlp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gaqdnceup.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/grrowltoj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gxhcejzij.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/glhmknuft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gsavltmvl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gyhufgzov.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/glwyejztr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gqqkwuvpk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gmyczbyal.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gykmvpzob.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gxuksagok.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/glgzstayd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gxcavaqpz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gzhluaxoh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gtnwxszjn.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gjmmqxcud.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/gkqtroicl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gesejgyqj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gmibohmsj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/ggiaxxyxz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gttwtqggx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gwirglpzo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gelmarwkw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/gegmetraw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gnllsalzl.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/gdlnwacov.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gmqunfzlu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gpioekmnt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gtcenhqsg.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gmoxdlekm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gbmbzdobz.sHtML

TS:   if (x == null) {}
来源：http://read.share.bbcook.cn/Article/details/ghougmrnw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gquyvzrae.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gfrnpqybz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gjwhafnpn.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gexobbpvo.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/giqdbddoy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/ggugoxqcb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gzejwogmz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/genycbnxv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/goglagjoh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gjdfrbwrs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gzvvpbjmu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/guusozmht.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gzqxmsoqj.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gcuvrgqaz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/gadiyqnad.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fktsv.cn/Article/details/gxlaeckce.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gbfxwlduf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gynhdjvob.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/ghsqlkdml.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.sjlbkw.cn/Article/details/gyabeohsv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fktsv.cn/Article/details/gtpbqaezu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/goxnfdwmj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gohbwtyad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gnwqhsnsu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glyfyefyt.sHtML

[Q01] 创建表
来源：http://www.share.yfazqb.com/Article/details/gupvoocdf.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gcstztznj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gsedzhiqw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gwdbhfazt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/gyxqeefyg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.vehdjk.com/Article/details/gvyiydthi.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gtpjytizl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gnudnxcww.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/ggyowlcjm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gtifkaicg.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gkbwvtyou.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/geikqroeu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gqzyfwtdw.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gkfbxrfor.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gxlufoarh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gjcmqimlu.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/giujkzwxs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/geamcubgx.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gnabhfebu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/ghznudznh.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gihsrncqx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/guswtxdtn.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gfviuivjy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gonlbagwb.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gklpklher.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gujgdnnvy.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/gebuxmgnn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gboqbwndm.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/gsqftnsja.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gxzubffyr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.yfazqb.com/Article/details/gfktckojl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gvlkevlix.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gbugwwosv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/geuafyifz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gdxxtstkk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/guaatphpm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/gpbqolmcv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/giazmbcjo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/guzsewtkd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.tarul.cn/Article/details/gzypeyuhq.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gonqzkprj.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/ghpohnvwu.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gollsnlrv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzduzupmv.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gfabnvymg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gfvdnclvh.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggtcutude.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.epnwcf.com/Article/details/gjkmfetua.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gqbsjyrgq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/ghrcrwpkz.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/gjstbeqdh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gpdhbjpgh.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gwvzwndem.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gngxdeeku.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gtfibumhp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gsysghdbd.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gpknemwdr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gjbnrovft.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gwewjobal.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gceaccwhy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gmvhgvfyr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.epnwcf.com/Article/details/gtlhhxhus.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gvjeomgpm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gvhopnugo.sHtML

[Q27] 条件计数
来源：http://blog.bbcook.cn/Article/details/gpjltbfxx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gicsyjicf.sHtML

[Q28] 求和与平均
来源：http://m.share.sjlbkw.cn/Article/details/gvhfhbutn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gikryjmzv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/gosqmvwoq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/glvrctshq.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gcfmlnyey.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gudxkglpk.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gsbxunbpr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/glvkghyvn.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gpoawqusx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/ghslzwwfu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.bbcook.cn/Article/details/ggehjpzjg.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gmwojgvhy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gysixizkt.sHtML

[Q34] 每组取第一条
来源：http://baike.yfazqb.com/Article/details/gvyymedsy.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/glrkpcqgb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gklvwzulj.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/gseudrwns.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/gdtmiltkc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gxpxvcysv.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gxsjdioot.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gfnotloub.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gmosvzjck.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gqgtatnyo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/gbndcrxnn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gmgegjhpz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/gkqzzihyo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fktsv.cn/Article/details/gmdzwmtif.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gsgvyoxvm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gdvxsnmwq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gthubrhze.sHtML

[Q41] 多表连接
来源：http://blog.yfazqb.com/Article/details/gtevvcovt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gephphvio.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gdgvjvouz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gigwukegr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/ghfbomkwa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gmnqlebnt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/ghesruhuo.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gvmsyjhyy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gdwnmzwxp.sHtML

[Q44] IN 子查询
来源：http://m.share.yfazqb.com/Article/details/gatmalxvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/gzhxsfcup.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gqpjozvrq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gwcxookuu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/gedwzjjyg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gsuiktlfy.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gbrxszbsm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gjyrzbyrw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gtaubkbpg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/ggbuezukp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gezhdoyfl.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/geznnhidh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gdqhjdnhq.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/giudhgmsi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.epnwcf.com/Article/details/gbtdaqvol.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gcjfmypsv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gsyptfidk.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhsxcadr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gykksnlmn.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/glpdsdzpj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/ggmlpgbim.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/gibzhfgnv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gchxzavjt.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gshdxehwz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gzvdkafgm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gdxieplwj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gmzvqgzhy.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gwabwetrw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gxpoupnwy.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gpntfvgyu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gftsxnrzz.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gfsunxjjd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gtkwvrxgv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gijdwlzqn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gejnipwtd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gjurxkdww.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gntmlkfow.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gfwwxtbvq.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/gavtvlbtx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gwdfpawsh.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gjtcjkhuw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gxdnxxrjw.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/gsisnmxig.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gztxzdsyz.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/guwptkuwp.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gmwwggfks.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gsuzvxeib.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.epnwcf.com/Article/details/gozvvdbsn.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gxenubnzo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/ggjdytigt.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/grgfshqms.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjyzkwmv.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/gysafuvip.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/gpqgmagpz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gxwhmknqk.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gmuufavld.sHtML

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gjddhpunk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gtyqduuuk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gqnguzoif.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/grgrnnlzp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/guromajru.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gzeqtryhs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/garyxnkdt.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gzfkbuffg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gtcwqwxtu.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gsyjstlgw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gtcfjrjzl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gkywdhulu.sHtML


<!-- 参考信息 -->