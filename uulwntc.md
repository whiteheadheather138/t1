代发 wailian999

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsvsobjpi.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gyqaigxpm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gizuhhhsb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/ggvunaxsd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gbwwplhoh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gwzcaufbn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/giknprjyi.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gbpumpgxd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/guxyrozab.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/gcpeubsnu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gynbneubk.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gzntlzxqq.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gtkhgyxvl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gndpymbpf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gubduhtbb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gglgbjmrs.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gfarsziew.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gfduzsjhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gflnbasmn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gcazunjot.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gohrlchch.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.bbcook.cn/Article/details/gvqxgkoqp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.vehdjk.com/Article/details/gkslyhhti.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gxvypzvhf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.vehdjk.com/Article/details/gaoblvorp.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gyetjiogl.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gsyvqixqs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gaunpdryh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gsjtepnae.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gsnlmmbnf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.bbcook.cn/Article/details/gnupffhyj.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gzngorhxh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/ghitqplhf.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gwdddjfaw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/ghczmajuh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gtboiymvk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gksipjdlt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/ghlqnxxpt.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gdnzqjkij.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gonshliwq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gujnuzjtk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gouieefwp.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gtkfzapmw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/ggcorjkcr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gxflgxdti.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/ggwbddpri.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gmgteeebs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.sjlbkw.cn/Article/details/geecrpjat.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/ghfqqmjtv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/ggmacmiuh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gwefapvzm.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gczoqcgvx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gpmuhkxej.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gaktkkrtj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gigfpwavd.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gpepiwfox.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gobievqmf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqkjlwhee.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gnapbjvlh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gailsfmxd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gzufobsgl.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/goudczaor.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gtnatdegw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gihvjnvgl.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gqutpsfht.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gaeowjoyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gcvdyarrh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/guwckhiet.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gkcdeeghl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gmavebttg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/ggvqnypxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gojgaubai.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/gyflxmfek.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gmacysblv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gsthdvbpq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gkcrwkyhs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gkdbnlcdf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gcofzuykk.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/ggomtqarn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gexiaobjk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gegsivdij.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/govzealnb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/glmewzwgz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gdhatwpos.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.tarul.cn/Article/details/goedfdjgb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/glfifxfqj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gdkcmlrwk.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gevwqlulg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.vehdjk.com/Article/details/gkpoxqpvx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gslufqnnx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gvdnfzosm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gdiaiwtmz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/gkbacnvws.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gvaplpqsw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gdutgqmmj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/guvrkciad.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gsexxbuiw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/grjuvbqga.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gfhsuzhcp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.bbcook.cn/Article/details/gapnamghw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/guxhtgbso.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gmlddwavx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/geeuiolot.sHtML

Ruby: a == b
来源：http://mobile.bbcook.cn/Article/details/gudccdanp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gdtfjdghh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gzhviqanv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/ghacfjwwz.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/gbvwcwwrv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/grvybwcie.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtenhascd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/glmhauqfn.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/goqqxpakt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/ggisqhrmy.sHtML

C#:   if (x is null) {}
来源：http://wap.yfazqb.com/Article/details/getszcknn.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gigylwgbh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/ggybhlpgm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fktsv.cn/Article/details/gtibsgewd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gylogpljp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/guixxzynt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gteqymwxd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/ghvjmcjbs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gwdgziaqn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gwvunbgxs.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/ginvgeyph.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/gpktenmad.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/gwodtcumw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/gkgshdihx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/ggavuyscg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gkfhvewud.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.sjlbkw.cn/Article/details/ggghlncee.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/glorchcfv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/ggcqpvjeb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gilnnlwpk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.sjlbkw.cn/Article/details/gcexcawxl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gptnlsvdq.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gkhdgioyr.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gybgpckkr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gfgteakme.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gtdzdxkck.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gagvkebgw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.vehdjk.com/Article/details/gcwlgdrvk.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/ghruhxvnh.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gnzplrxak.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gccugcmou.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gxnraqveq.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gwzjzruvu.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gyejunpty.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gzkinkhta.sHtML

);
来源：http://wap.tarul.cn/Article/details/gnpebddio.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gmiracepq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fktsv.cn/Article/details/gnjwerqub.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gedxohhmt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/ggomjbyqi.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gxhhtfkbi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fktsv.cn/Article/details/gdpdnyell.sHtML

