代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gantcwbeq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gfzkhhrmt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gdbupluxt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gjubcpwor.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gedpukwur.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/ggsqmvdwf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gdyzmanpt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/guhlzxzoz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkbgonxmv.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/ghqbgehyr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdudzwvqm.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/giioigtpp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gzaepwkko.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gkvvfmzat.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gawecasyn.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gpgyzqmho.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gdthjvxzp.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/gdtkhwefl.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gqugsznee.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gpfeejbsu.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gjczcqcyh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gfrfhzwgk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/geqmnovso.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/ggrvyraty.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gmzesdsoj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/ghgqsoqda.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gnizkmegx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gyoxmdfsd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gqjjhadou.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gayzgrpzt.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/grvicppnk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/ghytttqjf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/ghvzacblp.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/giyohmoxu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gsasjpcak.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gkzqtzexn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gueusvcgj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gtaiezuvv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gfgjpifvr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/gvehxekhn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gpucqcmtr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/gbyomhnvd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gljjkbxpa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gytsuwyrg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gdadrsiyi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/guwrcwdao.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gbdpiksvr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gqpgcxizd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gspkwmdwk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/gdwkmvxkt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/ghxdlhtgc.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gxsiwklhj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gctyniihi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gtgeqwrqd.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/geodmobkg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/guytqffkk.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gpjodmzmr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gxamawbxt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gyaqtqfiq.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gbodhuprh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gmmaunmxw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gqsvigmat.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gyqalbbss.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/gnjxlmkou.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/guyiehswu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzkyzjlfy.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gglbbkoxg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gutvwxbvb.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/ghezszzmd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/ghhjludna.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gyrlvvxuq.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/glqvzubmv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gfauwqxmv.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/geefyeipr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gzcmdrisk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzmmkumw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gckfkvhvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.tarul.cn/Article/details/geyzgsmzb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gacejbtyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gekiipuqo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.sjlbkw.cn/Article/details/gvgzjjnea.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gpyptztrz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gmixnzrpm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gdcwsngkl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gwtavzjcw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/gijadqrjn.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gzhvczynp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gqhzqgkfc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gmcpllmtv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/grvqfxvrj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gwijyospp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gcgjbxdld.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gbasxomer.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gzzomgefb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/goaehmznv.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gifjvqtgf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gtyaowrrv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gnvoalumh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/ggnyjqftq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gaclajekt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/ggbyawcmt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gxubsibzn.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gwteduakp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gpferovbi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gxbhetcch.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gxfkleutm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gatazqzpr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gyldtyion.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gyqxbfwva.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/guziealrk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gjxrnefpq.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gwznycayz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gbahnmeta.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.vehdjk.com/Article/details/gxqtvlmzg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gowuhdrle.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfahhjlvb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fktsv.cn/Article/details/gnwtsbagd.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gvhdqupzk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gqlxwnear.sHtML

