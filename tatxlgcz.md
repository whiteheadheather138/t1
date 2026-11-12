代发 wailian999

C#:   Parallel.For
来源：http://ial.shanyushiyangkeji.top

================================================================================
来源：http://rxk.quarkkingdee.top

P. 常用工具函数
来源：http://yee.zhengqikj.top

================================================================================
来源：http://afx.fktsv.cn

[P01] 生成 UUID
来源：http://kna.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://oki.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fzl.hesvh.cn

JS:   crypto.randomUUID()
来源：http://ldl.hesvh.cn

TS:   crypto.randomUUID()
来源：http://ntv.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://mla.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://hwf.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://evg.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://ziq.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://gqh.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hak.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xde.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gjj.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mzg.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qcf.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vvh.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pta.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hfb.yueranfly.top

[P03] 生成短随机字符串
来源：http://eur.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fmy.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ikq.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgb.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nxp.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aew.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jus.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hua.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kzn.hcnkem.com

[P04] 求长度
来源：http://qsp.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dxo.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vzl.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzt.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hhd.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://sly.xziqi.cn

Go:   len(arr);  len(m)
来源：http://nvp.yongpay.top

Ruby: x.length;  x.size
来源：http://glu.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pji.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://pmt.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hxp.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gry.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://que.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nyl.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lqy.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://rsr.yueranfly.top

Ruby: a == b
来源：http://osg.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dez.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vlw.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gcl.havefunace.top

PHP:  if (empty($x)) {}
来源：http://vom.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://reo.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://yyt.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ktu.zycfv.cn

Go:   if x == nil {}
来源：http://zot.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://njg.fehbvm.com

C#:   if (x is null) {}
来源：http://xwz.jinqigfzy.top

[P07] 防抖与节流
来源：http://hpr.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vyf.tanke756.top

PHP:  // 手写时间戳比较
来源：http://tuv.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msz.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yef.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://was.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://msj.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yez.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kad.fengsongda.top

[P08] 处理浮点精度问题
来源：http://nxt.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iol.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fvd.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qxw.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gol.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ajy.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qry.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://goi.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lmd.zhengqikj.top

================================================================================
来源：http://ieg.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uow.ivvv.top

================================================================================
来源：http://wle.cqqwz.cn

[Q01] 创建表
来源：http://sdz.jiagoushi.top

CREATE TABLE users (
来源：http://kxp.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://axx.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://eoi.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://wpf.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ddh.shuidangran.top

);
来源：http://mag.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://uai.hcnkem.com

CREATE TABLE orders (
来源：http://lcd.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uik.cdnleiting.top

user_id INT NOT NULL,
来源：http://ltb.yj20258888.top

amount DECIMAL(10, 2),
来源：http://xps.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yui.hcnkem.com

);
来源：http://ett.quarkkingdee.top

[Q03] 增加列
来源：http://mrh.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pvt.jiagoushi.top

[Q04] 修改列类型
来源：http://xcy.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bpg.fzhhl.top

[Q05] 重命名列
来源：http://bvd.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qfg.wangdashe.top

[Q06] 删除列
来源：http://cwo.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sjr.sweek.top

[Q07] 删除表
来源：http://pwm.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://siz.redwolf501.top

[Q08] 创建普通索引
来源：http://tno.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zqf.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://efm.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yrg.fzhhl.top

[Q10] 插入单行
来源：http://pvi.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ugv.andypj.xyz

[Q11] 一次插入多行
来源：http://xfr.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bob.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://swl.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://iwe.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ruy.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://aat.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gcj.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://dcw.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cjc.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qwb.hammf.cn

[Q15] 查询全部
来源：http://kyd.nanxinkj.top

SELECT * FROM users;
来源：http://fii.zhixingplan.top

[Q16] 查询指定列
来源：http://ykb.bjfxy.top

SELECT id, name FROM users;
来源：http://nts.jqgfzy.top

[Q17] 条件查询
来源：http://xov.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dzf.hfpthk.cn

[Q18] 模糊匹配
来源：http://jdx.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pjm.snrcjt.cn

[Q19] 范围查询
来源：http://azc.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://csd.hcnkem.com

[Q20] IN 列表
来源：http://ogw.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zhh.chenjidiqi.icu

[Q21] 空值判断
来源：http://upm.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://vdb.ivvv.top

[Q22] 排序
来源：http://dkr.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jfy.sweek.top

[Q23] 分页
来源：http://vnt.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pct.ydzc1.top

[Q24] 去重
来源：http://hsk.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://hze.jyoumei.cn

[Q25] 只取前 N 条
来源：http://plt.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bwn.cucudq.cn

[Q26] 计数
来源：http://yhe.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://fum.cheryme.top

[Q27] 条件计数
来源：http://ipy.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fru.yueranfly.top

[Q28] 求和与平均
来源：http://gba.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ous.tarul.cn

[Q29] 最大最小值
来源：http://xqw.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kxw.fehbvm.com

[Q30] 分组统计
来源：http://xxw.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rff.sufxvd.cn

[Q31] 分组后过滤
来源：http://ees.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gpg.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://fji.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bxy.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fks.jlsjyb.cn

[Q33] 多列分组
来源：http://evl.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wkk.zhijiandao.cn

