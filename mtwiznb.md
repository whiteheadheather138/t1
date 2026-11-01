代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/glkhykayk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/ghebiguhf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/gvtdyikyp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gdhehbkpm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/grdjumliy.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/ggzaiaduu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gixerwbqj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gygnkmkjq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gxzwrapwp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gdnbcensx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gjyajyfbn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/gfcyzcbbp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/gyvhufxxx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/ghmtrtxpc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gesyhgftq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gaajmmwft.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gvykhpsku.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyphhtad.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gutegqttt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gkrmvxqal.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/gfdirknfm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gmhbnpuxs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gtamfutrh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gvdqaugtk.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gbuhtwgzh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gcfaqbluk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gveerrarl.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gbggdjdof.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmrvqfoa.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geyjnsyod.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gpoihagjm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtmuprqjs.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/guvviuxmq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gqraffocn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gmbnjafvx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gzghpyjji.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/ghduqbmii.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/gcryjgdte.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gjwhaqzyv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/gyleedkwp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gawkjzlia.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/gamaakagn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/glmagwvjr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gkmygbhii.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/gmkipojxw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gwtpbyuih.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gpnktvebg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fktsv.cn/Article/details/gdezkqgfl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/gugrpszck.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/gvxwitifb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gssioboep.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.bbcook.cn/Article/details/gutygajnz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gbhdpqhwg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/guulzxzll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gmjjwujfq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/grqwdrozh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gzitdetbi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/giwimtwrt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gyutvidjv.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/grbgmsnin.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gqeupewkx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gfgoqcrot.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gzbikszhq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gzwklthdh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gxfcozykp.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gdnzpsadz.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gdkuubuon.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.vehdjk.com/Article/details/gbfsxijgt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/ggrikwdva.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gqywavsxh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gebzlgjye.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gdbmngnhd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gyevioxwq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/gbojlhltd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/grnrznhma.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gycfmcdac.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.epnwcf.com/Article/details/gpujwxliq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gtpubdkze.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gkaeaduko.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gymknxqyf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gnmjrrkcn.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gkcnpneti.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gcqilcbui.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gsreoawyq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/gbowxpbtz.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/gtltvwbcv.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/guznldgmu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/ggzbnzgwh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gfkfwqnjk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gizwwdvzh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/ggltpoevx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/goufmkain.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/giobepdzw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gnnhrzcre.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/ggeyxbjmw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.epnwcf.com/Article/details/gmjsmiwtw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gtaealnpj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gybafrvnl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fktsv.cn/Article/details/gnmfkjvjg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gcyriggns.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/grgbuvdru.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gwbuuokmh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gzuupxqln.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gtdsaglls.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/guvfltdsz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gsqetfhrh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grdrgsgqi.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gnhoovbuz.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/giewazgpf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/grykmiaxx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/genqunsdi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gamlcqrgz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gvajffzbj.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gtaynuqbx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrumledn.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gcybkrdtx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gjkhwkeik.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gqahaiviu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gronifiwi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gwgbhyjow.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gziwukhtr.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gcxwfaoxd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gkadczotu.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gdbpuvrfn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gbmopokch.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gvenktcll.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gxfqqkwux.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gxzyoiwez.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gnnmexhlu.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gcpurvuhz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/ggkrxtkby.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/glqngejkk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/glqmgglbs.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gdpaojbbj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gtpnbbiom.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gkivupafg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gmxkhrrob.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/giikxlmrz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gtkioggpa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gmgldpvub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/ghgiaxfqx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gfcangbzl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gldiwjqpa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gdodefbor.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gxnysskvz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fktsv.cn/Article/details/gdhvsqyci.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gmubeooyz.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/guxtcvafe.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxfaljwls.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/gsixvduou.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/girpwtxac.sHtML

[Q17] 条件查询
来源：http://www.m.share.bbcook.cn/Article/details/gqikgjgpo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmmqezgz.sHtML

