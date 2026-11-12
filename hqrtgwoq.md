代发 wailian999

TS:   crypto.randomUUID()
来源：http://cat.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://cpk.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://tya.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://orm.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://mtc.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://xmq.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hxy.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mnt.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fod.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rlt.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qdc.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lbe.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xhn.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cok.nanxinkj.top

[P03] 生成短随机字符串
来源：http://cjz.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nzu.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://unt.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chx.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dst.ppjwa.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rvb.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gee.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yni.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ree.vehdjk.com

[P04] 求长度
来源：http://ssm.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://han.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyl.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kke.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ayd.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://coa.zycfv.cn

Go:   len(arr);  len(m)
来源：http://cnh.zhengqikj.top

Ruby: x.length;  x.size
来源：http://wau.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jre.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://etg.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mex.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nvt.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xkc.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://szf.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fca.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://sns.yonumen.top

Ruby: a == b
来源：http://wns.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gjm.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zuu.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qvg.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://bsd.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xio.hfpthk.cn

TS:   if (x == null) {}
来源：http://lmb.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vxw.aizwys.cn

Go:   if x == nil {}
来源：http://ccl.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jsa.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://bdn.zhoulong.xyz

[P07] 防抖与节流
来源：http://ags.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://shq.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://ftm.hnxiangtu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://opm.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdx.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xld.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zga.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jjg.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ogm.cashguo.top

[P08] 处理浮点精度问题
来源：http://jac.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tyz.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fhv.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pnj.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ctt.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tep.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hqo.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jqj.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hen.aibaodan.cn

================================================================================
来源：http://trb.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://olv.aibaodan.cn

================================================================================
来源：http://bob.shzxlz.cn

[Q01] 创建表
来源：http://iek.shuidangran.top

CREATE TABLE users (
来源：http://ctv.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsl.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://fwl.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://drf.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pfo.vehdjk.com

);
来源：http://wbb.redwolf501.top

[Q02] 创建带外键的表
来源：http://qpx.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://ctp.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kqm.hfpthk.cn

user_id INT NOT NULL,
来源：http://fsl.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://fvx.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sfl.sweek.top

);
来源：http://fdm.yueranfly.top

[Q03] 增加列
来源：http://hal.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iks.hongshengwenyu.top

[Q04] 修改列类型
来源：http://oyw.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dix.jinghuilouyu.cn

[Q05] 重命名列
来源：http://tog.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gfi.aibaodan.cn

[Q06] 删除列
来源：http://hat.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://eob.zdbjq.cn

[Q07] 删除表
来源：http://xzy.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://eoj.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://oct.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gob.zycfv.cn

[Q09] 创建唯一索引
来源：http://vkm.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://loz.havefunace.top

[Q10] 插入单行
来源：http://ddg.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mfz.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://ybg.haohaochexian.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pbv.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://vwi.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://guw.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cct.dianchejie.cn

[Q13] 忽略重复插入
来源：http://pvg.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jha.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://mag.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://onu.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dym.ctjpmb.com

[Q15] 查询全部
来源：http://oxx.fengsongda.top

SELECT * FROM users;
来源：http://tnm.ehwqpu.com

[Q16] 查询指定列
来源：http://qum.yj202588.top

SELECT id, name FROM users;
来源：http://kiz.hammf.cn

[Q17] 条件查询
来源：http://phq.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lxh.316326.xyz

[Q18] 模糊匹配
来源：http://tnr.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dbz.cucudq.cn

[Q19] 范围查询
来源：http://piv.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://epv.xuanzx.com

[Q20] IN 列表
来源：http://oxe.hnqzz.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qkb.zdqjudy.top

[Q21] 空值判断
来源：http://rpa.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rxw.jyoumei.cn

[Q22] 排序
来源：http://yfi.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kvp.ctjpmb.com

[Q23] 分页
来源：http://fre.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://osk.quarkkingdee.top

[Q24] 去重
来源：http://yeu.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://ymo.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://iog.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kym.yj20258888.top

[Q26] 计数
来源：http://qaw.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://qrx.havefunace.top

[Q27] 条件计数
来源：http://tmo.cheryme.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qrv.52xcode.cn

[Q28] 求和与平均
来源：http://wpd.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rcd.zhengqikj.top

[Q29] 最大最小值
来源：http://evx.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eop.hywenlv.cn

[Q30] 分组统计
来源：http://ofv.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ikf.hnqzz.top

[Q31] 分组后过滤
来源：http://ydx.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://svc.hesvh.cn

[Q32] 分组拼接字符串
来源：http://yiw.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fgl.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iko.guannengcc.top

[Q33] 多列分组
来源：http://fgf.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uee.svipenyu.cn

[Q34] 每组取第一条
来源：http://xgk.yonumen.top

SELECT * FROM (
来源：http://juc.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jhq.yongpay.top

) t WHERE rn = 1;
来源：http://zsa.nanxinkj.top

[Q35] 内连接
来源：http://zqu.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qmq.cucudq.cn

[Q36] 左连接
来源：http://jxp.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bkd.nanxuanxn.top

[Q37] 右连接
来源：http://whr.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uok.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://uft.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qvb.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://mqk.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jxo.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://thv.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yxy.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gas.wangdashe.top

[Q41] 多表连接
来源：http://ivr.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://mxc.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://xdc.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://njj.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://bxx.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://czr.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fml.havefunace.top

