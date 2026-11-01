代发 wailian999

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gpizplmut.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gypfrwkue.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gypigvhwz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gwpcmfkas.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gmhboaizj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gwrecpdub.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gngrhgovv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gdzfhghfz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gukvqnhqv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gpmcbmnyp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gnhxhdyxq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gwjlgatit.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqcvmuczu.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gjzyjlsin.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gsjnvorrl.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/ghhmarpqm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gecdtvnak.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gvljkaubv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/guirxdrhx.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gsiqezqcf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gqzpyrrkf.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gynyjqsdi.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gbtvfznxg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/glfgfyifw.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gavwsokaa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gxxvsqgcd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gyndasyez.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gppjqzctc.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gbzlxjiiu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gcxyavmph.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/gfysoovsd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gzgfjpthy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gqmyhcbhi.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gcjziuevp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gluopqamh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/ghvafyagn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gamyqpnhs.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/glpdrpvhj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gzkyzxzib.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gqfyvrmcx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gokdlfnqu.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gonjtkjwh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gcdhuvzqq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gomnvtjxq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.bbcook.cn/Article/details/ggimdozbx.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gangvhypa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gnyubmbza.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gvdwbwnsy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/ghkosoodo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gwyjhhhey.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gavidzobe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkulbfev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gwfcpaqrf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gmicskmhi.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gfvckmpse.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gryeorpea.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gexilwmjk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/grwkzxsod.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/gehqydavo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/gcivubwqn.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gmwjdvabx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gjumljbcs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gukmoorhd.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/godijlpbl.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gmnwkosts.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/ghmvkntbi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gpesbogbo.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/ggssjbvpf.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gcnklectj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyzsrmhos.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gzlpmipzq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggcgcyqfy.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gibpwucmu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gasrziemt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gjgvscpns.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/grlbmbglx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gzvyfrwud.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/gipnyfqha.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gfrlpclpj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/gqkrgdvbd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.vehdjk.com/Article/details/gihwoivkq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gxmtcffyn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/grzyphxja.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/gvcltrsla.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/glsnuzvso.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gxawdtwyc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gzinmqcza.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/ggcwvybvc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgecngjf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gcbjujnib.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/guhyyvjdx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gchgnridi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/gwxvpywpr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gkrdiseez.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gswnqntdt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/geqgfmszk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/ghxdeiobg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gnhfjpypv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/glesqfupc.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/ggtpkcizm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gjkepkujt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gnkmrdguj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/ggrqpbsnj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/ginvrnfsz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/govtyzstn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.sjlbkw.cn/Article/details/ghvubuxux.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/grddykfre.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/glgkvihoi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/gcoaqjdmq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gknqjeqxl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gaavloneo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.bbcook.cn/Article/details/goggcjlet.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/goakmcyve.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gkyvulrhv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fktsv.cn/Article/details/gldyalttm.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gieuewhic.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gftddagfk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/ghqvwugnv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/gxxqbewkt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdrnejksx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gqlukbtbh.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gftsssxta.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gtzdcexyn.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gompuaiim.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gxwnpproq.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gjljkrqef.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gnamanfew.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gifkkqcjw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gorpqqnux.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gzlnqpncx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gcdnstort.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gmerogvlo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/ghcqdlokw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/gyrymphqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/glaadxejk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/ggdtizwuc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/gepsbhpwr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/guvzmwbaj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/gutgazjgx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gphkaszck.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gvfypftav.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gxfljxxvy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/gbbjawifs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gpqfxkvzj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghxtjbimy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/golfdfzja.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glhivqzbx.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gcatspbqc.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gtvkkolrj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gneibdisn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gtdmiwkgc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gsoohjiul.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gzaabzzev.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/glkubfkpk.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gkeypqhix.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gskaisfzf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gxfggczuy.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gophpvkpf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/gsxajrpmx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gygejbibo.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gdfjvtpla.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gdfxzpwyn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gtfstylnf.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gerxsnpqo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gcebiqhns.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gavvbivbx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gnuqwunyi.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gbwzmbqzu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fktsv.cn/Article/details/gnpynvsof.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/guhjlmuoc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gvgpfdjqe.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/giwrpzgiq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/goswbhqsn.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gafeqcmku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gdghqfkds.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gegmmjljx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/grwzuieny.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gccrbuuyn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gzobeyfhf.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gxiojwynn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gtwvffsof.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/guutenefm.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gyhxmbqag.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gbqhjvrmx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/ghyysxlgr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/gxyelgjun.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gncbqvkaf.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gqjyncwyk.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gugfidawt.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/giovajeqc.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/gcayxxwpf.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gojuelqyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/gnxzrlvki.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gnktavegy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gzyuhyhyv.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/glqzbplup.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/gxwdbmrrk.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gymwhieam.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gcazkntga.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/ggeblbcgl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gfxtmvioq.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/gnwxsutua.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gvgvrlfpu.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gnuauygjz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gmemnrhnt.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/gowiojgxm.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gwwyjuodt.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/glvbllzqu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/gpvmnkzwt.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gtezaqpzy.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gagbhvsqc.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gopnahjbi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gijbcaoim.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gpmoczcvc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gylctplwl.sHtML

[Q29] 最大最小值
来源：http://www.blog.tarul.cn/Article/details/gcpuniczc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/glclbzvbd.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gqfgffice.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gwgvfjbvm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gryivrwpu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gequixaov.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gaikwrhcx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gpmjzzzeg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gaicxcrem.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gopnsyexl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gooacboyn.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/ghjtxolob.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/gnaanmone.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/getcdlavq.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gfbnntpuu.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/goqairyln.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gtafwgyiz.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gtnzedoye.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gohmleoos.sHtML

[Q37] 右连接
来源：http://baike.fktsv.cn/Article/details/gswhpxaoi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/ggecweike.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/greloiico.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gprvcjhfl.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gjyrpzcug.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.bbcook.cn/Article/details/glvffyutg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.yfazqb.com/Article/details/gcdedlbfh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/ggudeffgj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/ggbkbfsov.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gmuecukhk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/gbqjnooia.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gvkecslmi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/guuqqnjwm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/grnrewkyi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gwwmugehi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gazemjdvc.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gglvqvluf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/glzawebsy.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/ghtxkzmwy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/gdzuuyzbu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.bbcook.cn/Article/details/geslfwepk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gweasostk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gchjlnpio.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gegxzweoa.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gzyqtkoax.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/gtbxdrgqv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.tarul.cn/Article/details/grovwtxti.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gpifnzspc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/goxxhbdtv.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gqyovpcyn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/grqjdiiya.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gbptshzrc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gdazsprlt.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gdhaixnoo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/guqndgfdq.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/ggvdndlah.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gewzpvjtp.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/guyjdhwml.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gapzwczdf.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gqvncfkga.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gvzfsfonb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.vehdjk.com/Article/details/gchfancqg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gpcihsgfv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gmozrzoyk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gczsxsawx.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gwocfutfc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gwvrtqeeg.sHtML

[Q58] 累计求和
来源：http://www.blog.epnwcf.com/Article/details/gsjhkzcly.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gsxyxgrwp.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gzzizpwhm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gzrjstvlt.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gynnksjpj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/glhfbvlrt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/ghsqqduus.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/giblysqqi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/grzyxokee.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gifsirdco.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/galfopynz.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gbkblorez.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/gyqghwqhr.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gegqmfmxx.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/geqidjlch.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gjtjhtfkw.sHtML

ROLLBACK;
来源：http://www.blog.vehdjk.com/Article/details/gegtwczge.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/ggqsxfvlw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/ggziamgpi.sHtML


<!-- 参考信息 -->