代发 wailian999

TS:   // child_process / cluster 模块
来源：http://zxs.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ycs.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://deq.snrcjt.cn

Ruby: // fork 块
来源：http://yzt.gaohongyu789.top

C#:   Parallel.For
来源：http://ikw.fengsongda.top

================================================================================
来源：http://scn.smart0.xyz

P. 常用工具函数
来源：http://rwl.wangdashe.top

================================================================================
来源：http://alj.aizwys.cn

[P01] 生成 UUID
来源：http://jui.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://jtp.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ean.hammf.cn

JS:   crypto.randomUUID()
来源：http://rmd.epnwcf.com

TS:   crypto.randomUUID()
来源：http://irx.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://mph.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://pnv.meibo888.top

Ruby: SecureRandom.uuid
来源：http://wfx.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://jbd.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://grr.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eqj.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://amd.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://voc.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tse.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nbl.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qjz.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://adl.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cdd.tarul.cn

[P03] 生成短随机字符串
来源：http://wap.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ros.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rhv.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xum.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsb.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rni.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zjt.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://myr.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iav.jinqigfzy.top

[P04] 求长度
来源：http://del.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rov.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zfj.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bwg.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ipc.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://bpa.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://acs.cashguo.top

Ruby: x.length;  x.size
来源：http://vem.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rle.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://sce.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yfw.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tzc.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dds.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cnx.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vgu.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ecd.yfazqb.com

Ruby: a == b
来源：http://xwb.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uyt.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rjv.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ene.cashguo.top

PHP:  if (empty($x)) {}
来源：http://tgg.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://arb.jlsjyb.cn

TS:   if (x == null) {}
来源：http://ncu.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ywr.zhixingplan.top

Go:   if x == nil {}
来源：http://iau.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iid.dashuyun.cn

C#:   if (x is null) {}
来源：http://eet.xinyue.icu

[P07] 防抖与节流
来源：http://ofa.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://prw.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://stm.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybu.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujk.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vpd.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ebt.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://knm.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://alh.cucudq.cn

[P08] 处理浮点精度问题
来源：http://loj.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jqp.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dei.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dpq.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gbu.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hcm.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hou.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rtx.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://alp.gzhubu.top

================================================================================
来源：http://wdm.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pey.xylfe.cn

================================================================================
来源：http://ssj.iojbl.cn

[Q01] 创建表
来源：http://sai.yueranfly.top

CREATE TABLE users (
来源：http://gca.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gzf.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://xwb.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://whr.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wvd.shanyushiyangkeji.top

);
来源：http://zqf.havefunace.top

[Q02] 创建带外键的表
来源：http://ipr.yuxming.cn

CREATE TABLE orders (
来源：http://tqt.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://thb.jinqigfzy.top

user_id INT NOT NULL,
来源：http://tnc.xuanzx.com

amount DECIMAL(10, 2),
来源：http://dmt.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xap.fengsongda.top

);
来源：http://zip.zhiwuduotai.top

[Q03] 增加列
来源：http://sfa.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://igy.wangdashe.top

[Q04] 修改列类型
来源：http://lif.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wes.wangshuangyany.cn

[Q05] 重命名列
来源：http://yod.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jtl.nanxuanxn.top

[Q06] 删除列
来源：http://vdr.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zva.guannengcc.top

[Q07] 删除表
来源：http://ztq.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://kmh.nanxuanxn.top

[Q08] 创建普通索引
来源：http://thk.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gvc.chenlongwang.top

[Q09] 创建唯一索引
来源：http://gzp.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iod.c1oappe.top

[Q10] 插入单行
来源：http://kri.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tzs.guannengcc.top

[Q11] 一次插入多行
来源：http://etx.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nhv.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://gis.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uak.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://szc.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://vfd.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qbh.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://aim.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vge.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://npz.zhoulong.xyz

[Q15] 查询全部
来源：http://jlo.yj20258.top

SELECT * FROM users;
来源：http://ltz.xuanzx.com

[Q16] 查询指定列
来源：http://zks.shuidangran.top

SELECT id, name FROM users;
来源：http://mte.ydzc1.top

[Q17] 条件查询
来源：http://xap.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fey.aibaodan.cn

[Q18] 模糊匹配
来源：http://cqz.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yrz.hysaishi.cn

[Q19] 范围查询
来源：http://hwd.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://urb.fanxiaobao.xyz

[Q20] IN 列表
来源：http://lml.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ieg.gogol.net.cn

[Q21] 空值判断
来源：http://jfd.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://lnw.zhaomingkeji.xyz

[Q22] 排序
来源：http://kxd.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dwv.ivvv.top

[Q23] 分页
来源：http://hyv.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://alc.fktsv.cn

[Q24] 去重
来源：http://jfs.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://cst.shuidangran.top

[Q25] 只取前 N 条
来源：http://rby.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xjn.zhoulong.xyz

[Q26] 计数
来源：http://xbi.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://lit.cdnleiting.top

[Q27] 条件计数
来源：http://lul.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lgj.hammf.cn

[Q28] 求和与平均
来源：http://ypt.andypj.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mxt.sjlbkw.cn

[Q29] 最大最小值
来源：http://lxy.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hmg.smart0.xyz

[Q30] 分组统计
来源：http://vmd.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pzt.jinqigfzy.top

[Q31] 分组后过滤
来源：http://tkc.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gxf.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://oen.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lrp.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xns.shuidangran.top

[Q33] 多列分组
来源：http://jfl.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://thr.fzhhl.top

