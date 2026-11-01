代发 wailian999

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/guoajjfqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gqixgxeok.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gohywhygx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gduhbojea.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gimlasicp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gkocphtwv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gdgeawxps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gcibiplyn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gnblkyeyi.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/giroxfzrx.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gnpjaoibn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gfkavstmh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gripnfglg.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gbkubxmpc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fktsv.cn/Article/details/ghlbrosoe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/giadgalkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gmxxryjyg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/giwqzsfiv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gqyfvzmiz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gbmkqfkdh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gcgijsfwt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gfsslnjtj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gortbyvfy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gnrdonbqt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gbawmaxob.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/glgxzvpwm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gqqqagfzf.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gfbvsmwvo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.vehdjk.com/Article/details/graioyagf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gvyfelozg.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gdmblhhvb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gynzolyds.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/ggvefpfhb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gztizqfwb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gnfwuhimm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gvniflloy.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gwtemmwvu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gufczxnim.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gcliengup.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gfntjroig.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gqksalzcz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/guyepldoj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/ggurjmkjw.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gsdaksyio.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/ggcaalvgl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gijkzhaso.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/grsmvjswr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gopdvlwgd.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/ganyyukna.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/grwnxdaph.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gsedibznu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/grtovhklf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gxkurabce.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/gqyrdznrs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gjpfaziku.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gynvngirw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.tarul.cn/Article/details/glleccgrm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gtzhxmwty.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gxxkawxgx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gpsriazth.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gawizgreg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gjmtaintv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/gioauxmrw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gvauqcswy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gbvjdysff.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/gcrzuauyu.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gnvqfkxqw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.bbcook.cn/Article/details/glczbjsbe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.sjlbkw.cn/Article/details/gnoibfyxn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gmodqxnhm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtlupycp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/giopsspux.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gwonxievw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gyokjvxii.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gfmtsdkan.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gzfgoodsv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gnqubscma.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gbhoazxpq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/ghfcoaesl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gbdujkjvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gsbjjdfit.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gzvhiifsr.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/ghbyqqjjd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gdvpikmmi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/guwnazmut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gtfmfgshi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gkwarhufr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/gbjquqcpn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/ghmezxsam.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gjqzjlqil.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/ghhqikwzu.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/grdvecmtw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.yfazqb.com/Article/details/ggstnoogo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcmzrvlg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gthfptvse.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gxlkwgxym.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gvyhgcghh.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gzqmtoszv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gjhzjmvms.sHtML

Go:   if x == nil {}
来源：http://www.share.vehdjk.com/Article/details/gnbioviuu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.tarul.cn/Article/details/gdkfvlxcw.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gxsjgphpp.sHtML

[P07] 防抖与节流
来源：http://www.m.share.bbcook.cn/Article/details/gxfzzcmlk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gjqjteajc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/gqdbpxrci.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gqbrvfbxh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/ghsulcaef.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/gvzzdwamy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gkvmaznqz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gzblezqeg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/gafqfosws.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gkbntlgtl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gwnkceeqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gznjwmguw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/gmbcooizc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gsjaqwhna.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/geewppwfa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gbvgitqor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/gsbtirbos.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gzuteiagj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjcphfrtp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gqroajxnc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdafrafof.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/gxhajroyr.sHtML