[Q34] 每组取第一条
来源：http://ave.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://fsv.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gvj.xziqi.cn

) t WHERE rn = 1;
来源：http://gzo.gotoacloud.top

[Q35] 内连接
来源：http://rqp.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tut.uphjek.com

[Q36] 左连接
来源：http://kdr.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fjs.yongpay.top

[Q37] 右连接
来源：http://kji.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zlk.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://yrw.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sxg.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://olb.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://imy.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kii.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iwc.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xcp.shzxlz.cn

[Q41] 多表连接
来源：http://hbi.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://foz.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://oxc.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://sdk.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://qei.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://xao.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ace.yuanzhike.top

[Q43] 标量子查询
来源：http://cgu.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://emt.zhoulong.xyz

[Q44] IN 子查询
来源：http://wro.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rlz.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://ksl.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ulf.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://llk.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xlx.dashuyun.cn

[Q47] 与平均值比较
来源：http://qts.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://keq.havefunace.top

[Q48] CTE 公用表表达式
来源：http://jtm.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eie.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://nkd.hfpthk.cn

[Q49] 更新单行
来源：http://lpq.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cbw.hfpthk.cn

[Q50] 批量更新
来源：http://ens.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tkn.jianghu66.top

[Q51] 用子查询更新
来源：http://lti.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vsw.jinqigufen.top

[Q52] 删除指定行
来源：http://voi.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://jwd.gzhubu.top

[Q53] 按条件删除
来源：http://dqv.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ntl.smart0.xyz

[Q54] 清空表
来源：http://qeo.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://mbk.xylfe.cn

[Q55] 排名（并列占位）
来源：http://lbe.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://izp.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://rjd.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pnr.yonumen.top

[Q57] 行号
来源：http://zyw.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vnd.jianghu66.top

[Q58] 累计求和
来源：http://jsk.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://apj.pengpengdd.cyou

[Q59] 分组内累计
来源：http://ouc.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://byc.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://pdy.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwd.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhm.xziqi.cn

[Q61] 移动平均
来源：http://dla.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tqj.fzhhl.top

[Q62] 分组占比
来源：http://deo.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wti.bbcook.cn

[Q63] 开启事务
来源：http://pjc.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://etz.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://syg.tarul.cn

COMMIT;
来源：http://rqz.gaohongyu789.top

[Q65] 回滚事务
来源：http://out.zhengqikj.top

ROLLBACK;
来源：http://bmg.316326.xyz

[Q66] 行锁查询
来源：http://blj.uphjek.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yus.zhixingplan.top

[Q67] 设置隔离级别
来源：http://izy.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lrs.wangdashe.top

[Q68] 保存点
来源：http://ods.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://wul.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://eeg.shanyushiyangtech.top

[Q69] 查看执行计划
来源：http://xwj.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ifx.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://wlk.c1oappe.top

ANALYZE TABLE users;
来源：http://xnn.andypj.xyz

[Q71] 查看建表语句
来源：http://gtm.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pwg.hnqzz.top

[Q72] 查看索引
来源：http://dxd.jinqigufen.top

SHOW INDEX FROM users;
来源：http://brb.zdbjq.cn

[Q73] 查看表状态
来源：http://wjv.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qae.epnwcf.com

[Q74] 强制使用索引
来源：http://jsu.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gra.tarul.cn

[Q75] 日期格式化
来源：http://mbg.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zsv.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://shq.jinqigufen.top

[Q76] 按天统计
来源：http://itk.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pfg.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://lck.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ygc.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://dam.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bln.dashuyun.cn

[Q79] 字符串拼接
来源：http://jsi.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ijw.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://ipt.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://byj.ivvv.top

[Q81] 字符串替换
来源：http://rds.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fsc.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://udo.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cnu.shzxlz.cn

[Q83] 大小写转换
来源：http://yyc.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ayc.dianchejie.cn

[Q84] 去除首尾空格
来源：http://row.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://lrs.jqgufenzy.top

[Q85] 数值取整
来源：http://agy.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vkv.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://rgn.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xez.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://wyk.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iwd.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://hdw.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ixz.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zna.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://ehq.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dut.haohaochexian.top

[Q90] 生成序号列
来源：http://ghx.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fvq.shanyushiyangtech.top

================================================================================
来源：http://dsu.svipenyu.cn

R. Bash 专题
来源：http://ojr.gaohongyu789.top

================================================================================
来源：http://kuo.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://wfw.aibaodan.cn

#!/usr/bin/env bash
来源：http://wmx.nanxinkj.top

set -euo pipefail
来源：http://wvy.uphjek.com

[R02] 变量赋值与使用
来源：http://joz.daria6918.cn

name="Tom"; echo "$name"
来源：http://fhy.ydzc1.top

[R03] 只读变量
来源：http://mma.ctjpmb.com

readonly PI=3.14
来源：http://cwg.sjlbkw.cn

[R04] 位置参数
来源：http://qlf.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hnn.mhx1999.top

[R05] 参数默认值
来源：http://qpu.pengpengdd.cyou

name="${1:-default}"
来源：http://dly.yueranfly.top

[R06] 判断命令是否存在
来源：http://gyy.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iqq.haohaochexian.top

[R07] if 判断文件
来源：http://dki.xuanzx.com


<!-- 参考信息 -->