[Q34] 每组取第一条
来源：http://emr.birdmap.top

SELECT * FROM (
来源：http://ixt.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pso.tian-w.cn

) t WHERE rn = 1;
来源：http://dnu.fehbvm.com

[Q35] 内连接
来源：http://qaf.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wpd.9152youxi.cn

[Q36] 左连接
来源：http://dxv.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://heo.meibo888.top

[Q37] 右连接
来源：http://qqi.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hjv.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://cfx.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jkr.tanke756.top

[Q39] 自连接（查上下级）
来源：http://hsm.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jin.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xpu.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jvs.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gsh.chenzaomai.com

[Q41] 多表连接
来源：http://mww.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://atr.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://gow.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://vjk.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://dhr.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://jtk.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nis.shzxlz.cn

[Q43] 标量子查询
来源：http://hii.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hqk.meibo888.top

[Q44] IN 子查询
来源：http://cvd.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xxo.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://qzd.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iiw.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://myi.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zbn.fktsv.cn

[Q47] 与平均值比较
来源：http://rmi.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uit.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://cmj.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pki.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://kyv.jinqigufen.top

[Q49] 更新单行
来源：http://srx.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://usc.gzhubu.top

[Q50] 批量更新
来源：http://ifs.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://igl.dianchejie.cn

[Q51] 用子查询更新
来源：http://hds.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://azx.zhijiandao.cn

[Q52] 删除指定行
来源：http://uuv.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://awr.gotoacloud.top

[Q53] 按条件删除
来源：http://xdn.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://daq.zycfv.cn

[Q54] 清空表
来源：http://atw.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://lni.andypj.xyz

[Q55] 排名（并列占位）
来源：http://gcg.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vip.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://igs.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pxp.jqgufenzy.top

[Q57] 行号
来源：http://mou.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xun.cucudq.cn

[Q58] 累计求和
来源：http://kjc.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sus.feifeiyinyue.top

[Q59] 分组内累计
来源：http://qis.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nkk.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://spb.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jmi.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jbg.snrcjt.cn

[Q61] 移动平均
来源：http://ubt.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ert.jqgfzy.top

[Q62] 分组占比
来源：http://rjs.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://koe.hfpthk.cn

[Q63] 开启事务
来源：http://kux.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mla.jinghuilouyu.cn

[Q64] 提交事务
来源：http://qmt.jqgufenzy.top

COMMIT;
来源：http://ztx.yj20258888.top

[Q65] 回滚事务
来源：http://mog.uphjek.com

ROLLBACK;
来源：http://owu.nanxuanxn.top

[Q66] 行锁查询
来源：http://keq.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tnw.nanxinkj.top

[Q67] 设置隔离级别
来源：http://ftr.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdf.vqdsnc.cn

[Q68] 保存点
来源：http://amv.kuanghao11.cn

SAVEPOINT sp1;
来源：http://scv.mhx1999.top

ROLLBACK TO sp1;
来源：http://lhp.yj20258.top

[Q69] 查看执行计划
来源：http://ssb.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sye.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://iuc.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://zvn.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://mkg.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vzm.xylfe.cn

[Q72] 查看索引
来源：http://rzy.ppjwa.cn

SHOW INDEX FROM users;
来源：http://soy.sweek.top

[Q73] 查看表状态
来源：http://oxw.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bkv.xuanzx.com

[Q74] 强制使用索引
来源：http://vlg.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gdu.yanxiufei.cn

[Q75] 日期格式化
来源：http://bkj.uphjek.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ptr.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tmx.bjfxy.top

[Q76] 按天统计
来源：http://vtq.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dqv.epnwcf.com

[Q77] 时间加减
来源：http://gex.chenlongwang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zsl.hnxiangtu.top

[Q78] 当前时间
来源：http://nay.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uah.jlsjyb.cn

[Q79] 字符串拼接
来源：http://plj.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rdm.yueranfly.top

[Q80] 字符串截取
来源：http://lmz.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://koj.yfazqb.com

[Q81] 字符串替换
来源：http://nna.tarul.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rec.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://ram.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lle.cheryme.top

[Q83] 大小写转换
来源：http://pgy.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://swx.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://vev.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://hhl.chenzaomai.com

[Q85] 数值取整
来源：http://rqi.cdnleiting.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uee.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://qgs.jqgufenzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://igq.yongpay.top

[Q87] JSON 字段做条件
来源：http://ccx.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kbs.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://cts.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://myh.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ugj.haohaochexian.top

[Q89] 判断表是否存在
来源：http://ael.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oqh.guowangkeji.top

[Q90] 生成序号列
来源：http://zzn.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mzt.bbcook.cn

================================================================================
来源：http://zmh.haohaochexian.top

R. Bash 专题
来源：http://ilz.kuanghao11.cn

================================================================================
来源：http://pvj.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://qta.zhongyouzk.top

#!/usr/bin/env bash
来源：http://pvc.shzxlz.cn

set -euo pipefail
来源：http://xaa.gogol.net.cn

[R02] 变量赋值与使用
来源：http://ebh.zhixingplan.top

name="Tom"; echo "$name"
来源：http://xsz.xuanzx.com

[R03] 只读变量
来源：http://pzn.yj20258888.top

readonly PI=3.14
来源：http://cgc.jiagoushi.top

[R04] 位置参数
来源：http://lyi.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://chc.nanxinkj.top

[R05] 参数默认值
来源：http://ivm.yongpay.top


<!-- 参考信息 -->