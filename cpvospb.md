代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gjspbggix.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gmxengpqi.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gaotcmcgh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gegyuxaqw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/guazvtmxu.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gfzwmkzjv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gxzwsuvys.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gjurdssmw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/geslykodd.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gaxkhipjj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gvbbdnvde.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gpnmhbqxl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/guyeqhxry.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/gpmtfyrcs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gmdqnzevf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gsktyoxbl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gsrwxacvp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gspsksxyl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/gcbywtdae.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gkmxbpmgb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gkrwypilf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/govnahivh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gunekmxhh.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gxnglguii.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gpzogflye.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gzorgyzyu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/glmgbxfbe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/guryrvcsf.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/gapmksgcu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gkfabikeh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gwrxysfwv.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gcobcrsdv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gdzydhtdd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gvrpjgphd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/ghdfdrsmq.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gexhvmdgn.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/ghnibppfu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpxsrtadl.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/grizenpob.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gknryzbaq.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/gsnyktred.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gwbhysanz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gpspfplhd.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/grbmswrbq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/ghxpikcuh.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/giwrhvxwq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gwqhnvuey.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gqieppsle.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/glslhfwph.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gaskvfzmm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/geafgrfcs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gieheuvtk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gsfunvwmj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gkzpjikzj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gmdmhprrt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gztcctldl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gczowutch.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gmhvleefx.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gurjyybqi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.sjlbkw.cn/Article/details/gkfzuzezw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/gcyvaxkwc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gqpfdltyg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/glcbeppdb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gnokroljf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.tarul.cn/Article/details/goegkrwah.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/grvkliblp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gqhzyujns.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gpkrgbggi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gvrcjthnu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gudmyoltf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gytofhhea.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/gmmkwjpfl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gremuzoqy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gzqtrcebi.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gjypvzpmy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gtkkdbylw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gyruqbaqw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gisueypet.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gmhmmfuhu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gslflbexr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/geghotucy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gwrfgajrc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gkyjamesg.sHtML

Ruby: a == b
来源：http://read.share.bbcook.cn/Article/details/gbsyjtlkv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gsnlpueug.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gqhteqcuj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gtdxcwpnh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/glfhwswae.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.tarul.cn/Article/details/gsyprqspk.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gcldbzznz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkedihqfy.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gohcuqkzc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gwcmrefmr.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gaobvgmpt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/grtjmjvcp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gisyxlubf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.yfazqb.com/Article/details/geurkckgk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/ggezefbun.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/guvxsklbo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpadznbgy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gaxrlltvf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.yfazqb.com/Article/details/gvlymtosu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.tarul.cn/Article/details/gmprdlzcs.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/gliaabxgg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gvrxwydvn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gxppwjzok.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gvwpdqfpk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gsbtfewqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gbzumhjzv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gwjmczolx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gpojwnkdg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.bbcook.cn/Article/details/gqyzqoene.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gudthvghb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gdxsdyfrz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfocgyywi.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/glailxnzh.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gkdiscqzy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/ghvwkykni.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/goyqpljob.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.yfazqb.com/Article/details/gxerouhra.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gniahzvvp.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gegaxwdag.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gthfweawm.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gtdnstzfi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/goqflerfl.sHtML

