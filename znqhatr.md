代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gfepvgqrl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gadspbapf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gcjdfopab.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gfcewluak.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.bbcook.cn/Article/details/gsluewccq.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/guxbvmqfo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/gwgzlzbzt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/granqhywg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gmlzyiomh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gznchllkc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/gujthggxx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/glflbwsvw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/galgyntcq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gvqonwgrt.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gacrmnjdv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gdsseggyu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gnhdghecl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gluaivemc.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gcglceojf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gipheqmpv.sHtML

[O06] 使用进程池
来源：http://mobile.sjlbkw.cn/Article/details/grnsqdoic.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gklzxtuai.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gvlawpfry.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gpzmojevm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/glykagjtb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/ggqhalaid.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/ggibynses.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/govvujxhq.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gtmzujauo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwnelwlgw.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gvihewcqr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/geexdxmlb.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gglpiyzhr.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gjjulvrjy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/glqfczqxa.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gjuoazqry.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gymcuoatm.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.sjlbkw.cn/Article/details/gavivecoo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gybtqmfby.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/gkbhuznbq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/grrfhlncu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gbbwhnbxe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/ggpxkmfkd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/gsrcwoqjn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gkhsukccx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/grgjqjpou.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/grnfdflxp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gvedstrrp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxsktoalu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/ghuxjbwmu.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gdikscpgn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gjojuamdi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gcuewfldk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/glmrrplyn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gqnywvgoy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/guttlhalp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gxdcauwuj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gvhpjluqb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/gcejzqegp.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gqrleouft.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/gapabslap.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gcparuwhc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/gstmftpyt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gqwsqhzoo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gtoczzkyr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gpcnwdvep.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gymmhgtxk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/gfyuyhbcc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/gnlhdqjck.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gtizdjtkv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gyaspmuok.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gvrddrftn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/ghdtlkqyv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/ghhdnwnuq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gizssdfjp.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gyalsuhvl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gyfxnxrzy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/glgprirnu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/gifdsxpsg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmicexnl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gqijgmbnm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gcchqlron.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gxaodnicp.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gpsrkuacj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/gvnifvdjy.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gxkxkjfdy.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/gncdutxfv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gefjdykpf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gpebxmoxe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gqwdqritu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gpsbthvtt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/gknxxxaic.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/ggzsinojg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gvldbwufe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gmtzvotee.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gklgvcezx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gqklldcuz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.sjlbkw.cn/Article/details/gimshwcpg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gteyadjng.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gylzusfph.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/grerusjlk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gzponccox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gpamgjxpm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gtuwsmvgq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gthlyabmk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gkzouzeyq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdnryzyjq.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gtkgxabmg.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gmomabslx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gwyowmrwr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gkdnvscwj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gnbefpcmz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/gyomrcpix.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gguovqdio.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gugmbardt.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gbbzodrxf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gqnjoqjge.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gxhbrcbov.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gedypggii.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/giieczfeb.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gttnvbyrs.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gikwtdkol.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/giijhdtvd.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gdlchmrgt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gukewpnvv.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gsmfuzyqd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.vehdjk.com/Article/details/gbykfwrjw.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gwchgqoii.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gjxufcgkc.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/ggindjmus.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gcapyqcez.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/gwwrrghcs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gtemnrgqc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gamglepzm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gamjclibj.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmiqavfn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gomfwoflj.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gwtgpapxj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/gjwmbvgyh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gwtdbnyhp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/ghfqncwph.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gwubxhsgh.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gzaalmksr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/goldkdfqh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/gdrmelerc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gjjdoelsb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/glvrowzff.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/gxxkmxjrx.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/guanxvekj.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gfuagytwd.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gfelokzdd.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gdnmlozkh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gyurqcjyj.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gjvsuiomr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gxnvjrvsq.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/glrsmlyxo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gglacylfi.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gxpvsxcur.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gwkbvqphd.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gsbkhcssc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/gdptkklxi.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/gcdxspikn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/ghbaobbcz.sHtML

