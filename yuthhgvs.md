代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://deu.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://rea.havefunace.top

Py:   with lock: shared += 1
来源：http://yfz.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://lym.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kjf.jinghuilouyu.cn

TS:   // 同 JS
来源：http://nwr.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://puy.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://shk.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://luv.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://tky.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://crp.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://cwi.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xjr.yuxming.cn

JS:   async function f() { await g(); }
来源：http://lwy.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ofs.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ggi.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jcw.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://ofd.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://xcy.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://olv.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://clr.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rfg.meibo888.top

JS:   await Promise.all(tasks)
来源：http://vus.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://fit.epnwcf.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://svq.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eop.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://ccc.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://zrj.shzxlz.cn

[O06] 使用进程池
来源：http://qhp.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yys.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kfq.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://oil.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://lss.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oxl.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://irp.ivvv.top

Ruby: // fork 块
来源：http://mlu.zhijiandao.cn

C#:   Parallel.For
来源：http://lnh.nanxuanxn.top

================================================================================
来源：http://dgz.yueranfly.top

P. 常用工具函数
来源：http://dnf.pycfn.com

================================================================================
来源：http://qey.sysykeji.top

[P01] 生成 UUID
来源：http://nsp.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://gol.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hcy.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://enb.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://mxb.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://pyp.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://ewd.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://shr.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://jgl.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://dmm.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fnd.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pkg.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tcy.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://czf.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://izp.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igc.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cpi.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bsn.yj20258.top

[P03] 生成短随机字符串
来源：http://hop.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jsi.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eff.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://osf.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dhu.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nea.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qkj.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nyo.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rrp.bbcook.cn

[P04] 求长度
来源：http://tdt.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jqs.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vze.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ydg.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xia.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://jkh.bjfxy.top

Go:   len(arr);  len(m)
来源：http://veq.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://jmk.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://nlb.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://mqs.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://tak.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wna.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hal.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sug.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xal.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://oco.fktsv.cn

Ruby: a == b
来源：http://pgs.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ssq.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dlv.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ika.birdmap.top

PHP:  if (empty($x)) {}
来源：http://ugt.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ref.gotoacloud.top

TS:   if (x == null) {}
来源：http://phw.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://pzb.sxryk.cn

Go:   if x == nil {}
来源：http://nuk.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ldf.sxryk.cn

C#:   if (x is null) {}
来源：http://rsf.havefunace.top

[P07] 防抖与节流
来源：http://txm.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vll.birdmap.top

PHP:  // 手写时间戳比较
来源：http://vzr.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gja.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cib.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://noc.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rlf.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://eir.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://owg.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://dqv.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ohp.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pyz.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://onz.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pdf.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dlt.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uge.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://abi.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://alr.nanxuanxn.top

================================================================================
来源：http://deg.kuanghao11.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://khx.ivvv.top

================================================================================
来源：http://gib.yangfankeji.com

[Q01] 创建表
来源：http://fat.hnxiangtu.top

CREATE TABLE users (
来源：http://diy.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyu.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://idx.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://rbi.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nmc.bjfxy.top

);
来源：http://qpz.hcnkem.com

[Q02] 创建带外键的表
来源：http://xlt.wangshuangyany.cn

CREATE TABLE orders (
来源：http://yzk.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vjj.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://dhd.ywan-chungtsiang.top

amount DECIMAL(10, 2),
来源：http://dmp.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ddz.0kj1m.cn

);
来源：http://mtg.hfpthk.cn

[Q03] 增加列
来源：http://lhn.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sgr.shzxlz.cn

[Q04] 修改列类型
来源：http://kgv.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jjy.ybcxt.top

[Q05] 重命名列
来源：http://gqs.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bqs.feifeiyinyue.top

[Q06] 删除列
来源：http://klv.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://emx.zhiwuduotai.top

[Q07] 删除表
来源：http://pqr.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://hkn.hysaishi.cn

[Q08] 创建普通索引
来源：http://awv.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ykd.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://cqf.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bss.ctjpmb.com

[Q10] 插入单行
来源：http://rcv.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dvv.xinyue.icu

[Q11] 一次插入多行
来源：http://iff.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fae.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://cuu.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://rah.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pkc.zdbjq.cn

[Q13] 忽略重复插入
来源：http://yly.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://axw.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://ykc.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://edp.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gpk.svipenyu.cn

[Q15] 查询全部
来源：http://iic.nanxinkj.top

SELECT * FROM users;
来源：http://srs.dianchejie.cn

[Q16] 查询指定列
来源：http://yuh.yueranfly.top

SELECT id, name FROM users;
来源：http://gmu.yuxming.cn

[Q17] 条件查询
来源：http://ahi.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oxb.yj20258.top

[Q18] 模糊匹配
来源：http://csr.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://omx.vehdjk.com

[Q19] 范围查询
来源：http://wsk.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hpa.vehdjk.com

