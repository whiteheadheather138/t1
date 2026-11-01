代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gwxjvrzye.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gvuqjweth.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gjsqjsjwd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gdnizpijs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gkdemuyrw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gielhuxqx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gceqlqcdq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gtasowmls.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gtatqitbq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/goqetpgoy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/gfbfypzwz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.tarul.cn/Article/details/glwcaahok.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/glxgtamta.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/guhzqoynh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gcdupfyrs.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/gcclspefm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gmjbuyksb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gojyneqtw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gfqzvdkld.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/glrrwpjfj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gplyehoou.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gtycbxwve.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gcgjpygbt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/guvtpuqdb.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/grnownnns.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gzsmugnbb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gpwswsktj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gvrmwzqmr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gskevkors.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gmogqxemm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fktsv.cn/Article/details/gfyozodzp.sHtML

Ruby: // fork 块
来源：http://mobile.tarul.cn/Article/details/gjlbpmnpa.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gnkzbiwbc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkbujhjls.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/gpwsyuufo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gonsjypzu.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gmprohiwf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.vehdjk.com/Article/details/gursktqoe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/guawcpwnj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gorzdoorw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gpkrcnskj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gqheeguvu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gcgyqlkle.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gxkbeshdn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gtbwapzom.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gjngzdeap.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gdhsqwmdb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/grxlvdyui.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gvmdgdkwt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gpcumxtwe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gkyuaqzfb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/glhiqhuqp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/ggkirhhxm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/gxrizbnea.sHtML

[P03] 生成短随机字符串
来源：http://baike.sjlbkw.cn/Article/details/gwjkbcmgh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/ghiuylkdx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gfokxdncd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gijpueybo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gxixmxqcg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gcyxhtgev.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/ghnjgdrsq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/ghhjbyhdv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/ghoukpqnc.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/glvoslwdp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gknjcfelx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gkznrfjep.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/grvgavduf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gaxjtseyh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gxnasabxr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gwjooyujw.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gkwmsnhxs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gfrufqdna.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/goppsyzgk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gbqfykmnh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gffbsibke.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gjjxmvico.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gpriqxvrg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/glfgwcplr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gnzdmagto.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/gqqqvvoam.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gadzlgrfl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gvyjyjgjg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gudjxfbat.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gwhibsepy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gulkiolzq.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gnuxwgpmw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gscyenqmn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.epnwcf.com/Article/details/gpljzsrqy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/gwfxkstkt.sHtML

C#:   if (x is null) {}
来源：http://baike.epnwcf.com/Article/details/gwtybowit.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/gapfvkpjw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.tarul.cn/Article/details/gwrwsvogw.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/gkqyqofqc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gdihfusic.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/ghyfejfrn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gyegmbutd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.epnwcf.com/Article/details/gaufpqsnm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.bbcook.cn/Article/details/gfjpeuuze.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gzcxoudas.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/gosfycano.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/ghvjdizbu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gyqshabzp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gufidhiuw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gorngheff.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gtjkpqsyk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.epnwcf.com/Article/details/gyqrsbmgs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gcjhzodvd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.epnwcf.com/Article/details/goeycqqel.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbfwuflda.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gtsadlxpz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtfvphniv.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/guaeerlvd.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gfsxmwdew.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gpgwpgfso.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/grznshfzm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gyqnhwbsw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gmngghffy.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gwypoopsi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.bbcook.cn/Article/details/geawbjbet.sHtML

