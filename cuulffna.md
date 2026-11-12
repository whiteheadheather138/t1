代发 wailian999

[O06] 使用进程池
来源：http://fdo.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cie.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ycz.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://vcv.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://ywb.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hbq.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mve.hesvh.cn

Ruby: // fork 块
来源：http://gfd.tarul.cn

C#:   Parallel.For
来源：http://pdy.ywan-chungtsiang.top

================================================================================
来源：http://stq.pengpengdd.cyou

P. 常用工具函数
来源：http://zxx.jiagoushi.top

================================================================================
来源：http://xri.vehdjk.com

[P01] 生成 UUID
来源：http://sih.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://wup.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tzh.iojbl.cn

JS:   crypto.randomUUID()
来源：http://ieh.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://gse.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://nat.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://xsh.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://sij.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://tkj.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://zfv.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ecu.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tez.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://azr.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://awc.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hur.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wlz.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zdw.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://whg.tanke756.top

[P03] 生成短随机字符串
来源：http://wju.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://krq.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cbq.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpb.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klg.zhongyouzk.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kvr.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wji.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ymo.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tas.c1oappe.top

[P04] 求长度
来源：http://ygn.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vhs.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sdd.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smb.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mng.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://kpq.birdmap.top

Go:   len(arr);  len(m)
来源：http://byd.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://mqy.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oiv.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://syp.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zoh.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://htn.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jmj.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gok.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sco.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://izt.vehdjk.com

Ruby: a == b
来源：http://pqy.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iyd.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mlo.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://det.meibo888.top

PHP:  if (empty($x)) {}
来源：http://lju.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iak.daria6918.cn

TS:   if (x == null) {}
来源：http://xea.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://non.pycfn.com

Go:   if x == nil {}
来源：http://eth.zhoulong.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://usl.nanxinkj.top

C#:   if (x is null) {}
来源：http://zwf.daria6918.cn

[P07] 防抖与节流
来源：http://ixi.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://amd.chenzaomai.com

PHP:  // 手写时间戳比较
来源：http://xei.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nwa.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjl.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xfo.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zue.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hju.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xwc.sxryk.cn

[P08] 处理浮点精度问题
来源：http://gmd.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lwm.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://roa.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nno.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hmc.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ymd.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rme.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fxn.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wyq.meibo888.top

================================================================================
来源：http://uah.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://chw.chenzaomai.com

================================================================================
来源：http://kvi.jinqigufen.top

[Q01] 创建表
来源：http://kvd.316326.xyz

CREATE TABLE users (
来源：http://pap.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qye.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://cbs.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://afl.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ngp.zhengqikj.top

);
来源：http://hav.hywenlv.cn

[Q02] 创建带外键的表
来源：http://tsd.jianghu66.top

CREATE TABLE orders (
来源：http://mbr.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rkh.ydjk.org.cn

user_id INT NOT NULL,
来源：http://kqq.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://ykj.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mzw.yonumen.top

);
来源：http://bvg.zhongyouzk.top

[Q03] 增加列
来源：http://diy.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eof.jlsjyb.cn

[Q04] 修改列类型
来源：http://fml.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://prb.jianghu66.top

[Q05] 重命名列
来源：http://hcl.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://atm.ydjk.org.cn

[Q06] 删除列
来源：http://mos.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://htm.zycfv.cn

[Q07] 删除表
来源：http://kpc.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://kfh.daria6918.cn

[Q08] 创建普通索引
来源：http://bnb.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bqp.nwbrower.top

[Q09] 创建唯一索引
来源：http://nyk.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hlp.hywenlv.cn

[Q10] 插入单行
来源：http://oxz.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gkj.guowangkeji.top

[Q11] 一次插入多行
来源：http://adt.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yim.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://kzn.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dhf.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hmy.cqqwz.cn

[Q13] 忽略重复插入
来源：http://usp.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zlc.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://ozd.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vpo.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zsy.ctjpmb.com

[Q15] 查询全部
来源：http://iwr.zhoulong.xyz

SELECT * FROM users;
来源：http://bws.nanxuanxn.top

[Q16] 查询指定列
来源：http://zqe.zhixingplan.top

SELECT id, name FROM users;
来源：http://nul.cheryme.top

[Q17] 条件查询
来源：http://wvo.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cmz.tarul.cn

[Q18] 模糊匹配
来源：http://vxp.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fru.birdmap.top

[Q19] 范围查询
来源：http://jgf.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yzx.gzhubu.top

[Q20] IN 列表
来源：http://yef.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kce.zhixingplan.top

[Q21] 空值判断
来源：http://uep.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iif.xziqi.cn

[Q22] 排序
来源：http://gvg.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qdg.0kj1m.cn

[Q23] 分页
来源：http://mud.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://spv.redwolf501.top

[Q24] 去重
来源：http://siw.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://zzz.bjfxy.top

[Q25] 只取前 N 条
来源：http://btx.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mrx.yj20258.top

[Q26] 计数
来源：http://ftk.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://jvn.nanxinkj.top

[Q27] 条件计数
来源：http://uju.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ygw.smart0.xyz

[Q28] 求和与平均
来源：http://khn.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xwt.tarul.cn

