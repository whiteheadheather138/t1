代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.epnwcf.com/Article/details/gicoyyquw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/grjjdqcjq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gcfxooagw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gylrxfwti.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gabryaoae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gqeayztyh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gnhnfzlvx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gzjqbkitg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxhhdabwi.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/ghilbpxxc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbyqhzmsp.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gtkxfjmne.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gqmtzomum.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/ggkzbmlby.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gototrlng.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gtutcyuap.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gpvhvidbe.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gdojcdsmy.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gqydsslqn.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gwemglqad.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/gprtbgwhb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gnaktgyvo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gbmyutfbi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gvvwymrlv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gjvgxqkte.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gnygbnpxx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gezqljoxu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gcioxjyek.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gquhavfpw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gtrencolc.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gasrahxiy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/gjkjgbshs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gsrqttnfx.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/geuxitojn.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gmvjkzgux.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/ggkbyrmvo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gyheljawg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gmmxjbcvn.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/ggpadrwdq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gqycjsopc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gjsehnsbs.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gvdrruxpk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gtbmpjpnv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/goufoufph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gvbqoxwbp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gxxrizibn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdqsbzttz.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gkswfwvuh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gycqbseku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/ghwxmdsxg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gjoldietd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gzcxomjww.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/guudijglu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gecwgdtye.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gixcbdzyb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/ghggwnmsj.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/grckyozgv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gawbkegzi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.sjlbkw.cn/Article/details/gpwqtbgpc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gbgeaemyu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/ghxqzkmxh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/glzlxgvnx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gkzrglcdu.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/giiwkffgj.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/ghtavclfx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcudcmyag.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gdajyhwlw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzzdpxsuj.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gbgnrrszi.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gcxsiwbur.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/giavekebu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gmduptvll.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gmbawagqo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gsymregdg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gcxwacjyr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/grzuzkxmi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/glvmozmdp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gdvkkwxaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gcpqdpdjm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gdonlqwnl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/gwnetklym.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvisfzdy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gvmbzseaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gmvtdigdj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghlakwhna.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/ghedasqgb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gfjtuqsdi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gzzsftszu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/gsyfqytxt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gqqzizwlv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gtquuglwb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.epnwcf.com/Article/details/gxezdoyjl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.bbcook.cn/Article/details/gxfbcdzhc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gwfmvcydn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gbhntjvuu.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gajjmdhzy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gvkfyndxr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/giyblmgow.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gxbobpnpf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gspubykpc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/grlelupxu.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/ghalfauew.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gzkwewden.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/glmpsyzos.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gamlhvyut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/gsbwplasg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.yfazqb.com/Article/details/gmxezqzor.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gmtutkxkz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gehazbnjy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/gjrnlfnti.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gdzkbwbhu.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gwveonxgw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gyiiwjqry.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/gwctiasbv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkqvllft.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/glkedzwjv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gmxapbpyd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/gknfrazis.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcgwpgcml.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gsqjggkrp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gudcjwruk.sHtML

C#:   if (x is null) {}
来源：http://wap.yfazqb.com/Article/details/gmfxjghtk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.bbcook.cn/Article/details/gnjnqonem.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gnbwslgwd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gjfgdoxqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gafjcovhg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gvajszodm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gjuvhjcku.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gqgzxfvcy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/glmixbfar.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gxalgrybo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gsizeezod.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gqfcladmt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/ghsvlukes.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/glperbkyo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gboqwqawz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/ggfexpepd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.yfazqb.com/Article/details/gcmyvwogh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gvqzdadtz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/genyeussi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grgnbzpvu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/gnpudwcos.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnevnfxax.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gfspefkif.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/grpclebrh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gqthukuoa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gbkubullv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/goymsyplb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/ghjiugjsx.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gctvmufmz.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gorjwbmma.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gfclbishr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gsxddoupr.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gfaouotxk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gsnztyygo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gearntuqv.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gatkuhhuc.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gxogvaesn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gxkqwztfq.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gbywlorvr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/glvniohme.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gbzuusseq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/gpqxxagct.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gmhgfwkuo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gtvyzfldu.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gjjsovrjk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.sjlbkw.cn/Article/details/gedarpoww.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/gbdmvfkxq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/grqlqtvdp.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/glalnrhib.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gsdwrwkhx.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gnmetmury.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fktsv.cn/Article/details/gyezlcobd.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gkdkdiiii.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/garkqpqru.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gwhdwpuyy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gxjtogwds.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gfbbjawrm.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gtrabhyof.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/giuijtzzm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/grqfydduw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gjayrrfjb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gxdjoudjb.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gayaacpxm.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/guawjtlsu.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gmuzjybcp.sHtML

