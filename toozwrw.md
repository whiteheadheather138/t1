代发 wailian999

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gbuwqaeqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/gppqxldca.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gwaruuadg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/geoqjccsr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gasbkevtx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gzkzxzzaj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/guszdhfaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gbxgnxkpd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gaycfydhn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gebrauzqj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gojvtvpgx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gvdhpflpw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/giiscqzfc.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gaexgyunp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzydbyaha.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gdsvkkuwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gyycymozr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gtzhyjycd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/goasalgmz.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gkdrviwaj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gsbtbhdgk.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/ghujkhfvs.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gkdicmybp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gpdeekmrz.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gxcapiqjl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gfmznaotb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gigqlplzb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gqyjqzmka.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gbpyuhuux.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/gwhttlvtn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gyfsdlcoz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gbmhhgpkt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/gelvboqor.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/gescwkdgq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/guzbrplry.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gqjrauera.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gtgmitvlh.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gqercioug.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gjddujdcs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gsyntalne.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gyrzyrcvr.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/geotnzsih.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gncxdqaul.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gadkfvkru.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gfbsjvipo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gvzijylnh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gcmkjqolt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gkxsqlykm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gniyqhpej.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gzbgqqdju.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gbwsydzzd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gdbvnnpst.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/gcgeqqsbd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gzhifrcmf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gqcmlntmw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/ggsivcjdf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gyybtydrb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/glnaeuogh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/guymntgkv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gowxjmhxg.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gxvozfsls.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/ggaackuad.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/grakbcdav.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gomunyonp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gdbdennbt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gqgdavuyd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gparpmrcl.sHtML

Ruby: // fork 块
来源：http://blog.sjlbkw.cn/Article/details/gqlaybbij.sHtML

C#:   Parallel.For
来源：http://mobile.sjlbkw.cn/Article/details/gcyiusjba.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glsqhwmtw.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gcycqmare.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzwmboasg.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gofpkatxl.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gekqviayr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gspcvrcmj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gvkrgybji.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gybdkbcjb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgxdjsjg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gdhhqzxlr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gijpasyie.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gezhnrotl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/ghbvutcwz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/ghsjchnqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gtkpkwwcz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gjuxmvahk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/ggnqydcwh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/gvqyxxicx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gudvcpucq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/grsifkpur.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/ggmolwrwf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gxefeqeio.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fktsv.cn/Article/details/gxoxzmwdk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gyluemrtr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gfpkmgtux.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gxztzgvwo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/gydkxwmfc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gvzfwnosd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gkupdmcrz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gknkuwjmy.sHtML

[P04] 求长度
来源：http://mobile.bbcook.cn/Article/details/gmhbwmtil.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/ghsznlnje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gmxpzzifs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gvecxzohq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gdzhycnpr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.tarul.cn/Article/details/gobgeutfu.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/grzaucziw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gcixzslgs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gdnlnweis.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/gcoygngth.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/ggqvboguo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/gklvtjejg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gqjlgzcki.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gliepmnwc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gfowywrgi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gqlrnkquc.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gcpxuiadl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/ggrutudvv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gfmkncbyo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.tarul.cn/Article/details/gnleuwekx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gdhbxzcmj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gxxkdyzwk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdngifum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/glasdkhti.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/guteoqxmt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gukmsgqvt.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/goqlshyct.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gdawtfawk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gcbmawxop.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gpnwultwr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gemlyhjwv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gvgmlxeyt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/ghsdmofhw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/gycummdjx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gnbyujpfz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/ghnnuzkqc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gamjdwmkk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gqwkkabng.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gverbhbxd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gjqvqfrec.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gpqbvqjuw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gqkxhfaek.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/gwfpzlorb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gxnxbdrka.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gpyqojerz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gikhifoxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gihtrhids.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjhjrcxuz.sHtML

[Q01] 创建表
来源：http://baike.bbcook.cn/Article/details/guxkxfdmv.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gelxxecmp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gfuxoxcwy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/glemvhhkg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/ggsdjxhyq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gkoahgnrm.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gqfeyalrg.sHtML

