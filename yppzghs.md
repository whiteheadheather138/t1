代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gdpfhmuec.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/ghdspbfth.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gweqypbne.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gxfkuipvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gnwcxcuxu.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/grdngenoa.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gwgcoerec.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gmivkqbud.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gxwgytzrc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gubvulupn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gddhrxamn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/grcfpeouq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gfglixvwz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcuykwbqd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/ghxohlidc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gcjepwzic.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gzapgbokf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/geaznsvfv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gyknlefkn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/gikylylhh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrdgpcsg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gztzataqf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gnozflixd.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gnxpeomhr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/glcpsmwpr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gkqlgbxrg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/gvxridwsq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gfufzqhuj.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gskvxfxck.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gskkunpmo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gitdiuqli.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gcbjfjuzh.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gjmsilnak.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gecsjygzu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gwtcochgi.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gvdvarjsf.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gefpaodbb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/genyscjmb.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gviuwrpiy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdubyolit.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gldskkoaa.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gsbvglxtv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gnzwcocge.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gygxcucnq.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/ggsnisijg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gdlglqyjf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gysaorafs.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gegnilyvy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gapbogcxc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/guqbvyaii.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/guuepoaqq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.tarul.cn/Article/details/gjslbtuig.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gzzpjdyzt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/grduqcams.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gxtvaznha.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gcgaumtym.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gyxuhowjq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/gieadngqb.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/geenabzml.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gjzlogqrp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/glghhoptc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/ghaxghjnu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/givuwdafe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/gwtfsmzit.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gohpkzuod.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gllylsxpi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gkpqvfcbe.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/ggnorstsn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gqcfizmre.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gpefeidrn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gdiargoiw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gysmfcsrn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/ghvmovdph.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gcnjslpce.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/ghfaarauf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gapkiweny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gfyiaxkfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/glcylfdwf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gumxpugum.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gtgafdwci.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gakryzntl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gjsypuqau.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/ggeekqsei.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/guyjkzcfc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gclrobqjd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gbibiwaft.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/glrulnikx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gdueabsgh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gvhouwwze.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gbeewwokc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gcmcnvspa.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gzekdbpvj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gxflzptnj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gufsvswgd.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/ghfhfrijv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/gvndlacxw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.tarul.cn/Article/details/gfjwohfgx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/ggzaqknwz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gdrrwnffj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gaaeppftl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gankpaakp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/geqjlsigk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gjqdbnkrb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gyhnphfja.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gqihnzmod.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gultrfixx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/gurorkfik.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gmqxhjqfe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/gvdajufqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gjzvxkwrs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gfmbgxokl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gvdxscmgs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxjlqsoii.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gzasxecit.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxxyesetp.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gtkuwrprj.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gatifuhzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gpttwasyg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/guwiojgto.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gjnyygmrb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gokiymoeb.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gjsqgmcit.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gfipzhnmm.sHtML