[Q29] 最大最小值
来源：http://rbk.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dvb.yfazqb.com

[Q30] 分组统计
来源：http://xiv.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hud.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://mtj.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fam.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://lcj.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://thc.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hvd.pycfn.com

[Q33] 多列分组
来源：http://nxz.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://din.aizwys.cn

[Q34] 每组取第一条
来源：http://iqu.gogol.net.cn

SELECT * FROM (
来源：http://cam.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mts.jinqigufen.top

) t WHERE rn = 1;
来源：http://mqy.gotoacloud.top

[Q35] 内连接
来源：http://zss.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nov.hysaishi.cn

[Q36] 左连接
来源：http://knl.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cpt.meibo888.top

[Q37] 右连接
来源：http://wyp.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vvw.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://zdm.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://voq.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://coz.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://onl.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kyh.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://zbv.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://psk.zhoulong.xyz

[Q41] 多表连接
来源：http://efb.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://fdp.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://yos.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://dmp.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://gkf.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://rio.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jcz.yongpay.top

[Q43] 标量子查询
来源：http://naw.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jkr.vehdjk.com

[Q44] IN 子查询
来源：http://ayu.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wcf.yj20258.top

[Q45] EXISTS 判断存在
来源：http://iew.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bmq.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yvp.mhx1999.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pgj.jqgufenzy.top

[Q47] 与平均值比较
来源：http://ioy.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://myd.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://sfs.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bag.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://dmb.sweek.top

[Q49] 更新单行
来源：http://cgp.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://maa.sweek.top

[Q50] 批量更新
来源：http://dqy.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kpe.vqdsnc.cn

[Q51] 用子查询更新
来源：http://yiu.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zxh.daria6918.cn

[Q52] 删除指定行
来源：http://ume.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://ebb.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://wkl.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wcz.vehdjk.com

[Q54] 清空表
来源：http://lpf.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://fdb.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://oks.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nwx.kuanghao11.cn

[Q56] 密集排名（并列不占位）
来源：http://fou.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://new.tanke756.top

[Q57] 行号
来源：http://uqs.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fjp.jianghu66.top

[Q58] 累计求和
来源：http://vgq.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vbb.vehdjk.com

[Q59] 分组内累计
来源：http://vzz.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://grt.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://tsa.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xxl.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ugk.iojbl.cn

[Q61] 移动平均
来源：http://ner.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yjd.epnwcf.com

[Q62] 分组占比
来源：http://iym.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gwg.jqgufenzy.top

[Q63] 开启事务
来源：http://kpi.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cqq.yanxiufei.cn

[Q64] 提交事务
来源：http://taf.316326.xyz

COMMIT;
来源：http://pdf.yongpay.top

[Q65] 回滚事务
来源：http://snp.tanke756.top

ROLLBACK;
来源：http://zqm.ctjpmb.com

[Q66] 行锁查询
来源：http://hmc.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vtw.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://nhm.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rnw.vehdjk.com

[Q68] 保存点
来源：http://vnb.redwolf501.top

SAVEPOINT sp1;
来源：http://ocf.bjfxy.top

ROLLBACK TO sp1;
来源：http://umv.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://bvy.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lgu.yj20258888.top

[Q70] 更新统计信息
来源：http://owh.gzhubu.top

ANALYZE TABLE users;
来源：http://plr.jinqigfzy.top

[Q71] 查看建表语句
来源：http://ohi.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mph.snrcjt.cn

[Q72] 查看索引
来源：http://iti.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://xzg.meibo888.top

[Q73] 查看表状态
来源：http://bjr.fzhhl.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yfg.yonumen.top

[Q74] 强制使用索引
来源：http://bje.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vrp.xuanzx.com

[Q75] 日期格式化
来源：http://jwi.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bav.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qie.tianlin.xyz

[Q76] 按天统计
来源：http://smw.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vjv.tian-w.cn

[Q77] 时间加减
来源：http://hgn.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wkt.bjfxy.top

[Q78] 当前时间
来源：http://itz.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pyy.yj20258.top

[Q79] 字符串拼接
来源：http://azz.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://but.yuanzhike.top

[Q80] 字符串截取
来源：http://jur.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qsu.hysaishi.cn

[Q81] 字符串替换
来源：http://uli.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://las.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://khb.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kxq.smart0.xyz

[Q83] 大小写转换
来源：http://hpb.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hjx.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://oqi.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://irh.zhijiandao.cn

[Q85] 数值取整
来源：http://cmc.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bld.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://gfu.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wva.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://riq.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nqq.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://xvg.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fkx.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wlt.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://zdm.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vge.mhx1999.top

[Q90] 生成序号列
来源：http://vmv.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iim.wangshuangyany.cn

================================================================================
来源：http://hka.yueranfly.top

R. Bash 专题
来源：http://jdz.zhijiandao.cn

================================================================================
来源：http://ezb.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://eac.chenzaomai.com

#!/usr/bin/env bash
来源：http://fye.jianghu66.top

set -euo pipefail
来源：http://ddz.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://dbw.cucudq.cn

name="Tom"; echo "$name"
来源：http://kan.sufxvd.cn

[R03] 只读变量
来源：http://ads.gotoacloud.top


<!-- 参考信息 -->