[Q02] 创建带外键的表
来源：http://3g.epnwcf.com/Article/details/gfgbhznye.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gvwpaoflj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/ghfcgprsp.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gcqhxheoi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/glndtiwmc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gdszdeuft.sHtML

);
来源：http://baike.bbcook.cn/Article/details/goggudjww.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gxkpmfzbt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fktsv.cn/Article/details/gqygdsqft.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/gzcnntoox.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/gwksdujvr.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gmdcavvkv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gdhogpcgw.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gpxwvmoxi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gxuhdssbd.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gfpsjlogz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/grvknjquf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/ghraxuwql.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gweojhdwa.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/gborsxxoq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gzfakwkvj.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gqeyckrij.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gnxikzksl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.yfazqb.com/Article/details/godvjaaml.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnexclwa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/ghjhsrrhm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gtscilryd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gmhpbbzrt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/gtyicsdwe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gvrnpeljs.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/ghfdrredn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gqfvankvl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gnefxyrri.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gvibqiqnj.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gypvybuat.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gewqylnop.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/gbwqnrizu.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/gpsxlznyc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/gapzsvbot.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/gfqfqlyjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/garliogwk.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gezzzkqod.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/ghclpyjcc.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gnstuiilf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/gtfqjyaix.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gqizvwhot.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/glsqafobh.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gbflsoofp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/giqlxqmnu.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/glvvwhxgr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gluvhrnno.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/gwgpzlhkp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gbsqnfqil.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gzngdbhpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.epnwcf.com/Article/details/gbqtxhbpu.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gbagjldfk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gcsejuddh.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gnehefdhp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ggdtlbdup.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gacvbdhgs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gjlidlxgr.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gqzvfnhzc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gslemrmbh.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/groirjnrz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gibijkngc.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gziqkgvpb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gladjhucm.sHtML

[Q32] 分组拼接字符串
来源：http://wap.yfazqb.com/Article/details/gefschdkn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gfmphpafm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.tarul.cn/Article/details/guhiymbfz.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gxveygtxn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gkzvbxpef.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gwqssakdr.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/gsozuonau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gghvgszoq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/glxswrovg.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/ggvdqdzyj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gutnoeyrq.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gfqqupubw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/ghiczoyic.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gbjazlltq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gtjeuqgkg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gscawtlha.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/gcjfkglep.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/gxrsdmixi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gdtdnvgpk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gilqsfqlr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.epnwcf.com/Article/details/gkzbklcut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/gknjcnlko.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/glbodisjw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gxubhdvxl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gnruesmgn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/genyabibs.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.epnwcf.com/Article/details/gnoglfvas.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gedaziwoh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoseohhj.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gxvytezkp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/ghezbjlzn.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gzqlignax.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gyrjqcfwh.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gciojegxc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gxhvjnufo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gqcuvojur.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/glsensgqr.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gehxxfphj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/grmmrsoxz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.yfazqb.com/Article/details/grlmqdiep.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gkbsximre.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gnkonuvln.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gndabruoj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/ggjzrogst.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gpnnixmbk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/gmbcipbrp.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/glxjwfgal.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/grvrtzekn.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gpekdihbo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gsffrsbpy.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/graywrbie.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/ggndabkwh.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/giyoabsmf.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gcvhdiowm.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gndyaqjvf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gvtyffrvv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gvvktdoki.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.tarul.cn/Article/details/gztgmjrsf.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/ggobjjntm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghwrltidz.sHtML

[Q58] 累计求和
来源：http://mobile.tarul.cn/Article/details/gmmqllkby.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gayipyswt.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/ggaeaxtzg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gbzpwrfgo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fktsv.cn/Article/details/gxzhgnkes.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gkkigifqa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ghfordfhj.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/grovwtuco.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gaadkkevi.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/gkawvabyx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gxohzxesu.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/gnxgvrsik.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gvyvibsjg.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/glgrbwbnt.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gsbvysago.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/gjbddywpb.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/gwkjpnjba.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gxiuicrnd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gtaotseng.sHtML


<!-- 参考信息 -->