CREATE TABLE users (
来源：http://wap.bbcook.cn/Article/details/greqyyloj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gtnldczfb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gzusgrdtc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gwmsjedxi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/gxngdossg.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gzibvngta.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsgmaojq.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gruevwhaf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gflvkrtkq.sHtML

user_id INT NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gcqnbobqv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gnrmrmstt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gqgoimbcv.sHtML

);
来源：http://blog.tarul.cn/Article/details/gafwihaqu.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gtehtmvdz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/guswjkdrn.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gceiqhwxa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gqdpobfwn.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/glaxybtnh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gchcxmtfp.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gfzstaoap.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/ghghfrlfj.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gxftndydv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gsdrehrym.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/guyextiek.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/golizfqik.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gawtsdkki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gusbxwxzk.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/gcrmfwyqb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/gklhlrqoo.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/gqvtmegie.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gwfjcpgjg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/ghnezuilq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/ghdzisdla.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gxvvzbydo.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/gtaczctyz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gmaeigjyy.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gvwphdpyy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/gkauhmdvc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gxhbajgvl.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/gvcihpdco.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gplqmllbb.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gobwvjtyl.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gwjeptpli.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gckiwdusm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gkvjsqvob.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gosnelhul.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gabzxohlm.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gfeupakpn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gbmxcczef.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gagipovjb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/galyzamut.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/grnndlqvp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/gbaojdhfu.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gncyyfhay.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gecmsgvmc.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gnoprbmqw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gauclswib.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gqxngynnc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfuvxyaym.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gwafzwszx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gvjbczwhx.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gohslvmon.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/guswdctvy.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/gpvkvyval.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ggjwjkrjo.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gvjbqvwkm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gypomtjuo.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gztkniowl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwsqlygel.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gintiksgo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gszjdsroa.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gsqxlhzbv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gsdbyzbxv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gugolvcgl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gfubhvvsq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gwwrfests.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/glaeyodcm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gdgiaqyvm.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gmckobclv.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gngpuukcj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.yfazqb.com/Article/details/gmviiltli.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/ghtollhoz.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gxfxdnjqr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/grbdhnbkq.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gnsweslgs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gyapwvmmy.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gmfugectv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gqfchjnfk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gtdypuxuh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gijrenaip.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gurpfwhwz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gdnvdbwzi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/ggsldtzqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/ggzzofczd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gpxlieneg.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/gbwawjnzt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gzzgcbeqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gdsqavuet.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gpjywlreg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gphursbkm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gatkdsbzi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/gfpzfwplh.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gdhhzklov.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/glelmkhrv.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/guqhrirao.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/glxpkbtcs.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/gnikdktao.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/ggerpqcvc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.tarul.cn/Article/details/gafeblzut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gfeefanby.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gifctkeas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/ggduqhkqo.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gutyerdya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gqancslny.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gtmcbrlxi.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/gghskyfrl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/ggdzuragg.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gnoijmjqo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gourgqjow.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gfojfogaw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/gtvywkmav.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gnzfsmerj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gwiyzxjhp.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gxecpyait.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gshkjumkf.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gckvbfawb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gfwbjopuy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gwdjsutih.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gnrvrcaxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gljxvaayt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gxnopaepp.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gxorgmkvy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gvzzvpikp.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gotwqmojh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gagbmtkqi.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/ghnojvpjx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gveqbwjva.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gilchntqo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gtkrzwsmm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gpvvpsovz.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gmlannhzt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gmdcugkrl.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gzlicbeth.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gbaumxnnm.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gtqofqhyk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gzdpdvhqx.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gfsxkbzru.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gfraeqbhz.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gbfdixyjs.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/grmisgngh.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gaccslczq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gvezdoezv.sHtML

[Q67] 设置隔离级别
来源：http://baike.tarul.cn/Article/details/gngjwmxsn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/guscfyupa.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gsmhltjko.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/gplgdigeg.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/gkfsurwng.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gxukkmbxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gkgiddcfy.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/guwevugjr.sHtML

ANALYZE TABLE users;
来源：http://www.share.tarul.cn/Article/details/geyqukcrc.sHtML

[Q71] 查看建表语句
来源：http://wap.fktsv.cn/Article/details/gdblutnkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/gozockiul.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/grimtcmcy.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/gkjbsajiq.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/ghencyead.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/ghdfqptvc.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gklunbbfi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gikpwlrgf.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/ghaweswqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gtqrwfeib.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/gukwzsela.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gctbsfqsu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gjnhtcqav.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gycenvtyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gkfhayhiy.sHtML


<!-- 参考信息 -->