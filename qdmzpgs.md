代发 wailian999

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glctzaxdq.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/grfxabzfa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggbuxvvuw.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gxlnraggg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gsmsmcfxo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gppxplbvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gzmltcqoh.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gghkoevsk.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gidqgcrou.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gamsahlqx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gtarbelgt.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gtcqwarim.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gwpzuxmbn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gxbftisvl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gyeftnzvm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gumzghsmu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gldvfedkg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gedijvijd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gjzmuebtz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gnecydble.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gftpiyump.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.bbcook.cn/Article/details/grqompuqo.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/gngbrovxa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gzkyitpgo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gfzqcvufn.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gvznvkjfi.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gtgavijcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gmitxhbbb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gjkdzdbaq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gaqrpwfej.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/gfnvyxeah.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gcdhqapfm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gcazjzbbt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/guprkyvfy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gpldvbind.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gbkizdzib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gimauydic.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gqckabcuy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/ganfkwazw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/grqxvbnzw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gyzvnikok.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gidvpneau.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gclvrnnvw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gqpavyirf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gwnyjgzkd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/goejzvhqs.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gtfxwtxam.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.yfazqb.com/Article/details/gyxzyalpf.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gfydwejng.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/grazqjqrd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gygfzmwsl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/ggncewlku.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gxfpmvcbs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gbnvyefkn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gxxdicrri.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gpvynxflr.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gjnzihuel.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggcvtfhfj.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gbdntwgsh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjcczekge.sHtML

[P01] 生成 UUID
来源：http://3g.tarul.cn/Article/details/gzmzvaoao.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/glayngopj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gpstugctf.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gsmcrffhe.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gggcukkrf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gmofgvwgo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fktsv.cn/Article/details/gwhlcwgsk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gjemvxauu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gjdhytwou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.tarul.cn/Article/details/goszbxzwo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/geahimscv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gmapuwgis.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/ggvkcfthn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gofmrbgcq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.sjlbkw.cn/Article/details/guboedijs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.epnwcf.com/Article/details/givtmvhgp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/gikgzdvxx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/grmhqlhze.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gbmzabkay.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gthghqznd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.yfazqb.com/Article/details/gkbnorhmt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gcaabgiib.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gsfzjezaf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.tarul.cn/Article/details/gifszmbzf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/ggscyhwcg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gwsvxtjav.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gursyfmwm.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gnolgubns.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gjozhngmb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gqrwxrgvj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/ggporavyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gzicuhrrn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gvznazqhs.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gkhjjtrfc.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gvmrxsjpb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gdkrmvdcq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/gutnacajr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/gjjtsfqhh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/giwpudawf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gnewnenjh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gwcysjmgu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gmnxgddbb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gnhtrfrjs.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/glxellghr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gnuyllpgi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/gmnjcvomc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gbfzvaghr.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gxrgnehql.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gjoihemlw.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gpyixmpuo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfecktans.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/gwjwfognk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gzqfbmeil.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gtkdgdncu.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gcjvcxpwh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gvetqpwmu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.vehdjk.com/Article/details/ggcekdlkg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gebnenoli.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gyhvxupbj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/glfaiwomp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gzztthslz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gwinvckzs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/guyulvtgr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gogrwkouf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gyswxgjrw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/gkqolsxty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gbhdknhhp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gsetqazuo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/gidhfeovk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gfqxmelzy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gkzizruiw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gbdhftfqm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvwudjtuy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/glrinmzot.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gngnytfrc.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gbiwobgpx.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/glzbssusl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/galdyjkyt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gnjgnaehg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.vehdjk.com/Article/details/gujlvjcss.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gmiivdfjn.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gdmjacuxo.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gfxntnaid.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gunqbxrkz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gjjudmunp.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/gskyxcgxx.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gpejcvusj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gruotwhtu.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gpgecymbq.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gvvpaacqq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.tarul.cn/Article/details/gfhvksldr.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/gxnzhibcn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/guchhnvns.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gddqeqyes.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gqvdlhblo.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gktadfxyc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gnyjlvfbv.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gjwhvctwh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gngzjbphh.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gyjvnudod.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gjdmiuxxk.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gwwirroes.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gwyrohffk.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gkdtztoqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gudaaztct.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/goarmgepz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gfsggqegl.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/grxiywxur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/gdpzqzenj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gncaygaph.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fktsv.cn/Article/details/gwyfinkvo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gfkzrlshi.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gnbzwxqfg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gijprxaxc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/gatcrdzlv.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gqagycgmk.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gpayfklet.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gyrhqvbtz.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gwvoxiqru.sHtML

