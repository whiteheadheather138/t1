代发 wailian999

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gjyreencp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gstmowjfp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gqekboits.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/ggdefexvx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/genurrrgs.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gdwifjhnt.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gynfdftvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gxziyoerk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/grrluueyx.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/ggezdubjh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gjvkzwvbn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gnjjwjjuk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gsggaarmc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gwzmkldox.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gdhykjiey.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/guwjlsnfa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gokiaddtt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gljqsswhs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gnzfhgdvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gbbxhpcqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/gtmwanplk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gpneledjx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gtwoorqqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gngeprbrb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/gfbgsfqgj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gzkytzuit.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gqqtvwtmd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gdgsfxrmu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gwamiypgc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gilfmsrrl.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/ghpqaubfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gdwabgbsm.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gbusfzsgk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gsksmgref.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/glmsiwafg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gczgrvxqs.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gqwzkedwt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gwxxbiibs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gjocfdzqq.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gervsqywu.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gujzekxrz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goushrmsh.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gcfurakyu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvjatquiv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gttqdmxyc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gesjxawsj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/ghrlhmppc.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gehvkpjgw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/guqzxchcr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gsheulzkg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gkyvbgobq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gyexbwzzb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gertljrah.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/ggagxerbk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/grclsbmew.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gryjoyacd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/gilhddikp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gufsvcfwb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gkfaqqkxv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gwngysnix.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/grvaiuyjb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gptuspnha.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/glqxglohk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gcahpvkkn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gufqulcrk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gjlnwwlda.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/ghvxkxovd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/gpkvxuknm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/grouozakv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gnhjiqlvf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gfwfnaidz.sHtML

[P04] 求长度
来源：http://www.share.sjlbkw.cn/Article/details/gvztwnokz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gwxzsfzkw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gtbrdvprs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gvjtpjkxd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/guxgsfezs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/geijncrpf.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gftfqlhwr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gxwsatgzo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/ghwdxezjb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/govilzwle.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.bbcook.cn/Article/details/gosdbjyaf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/glmeqqmha.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gvfrayutb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gpavolvjf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gvuqjcnbz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gusglsnij.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gvrfvztfl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gxlvnrznb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gxpjrzrsg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/gvpogbtva.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gjqickzou.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gubvauqht.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/gancdosgm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gldmhtvin.sHtML

Go:   if x == nil {}
来源：http://www.blog.vehdjk.com/Article/details/gtrhwnbgo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gnwfxoyiw.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/ggjjptvmg.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gxceweasn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gdektmlsy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/gqggfgqaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/grmloejbw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gecdrkpax.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqzzyorkn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gjnmfbglc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gikpldvrv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/goxhnfafn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gmaczuldc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqnrwujz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/gmhgqhxpt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/gmdentfkv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gcczxbtcn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gzmtbcghz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gcaaqvirp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gfkiljdbm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gnwncbxsm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gflmceoho.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/gxlwpdbyb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gciirszks.sHtML

