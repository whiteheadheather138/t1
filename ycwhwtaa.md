代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://kgi.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://puu.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://snl.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://yuk.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eit.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhe.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bhh.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xfr.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://drh.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iwb.ybcxt.top

[P03] 生成短随机字符串
来源：http://hmb.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fuu.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rum.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sen.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsi.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nag.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yud.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uuu.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rjs.sufxvd.cn

[P04] 求长度
来源：http://igz.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wof.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rqr.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uec.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ull.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://vdy.fehbvm.com

Go:   len(arr);  len(m)
来源：http://cbd.aizwys.cn

Ruby: x.length;  x.size
来源：http://npq.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wtg.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://lvk.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ihi.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ylh.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sys.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sdw.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fkk.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://yip.vehdjk.com

Ruby: a == b
来源：http://jtf.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vac.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://day.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xdc.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://smw.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ars.mhx1999.top

TS:   if (x == null) {}
来源：http://foq.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yff.yj20258888.top

Go:   if x == nil {}
来源：http://blx.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cpc.svipenyu.cn

C#:   if (x is null) {}
来源：http://pgl.havefunace.top

[P07] 防抖与节流
来源：http://lha.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://awj.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://kzx.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eln.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://adf.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://koh.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ngo.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lgk.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ysv.ydzc1.top

[P08] 处理浮点精度问题
来源：http://yrf.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sns.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hlo.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ven.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qvw.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gvz.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ocz.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rre.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hym.yongpay.top

================================================================================
来源：http://zuu.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://loj.yuanzhike.top

================================================================================
来源：http://akx.xinyue.icu

[Q01] 创建表
来源：http://fhy.hesvh.cn

CREATE TABLE users (
来源：http://nzm.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pja.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://gnm.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://txf.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://orh.yanxiufei.cn

);
来源：http://fkp.sysykeji.top

[Q02] 创建带外键的表
来源：http://ciu.cheryme.top

CREATE TABLE orders (
来源：http://hvn.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cft.dianchejie.cn

user_id INT NOT NULL,
来源：http://mfy.vehdjk.com

amount DECIMAL(10, 2),
来源：http://rqy.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wpl.bbcook.cn

);
来源：http://oab.dashuyun.cn

[Q03] 增加列
来源：http://dcc.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rro.zhoulong.xyz

[Q04] 修改列类型
来源：http://goh.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vtk.hammf.cn

[Q05] 重命名列
来源：http://xnl.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pbx.zdbjq.cn

[Q06] 删除列
来源：http://yws.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://xqr.ppjwa.cn

[Q07] 删除表
来源：http://igo.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://eib.cashguo.top

[Q08] 创建普通索引
来源：http://piz.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yxi.xinyue.icu

[Q09] 创建唯一索引
来源：http://owp.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wxa.xinyue.icu

[Q10] 插入单行
来源：http://twc.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tla.zhoulong.xyz

[Q11] 一次插入多行
来源：http://avn.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rau.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://ogv.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://ypq.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ssh.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://dth.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://psc.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://hhs.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vrk.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jwf.cdnleiting.top

[Q15] 查询全部
来源：http://gia.vehdjk.com

SELECT * FROM users;
来源：http://lhi.sweek.top

[Q16] 查询指定列
来源：http://hky.zycfv.cn

SELECT id, name FROM users;
来源：http://xqq.hongshengwenyu.top

[Q17] 条件查询
来源：http://ims.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uur.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://wqq.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://odm.gogol.net.cn

[Q19] 范围查询
来源：http://bbm.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gfn.daria6918.cn

[Q20] IN 列表
来源：http://gtk.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mgl.ybcxt.top

[Q21] 空值判断
来源：http://ijs.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yjt.zhoulong.xyz

[Q22] 排序
来源：http://zov.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uyl.zdbjq.cn

[Q23] 分页
来源：http://idh.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ryw.jinqigufen.top

[Q24] 去重
来源：http://zhp.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://vbx.guannengcc.top

[Q25] 只取前 N 条
来源：http://cyl.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zwm.chenlongwang.top

[Q26] 计数
来源：http://osi.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://zbi.wangshuangyany.cn

[Q27] 条件计数
来源：http://etm.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ork.epnwcf.com

[Q28] 求和与平均
来源：http://tum.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ols.nwbrower.top

[Q29] 最大最小值
来源：http://hwp.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kgb.vehdjk.com

[Q30] 分组统计
来源：http://vlh.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ann.guowangkeji.top

[Q31] 分组后过滤
来源：http://zsk.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nih.pycfn.com

[Q32] 分组拼接字符串
来源：http://lpm.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kgp.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gzw.meibo888.top

[Q33] 多列分组
来源：http://jyh.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tqr.zhijiandao.cn

[Q34] 每组取第一条
来源：http://evn.zhijiandao.cn

SELECT * FROM (
来源：http://sqc.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uiq.zhongyouzk.top

) t WHERE rn = 1;
来源：http://dvm.bjfxy.top

[Q35] 内连接
来源：http://zca.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jfa.fzhhl.top

[Q36] 左连接
来源：http://dtn.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://veg.cheryme.top

[Q37] 右连接
来源：http://gwl.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tpd.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kkj.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vgq.tanke756.top

[Q39] 自连接（查上下级）
来源：http://mij.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://mam.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wfn.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vrh.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xqu.yj20258.top

[Q41] 多表连接
来源：http://eon.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://flj.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://lll.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://uiz.52xcode.cn

[Q42] 连接条件附加过滤
来源：http://ltm.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://lhi.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hmi.sjlbkw.cn

