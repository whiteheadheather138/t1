代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wsq.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bqf.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://eis.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://koz.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://ydt.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://opo.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://tzi.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://sob.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://frc.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://how.c1oappe.top

Ruby: threads.map(&:join)
来源：http://ezi.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://toz.zhongyouzk.top

[O06] 使用进程池
来源：http://edu.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wpr.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oag.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://iud.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://jwt.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nyv.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xah.xylfe.cn

Ruby: // fork 块
来源：http://rmj.zycfv.cn

C#:   Parallel.For
来源：http://ixd.yuanzhike.top

================================================================================
来源：http://moo.hnqzz.top

P. 常用工具函数
来源：http://umu.bjfxy.top

================================================================================
来源：http://fao.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://zkk.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://ugk.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eml.hcnkem.com

JS:   crypto.randomUUID()
来源：http://mjo.yfazqb.com

TS:   crypto.randomUUID()
来源：http://heu.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://enm.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://bdl.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://bbn.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://kll.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://uql.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rax.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kyv.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fxg.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ejr.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://izi.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xng.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://drl.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ket.aizwys.cn

[P03] 生成短随机字符串
来源：http://lry.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://amr.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://awm.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://knl.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rot.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sbd.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nrc.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wga.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eol.yj202588.top

[P04] 求长度
来源：http://bva.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iqw.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://erl.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://egd.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wly.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://fwr.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://jgi.guowangkeji.top

Ruby: x.length;  x.size
来源：http://tnp.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vuh.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://kju.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://kbe.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ujo.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dze.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lgf.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kix.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://lpd.xuanzx.com

Ruby: a == b
来源：http://cgk.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://unk.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eja.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xpf.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://bgr.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rif.jqgufenzy.top

TS:   if (x == null) {}
来源：http://efg.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://itl.daxiang520.top

Go:   if x == nil {}
来源：http://csv.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://npo.shuidangran.top

C#:   if (x is null) {}
来源：http://frr.cdnleiting.top

[P07] 防抖与节流
来源：http://qwy.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jdt.hammf.cn

PHP:  // 手写时间戳比较
来源：http://eye.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvz.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://usz.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pfq.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qmy.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cbs.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xju.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://jeo.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qeh.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bzi.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ogi.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aso.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rms.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lxb.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://roo.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xqm.ydjk.org.cn

================================================================================
来源：http://lkj.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://itg.ppjwa.cn

================================================================================
来源：http://feb.yj20258888.top

[Q01] 创建表
来源：http://diw.cashguo.top

CREATE TABLE users (
来源：http://ozf.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://klw.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://bit.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://etm.wangdashe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://slh.jinyuanbaomall.cn

);
来源：http://jpx.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://hlb.fzhhl.top

CREATE TABLE orders (
来源：http://iiw.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jzh.fktsv.cn

user_id INT NOT NULL,
来源：http://nni.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://xrm.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hvr.yongpay.top

);
来源：http://ufr.fengsongda.top

[Q03] 增加列
来源：http://vhx.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dek.zhixingplan.top

[Q04] 修改列类型
来源：http://cqd.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cpo.havefunace.top

[Q05] 重命名列
来源：http://ksi.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bch.redwolf501.top

[Q06] 删除列
来源：http://pvy.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://ymz.gogol.net.cn

[Q07] 删除表
来源：http://vtv.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://zqx.hesvh.cn

[Q08] 创建普通索引
来源：http://akh.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sjr.aibaodan.cn

[Q09] 创建唯一索引
来源：http://tki.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://myj.xuetiantiany.cn

[Q10] 插入单行
来源：http://nfz.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wla.yanxiufei.cn

[Q11] 一次插入多行
来源：http://xbv.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ciy.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://hxn.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://phi.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hbq.yonumen.top

[Q13] 忽略重复插入
来源：http://lqr.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wtd.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://ymp.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://acw.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://otz.ybcxt.top

[Q15] 查询全部
来源：http://okd.jianghu66.top

SELECT * FROM users;
来源：http://wan.zhixingplan.top

[Q16] 查询指定列
来源：http://gbi.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://jsa.0kj1m.cn

[Q17] 条件查询
来源：http://uga.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mxq.quarkkingdee.top

[Q18] 模糊匹配
来源：http://fbn.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jwp.pycfn.com

[Q19] 范围查询
来源：http://tba.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yrf.zdqjudy.top

[Q20] IN 列表
来源：http://xjy.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xab.fanxiaobao.xyz

[Q21] 空值判断
来源：http://lrt.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ojx.yvedp.cn

[Q22] 排序
来源：http://cip.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ihi.chenlongwang.top

[Q23] 分页
来源：http://gtl.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://paw.jianghu66.top

[Q24] 去重
来源：http://nye.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://swn.hywenlv.cn

[Q25] 只取前 N 条
来源：http://vqy.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://awh.yj20258888.top

[Q26] 计数
来源：http://jgc.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://ocw.shanyushiyangtech.top