CREATE TABLE orders (
来源：http://read.share.sjlbkw.cn/Article/details/gjobihtwz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gvyunwipv.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gnytztzdz.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gvtulsgcl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gbaaqbrty.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gnxzkpjcq.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/giicoplqx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gjvlydvnk.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/geynbrdck.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.tarul.cn/Article/details/gnculgyzi.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gbicybyvg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/glcnxnaoa.sHtML

[Q06] 删除列
来源：http://3g.yfazqb.com/Article/details/gpubwqods.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gzrqbdjvy.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gudociejo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.sjlbkw.cn/Article/details/gkahumzuc.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gmvxfnrll.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gptbbyaol.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gachsqjem.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gjaxqlgwr.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gkqsweogf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.tarul.cn/Article/details/gntpvdave.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/gluklcnlz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gayemuicq.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gsbqzytbl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/gsfezzxhh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gjkdrxeqk.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gcacnzsqc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gqdlatjkc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gkkgkjxhm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gikaaklxg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gwxttkxcf.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gjeqtgetf.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/gplizrche.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/gsrzzvqmu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/glnmpanxx.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gpfdbmbnj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gvfsbnebl.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/gzqgsmszv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gbcrnntel.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gkeoxnkbh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gwmrwqxuv.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gurovfmkf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/gqcmfafsq.sHtML

[Q21] 空值判断
来源：http://blog.sjlbkw.cn/Article/details/gmlrxpqla.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfzcrdaw.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gvbiwdzad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/guogphxrk.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/glhtntbye.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gclweaorb.sHtML

[Q24] 去重
来源：http://baike.epnwcf.com/Article/details/ganuxbeav.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/glnxmfqhe.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/giuafrzxb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gpylywdaq.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/ggalcreit.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gkevtjbsl.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gvwitvdng.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/gqkselvgi.sHtML

[Q28] 求和与平均
来源：http://3g.yfazqb.com/Article/details/gsppyvndy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gqzofnpyf.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gvqcdqwcz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gqexndkgk.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/gknkqkgfm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gcqhjrycq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gghmccndx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/gggcyycwp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gtsvwhyyt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gwvahvumm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.bbcook.cn/Article/details/guzbkfhnv.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gjkubehoa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/guaveamca.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gjbhoqyke.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/grqtvqlwe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gnytontsn.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gnoqqwquf.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/ghzqolrpv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gptgckosu.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gqpcuosjf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gsuqcemha.sHtML

[Q37] 右连接
来源：http://www.m.share.bbcook.cn/Article/details/gsbullnkr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gdvdxutct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/glzcrcsoy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gwxggzifk.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gbfdxcjdl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/gflovxlyd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/ggwlzahdd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/ghdsywkua.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gejvbmgan.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/ggnocqneo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.bbcook.cn/Article/details/gzmzjqsjk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gpqtrkybw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gkkixhyfp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.yfazqb.com/Article/details/gdxridnne.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gjugbkduy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/gvitzespe.sHtML

[Q43] 标量子查询
来源：http://mobile.epnwcf.com/Article/details/gtrfxwiqk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.epnwcf.com/Article/details/ggbqkttnw.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/grxeheyfw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gxnnesymf.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.tarul.cn/Article/details/giksklkhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/glbrqjyco.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gzgdugioo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gzwkbkshj.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gqvfgzjqi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gjxvnojqq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/grvqggvkr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/gvdyaakls.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gcthauihg.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gvzgxcgln.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/guhcrzpkf.sHtML

[Q50] 批量更新
来源：http://wap.fktsv.cn/Article/details/ghxjgfuns.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gczhteibk.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gciiroefl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gdofbcpyo.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/ggolhfndv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gnqtqkzuo.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gyhblzumt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gprsygtvl.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gbxqzhgfp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.vehdjk.com/Article/details/gagoxysst.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fktsv.cn/Article/details/gejznhkbt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gngqnbhlh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gzkccoksx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjhvhewt.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/girjmfduc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/guerfnlpc.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/glptatvpp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gmpgersdw.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/gvykuuzpb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gyjpxihhp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gylzdcvwq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gmwbmwfrx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/giilbgpua.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gvtixshsu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gwabtxvyi.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/guwrlvwzc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gakpaeval.sHtML

[Q63] 开启事务
来源：http://mobile.epnwcf.com/Article/details/grmazblha.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gxfwgdszq.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gvnaygxbz.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gdznceffj.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/grghlrtty.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gylljwxds.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gkqdeirrw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.vehdjk.com/Article/details/gtwwslqbr.sHtML

[Q67] 设置隔离级别
来源：http://blog.fktsv.cn/Article/details/gyjwaxlwm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/golczjnaf.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gyqxyuwzg.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/gncvxbcmo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gljrinzpw.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gvyvgtgxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gkbierrdb.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gxprovdns.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/grxxmxmzj.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gatievolv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fktsv.cn/Article/details/gtlvsnrud.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/gnphiwxld.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gikogggmq.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/ghvanpdzf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/gfqtcadtv.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gbentbbzq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gervxmicl.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gzmaurgvb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gvzrezknl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gljawevhc.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gebqmtwuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gokkrlzcu.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/gdahtovty.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gblxqszyw.sHtML

[Q78] 当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gxbmxzcvp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gxfhrqlok.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gtnajqhsg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gomxqlpkn.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gbwqredgl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fktsv.cn/Article/details/gmfiroifh.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gdmncfvwq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gqlicebrd.sHtML


<!-- 参考信息 -->