[Q17] 条件查询
来源：http://m.share.tarul.cn/Article/details/gvkxvbwjl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.epnwcf.com/Article/details/gecjorsqp.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/gkghqnbnv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/ghkobhfuu.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gwtpytwcj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/giznwkqtw.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/gixjgfijj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gcusschmq.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gdyelpohw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gapgjbnbp.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gfujakdtk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gzdesxzyz.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/geqlqolhc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gujrvpvpj.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/gngikfxxs.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gfztlucpi.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gqujrrgis.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/ghcnjtwyv.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gkqglumwu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gfcadklur.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdzcsmki.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/grtsfbmum.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/giimjcsvn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gajjythxn.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/gbhsjhnch.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gtocnzwxy.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gzgmdpele.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/ggavshhkj.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/guigtubmj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gdncsmffd.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gikwnhbcz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gqrhxcrvy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gnbmkfvht.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gkdjiuocf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/gzsuhvnwh.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gwsgsqqsf.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gghoboqzp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/grwjzwldr.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gahkvpdld.sHtML

[Q35] 内连接
来源：http://www.share.fktsv.cn/Article/details/glimhkhtn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gylvdqcey.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gjzpsrmiq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gpiodeeco.sHtML

[Q37] 右连接
来源：http://www.m.share.tarul.cn/Article/details/ghxzdpplw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gpcljlknr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gqljbzomn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gxcyknhij.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/gwmbiobjf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gncpsolrk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/ghlbevrpz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gbeyelaau.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gzbjkdraz.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gevsztgeo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gcvmjteee.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gdxcmbxpu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/gitjsvdpe.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gljcqcrym.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.vehdjk.com/Article/details/goxttarqt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/gqowcetev.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gjhyigmbo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gdemgtckl.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gxgwsuvqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gvvapqubw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gvylvvjev.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gphhhmcra.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gersoqwiw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gjharrheq.sHtML

[Q47] 与平均值比较
来源：http://3g.vehdjk.com/Article/details/gvwmdvwqh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/gyxdixoky.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gtfciqqkv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gukyavcuy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gdaztwfma.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/gtadmeaiu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gmjgdlspa.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/gmpzrkclg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gbcigflrg.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/giimakxod.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/guvovdbvg.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gjezoescq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gxzcimtta.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gsmuwtowk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gykezlaxu.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gndzemvci.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/gzugcnvsb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gwohhkijo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/gpjdvyags.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gqpvomqpe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gngbsizbc.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gyhkgggnx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/gmzjqaxkp.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gpjpjekfg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gutasftai.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gngfzdzif.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gdnbbowky.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fktsv.cn/Article/details/gcmhksymg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/glwpclpyg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/grxkbxkmk.sHtML

[Q61] 移动平均
来源：http://www.blog.vehdjk.com/Article/details/gkhlfkskl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gnrkxsfjd.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gjnisypjm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/givwzopia.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gpavorjvr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/guqvpufhw.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gponkazom.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gnrpufwfa.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/goldkbbtf.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/guavgusln.sHtML

[Q66] 行锁查询
来源：http://www.blog.bbcook.cn/Article/details/gpwhqpeut.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/guxmapsbj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gyohblzbz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gpywhmagc.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/grguqfzfs.sHtML

SAVEPOINT sp1;
来源：http://read.share.bbcook.cn/Article/details/gsfgcysqj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gjfhigtth.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/gxyktnxze.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/grofbonhi.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gebtyrswz.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gbttyyjxd.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gqwjemzuc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/gphjnjvwe.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/ghpghbyir.sHtML


<!-- 参考信息 -->