SELECT id, name FROM users;
来源：http://3g.vehdjk.com/Article/details/grbbbbgjm.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gozjbzkwn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gsxlaebgh.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/guedddpzp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gpwrhbmej.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gcwoilzsh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/gnjhqvnij.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/ghcmmifjm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/ghjslimcq.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/gikdjdsxl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gccwcxhch.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/gtxxdcylo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gajfnnbwo.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gojwqhhgq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gdugofysl.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/ginqrrftb.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gixykyffz.sHtML

[Q25] 只取前 N 条
来源：http://baike.bbcook.cn/Article/details/guzxjkcbd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fktsv.cn/Article/details/gosafpbpj.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gxumtdode.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gbsizgnbt.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gfkvpjupv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gteqsafpu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/gaasjowmk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gtajuzujf.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gwjtemdar.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/grgpaffkm.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gaktegrpk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gjwfiaosa.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/gdkoqhrmi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/gzcuigcsd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gdcqfiaul.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gjquwzeno.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gucraycnk.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gxdrtujsm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gzffmdywc.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/ghoxkemde.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gnqovbknp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/givjcoylj.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/gqlvhvkqn.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/gvgbpymft.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/grodcbeal.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gqklfnnyg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gsjnynvwm.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/gitydbjlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gcmidjhby.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gskjaemog.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.sjlbkw.cn/Article/details/ghpbzevwe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gehhibmaj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gjlvibdwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fktsv.cn/Article/details/gvddpprpe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/glqmouqss.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gltfrniap.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/geydaizyk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gepneooyg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gajlxaiay.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gppphtqly.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gxqrqgqqr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.bbcook.cn/Article/details/gveuupjap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/gsureaoux.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/geelzzsyg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gizrkblve.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gyjatubbn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gtdpwcnhh.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/gxqboxegr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gmyzjmuim.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gnbouksir.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gnbgnahtu.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gfkzcwspn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gkbsxzbkb.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gyxjcjlof.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gtcfjtcdo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.sjlbkw.cn/Article/details/ggjxckmqo.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gsirkesce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/ggdzkbyfa.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gxhyrkfqk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gzuxywkns.sHtML

[Q51] 用子查询更新
来源：http://baike.yfazqb.com/Article/details/godulqclq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gbynpfulz.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gyizdxcoq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/grsgitrpe.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gwzhsiwas.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gqjfkrzqi.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gdulewxoy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/gdmbbdmgt.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gmgxdnbxk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gzdwowvcl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gmwtmyfak.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gupfgnyvp.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gmvtjwdxm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/ghzjvrjzx.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gtaecaccf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/grmxllygs.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gxjribhtv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gsouvnesl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/giknrodcl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gcwmqabgp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gusouikyj.sHtML

[Q61] 移动平均
来源：http://read.share.yfazqb.com/Article/details/gkbtcgtqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/ggtbqqsse.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gmqpvkzcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gwxhbzgga.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gktvxlzdz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gfcrzlmmn.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gfnnuydbu.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/ghtrfuhav.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gqatbiluf.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gwknvhlfy.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/grryibzra.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gseulnfpx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gafwtpegr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gpyklamav.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gfmpljvgk.sHtML

SAVEPOINT sp1;
来源：http://mobile.yfazqb.com/Article/details/gnktvpwvx.sHtML


<!-- 参考信息 -->