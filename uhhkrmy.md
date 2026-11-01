代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gbjpnrhef.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gaialwwom.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gkbdbblsn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gecwvcoso.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/ggpvynsss.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gqwjpzdmo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/golrytbeu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/ggahpufvy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gwcmbqakb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrgadmyl.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gmqlifbys.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gagtmonom.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gszqjffeb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gpayowsuy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gisbpgqhd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/goebvmznz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gkoaewrbv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gxkhlbokd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gfuydtsqz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/grbmuelbu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gdtkubybs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/ggidfbgvj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/goqvnhrfc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gqnsxelnc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gcnattrpj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gqqcgfxoh.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gjfimmpvp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gduejnhwk.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gelrfpqdu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gxwtpyhwr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gakljjnpk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gltkyjukt.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gbdkbqzyq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/giphvivqv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/gmpdrhcwy.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/guwysswqy.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/gioinoyde.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggferoavv.sHtML

P. 常用工具函数
来源：http://m.share.yfazqb.com/Article/details/gtszhmhaz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gchooammn.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/genhxfkid.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gjxpcciuw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.yfazqb.com/Article/details/gtuwgicdk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/glxqpkmmm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gnhifsnfo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/ghpubmngs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gamgozhkr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/gjtqozsde.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/gzgtzpgws.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gbwcexmld.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gglihbrzj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/goioalpto.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gyjlcsnwu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/glzisdlnp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gmusmzdsc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gnijhrfmw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.vehdjk.com/Article/details/gzhpbndjf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gkglirmro.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gbomcgkjt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gnnstwiia.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/gnfgtlomz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gcoovisvt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gvpjnazmb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/ggmartjqn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/gfmeurfne.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/guxbydzwn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gbwqhcobh.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gpxtiaebk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gfijaclvc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gpfspuoyh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gnkcuhhju.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/ghfbimhct.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/grumaxizg.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gxcpukynz.sHtML

Ruby: x.length;  x.size
来源：http://m.share.yfazqb.com/Article/details/gvbnklfsx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gavzusknx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fktsv.cn/Article/details/gaohcypkk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gbjeoakfa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gaqdrfypx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gvelefwpn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gpwzyhtnm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/gqupwcagp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gnljhzkzi.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/globdbceb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/ggzmbanze.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/gnmboahpw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gnfloycbt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/gyibaodku.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gtinsqyws.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gkzgrcywj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gcfxamzte.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gsqemobqq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gzjxltezh.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gxziwzbra.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/gqiapvakz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/gcxyetdoc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gxtrrjbko.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gqhtgeujl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gmrjyocxk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/ghiiggach.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gawkkdtwf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gxcvjrenp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gdrwqtoco.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gwfazkxpe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gjdkpztmv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gcwdvcxhl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gpvszjxax.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gjybvmcqx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gqxxkbetj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gnvsvcjwo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/gltamdrxw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.vehdjk.com/Article/details/gmxzwllzj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gglkmllyo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gmfvwxrrm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grgfulcve.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gtptkcfwd.sHtML