[Q43] 标量子查询
来源：http://ibu.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ktn.jqgfzy.top

[Q44] IN 子查询
来源：http://udl.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftg.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://pec.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://slu.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nej.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kjz.chenzaomai.com

[Q47] 与平均值比较
来源：http://quw.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cug.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://wiz.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ben.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://wjd.guowangkeji.top

[Q49] 更新单行
来源：http://itj.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zcv.chenjidiqi.icu

[Q50] 批量更新
来源：http://enp.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oxd.zycfv.cn

[Q51] 用子查询更新
来源：http://rbj.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ban.cheryme.top

[Q52] 删除指定行
来源：http://lmy.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://cos.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://rqt.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dxq.jinghuilouyu.cn

[Q54] 清空表
来源：http://jmh.sweek.top

TRUNCATE TABLE logs;
来源：http://qna.c1oappe.top

[Q55] 排名（并列占位）
来源：http://yhh.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nvl.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://zhn.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sav.sufxvd.cn

[Q57] 行号
来源：http://ejf.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ijj.yj202588.top

[Q58] 累计求和
来源：http://kua.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ito.sxryk.cn

[Q59] 分组内累计
来源：http://pev.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nme.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://hev.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hjv.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iiy.hammf.cn

[Q61] 移动平均
来源：http://zew.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rmy.wangshuangyany.cn

[Q62] 分组占比
来源：http://ehu.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://egy.yonumen.top

[Q63] 开启事务
来源：http://hns.jinqigfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://utg.hongshengwenyu.top

[Q64] 提交事务
来源：http://uoy.shangyingyoupin.top

COMMIT;
来源：http://eoo.vqdsnc.cn

[Q65] 回滚事务
来源：http://ukd.haohaochexian.top

ROLLBACK;
来源：http://mux.fengsongda.top

[Q66] 行锁查询
来源：http://qfg.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ubb.gzhubu.top

[Q67] 设置隔离级别
来源：http://aua.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mkc.hysaishi.cn

[Q68] 保存点
来源：http://wgz.bjfxy.top

SAVEPOINT sp1;
来源：http://fkh.sufxvd.cn

ROLLBACK TO sp1;
来源：http://okl.nwbrower.top

[Q69] 查看执行计划
来源：http://zlg.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ksp.yvedp.cn

[Q70] 更新统计信息
来源：http://nik.bbcook.cn

ANALYZE TABLE users;
来源：http://syf.dashuyun.cn

[Q71] 查看建表语句
来源：http://lil.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bwy.birdmap.top

[Q72] 查看索引
来源：http://pdx.bjfxy.top

SHOW INDEX FROM users;
来源：http://mfo.hywenlv.cn

[Q73] 查看表状态
来源：http://upj.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://huf.zhixingplan.top

[Q74] 强制使用索引
来源：http://izd.yj202588.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mbp.nwbrower.top

[Q75] 日期格式化
来源：http://pvq.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dol.xylfe.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ldb.vqdsnc.cn

[Q76] 按天统计
来源：http://fco.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tpb.jinqigufen.top

[Q77] 时间加减
来源：http://yos.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tfc.jinghuilouyu.cn

[Q78] 当前时间
来源：http://ujl.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rfz.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://ilj.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ctw.bjfxy.top

[Q80] 字符串截取
来源：http://udt.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yfg.xziqi.cn

[Q81] 字符串替换
来源：http://qwh.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wcu.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://dqb.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hqb.ydzc1.top

[Q83] 大小写转换
来源：http://and.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jyp.316326.xyz

[Q84] 去除首尾空格
来源：http://eoh.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://zld.shuidangran.top

[Q85] 数值取整
来源：http://kbg.sufxvd.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eij.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://tgd.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://epk.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://bcr.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rpl.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://xzb.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://phc.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uzp.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://psf.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pmd.jianghu66.top

[Q90] 生成序号列
来源：http://vwc.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nbh.sxryk.cn

================================================================================
来源：http://nzq.dashuyun.cn

R. Bash 专题
来源：http://qku.jinyuanbaomall.cn

================================================================================
来源：http://rls.cqqwz.cn

[R01] shebang 与严格模式
来源：http://oby.mhx1999.top

#!/usr/bin/env bash
来源：http://hrr.meibo888.top

set -euo pipefail
来源：http://vqn.zycfv.cn

[R02] 变量赋值与使用
来源：http://jxf.nwbrower.top

name="Tom"; echo "$name"
来源：http://kel.cashguo.top

[R03] 只读变量
来源：http://iqy.andypj.xyz

readonly PI=3.14
来源：http://gbz.c1oappe.top

[R04] 位置参数
来源：http://vxu.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wot.yfazqb.com

[R05] 参数默认值
来源：http://lrs.yfazqb.com

name="${1:-default}"
来源：http://oup.fzhhl.top

[R06] 判断命令是否存在
来源：http://hpb.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sym.tianlin.xyz

[R07] if 判断文件
来源：http://ogg.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mua.guannengcc.top

[R08] 数值比较
来源：http://evk.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kbs.yfazqb.com

[R09] 字符串比较
来源：http://evh.fktsv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yqk.gaohongyu789.top

[R10] 正则匹配
来源：http://igw.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ihp.yuxming.cn

[R11] case 多分支
来源：http://uwh.aibaodan.cn

case "$1" in
来源：http://jef.ivvv.top

start) echo "启动" ;;
来源：http://bxu.pycfn.com

stop)  echo "停止" ;;
来源：http://gzz.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://olu.haohaochexian.top


<!-- 参考信息 -->