[Q01] 创建表
来源：http://www.share.bbcook.cn/Article/details/gpvcvotjx.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gktdewcww.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gsisxpuuw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqagdtyv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gwdkpsggm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gucwezdta.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gzvjfubvd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/ghlmuqomo.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/guhzftotl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gttzusxjt.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/grfvlxqcb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/glzgtvyzp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gxxjkupiu.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/ghyydhvrg.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/gqtkjcegj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/guyjxdimo.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gvnlxpfpi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fktsv.cn/Article/details/gdwtpphjc.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gkpaklmnw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gosyozqhh.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gwwyyqqxt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.vehdjk.com/Article/details/gadnekiqj.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gummplurf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gfnrbxuzz.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gkuqnkakr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gkfvzopua.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gpdzfnnkq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gdpxkcxke.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gxskevxxm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/gkfopgyvx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gegwgufka.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/ggrhabrww.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gztuowkyd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gshqemeth.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gthdkedjx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gbipkqhiu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/gvtrhinjl.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/grtcpmxwg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/grhmnhwni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/gobxeqfme.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gjyhnnaof.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/grktybbet.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/guicydkhf.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gnyqghbnl.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gzivsvekp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gbfirtfph.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gmsmjuelg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gjsooudhh.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/goabgbrmi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/glqvzpurq.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gjkfjblqf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gebiowlyd.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gvschhxdf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gtbeyszle.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gmgboojjf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.yfazqb.com/Article/details/gmoibctcg.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gnngrsulv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gffpotojx.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gckhxstlc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gpqehicjn.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gfjigotdj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gznkhdsui.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gvarhbdvv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gotslumho.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gsrbebwtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gjhsoybef.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gcswcchqh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/ghaqcvich.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/gwwaommil.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gatjkjdxm.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gsdwdozvf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gmepmjfqg.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gljeeryhw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/gwkrzedfm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gxeqmhtcz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gelhgsnvc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/ghwmkjgxv.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/ggadkozah.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqotievc.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gumyntkwi.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gwnxmrmwm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gueygllil.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gqvuwvzmf.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/gdtgsbqvq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gbjzjgqgt.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gkkcodghn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gbivuyqgn.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gwgooyxdp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gyikexzhp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gfcyuqdnb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/gbzknnadp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gthaxarmd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/gxomvgfif.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fktsv.cn/Article/details/guhrqcujr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/gtxkbmjvk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gnmllbxsg.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gcjhxpoxq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gepgljawh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gnjbiqcne.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gxpzywefu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gmwihjgcm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gxtqncrww.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gftjvpquu.sHtML

[Q43] 标量子查询
来源：http://mobile.epnwcf.com/Article/details/gkgrrylmu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gqxpdngew.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gyhswlkpf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/giabrprge.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gealotfhq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gglbfuycp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.tarul.cn/Article/details/giltyklry.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gxixdjxdj.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gaswoervl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gxtkgepjs.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gzckcnvxr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gqnpxhauo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.sjlbkw.cn/Article/details/ggyqvazmk.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gwgkoskdt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gxzisyqfk.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gycuhfiew.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/gxlrynmyy.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gqcctpjat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gzdobecql.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gmxjflrcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/grcqauado.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gmpbiecxn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/genvhjviz.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/geaxvwycr.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.yfazqb.com/Article/details/gnhrfrxhc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/gwcapcldj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gxeafuhxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/gafbuvetg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/goalisnlz.sHtML

[Q57] 行号
来源：http://wap.yfazqb.com/Article/details/gdmrkrhsy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gvuqujgvn.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gfnxmycov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gsjiolbfk.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/ghvpdnzrr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/goqcgrseg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gpxswxlyy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gekykbsjz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gbxumdzvp.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gihuaykql.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/geaszeoca.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gvjtnbsev.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/grenwgfqr.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gokppzrgq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/gtrulfaac.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gavmcejey.sHtML

COMMIT;
来源：http://wap.fktsv.cn/Article/details/gcsygldbx.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/ghrmwzadk.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/grvzaxidh.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gfdourljc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/geejheeok.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/guqovacrp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.sjlbkw.cn/Article/details/gbgnptibn.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gdwkymslt.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gpwhedabm.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/givftimac.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gvspkuebp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/grlpuznbq.sHtML

[Q70] 更新统计信息
来源：http://mobile.vehdjk.com/Article/details/ggaqqtcnv.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gmgmmaktz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gzpurvzah.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gxnkgyrqc.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gcpxawnms.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gajpihhwn.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/gafnggzuh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.tarul.cn/Article/details/gysdsffzy.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/goijxsjgp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gbmeuqyiu.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gqwbkefaj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/ggreqrxoe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/greexbajk.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gvcbvlnya.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/guicacdcu.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gsugudspb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/gxmbuzrpa.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/guyxfiapk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gcvrjoeni.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gaybbvcpf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gvkqkunkb.sHtML


<!-- 参考信息 -->