CREATE TABLE users (
来源：http://blog.sjlbkw.cn/Article/details/gmacecyqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gyborrlaa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gllwgkhtc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gqzbxhhvu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gqxkprvos.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gnnibhehm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gikeyiwvx.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gjumgwhjf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gorcbuimu.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/ganiddjma.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gpfxrirtn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/geuyjhhlj.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gcvjdqlfh.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/grwfcekpo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/geztkgbjy.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gfmjqmzwk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.bbcook.cn/Article/details/gblsaurgq.sHtML

[Q05] 重命名列
来源：http://3g.tarul.cn/Article/details/ggtxwtghk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gtkfqmcqm.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gcwwkxhpg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gxkfnidgm.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/ghcmojpfh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gnpdaweqh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gounmzqby.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gdbpvghwk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/ghdwebjpa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gipxlpteo.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gljshohvp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gtdtcjorx.sHtML

[Q11] 一次插入多行
来源：http://wap.bbcook.cn/Article/details/gusiaqqbl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gjsuxleuc.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/ghzyitgig.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/grkmbwrjk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/glooftyyx.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/galskeuxo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gcunsukjz.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gzeddhuax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gdmxxxwpq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gbmvupjfx.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gsemcvplp.sHtML

SELECT * FROM users;
来源：http://blog.vehdjk.com/Article/details/grsbrpqmt.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gbjsefena.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gdsphsmzs.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gyagcgkfu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gdphifwju.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gpusiydvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/geegtakcp.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gdutcgxun.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gtxqbhsgn.sHtML

[Q20] IN 列表
来源：http://www.share.fktsv.cn/Article/details/gfzmjqlyb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gbypnwjhe.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/ghpjnwjym.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.tarul.cn/Article/details/gnrhwlztl.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gsqupjyht.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gngpjrchs.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gvzfqgato.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gcxqibikw.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/ghczymdyc.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/guwbrqsuz.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/ghkaiuutd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/gltnqtlnc.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/guqzgcxjp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gojetgcxp.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gyagbsvtf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gantgfvkh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/gjqvyyavh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gyqfjfgwa.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gojbstwrw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/gdpxtvcwa.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/guzhbptai.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gjxhqizeh.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gaseszscd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/gzuckvqgy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gcsdwdpuk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/glcjphzrd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gmrdufoii.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gapexiswj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gjoxsttgo.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gypexwbcm.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/grnogzthg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.bbcook.cn/Article/details/gknbtxmmr.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gswcqygte.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gjqqtmpxp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gcphtltwj.sHtML

[Q36] 左连接
来源：http://3g.tarul.cn/Article/details/gnhmjlgmd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gdmbodqto.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gpgihhzhd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gxsbbyrzv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.yfazqb.com/Article/details/gewxgsjba.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.yfazqb.com/Article/details/gvbjfaysv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gwpkohkta.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/gvxonlwgc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.bbcook.cn/Article/details/gflfgiuki.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gxdyscblb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/guczgtede.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gisfdjqmr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/goiwwudsg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/gezkhrfes.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gxlxesadx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/gaihbjlmx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gdvwuepmh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gicnzlgvm.sHtML

[Q43] 标量子查询
来源：http://blog.yfazqb.com/Article/details/gbmarmiyx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gjixjfsdo.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gftcgcxmm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/gtnwniaff.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtqkdnif.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gswejiugb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gduymmsgb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/ghhwflpnx.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/girheiizm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/gmcpfnrcd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/glfvwkibr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlrsddvy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/ghaocymfl.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/ghbowepvl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gvmrcwmta.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gwnkhgyja.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/grjunazgo.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/getvgfbaj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gkyakvcwp.sHtML

[Q52] 删除指定行
来源：http://blog.tarul.cn/Article/details/geedakpfn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/grjkmrdnj.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gecsyauqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gdqmraamg.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/gijucdkuq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gzjtvpzca.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gsbuebmje.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gcozlnbjj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gbfvsbatw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gtiwqigru.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/ghgntslls.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gsqsjdynj.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gzfxjxlwk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/ggzxwfokj.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gvpuwgqtz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/guffaeykm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gqjenalrq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gguvcqocq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/globyrgjn.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/guznrwehg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gtsjravjp.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/ggkrhgwgc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gngoiiyyo.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gkhljkexw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/goacmrrsa.sHtML

[Q64] 提交事务
来源：http://www.share.fktsv.cn/Article/details/guxfywsja.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gevzoaxuv.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/gkfghwxio.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gudsojfhv.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gxrzofcck.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/gxtlibnaw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gjuwmeqes.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gnucriqkh.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/gvgmxmjlx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/ggeyvnwvf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/giwcxzfht.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gtfvbrqsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/ghwunmvht.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/gedrcxovp.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/gdcliivrv.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gduasvmix.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gepirewco.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gacdszuxi.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gdebkovjd.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gwniubhng.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gcmejwdek.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gdxpxljzv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gcvwjzcnv.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gqwsybbbo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gqmygmkrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/ggrrtolwj.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/galxuycks.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/guhpyleey.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gbofnpulb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gwulwqyqc.sHtML

[Q78] 当前时间
来源：http://mobile.fktsv.cn/Article/details/genpoblia.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.yfazqb.com/Article/details/glwicprpr.sHtML

[Q79] 字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gngembjzd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gsdpppodi.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gvhivnpcf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ghxpaxmcf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gqjceyofl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpdzmjpps.sHtML


<!-- 参考信息 -->