[Q43] 标量子查询
来源：http://bzd.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ktc.316326.xyz

[Q44] IN 子查询
来源：http://zvo.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vhe.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://uyx.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvm.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://grd.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mdb.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://ttu.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://exv.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://zdx.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://esd.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://now.pengpengdd.cyou

[Q49] 更新单行
来源：http://lkg.vehdjk.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ijc.vehdjk.com

[Q50] 批量更新
来源：http://bhi.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tcs.ivvv.top

[Q51] 用子查询更新
来源：http://omu.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ilh.ppjwa.cn

[Q52] 删除指定行
来源：http://ras.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://cmq.yuanzhike.top

[Q53] 按条件删除
来源：http://pfs.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tmj.hfpthk.cn

[Q54] 清空表
来源：http://vrh.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://ndg.gzhubu.top

[Q55] 排名（并列占位）
来源：http://nzv.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uut.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://dkn.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tgo.daxiang520.top

[Q57] 行号
来源：http://pkt.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ruc.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://jbc.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dcq.ydzc1.top

[Q59] 分组内累计
来源：http://tdf.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kah.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://bou.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yrc.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zxf.jinqigufen.top

[Q61] 移动平均
来源：http://teb.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pyz.0kj1m.cn

[Q62] 分组占比
来源：http://bnd.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tpj.redwolf501.top

[Q63] 开启事务
来源：http://hon.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://dtr.chenlongwang.top

[Q64] 提交事务
来源：http://nzv.nwbrower.top

COMMIT;
来源：http://ouq.gogol.net.cn

[Q65] 回滚事务
来源：http://bmo.shangyingyoupin.top

ROLLBACK;
来源：http://kbp.chenzaomai.com

[Q66] 行锁查询
来源：http://pqy.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://opc.tanke756.top

[Q67] 设置隔离级别
来源：http://blr.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lxe.xuanzx.com

[Q68] 保存点
来源：http://wtz.dianchejie.cn

SAVEPOINT sp1;
来源：http://kze.hcnkem.com

ROLLBACK TO sp1;
来源：http://jgq.kuanghao11.cn

[Q69] 查看执行计划
来源：http://ckt.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cyy.guannengcc.top

[Q70] 更新统计信息
来源：http://ugr.yongpay.top

ANALYZE TABLE users;
来源：http://vbz.yangfankeji.com

[Q71] 查看建表语句
来源：http://oqn.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jtk.tian-w.cn

[Q72] 查看索引
来源：http://mho.hammf.cn

SHOW INDEX FROM users;
来源：http://yjd.sysykeji.top

[Q73] 查看表状态
来源：http://gjh.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bns.cqqwz.cn

[Q74] 强制使用索引
来源：http://ssv.yuanzhike.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ntv.gzhubu.top

[Q75] 日期格式化
来源：http://jmg.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dda.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lak.wangshuangyany.cn

[Q76] 按天统计
来源：http://yew.xuanzx.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iex.fanxiaobao.xyz

[Q77] 时间加减
来源：http://tnh.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ulq.fzhhl.top

[Q78] 当前时间
来源：http://pbf.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zmx.fengsongda.top

[Q79] 字符串拼接
来源：http://bpj.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bxr.gogol.net.cn

[Q80] 字符串截取
来源：http://kkb.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mjk.jianghu66.top

[Q81] 字符串替换
来源：http://uud.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tou.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://itj.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://liq.vqdsnc.cn

[Q83] 大小写转换
来源：http://ppe.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://epk.hammf.cn

[Q84] 去除首尾空格
来源：http://nsr.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://abq.hfpthk.cn

[Q85] 数值取整
来源：http://bik.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nhm.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://llk.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dud.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://vfm.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qzg.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://fvr.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vcz.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pfp.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://ztd.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://djd.havefunace.top

[Q90] 生成序号列
来源：http://wkz.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ihf.jinqigfzy.top

================================================================================
来源：http://hlj.andypj.xyz

R. Bash 专题
来源：http://mfa.dianchejie.cn

================================================================================
来源：http://hyz.ybcxt.top

[R01] shebang 与严格模式
来源：http://oza.hesvh.cn

#!/usr/bin/env bash
来源：http://egt.xylfe.cn

set -euo pipefail
来源：http://oyw.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://xjt.tian-w.cn

name="Tom"; echo "$name"
来源：http://yzp.fehbvm.com

[R03] 只读变量
来源：http://cdu.xziqi.cn

readonly PI=3.14
来源：http://xaw.hnqzz.top

[R04] 位置参数
来源：http://wab.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ais.ehwqpu.com

[R05] 参数默认值
来源：http://ssd.gaohongyu789.top

name="${1:-default}"
来源：http://fdl.hfpthk.cn

[R06] 判断命令是否存在
来源：http://ycd.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://exz.birdmap.top

[R07] if 判断文件
来源：http://ehy.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wid.zdqjudy.top

[R08] 数值比较
来源：http://gzm.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xpw.yvedp.cn

[R09] 字符串比较
来源：http://zik.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hda.guannengcc.top

[R10] 正则匹配
来源：http://xmy.zhongyouzk.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xjc.hesvh.cn

[R11] case 多分支
来源：http://zmj.jinqigfzy.top


<!-- 参考信息 -->