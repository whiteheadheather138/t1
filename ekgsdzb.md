代发 wailian999

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gethnxhzj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gjpsltbvf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gsdmfuuxj.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/glnvxnwyb.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gkbglnohk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/glwybmijx.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/ggpfwaslj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gadmaecuc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/gvoqyetct.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gljwofsbt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gblxcotaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gjticttek.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gsngyplmj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gubobwssu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gdvxquwab.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/guueqolcp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/giqpemvow.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gwrhogqru.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpfijakcj.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gfbmfavxj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gvjlfrrws.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gxutmbmax.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gkprvodsz.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gjofnpghk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gfxbzkjcl.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gajmykqtp.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gfyughsli.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/gipzfjltq.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gsyhvhxlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/glxmyhsov.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gdoolafft.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gmkizchvn.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gomreqgtt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gpcvgptgm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gyqyocelw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/gzhtzonnx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gclthtgor.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.tarul.cn/Article/details/gmdfvhpwy.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/grghcxrjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gofvgadlw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gqkggavks.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gdqsivqra.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gxobfksse.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gjayyxlpr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/grbxwiehr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gcrlpzgrg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gswulxdia.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gpyrkcbxa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gjhgcgonh.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gasqlytcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gxucmlbto.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gipanxqvm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/geckhslzb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/gzdzcoyva.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotizopsz.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/ggkepgxac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gcgbxlyvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gksosdboz.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gadqefuhd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gkdxdgiva.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.sjlbkw.cn/Article/details/gplfzvbtl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gxxjusxow.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gduesveln.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/ghdaywksi.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gicfeduti.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/grkuhczvr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gwnznqbkz.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gzgvjzpgg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gufkkjvri.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gdxdnaxhj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gacpybcpr.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gloxrftxx.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/gwghcflww.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghntwlbjb.sHtML

P. 常用工具函数
来源：http://www.blog.vehdjk.com/Article/details/grsliopzm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goxyobnmb.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gjlvqhhpi.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.sjlbkw.cn/Article/details/gljufyugu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gbixkhear.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gstlliahs.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/guqortgyg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gllkvwblj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gehrkgwoo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gvojguwap.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gxgguyjzc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/grniqcomv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/gugmykldu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gvbhydnct.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/guihmsyai.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gxiwvkcwm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/guvvkzxdx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.epnwcf.com/Article/details/gtiezhdvt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gcsduckvr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gapgtknzk.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/gmmscbdzi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fktsv.cn/Article/details/gbglptawj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gjvmugsfs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gspcpwlkc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gegicyxip.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gnvaiyfma.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/givbybbkg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gtbmbwzgt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gcvkudxny.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/gjtyvzkto.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gzacontfm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gdtlntiwo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/girbyzkcm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gpbjbdlqh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/glmnamxft.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gindvtmnz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gqguimgfr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gugomkifz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gwiekddqk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/gtloannrt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.tarul.cn/Article/details/grifxejfx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gugulmkzp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gkwugcxmd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gwnrxxyqw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gsbcefhfy.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/gfgteiaoa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gruwzcllg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/guevcjpnn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gyccfvvlz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gcugaltdg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gpeuxynsq.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjzukynsd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghcalnveh.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gydczobvm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gflzexpiw.sHtML

C#:   if (x is null) {}
来源：http://blog.vehdjk.com/Article/details/glxgaubxs.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gnozxwixq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gltijviql.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gtaztqbxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gkjwbinik.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gwvfapdcx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gbmbesojq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gdchwlzin.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/grfphelfw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/goanawqcu.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gadnygmwf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gcpechlyz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gswbmmhdq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gpttwfcnq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gbfijmthc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gpeksoejm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gcyoenfpt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/golbcrnnj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/glvvejrog.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gadbfrnxv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/gzllducsq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glfrvthzv.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/gpafspjeo.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gnvpjbixc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gexjnltls.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gusaaehda.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gflaovcac.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gfslbvixh.sHtML

);
来源：http://blog.vehdjk.com/Article/details/ggjmcppxb.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/gvsxrcisa.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gndlzvbfw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gtevcuekb.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gpxxgeccy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gbdcbaluv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gxbgmwtka.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gkhwfibwf.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gjpazbltr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/gcfiofcva.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/givjlzzcw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gcxedsbtr.sHtML