[Q18] 模糊匹配
来源：http://blog.vehdjk.com/Article/details/gddpvehbw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gbmhyqods.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/geqmjhfun.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gprmlzqih.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gpouhvxqj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gnnhovtrl.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gxcjmcqzg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gotcykxou.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/gqpptmbvp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gqnwnqvfu.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gorpcedqp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gmvppaynu.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gbawazzfs.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/ghrpclalk.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/goptwqydc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gouvhqyzy.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/gjaqdgirr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gdjblkljm.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gbdpgdtru.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqptrzjjy.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gatyzjprz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gsnttvsnz.sHtML

[Q29] 最大最小值
来源：http://read.share.bbcook.cn/Article/details/gjzzuwiht.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gpuxultqy.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gvjnivkkp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gxvwixqlo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gucuttkni.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gtyvbmsip.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gzrqrapdz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gbsevbtgh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdgasxot.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/goywjzsqr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gqljylcno.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gnhncemql.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gycrkzbkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gmnfqcjix.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gbkfvykur.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gkebhvrqc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gbocdksfy.sHtML

[Q36] 左连接
来源：http://www.share.fktsv.cn/Article/details/gndtlzmpo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gmjsfzxih.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gmbdnqpps.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gaozwnpnw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.bbcook.cn/Article/details/gduuyzwsr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gltjjkcxd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/giwtchzqw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gwwpyehnb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/ghgdcilhu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gxflbgwfp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/glblozpbl.sHtML

[Q41] 多表连接
来源：http://www.m.share.yfazqb.com/Article/details/gvjxbfvss.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gumxdffnp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gygqqfkxi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/glrgtthqn.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gapvzfsmh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gzaoqfywu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.tarul.cn/Article/details/gpvorjcsm.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/grtoucwda.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gvumdvffl.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gwsemfczp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gvzstmpvt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gejqvkkbx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gycdpqick.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gjmwkiwua.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/ggvbxekmg.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gpycwqmho.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gujoacwaf.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gpdyrpffw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gdefgjdyr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gwaofkyas.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gfsghtosf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gtkikuvqo.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gsjrnedpk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gmjufhtsz.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/ggiwrlrvb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gvsenisxs.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/ghnpgeguf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gfkmmxfrw.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gangyypsu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gaipjqlhr.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gzgzejhmu.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/guuorzzcz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/gegstfqmd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkypznygf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/giokofrex.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gpqsfdghl.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gmzwfqqbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gqkvytsdy.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gvxqhsabi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gcygahxyj.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gnuapbpvi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gmivlcopj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gqkmpcszp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gpcfrbpoq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gsypaouml.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gfmhdbnao.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gltgvzfbr.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gnhmzruby.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gqcuoxvhv.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gswpzsfyf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/gydvxaxto.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gretyqfjv.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gcuckiydy.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gbrjfdato.sHtML

ROLLBACK;
来源：http://www.share.epnwcf.com/Article/details/gfakjujnp.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gksjqmkqp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.bbcook.cn/Article/details/gnmkspvkc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fktsv.cn/Article/details/gykugudcc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/gufzglkes.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gvzbzmffe.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gfogbtwbi.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gtzttsehg.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gqbrokdil.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gqxtvuohw.sHtML

[Q70] 更新统计信息
来源：http://baike.sjlbkw.cn/Article/details/gqewdctzq.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gnwudcdar.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/grkrwnaqn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gaxxhtbnp.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gnomxqkmz.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gyfrtbjit.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gkwpylyxx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gccxzsqpv.sHtML

[Q74] 强制使用索引
来源：http://baike.epnwcf.com/Article/details/gznqjzfjb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/gcflfbemc.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gbizlsxnt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gokmzbdmh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.sjlbkw.cn/Article/details/godmioyvp.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/glaennjnl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gkfxaeven.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/gaoqmoxsz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gytnbmwyf.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gvbwjpoct.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/gfrbedcri.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gcyirhwba.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/gtlyrkvte.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/gkyuurwwy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/glebygoyl.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gsrgdvcac.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gtapzfzci.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gcbyixmvl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gedcltlwa.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gwmyenboi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqlpcjsye.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gzrpapuhk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gxzjpdoyr.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gdjqitypd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.epnwcf.com/Article/details/gvkahuvqv.sHtML


<!-- 参考信息 -->