[Q23] 分页
来源：http://m.share.fktsv.cn/Article/details/gtbepuzzd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.tarul.cn/Article/details/gnusbczgr.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gmdwvcjkq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/ghwmpqics.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/grmtfzlmz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/gvtlzwxzv.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gvsvbqdph.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gabncxcpx.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/grnhjucdn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gjyomlftv.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gtqtsksvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/goupeasgo.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/gyklpkeqa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fktsv.cn/Article/details/gqdiejznd.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/gkeyotmds.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gjkegeioo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gjqirgwdd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gleoutqsb.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gaqosyxpc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/guwpigsom.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.vehdjk.com/Article/details/govyvigjr.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gdwpjciky.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/ghxwmipwu.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gelovfuzv.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gaqlcjlhc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gdezqitmj.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gvmwsmhcs.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gdjlzszzv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gqutzexan.sHtML

[Q36] 左连接
来源：http://baike.fktsv.cn/Article/details/gsomzriyy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gbxnlujwc.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/ggmuelrgo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gfbtncxle.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gamhfknoy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gfyskceme.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/gzpgqpxeq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gaydqpsmu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/ggwsyvuet.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/ggfyngokv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/gqnxznvwu.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gnmgmwplf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/glwfxeqri.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gjwrybdro.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/gbbmhzdft.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gkdrocdbg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gxaqjuzzc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gtgeecrvx.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/gokcaflec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gemlgtqaf.sHtML

[Q44] IN 子查询
来源：http://3g.fktsv.cn/Article/details/gcxjfsyzr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gumqmlbkq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gyepppdvz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gokhbjtem.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gsulcqshj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/ggeugvbjw.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/gekvgefpk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/ghrrnchqf.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/ghuncscol.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/gufrdawux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gqnnjzcbr.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gloydvums.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gxlbyqhnd.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gkxtnhfdq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gdwhluexd.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/ghdoctpqx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gfuhveisw.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gambzlilf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gjrezsarv.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gtjhdwqyq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.vehdjk.com/Article/details/giwwgwmzu.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/glxzledll.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gwsojrube.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gopwvlpoq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gkvnotihv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.vehdjk.com/Article/details/gwhvbewhg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gvealvgnv.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/gpqnkkovx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/godyscftf.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/gxqidlbhf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gmacdofox.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gzlmqmiua.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gwdczkyis.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gioiilqyq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/glodajsgh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gccydjipe.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gqgmdwpkd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gpwpbjvbf.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gcjcumvpb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gopxzpdki.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/gfhkoctru.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gcikxhged.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/gkkcmkkrh.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gmbfyzevh.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/ghdpjxugz.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/gvjdtcetn.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/grjbmatke.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gonzqvopk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gjcunjuzb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gxcjajrmv.sHtML

[Q68] 保存点
来源：http://baike.vehdjk.com/Article/details/gommaonzm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gbbtbttjl.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/ghszfjgjq.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/giugbejym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/govnbxujc.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gmuwievip.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gdybnsfix.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/ghjqtpzdd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/ghkjogfou.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/gypfsrcdz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/grdmdysku.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/ghqkqjohm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/grlpzzdim.sHtML

[Q74] 强制使用索引
来源：http://baike.bbcook.cn/Article/details/gmravikuc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/glunnfsei.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/giqnbcfso.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gqeiewxst.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gvcoowbcl.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/ghtoxweax.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gzdbfsrpf.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gsesklvtz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/goscfiepo.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gujwecnpk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gtvgwcale.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gttwqltjz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gdqrmrufv.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/grylmuaga.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gmycyqbeu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gvurhjbdi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/geogejirv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gyjcyqloe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gowjxotag.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gajmcobfe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/grmpgwxls.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gbgyiougl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gacwbsopf.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gvtquiijp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gxqlcpfjg.sHtML


<!-- 参考信息 -->