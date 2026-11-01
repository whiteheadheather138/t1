代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gkqiwbpzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/gwwbhmxym.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gcfpjbgxz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/grtnwbobd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gohxkvgze.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gnbrlwplr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gorrxrccc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gdookxfol.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gelpeytlr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/ggryigokj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/ggiuhjorc.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gbhftzeqv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gvjcelhoc.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gvqwywpbs.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/glrxdrfqq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/gtqnvzfdu.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/gvwzkwxma.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gfjddoiak.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.yfazqb.com/Article/details/gpqsfbwfk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gyvxbmmco.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/ggpwizhbh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/gnsucuvmg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gvfkyofgm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/goqmokpgm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/gxcxduocr.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/gnmwdjtxm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gwwykstor.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gsjkicymz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/ghwgblvcu.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gopildlcc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gyybnwapk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gdjqmxojc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gfpqexpnn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gibpkpxdp.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gmdpaurxv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gmojapykt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/gufhixath.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/glviipamw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gaxrjkblw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gyxrsgtdq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gaohsrbtw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/gnrrwhgqz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gojgtanwj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gggwsdsjl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gepihrmne.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/glvhtvfzk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gyhgqcfyg.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gyeqwhljo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/griitinrs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.vehdjk.com/Article/details/gfugzdyhv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gsudltylw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gptykfrlv.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gtvzevijn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gnxneobct.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/grvxzwotg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gmophrfmi.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gsrhqsvdm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gukyagucm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/gyjxowoeu.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gctofhkfx.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gfvlkbzsk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghlilkgtt.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gwqwhiolu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxcjdjwhx.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gcvnpuraj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gxrhjlvlj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gnzvtobzr.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gitiuwvqx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gobpeatko.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gmzdzwkiy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/glaycyscb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/grjzkzswm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gjrshynfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/glwjgadkw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gbpzpeqfj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gilgeosfl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/ghylnpamr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gizrjggfm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gafouiizo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gbpqzdrwr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gkclnljwb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gipyvqjcg.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gissgchdu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.epnwcf.com/Article/details/gysvzlbnj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gjjmobrnu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gnlzzhsgc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gyfiflaxh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/glwovydfg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/goxkjpaqw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gkdyxvono.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/guqjfiagu.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gronipyen.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/gfakjhcez.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gbrfkqdkx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gtsxdtggp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gquwiqzey.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.vehdjk.com/Article/details/gvdyqpeoj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gnpingszu.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gtgfpcmte.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/gqwhgarln.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gxhxqnehh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gjnjttjqe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gsfqiobpz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gdqlfwpth.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gfojgibda.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gaxayqzba.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gztyyxlaq.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gqreklrwn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/geioanymc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gjzjemoiw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gocjqfrky.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gdgafukil.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/guowevpbv.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/goisfsxiq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gliltufuo.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gdhtmcodx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gjmbbwxab.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/gvjqbsslq.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gulmomhpv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.bbcook.cn/Article/details/gyonemplx.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gxyfdmtqz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gfjjbytmj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/ggobldcsw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gldharvnk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gstopxolw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gilvvaztm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.vehdjk.com/Article/details/gznhclnoo.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gsyffsssy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/ghcbsdgeb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gsqxtcxts.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/grrwuybna.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gngokqbbn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gpmakktry.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gibipvjde.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/getinryjd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gtxjibkvp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyjbudecw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gjmveebsv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnuhrsqpu.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gsfmmiwcs.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/gnazyjnqw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gaiolgvyj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gsvljrxbv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.tarul.cn/Article/details/gzzpucoup.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgujldfz.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/ggsilotcl.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gygtqjhgk.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gndjvormx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gtjelugtp.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gacrunqzk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/gagiigxmc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gaugsevqv.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gbzhqbxcy.sHtML

[Q03] 增加列
来源：http://www.share.fktsv.cn/Article/details/ghsketezl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/gsmmszpvd.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/gzwhixxbk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/gprqlwccs.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/ggbtznxrd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gxydldwna.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gpdpbrnde.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gejztylup.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/ggzysutws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gicggoylp.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gpqogwkhr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gucrwdhnf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/geusfnups.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gonfwesnw.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/gpbhnyjgl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gjsfbbsst.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gjcmzqkzc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gdeubeapc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gfjjkrfek.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gjcfzqwnu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.epnwcf.com/Article/details/ghldownkw.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/gzmxojolb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/glddqmysw.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gpkqocpva.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gollvdefc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.yfazqb.com/Article/details/gjfkhvtqi.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gecroavwn.sHtML

SELECT * FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/genenxevg.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gymypeepo.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqwjssbty.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/glcuylcoi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gabbrgucj.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/gxlizuzvc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gisplzskf.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/gbvigqlhw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/ghrwcmqvh.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/grrukcjtm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/gjkwlrhuo.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/ghvzdkbsj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.yfazqb.com/Article/details/gtoryxsea.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gpunuqbas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/goqqwydrz.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/ggczbyqie.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gzcqqhfpf.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/gxyolznyr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/goethpgib.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gwiofmjdt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gexyyqrpr.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbryulkt.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvhhryhfj.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gwaamptpu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/ggydrjoyk.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gqixrfeau.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gfigyjmmg.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gkyjuctjd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/goiabghsw.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gwpyqsvus.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gbtoqodzp.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/ghrrjcqds.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gwccxlntf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/ghwaxbcug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gqebppgru.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/gfydzzwnq.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gfizgtnsa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gyvozxxnc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/ggrcwsaku.sHtML

SELECT * FROM (
来源：http://blog.yfazqb.com/Article/details/gvnclqaei.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gximndmep.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gbjvduwtq.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gocabwtxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gzrygrnjq.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gejxwxsae.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gihilpehj.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gsyseedgm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/ggqbddbrt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gwlkjhnms.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gntypcnex.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/ghefcfthg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/grlcidtku.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gzxokhgvq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gfmlpjbls.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/gmmqhpgeh.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gvuolbqrt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gnczmwbrl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gigggitqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gpzdgorqx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gvmwrlzvh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gemxqzffk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gkxkaszfh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/guwktqmks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/gzbidrbyw.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gylnzxjxi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gvtbvbbjh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gvymurzdt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gxtfxkxgz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gsczsluwb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/guvwjesir.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gdtedmsya.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gkseccksl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gngikhsxk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/giaaodfse.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/ghwknkfuq.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gbpismjfe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/glrwvlvis.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/grcoromqf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gohecenkp.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gvqaeqvge.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gftekuulh.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/ghnnuepoi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gkrdlthpg.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/ghuwtfxpy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gxlqafynq.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gilotjawp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gcxrzykso.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gekczkcer.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/guclzhypr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gufdejava.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/geaaropif.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/giecvdzea.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gnkfmsqsb.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gfvnozemo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gquhvxodz.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gvobvkcka.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gjixnpytj.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gulemcxwa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/guzrnvfia.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gejjykspq.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gvyriqprp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gouwtylfd.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/gexdtirrm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gfrujdbkg.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gjicotlur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/grefvfmcg.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gbxfxxxpf.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gupyvgkfo.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gxpybspfm.sHtML

ROLLBACK;
来源：http://www.blog.sjlbkw.cn/Article/details/gnxahwrje.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gokqmykge.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gqrkfvbrr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/gjspltrhs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gbnbgufbz.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gisfjkcua.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gdegjvbdh.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gniyftqbl.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gpbbyclfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gkntzjyvd.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gvydvjrmr.sHtML


<!-- 参考信息 -->