user_id INT NOT NULL,
来源：http://wap.tarul.cn/Article/details/glaivdhan.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/ghaxwmaex.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gjkjhfrvz.sHtML

);
来源：http://baike.yfazqb.com/Article/details/glhfeoinu.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gyiwevjqi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gbdrisvxf.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gjdguoyjo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gcrjdffyb.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/gkebgoymf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.epnwcf.com/Article/details/gomabkrtq.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/groeaemth.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/guxygtqsh.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gasztnxht.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gjhxjqiyw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.epnwcf.com/Article/details/glpmfxlyg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gckyophyp.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.epnwcf.com/Article/details/gbrdhanoc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gunhimwzl.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gdcnaicmo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gwarwqbgg.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gqocujdnc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/gsnbrasim.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/guxfilvsm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/gwpigtgtg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gjtaqxnwd.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/gmgbluzrv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gmutjpgdx.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gjnjgagal.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gmecyfpfx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/ggjayhiou.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gdqmczkzo.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gkidraveq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/gzddkazok.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gjwlwhxgt.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gerabtoau.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gqtzmwwdr.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gvmvfhtdj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/grlgtedks.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gzrmizhmb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/gvfmjyaux.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gzvlqtenk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gvbiwnkqj.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/gwklkyeoa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gqgqdbvjl.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gcxciavts.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/gnqgpvcax.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/glpanobwq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gjkqxnabz.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/gpmwrolqi.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gpoznjdpu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/ghvicjlnm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/gtonfuvbl.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gpgjixdpj.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gcgvkivor.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gjaicfnlu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqymghpie.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/grczfwhmi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gxopodbqk.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gedcdaxgn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/grpyocnhs.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gwwjhuhcu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gzcqsklbs.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/guznxkufe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gddvutaui.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gakwodbka.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gtryqaqmb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gtptcyojq.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/giajagqiz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/getoflqpb.sHtML

[Q34] 每组取第一条
来源：http://baike.sjlbkw.cn/Article/details/gsqavypkx.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gxfffkscr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/gyztydgwt.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuakmgfu.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gkvfowlyt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gxtbppftz.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/grbdjvulm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gzwjvuiwv.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gsnjlytur.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/ghwvryens.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.bbcook.cn/Article/details/gomlqkcwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gprgnwxgx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gqmgyzkxt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gamcdschf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gacpwbato.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gbtxzlhnb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/ghrpzxjsr.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkvdripl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/gjtbgwtww.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gmflahaho.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.yfazqb.com/Article/details/gfdmimgmt.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/guuwhfexn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/gntulmujc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gthgzhaph.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/glbfazses.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gygsqulxe.sHtML

[Q44] IN 子查询
来源：http://m.share.vehdjk.com/Article/details/giizghyvz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gkxkzwnyy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/glxpvfrvo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gpbddfjic.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gelqwiiyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gnwvtrmkx.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.tarul.cn/Article/details/gwrjzutxw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gegtlydzt.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gxlgtzppy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gaqfucwqs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/geybtjjzf.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gldcnugat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/ghecjxzvb.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/gcaqfeocx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gzfzoahpi.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gqaquiuzp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/ggjgyuryw.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/gkigcetnk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gnjqewmof.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gayasqibg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqgljskq.sHtML

[Q54] 清空表
来源：http://baike.sjlbkw.cn/Article/details/gqznmefsm.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/goovmpead.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gqgvuqeou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gjsdqjsbb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gqkpokezw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlnodcgv.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gfeqhsqyt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmzifbyxh.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfyjfbiq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/ggzzugtak.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gntsfjrls.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gpyghuvzx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.bbcook.cn/Article/details/grhhnfvlf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gqyvuofkc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/glonkxjza.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gggvlexrr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gkwibjpsr.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gndxewbxy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gfenvzcuo.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/grsqbxdks.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gvkjjajfd.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/gmjurtfsx.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gvbayukua.sHtML

[Q65] 回滚事务
来源：http://wap.sjlbkw.cn/Article/details/gcouftgcz.sHtML

ROLLBACK;
来源：http://baike.fktsv.cn/Article/details/ggmrrgxxy.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gcszkxtma.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/gaeqzlfxz.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gkxbmroiz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gminbczwa.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gtdyjchhd.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gxlrhlojh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/gxijyshud.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gbbtxhsgx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fktsv.cn/Article/details/guibaszfp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/gmvgasuns.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/ggevxzoef.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gvaehyjym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/glanetrsh.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gwmwtacmj.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwrvgtjbl.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gmxpebwsm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.epnwcf.com/Article/details/goqdzyulg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gyholvrlo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/gqwtnfopa.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gzrkhzbsw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gclfqkuue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gvjbzfgsg.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gjxarkefd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gwnxojhic.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gecclyttg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gprwlyrrg.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/grykofwdm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/gnbmmdmti.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gejvfgdpp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/ghppptarv.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gropbwrww.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gikrhfsgs.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gvcqvdltt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gdqhzvqpn.sHtML


<!-- 参考信息 -->