[Q20] IN 列表
来源：http://nrb.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uvl.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://mvq.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://jxv.xuanzx.com

[Q22] 排序
来源：http://ltc.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uqo.yueranfly.top

[Q23] 分页
来源：http://bzc.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dvp.jlsjyb.cn

[Q24] 去重
来源：http://oms.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://wem.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://jpe.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ecm.yj202588.top

[Q26] 计数
来源：http://hez.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://jra.jiagoushi.top

[Q27] 条件计数
来源：http://gap.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cjv.bbcook.cn

[Q28] 求和与平均
来源：http://hkb.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ioz.9152youxi.cn

[Q29] 最大最小值
来源：http://isx.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://awy.jinqigufen.top

[Q30] 分组统计
来源：http://wmj.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzl.jinqigfzy.top

[Q31] 分组后过滤
来源：http://asj.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://umj.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://muj.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bun.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://udx.jianghu66.top

[Q33] 多列分组
来源：http://bke.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tgp.chenzaomai.com

[Q34] 每组取第一条
来源：http://bvk.ivvv.top

SELECT * FROM (
来源：http://sfw.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://taj.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://hks.redwolf501.top

[Q35] 内连接
来源：http://okj.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lgu.jqgfzy.top

[Q36] 左连接
来源：http://lkl.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xfd.tian-w.cn

[Q37] 右连接
来源：http://vmc.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://txh.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://tyy.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nzq.cashguo.top

[Q39] 自连接（查上下级）
来源：http://zjx.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sdv.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iju.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pmr.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oqk.gogol.net.cn

[Q41] 多表连接
来源：http://bag.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ziq.hnxiangtu.top

JOIN users u ON u.id = o.user_id
来源：http://whp.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://kzx.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://hgf.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://ass.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://alp.tanke756.top

[Q43] 标量子查询
来源：http://mss.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://maf.316326.xyz

[Q44] IN 子查询
来源：http://oro.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://phw.yj202588.top

[Q45] EXISTS 判断存在
来源：http://jkc.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jco.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pbl.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pue.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://tvq.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zzp.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://sfd.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqb.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://paq.zhongyouzk.top

[Q49] 更新单行
来源：http://zro.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xps.nanxinkj.top

[Q50] 批量更新
来源：http://ldx.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eko.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://znw.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nnz.yvedp.cn

[Q52] 删除指定行
来源：http://icw.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://ukr.yj20258.top

[Q53] 按条件删除
来源：http://gdq.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rek.yongpay.top

[Q54] 清空表
来源：http://toy.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://tfb.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://zol.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oam.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://ppp.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tca.fehbvm.com

[Q57] 行号
来源：http://ndl.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ibt.wangdashe.top

[Q58] 累计求和
来源：http://clj.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mqv.sxryk.cn

[Q59] 分组内累计
来源：http://rhi.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jvd.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://hkx.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pgq.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ibz.hongshengwenyu.top

[Q61] 移动平均
来源：http://nay.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gmm.hywenlv.cn

[Q62] 分组占比
来源：http://ozj.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pib.ctjpmb.com

[Q63] 开启事务
来源：http://rhy.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gzw.hnxiangtu.top

[Q64] 提交事务
来源：http://vyq.haohaochexian.top

COMMIT;
来源：http://ube.c1oappe.top

[Q65] 回滚事务
来源：http://jgq.xuetiantiany.cn

ROLLBACK;
来源：http://clc.pycfn.com

[Q66] 行锁查询
来源：http://ntq.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ijs.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://dpl.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ixy.chenlongwang.top

[Q68] 保存点
来源：http://tbs.zhengqikj.top

SAVEPOINT sp1;
来源：http://dmw.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://mfd.vehdjk.com

[Q69] 查看执行计划
来源：http://jjs.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqe.fengsongda.top

[Q70] 更新统计信息
来源：http://ibp.fehbvm.com

ANALYZE TABLE users;
来源：http://hfh.vehdjk.com

[Q71] 查看建表语句
来源：http://ofb.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tts.hywenlv.cn

[Q72] 查看索引
来源：http://xtl.uphjek.com

SHOW INDEX FROM users;
来源：http://wbk.zycfv.cn

[Q73] 查看表状态
来源：http://mjh.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ypj.bjfxy.top

[Q74] 强制使用索引
来源：http://qat.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wjd.redwolf501.top

[Q75] 日期格式化
来源：http://roi.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://chg.zhaomingkeji.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zhp.sweek.top

[Q76] 按天统计
来源：http://cls.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gcu.cashguo.top

[Q77] 时间加减
来源：http://rim.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ulg.haohaochexian.top

[Q78] 当前时间
来源：http://lnm.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vww.zdqjudy.top

[Q79] 字符串拼接
来源：http://kuv.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qmu.cucudq.cn

[Q80] 字符串截取
来源：http://ofp.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rog.0kj1m.cn

[Q81] 字符串替换
来源：http://dbo.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nis.zhongyouzk.top


<!-- 参考信息 -->