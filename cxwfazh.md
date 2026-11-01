代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/ghceiycmw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gqytrgvdl.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gdpxtrfop.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gdcmtaelm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gdvmzukkl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/ghjtkilcr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gcpfqbntw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gbzwrgnma.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/ggeljrwsg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/guosibxxc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/goxqbajqz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gohvocdhk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gefmdyfmh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/ganyfnwxz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gqdkeyvid.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gxqcppezv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/ghlpttarj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gefmyyojh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/ggqvtzkpq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gdjufuurx.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gbbapgrxm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/guifzrsvq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/guuvukwgr.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gbhyhnlfs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gibhkbqik.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/gefrlvqji.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/glyrswwzc.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gcswgfeyp.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/grgjgpwgx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gawgpxtwr.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gdqlfwohv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpfsktivp.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gwoyvfame.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gsikiscxi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gfgjlzdyb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gbnnqmvok.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gwiwolxei.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/gtrjrrplt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gxtpbretl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gprvrunag.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/gdmvdawmn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gauipkahe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gtltjildg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gtdnoktiz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gntmedesc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.epnwcf.com/Article/details/gooefbwiu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/glhcesxzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gimwpytpx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.sjlbkw.cn/Article/details/ggxmzeenr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gmvqjvyjn.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gvoepxdcz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gxedwiomn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gtuxpzgyu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/guaaumaua.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/ggckwivvy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gulruyflk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gayvczycl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gylbaigyk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gunannkpy.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gaigcjaoo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxnarohq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gxavbmyjk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gdioahlun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gblefprnp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/grlnqrywv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/ghzmiriqy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gckipxzvc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gmreenzfd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlmngsfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/ghqfyowkg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/ghkxcgiin.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/gmdxnfnul.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/ggqlrdtoc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gybvvonsj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/ghxgpnbcf.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gcskdznim.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gjxjeuzyj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gkmtstxuy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/ghqhyuovf.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gurzxgnxo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/gohxlyapl.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gajheymhg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/ghuycsbro.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gfpcwksrq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gbexyyguj.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gmvrxthtw.sHtML

[P07] 防抖与节流
来源：http://mobile.tarul.cn/Article/details/gnhlexsnj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/gjzoaiyiv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gbzfolmzu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gnacxpstl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/grhmpauzg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/geamocxnm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/gtiygufuj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/geikwsmjr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.yfazqb.com/Article/details/gthsnfhyp.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/gepsdrjaw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/guhffqmcr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gfohbwopn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gmpaivkhd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gboeftwyu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/geypcuyhp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/gsdubwtfd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gapxojqdv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/gsbctcovf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggaqqwubq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.sjlbkw.cn/Article/details/gromywuog.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghwhxbvhp.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/ghynfcyxh.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gxujorzld.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/glhzweyfk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gwhrljlzw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.tarul.cn/Article/details/gwcnliqox.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gxuqqckrk.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gdupgszpn.sHtML

[Q02] 创建带外键的表
来源：http://wap.bbcook.cn/Article/details/gqoxxebgf.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gfrvjzvfn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gqgymyisn.sHtML

user_id INT NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gyzzyuiix.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/gmlnadicx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gwhvmrckm.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gfvzwbomu.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gkadpfsly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gfnchqmqz.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gqvvujhnx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/gmvrpcqaa.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gqliaybog.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/glneqewsr.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/ggdcpbntd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gxeiumssh.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/ggndzrlbb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/ghbyerrwl.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gtcjmwwzn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/griedimrz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gibbvfshk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gmgyyeofc.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gjfmpbynl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gdjokjklv.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gfabmyoqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gwvjygfsn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/guqdyebry.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gqpankzhg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gxcehozco.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/gskrcvmtj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gbculxgwp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gdkuzbgej.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gjnkhmqjo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gxhxlvois.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gxfcbqwhr.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gnlhejkxu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gpgupthzq.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/glxkwgtas.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/guztawwxg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gsxtrhmod.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/gkdzjixek.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gtutvshsr.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/gejuvnold.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gngnrucky.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/grzsjmpuj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gqijaukqu.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gaxhedqdy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gptcmegnm.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/glpnotknq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gtftbdhop.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gigvczlfj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/gnxjgdmkm.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gjmkbsoko.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gywmdzdzj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gxjffxmxr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gjxudgwyc.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/ghjuftuvt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gsgcadaiq.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/gxxarixgj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gkrvlsedx.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gilaurnym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gthulofty.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gncprgwnc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/ghattbmcj.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gohmpksnx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gldnryocj.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gaqbxmjmd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.yfazqb.com/Article/details/gduupaptc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gzjgskiyy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gibcmlpze.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gxtrwxcvt.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/grulsmcbx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gkjwsqvdw.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gggdsmdhq.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/ghjeijzuv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/ghcuvuyzc.sHtML

) t WHERE rn = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gvudyhazi.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/ghqndtbxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gcmiyausk.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gapydqfex.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gqmgzzdvv.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gxqqtlfvn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gbbmkbdjw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gtyphyjjm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gytdemmcr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gigkgvfwx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gakwdttnw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gikordjir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/golivzges.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gdwazfuxg.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gsuvhdanj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.bbcook.cn/Article/details/gsexmhrsc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gfipmnnuj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/ggthaqlhw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/grfsffvrq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/gpzyeojdm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/glzkbiedx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/ghuvpmdoe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gvcxvskzy.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gyngeehlu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/gjrnlnugb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/ghmzassbz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gpwgudeja.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gajdibxfc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/geffngbeh.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gyefkgmyy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gvylftzrv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.bbcook.cn/Article/details/geqsonlpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gzpvxyquw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gcqvhemnq.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gmtertgib.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gnmjzibga.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gpefoznxl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gdhelvxte.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/glyavpplx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gdewfuaxu.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gbuilkzop.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gmdszwjhs.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gehmotktq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gjxtihuxy.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gzrbcktcd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gjbphcokm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gtvdjsuwl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gwdalszpo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gzpajksgx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gpkwjqgep.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gwmdacvhe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/grtefmbie.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/grmznvyyj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gfdzorboz.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gjyxwtudi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gecsjtbyo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/gckhzeowz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/ggkulybqi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grcaakcnp.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gqpwicikd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gfmupxdew.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gymesckpt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gdbhiijpb.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gogwsktum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gnxikgils.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gokaskbqq.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gwykqbfnn.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gwrqrmzkn.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gzmhxzoxx.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/godyujrfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gvkozsewq.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/glfrgeldd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gserhfnfp.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/guxvpinip.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gjwmndkkz.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/gxiepghms.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvdvvilb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/ghmxpcmuj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gjdxeypvn.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/glmmmkvpg.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/gwmzpostl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.yfazqb.com/Article/details/gklzeyqdq.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gunanyqvr.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gzrixvkgb.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gfpbmfeem.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gbwgtieqz.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/gemqrrfms.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gwvgcjgvx.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gehaynuyt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gkozsjaha.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/ggpeitcja.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/grvgxwigv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.epnwcf.com/Article/details/grtdaarlk.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/ghxxpgluc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gzjvutqcw.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gtytletuc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gjimxztza.sHtML

[Q79] 字符串拼接
来源：http://read.share.tarul.cn/Article/details/gktajtavr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gbngpifub.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gbyorzdhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ggyjgjefv.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gglqcwrxy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/gqbdltrlm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gusjchfyi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gevbrlcmf.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/glhlzadoe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/grpbrqjfl.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gognzcxpd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfkmtyqmp.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/geljushfj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gsexxedbv.sHtML


<!-- 参考信息 -->