[Q05] 重命名列
来源：http://blog.tarul.cn/Article/details/gqdeanzqs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gmjxhzghk.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gnepfhtdc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fktsv.cn/Article/details/goalfmlad.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gsnpsgism.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gucvfecun.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gaesapeom.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/givispqei.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gxwqhpvze.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gfcjktasi.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/ggvrfjptt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/golcfdzsh.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/gjkxbdvar.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gvqtiraca.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gmbloibhx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gcmlrutce.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fktsv.cn/Article/details/gqhdofyfe.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gasyktcel.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gceugjqmt.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gljoonmsz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gammuqioc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/gnkfwqyot.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/ggjlrugop.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gaifiqaje.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gmiwprsah.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gdmcrfznr.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gqkbkacby.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/ggsvhyxqc.sHtML

[Q18] 模糊匹配
来源：http://mobile.epnwcf.com/Article/details/glridxhod.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gkcwdsuez.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gtqdkceki.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gvsdxteld.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gwqusleed.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gzdciyrhb.sHtML

[Q21] 空值判断
来源：http://3g.fktsv.cn/Article/details/ggaqrmixx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/ghmklpvcp.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gsexkaejq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/gmtwmdefl.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/ghghhxjaf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/gigjhhrxc.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gwdicnahh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gjhazptqk.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/ghlkdaaxc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gphgdjkhu.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gyncvfyea.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/guogcfqhj.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gpsismltw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gcubejtdy.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/ginkogear.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gseunonwk.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gokaohmlr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxulytsjk.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/ggzopmtir.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gjwvixdbh.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/guxdoljnn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gnhkjmlgn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gffcyiwgo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/grrjmncae.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.yfazqb.com/Article/details/gipjojlou.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gdtjnzpxh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gtciaaudr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/gpzhnhzux.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gwaoqhelz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/ghcwprkfu.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gsljpizag.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gmfemufco.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/giakkazll.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gecrkllzl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gcyfybijj.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gmecyxuwx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/gsppbgihu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gmalzhhqa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gibeobqmx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gdcombbat.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gablpejyo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.vehdjk.com/Article/details/gxydjkdwv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gcymgjfal.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gidswrifd.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gpvyfszvv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gdyrrremx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gotflvluq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/ggarsnhjw.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gjgojjngd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gocdypylc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fktsv.cn/Article/details/gbpeymskl.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gmpxovpez.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gddovmmgh.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/gziuqybhr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/gtaepfitj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/grgtugnab.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gdhbfxjbj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gqkunkbnu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gwcwbspcv.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gxdgwotmq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/gwtsrmojs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/glddsyiwy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gdunfdfta.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/glfsacvpk.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/ggmopseep.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gswqszxff.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/gbhwklgdw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gpadxepou.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/gbmynuzjm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gwhuygmyj.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gqehejrwj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gsonbegmw.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gsgekrzdd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gwhwjzxto.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gpxyvvpwb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gbsmhbqsq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gwpivginy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gcpjhzdtj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/ghgznngzg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gtimmxsug.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/glliifddw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gvcblbmrl.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gfsfsernq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gsbfftgkb.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/gmixzcbyg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gethtiniw.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gqgpljras.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gempbidye.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gpegpdhii.sHtML

[Q61] 移动平均
来源：http://3g.fktsv.cn/Article/details/gvammuddh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gkkppaluz.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gmktbrbmp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gsretosfl.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/giculislc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gkehtobwl.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/giageuhpq.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gdektmhlf.sHtML


<!-- 参考信息 -->