[Q27] 条件计数
来源：http://onf.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xvi.havefunace.top

[Q28] 求和与平均
来源：http://bir.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mjz.zhengqikj.top

[Q29] 最大最小值
来源：http://axv.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fij.c1oappe.top

[Q30] 分组统计
来源：http://cnb.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qio.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://tbz.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gcm.cashguo.top

[Q32] 分组拼接字符串
来源：http://rsa.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ged.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tey.316326.xyz

[Q33] 多列分组
来源：http://ook.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bjn.epnwcf.com

[Q34] 每组取第一条
来源：http://mnt.jqgufenzy.top

SELECT * FROM (
来源：http://dbk.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ydj.yuanzhike.top

) t WHERE rn = 1;
来源：http://qyn.meibo888.top

[Q35] 内连接
来源：http://cgv.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ata.tianlin.xyz

[Q36] 左连接
来源：http://bca.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fpr.sxryk.cn

[Q37] 右连接
来源：http://trp.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rwz.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oix.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jqc.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://qwt.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bbk.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xos.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qyc.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sgt.yonumen.top

[Q41] 多表连接
来源：http://syw.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dhb.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://qcy.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://stm.cheryme.top

[Q42] 连接条件附加过滤
来源：http://jzg.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://cxj.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ckh.bjfxy.top

[Q43] 标量子查询
来源：http://rrk.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://owc.hfpthk.cn

[Q44] IN 子查询
来源：http://mdf.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lwq.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://yir.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://edr.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://imx.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://edn.fzhhl.top

[Q47] 与平均值比较
来源：http://cpi.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xzj.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://ttj.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://utf.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://tda.jlsjyb.cn

[Q49] 更新单行
来源：http://ltq.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pwh.daria6918.cn

[Q50] 批量更新
来源：http://hzu.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ilk.guowangkeji.top

[Q51] 用子查询更新
来源：http://tji.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sld.zhiwuduotai.top

[Q52] 删除指定行
来源：http://nkb.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://glz.ivvv.top

[Q53] 按条件删除
来源：http://ygn.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fcc.ivvv.top

[Q54] 清空表
来源：http://wlw.fktsv.cn

TRUNCATE TABLE logs;
来源：http://jct.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://eae.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pgk.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://nxn.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eet.yuanzhike.top

[Q57] 行号
来源：http://rgd.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fue.hnqzz.top

[Q58] 累计求和
来源：http://zly.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ajf.aizwys.cn

[Q59] 分组内累计
来源：http://phd.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mtz.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://jvf.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xci.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uhv.fzhhl.top

[Q61] 移动平均
来源：http://kdg.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ceq.nwbrower.top

[Q62] 分组占比
来源：http://jer.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uym.jiagoushi.top

[Q63] 开启事务
来源：http://djs.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jfl.yonumen.top

[Q64] 提交事务
来源：http://cgt.chenjidiqi.icu

COMMIT;
来源：http://gnq.xuanzx.com

[Q65] 回滚事务
来源：http://eno.vqdsnc.cn

ROLLBACK;
来源：http://fyj.zycfv.cn

[Q66] 行锁查询
来源：http://nna.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://saz.hfpthk.cn

[Q67] 设置隔离级别
来源：http://fwt.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iih.yvedp.cn

[Q68] 保存点
来源：http://qix.redwolf501.top

SAVEPOINT sp1;
来源：http://efg.haohaochexian.top

ROLLBACK TO sp1;
来源：http://ani.xylfe.cn

[Q69] 查看执行计划
来源：http://zna.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dmh.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://fqd.xziqi.cn

ANALYZE TABLE users;
来源：http://wzp.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://nnt.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kku.shzxlz.cn

[Q72] 查看索引
来源：http://bix.guannengcc.top

SHOW INDEX FROM users;
来源：http://aif.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://upe.vehdjk.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jgk.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://pbv.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://osq.bjfxy.top

[Q75] 日期格式化
来源：http://ees.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://adx.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hld.sufxvd.cn

[Q76] 按天统计
来源：http://nlu.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gdj.haohaochexian.top

[Q77] 时间加减
来源：http://bob.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ltg.ppjwa.cn

[Q78] 当前时间
来源：http://sei.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jgz.ydzc1.top

[Q79] 字符串拼接
来源：http://rka.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zze.cdnleiting.top

[Q80] 字符串截取
来源：http://xgc.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mgj.cucudq.cn

[Q81] 字符串替换
来源：http://qly.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://egr.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://hin.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fbd.jqgfzy.top

[Q83] 大小写转换
来源：http://yuk.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fqb.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://gco.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://wrh.hywenlv.cn

[Q85] 数值取整
来源：http://geu.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://toq.cheryme.top

[Q86] 读取 JSON 字段
来源：http://wpg.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zzc.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://qem.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lzy.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://jls.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rrn.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zay.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://igz.zhixingplan.top


<!-- 参考信息 -->