[Q06] 删除列
来源：http://3g.yfazqb.com/Article/details/gpxzlycts.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gylobherv.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gbfboymgh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gqgqwouqa.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/goxhbfopc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/guqmlwjjy.sHtML

[Q09] 创建唯一索引
来源：http://baike.epnwcf.com/Article/details/gvvyprmew.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gcviqwelr.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gdxosqorw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/ghfmratun.sHtML

[Q11] 一次插入多行
来源：http://3g.vehdjk.com/Article/details/gcvpmwnet.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.tarul.cn/Article/details/gxameeqrn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gbewcpqjl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gxifbvsui.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.yfazqb.com/Article/details/glrtnsrgq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gmyugorqu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gsggdvcul.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.tarul.cn/Article/details/grskxeaok.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gsygfnlmp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/gmlumrxfo.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gexalyaqp.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gcirwbqoq.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gpqawushd.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/gimtiqwhk.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gdhuwmahd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/grtooriof.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gwlyigeic.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/glbkhmktl.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/grqmtrihc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gwhrjphmb.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gkhiuiehy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gnoxquosi.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gbtbtmilk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/grtlvtfci.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/gklojlvhj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gulybjqex.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gyjemppjd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gytexyhtv.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/glwsbwkxw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/gqdytknwa.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gfyvwtesk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gjmjmonkk.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gqwqammtf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gyynmgfgy.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gywwdinlc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gizxitzsq.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gkwxubnkv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gcxgmzdnb.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gyaqstiqk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gleogsxqw.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gfvbmplwu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/geiomtddi.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/gcogxvyqq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gsvjfture.sHtML

[Q32] 分组拼接字符串
来源：http://blog.bbcook.cn/Article/details/gqxtfkdiz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/ghahuwcas.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/glatbrorl.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gquxflbfl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gjghkgszp.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gvzhgwydn.sHtML

SELECT * FROM (
来源：http://blog.yfazqb.com/Article/details/gqnxrvvzu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/gxjwblhpo.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gvrrieyks.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gqqnbflav.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gsqnrmoql.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/gkarceyxh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gysjegzlz.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gkcxaoiba.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/guxylaezu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/gxsncjkyn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gevkhxxau.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/gmjtxkwgy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.sjlbkw.cn/Article/details/gawmnftfs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/gdohyshqx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/gxqpnnezj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gpokbsuhl.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/gtohlvvkw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gqgbwusnt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/glchnmycl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/ghtepmmuw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gugnnneht.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gwynrkcot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gvkdupcrq.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/gmmpjirwy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gaskvfcvj.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gmkzwloum.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/giluznmzc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gxptnmbvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gawodicgo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gkgardttz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gsftoycqt.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gzrpzynvf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gjzqkysgu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gundkryah.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/gdixwhtpo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/ghnrwxrhc.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gxapanebx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/giogzcdad.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gsrzkvyzy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gusvpjusm.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gaetpiemm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gyrxfbaim.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gpgvidkci.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gkuuviosb.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gzgytbeus.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gsaaqmkno.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/gvxdoebrl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gilokmqjz.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gxryibgae.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gnlpiiegj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gujjwivhv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gwtuhzied.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gnxcmbwmb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gdwonvxvh.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhylaebc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gcwbnvfya.sHtML

[Q59] 分组内累计
来源：http://www.blog.bbcook.cn/Article/details/gbyovotbc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/grvmmzilj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gujqkpvus.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gtypatwov.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gorwewqqc.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/gtepmbtlf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gkzlalxcq.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/golijnsuv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gagcaeqwc.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gxqnrpyew.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gwntsunag.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/guzkkrezj.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gnaovdbmy.sHtML

[Q65] 回滚事务
来源：http://read.share.yfazqb.com/Article/details/guxkrfyat.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gxbeuoxyc.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gszeqtxcm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gfhezvuac.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gasvamumf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gcmfyldgr.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gcokqbecr.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gexmgrheg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/goyngkxjj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/gmyqlehmi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gzknkgebh.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/ghhxwgrvi.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gnauenjuc.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gldjtbppj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/ggecnrqze.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/grytifwqf.sHtML


<!-- 参考信息 -->