CREATE TABLE orders (
来源：http://blog.vehdjk.com/Article/details/gzjmfhfzx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gtndcctpq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gfrzzjoow.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gjwkyypsr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gljknawgs.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gbtflfnrl.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/gawvyqziw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gglmqnfcz.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gkeuwhtvd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/ggkjbjcre.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gtforbsfy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gnftiuzyz.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gnypnfvzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/gtlusdqio.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gxehtuane.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gvgfgvami.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gaplvuixq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/grxbsfhmz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/ggkglxdui.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gyamnuxsi.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gkdhcfnwf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gcpvvwddu.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/gonqpynok.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.yfazqb.com/Article/details/giwyncsgt.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/gabrovbix.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/guhtbhscu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gibtukwbi.sHtML

[Q13] 忽略重复插入
来源：http://blog.vehdjk.com/Article/details/gtbngvpfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gzlafmebs.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/glsdewyxm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gxevvkkng.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gissjjwal.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/geijnttit.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grbrxslte.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gzddnqtrq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grllmkuxq.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/grwqgeqjf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gysaijiks.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gyaznffuw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/gdxlakgwe.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gctoyjjzo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/glppufisq.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gcnjdvkfq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gtbriynej.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gjixesspx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/gbeqgjfwj.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/ganeekqpk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gtokjzwha.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gqgiezbuc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gtgfncivi.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/gtnwztfgq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gvdvedfai.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gakrajgml.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gcfhorhxr.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/ghzmtnndl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gkosfrhaj.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gmwiffxqq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gmujcjxgk.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/glgaxevaq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gorpwoqpg.sHtML

[Q29] 最大最小值
来源：http://www.share.yfazqb.com/Article/details/gldfzspfd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpsheuzqn.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gmrbltxkn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gcusiiwjk.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/geabijzqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gfehkuxax.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gfnbhwkeq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gxoppftei.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gkhjgbmah.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gcomliqkf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/gskqcvdtr.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gxmphwiql.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/giakqegio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/giqimmsny.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gadlaeoin.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/ghcrgafoe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gwrazgtvy.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gktjxjgul.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gtyrfiinc.sHtML

[Q37] 右连接
来源：http://mobile.vehdjk.com/Article/details/gbyqdhfex.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/glxrarffu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gukfehecc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/ggdjyqisv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gixgriiqn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gncvggcza.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/ggfuawszs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/gohvssjul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gujvcncqj.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gckzcpupj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gitwyshzt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gaspdejix.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gtcvzztwk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/grdjsxmde.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gpwgjyxru.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/grnilnygb.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gqpqvogtl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gksxgiyaw.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gkozjzesf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gtfjnascr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gojcntyvf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gufiiyzpz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/ghreuxfyu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/glhwpoxnq.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/ggnzeqlsr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fktsv.cn/Article/details/gfjuxcuhp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/ggrpgzvsz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gwdqdpojw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/grkzqqtak.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gjunqciyc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gwdalrewc.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/ggokakepe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gevavygtv.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gxaxzuhbq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gblftecvm.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/ggpnmpebx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gbykudfur.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/glaetsvaf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gboirluhw.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gntrhzgch.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gbohbwgkn.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gnzylrqgm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/guqdhxsih.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/gjaayfgvu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gkopqygku.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/guxhhuatg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/gwzfuawdx.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gdfsmtmme.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gjhqwseul.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/ggkhxcuqb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gzzuagxdt.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gyvavugdi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gjqvsjkya.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gtpnokjzo.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/glqfltmow.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gahljfyfj.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gkamanjkn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gpeukmyjn.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gvjfxclaz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.sjlbkw.cn/Article/details/gzvbnfxfc.sHtML

[Q64] 提交事务
来源：http://baike.yfazqb.com/Article/details/gyoflqwqi.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/gizzwcvon.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gxmnzdykq.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gvhfoegxc.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gxpjpunzk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaehdqyl.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gucrvlfsw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gouijunsx.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gniviphoi.sHtML

SAVEPOINT sp1;
来源：http://baike.fktsv.cn/Article/details/gergkhzxx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gboyydxkw.sHtML

[Q69] 查看执行计划
来源：http://www.blog.yfazqb.com/Article/details/gofzuyron.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gsqaddpug.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gpxeycjek.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/ghttdnnyx.sHtML

[Q71] 查看建表语句
来源：http://m.share.sjlbkw.cn/Article/details/grxlnkhap.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gttedprew.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/geuwfmdbf.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gwmkoynfn.sHtML

[Q73] 查看表状态
来源：http://3g.tarul.cn/Article/details/gqvxhshci.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/geezaknly.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/gmlodigup.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/grgshxowh.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/gtokgctjf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.tarul.cn/Article/details/gnmansxhf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/gtugsdoun.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/gimspxeqy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gkbdfmmkm.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gjistneln.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/gvemtsaqm.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/grkmhkuds.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gbyteupps.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/glpvgyphq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/gfslbfytj.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gmfmwjhsu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/glkrnegwt.sHtML

[Q81] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gksgesloy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gdnjxqrks.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gpedovydz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/ghfkunalg.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gucnzofbh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gdphdarzw.sHtML


<!-- 参考信息 -->