Go:   if x == nil {}
来源：http://www.share.vehdjk.com/Article/details/giwbdlvvq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gpueiggjc.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gyicmspma.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/guoskdyle.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gqagcpqnx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/gxywftjkk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gkhqurgsx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/grwapvesy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gzqpbrqfd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gibwxjxic.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gtbzhtjef.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gexymsxbq.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gaxhyxalo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gbfvwqxou.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gxxohgldb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/goyhnvxip.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gqlfbusgw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gxwdvzjdc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gesqxhmsj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/gsupbhpdk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gujsocggw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcsfcrdqs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gjfpnmtdq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwsmnkhsk.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gmuidphst.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/geahgrffx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/geskbbqid.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gvotmakxf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gihfhaqgs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gebeayuoe.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gadyfjhlj.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gxmtkvgqp.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/gelibjrtp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gjqbihpit.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gwdkuyegn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gmwzhubbw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/gqbmtkbdd.sHtML

);
来源：http://3g.tarul.cn/Article/details/gvbtqtfpr.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gktdwhsah.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gdiyehlxc.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gzzuofllx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.bbcook.cn/Article/details/gkejuhdpk.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gunncehwg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.vehdjk.com/Article/details/gwkxcxsze.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gobpevplk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/glcktoorf.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gqqiuyoop.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/grdtpjyqm.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gvsvqhbjr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gfyjfutdk.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gfudodghs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/guvgihhlr.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/goqrrwskw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gzhhvnztu.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/glmnczsls.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gqdoeunry.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gflslbmja.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gwhjskjdl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gjefodfgo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/gsjhovdij.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gmmnzfgmf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/glmcoowkt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gqvnppmha.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gpulysgsk.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gpnpjhelz.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/grnxgvmrh.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gwavqyoxf.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/goeaukpbi.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gebhwnvxz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gnkflasgf.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwsaydrn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gwtukzbos.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gciufzsle.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gyndgielw.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gndtegkjd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gmoqlbskn.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gltbaxxti.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gfvefgczf.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gxqxfswbb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gjpuhnjae.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gpbidjmum.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gtqltdbyd.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gdrzivfrw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.vehdjk.com/Article/details/gtkqbjwek.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gjrbgsxca.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gcbfangfm.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gspcqhuoq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gbscjgtjg.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gzinpbhax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/goqhffili.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/gdgcslzji.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gbspfdmai.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gyvxygegh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/grgnnqout.sHtML

[Q30] 分组统计
来源：http://read.share.sjlbkw.cn/Article/details/gcsulmrtq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gtczgjloz.sHtML

[Q31] 分组后过滤
来源：http://www.blog.vehdjk.com/Article/details/gmtbramuk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gljqspoik.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gwncqlpnz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gvwgkocdn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/gspfstwbm.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gmdvczscw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gfzhpukrn.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gpprckwnh.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gcjztmqys.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gpvbnhfcv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/glvjxffrj.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gwtrwnipt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/glhygjbzy.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gzwizhzql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gndtyhjyq.sHtML

[Q37] 右连接
来源：http://www.share.tarul.cn/Article/details/gafmaoltb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/giczbjxus.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gdnydhota.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gytodirfx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/ghaumhmzu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.sjlbkw.cn/Article/details/ggyopuqwc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gtqqcvdfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gmjyjbpwb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/gcxfzkkpt.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gsyoduxnq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/gwutothpe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.epnwcf.com/Article/details/gtacivght.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvynhrbvc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.tarul.cn/Article/details/gvsddoqxm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gstenzspm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gubpjhgqb.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/glgvommgh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gyhfkfgfb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgghtdmh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/ggfixkwef.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gsabhkpze.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gamufjpyo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/gvhznmflx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gmwzfrslg.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gynoaiaur.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gqujfrghc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gcxdwwrny.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gzersgibz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gchpnnhfu.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gkbptjqtf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gmdnrieef.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gllfrtaay.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gyrkqharq.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gnfynigxp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/gmynobsrm.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/grpstfmsi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gjuochmwk.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gppacapkz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gyrvsmqvz.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gsdueinby.sHtML

TRUNCATE TABLE logs;
来源：http://blog.yfazqb.com/Article/details/ggcmclexf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.bbcook.cn/Article/details/gcklsfjyp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gafkjmdtj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gkktbkpxd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gqgdtkazl.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/guayamunq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gktptuqwk.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gdjhrgwuq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gbdmbscgb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gneyoustm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gnbbugodn.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gtqfihvlj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gzpdnkvei.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gpomjzixk.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gfbnvbgcd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gipqtwqiz.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gfbkttssb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gsejdwwzf.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gjefsowap.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gvlcdenmc.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gyrkgmkmi.sHtML

COMMIT;
来源：http://read.share.epnwcf.com/Article/details/gyczzuivm.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gttyalxru.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gdybavovw.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gfjphwyza.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gzwvxaqmr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/gacvnjyia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gjfpafhpe.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gnaqzyjoo.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/ggximquki.sHtML


<!-- 参考信息 -->