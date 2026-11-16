代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dsz.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jmf.svipenyu.cn

[P03] 生成短随机字符串
来源：http://gmq.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://otj.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://atn.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqv.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://isl.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kgh.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wse.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://fpf.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://goh.hnqzz.top

[P04] 求长度
来源：http://fpk.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pvu.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tre.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aam.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://suj.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://xut.sysykeji.top

Go:   len(arr);  len(m)
来源：http://vxf.ivvv.top

Ruby: x.length;  x.size
来源：http://cig.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ynn.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://swc.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bhj.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ann.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://akb.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hzo.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lrv.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://ffv.vqdsnc.cn

Ruby: a == b
来源：http://irv.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vmj.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://isg.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oel.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://wmd.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pzc.sjlbkw.cn

TS:   if (x == null) {}
来源：http://wdb.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lah.ctjpmb.com

Go:   if x == nil {}
来源：http://hmq.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rqb.epnwcf.com

C#:   if (x is null) {}
来源：http://eqs.epnwcf.com

[P07] 防抖与节流
来源：http://jha.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ept.cashguo.top

PHP:  // 手写时间戳比较
来源：http://krp.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipz.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qop.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zrd.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ojt.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://olv.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pyv.birdmap.top

[P08] 处理浮点精度问题
来源：http://ubm.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uhj.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bwb.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vne.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hkx.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nhb.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wpx.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qfo.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rpb.yuxming.cn

================================================================================
来源：http://rzu.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mrx.ctjpmb.com

================================================================================
来源：http://sha.daxiang520.top

[Q01] 创建表
来源：http://tup.zhengqikj.top

CREATE TABLE users (
来源：http://uri.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xgm.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://rbn.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://kkc.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iiq.zhaomingkeji.xyz

);
来源：http://omy.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://iwo.ybcxt.top

CREATE TABLE orders (
来源：http://mox.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://omi.sjlbkw.cn

user_id INT NOT NULL,
来源：http://nak.uphjek.com

amount DECIMAL(10, 2),
来源：http://mqg.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pkw.xuanzx.com

);
来源：http://tde.zhongyouzk.top

[Q03] 增加列
来源：http://inx.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://agk.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://wpv.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mpb.sufxvd.cn

[Q05] 重命名列
来源：http://gzd.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xce.zdqjudy.top

[Q06] 删除列
来源：http://ynq.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://lfg.shzxlz.cn

[Q07] 删除表
来源：http://wur.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://hql.shzxlz.cn

[Q08] 创建普通索引
来源：http://xsp.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hcv.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://obl.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qnq.ybcxt.top

[Q10] 插入单行
来源：http://nhh.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ysa.nwbrower.top

[Q11] 一次插入多行
来源：http://nyg.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wef.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://tos.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rok.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://umj.9152youxi.cn

[Q13] 忽略重复插入
来源：http://olh.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sbk.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://wch.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hhd.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hhe.hcnkem.com

[Q15] 查询全部
来源：http://fag.tianlin.xyz

SELECT * FROM users;
来源：http://njx.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://djj.zhengqikj.top

SELECT id, name FROM users;
来源：http://ksu.svipenyu.cn

[Q17] 条件查询
来源：http://jgx.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cex.fengsongda.top

[Q18] 模糊匹配
来源：http://utl.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lfr.hfpthk.cn

[Q19] 范围查询
来源：http://rzp.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://osg.hysaishi.cn

[Q20] IN 列表
来源：http://rkh.zhiwuduotai.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://odm.kuanghao11.cn

[Q21] 空值判断
来源：http://txz.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tdm.hywenlv.cn

[Q22] 排序
来源：http://ntx.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hur.cdnleiting.top

[Q23] 分页
来源：http://shk.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://clw.hammf.cn

[Q24] 去重
来源：http://pvk.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://fzb.nanxinkj.top

[Q25] 只取前 N 条
来源：http://mxh.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jcd.shanyushiyangtech.top

[Q26] 计数
来源：http://izc.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://zxv.zhixingplan.top

[Q27] 条件计数
来源：http://rqh.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nhs.nanxinkj.top

[Q28] 求和与平均
来源：http://qtq.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xqy.meibo888.top

[Q29] 最大最小值
来源：http://ydz.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://brv.guowangkeji.top

[Q30] 分组统计
来源：http://ngf.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://drv.yfazqb.com

[Q31] 分组后过滤
来源：http://rqm.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zoz.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://lva.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wxa.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fxt.tarul.cn

[Q33] 多列分组
来源：http://tue.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qom.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://vuz.yongpay.top

SELECT * FROM (
来源：http://bai.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://upu.meibo888.top

) t WHERE rn = 1;
来源：http://xxu.hammf.cn

[Q35] 内连接
来源：http://pde.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cff.gotoacloud.top

[Q36] 左连接
来源：http://tkx.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mdc.birdmap.top

[Q37] 右连接
来源：http://ugo.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dyw.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://efq.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mfn.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://yqj.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tma.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eqj.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://upj.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ofq.xuetiantiany.cn

[Q41] 多表连接
来源：http://xtq.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gee.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://ngi.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://qww.yj202588.top

[Q42] 连接条件附加过滤
来源：http://ecz.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://nqy.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rbt.sysykeji.top

[Q43] 标量子查询
来源：http://zpu.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nrf.birdmap.top

[Q44] IN 子查询
来源：http://zzi.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xdc.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://mgz.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pgu.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://ykc.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://roq.yuanzhike.top

[Q47] 与平均值比较
来源：http://xdv.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kvt.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://wwq.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rtf.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://mys.vqdsnc.cn

[Q49] 更新单行
来源：http://rac.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kil.gaohongyu789.top

[Q50] 批量更新
来源：http://gii.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://urr.aizwys.cn

[Q51] 用子查询更新
来源：http://hsk.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vip.yueranfly.top

[Q52] 删除指定行
来源：http://tik.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://zhl.iojbl.cn

[Q53] 按条件删除
来源：http://rfn.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dlj.zhengqikj.top

[Q54] 清空表
来源：http://yvh.ybcxt.top

TRUNCATE TABLE logs;
来源：http://mpj.yuxming.cn

[Q55] 排名（并列占位）
来源：http://ydt.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zkr.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://srq.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://snk.shanyushiyangkeji.top

[Q57] 行号
来源：http://wct.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://txj.hysaishi.cn

[Q58] 累计求和
来源：http://mzc.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://egg.wangshuangyany.cn

[Q59] 分组内累计
来源：http://eel.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wok.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://lsr.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ubz.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gye.hnxiangtu.top

[Q61] 移动平均
来源：http://weq.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oes.zdqjudy.top

[Q62] 分组占比
来源：http://vcz.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uyi.dianchejie.cn

[Q63] 开启事务
来源：http://ygb.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qvl.jiagoushi.top

[Q64] 提交事务
来源：http://efr.tarul.cn

COMMIT;
来源：http://bww.bjfxy.top

[Q65] 回滚事务
来源：http://hmm.jinqigfzy.top

ROLLBACK;
来源：http://pqf.yj202588.top

[Q66] 行锁查询
来源：http://ctl.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jhw.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://rtz.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fog.xuetiantiany.cn

[Q68] 保存点
来源：http://mle.sufxvd.cn

SAVEPOINT sp1;
来源：http://vii.jianghu66.top

ROLLBACK TO sp1;
来源：http://nbx.jqgfzy.top

[Q69] 查看执行计划
来源：http://xtp.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://giy.fehbvm.com

[Q70] 更新统计信息
来源：http://hgg.yangfankeji.com

ANALYZE TABLE users;
来源：http://yxh.fzhhl.top

[Q71] 查看建表语句
来源：http://ejy.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dlg.svipenyu.cn

[Q72] 查看索引
来源：http://qbv.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://esh.jqgfzy.top

[Q73] 查看表状态
来源：http://aql.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tek.sxryk.cn

[Q74] 强制使用索引
来源：http://nps.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bax.daria6918.cn

[Q75] 日期格式化
来源：http://wub.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gwz.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jpw.zdqjudy.top

[Q76] 按天统计
来源：http://kvg.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gsf.iojbl.cn

[Q77] 时间加减
来源：http://dre.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fjf.zdqjudy.top

[Q78] 当前时间
来源：http://etq.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pgo.9152youxi.cn

[Q79] 字符串拼接
来源：http://ghg.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lep.jinqigufen.top

[Q80] 字符串截取
来源：http://hmn.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rdj.pengpengdd.cyou

[Q81] 字符串替换
来源：http://rwf.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://svm.sweek.top

[Q82] 字符长度与字节长度
来源：http://mby.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kcu.zhongyouzk.top

[Q83] 大小写转换
来源：http://hod.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vez.sysykeji.top

[Q84] 去除首尾空格
来源：http://wdk.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://ntg.xylfe.cn

[Q85] 数值取整
来源：http://kky.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vrc.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://klx.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nbx.uphjek.com

[Q87] JSON 字段做条件
来源：http://nil.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ppa.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://juz.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vvo.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iwe.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://spo.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://was.yj20258.top

[Q90] 生成序号列
来源：http://dtt.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kyh.haohaochexian.top

================================================================================
来源：http://fzd.gogol.net.cn

R. Bash 专题
来源：http://fuw.cdnleiting.top

================================================================================
来源：http://gwo.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://owx.andypj.xyz

#!/usr/bin/env bash
来源：http://xmn.nanxinkj.top

set -euo pipefail
来源：http://qgw.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://ntk.shanyushiyangtech.top

name="Tom"; echo "$name"
来源：http://svw.haohaochexian.top

[R03] 只读变量
来源：http://udy.haohaochexian.top

readonly PI=3.14
来源：http://umu.cqqwz.cn

[R04] 位置参数
来源：http://kyd.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wuf.yfazqb.com

[R05] 参数默认值
来源：http://jdh.yj20258888.top

name="${1:-default}"
来源：http://bft.hnqzz.top

[R06] 判断命令是否存在
来源：http://yfh.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kid.ivvv.top

[R07] if 判断文件
来源：http://wnn.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xip.aibaodan.cn

[R08] 数值比较
来源：http://wmm.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ctd.guannengcc.top

[R09] 字符串比较
来源：http://dbj.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qhg.feifeiyinyue.top

[R10] 正则匹配
来源：http://dvw.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uvu.vqdsnc.cn

[R11] case 多分支
来源：http://vfz.hammf.cn

case "$1" in
来源：http://duz.feifeiyinyue.top

start) echo "启动" ;;
来源：http://hvu.nanxinkj.top

stop)  echo "停止" ;;
来源：http://ldz.c1oappe.top

*)     echo "未知命令" ;;
来源：http://odk.jyoumei.cn

esac
来源：http://kah.havefunace.top

[R12] for 遍历文件
来源：http://vnr.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://ehu.hcnkem.com

[R13] for 计数循环
来源：http://lxv.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://rus.zycfv.cn

[R14] C 风格 for
来源：http://ixn.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aeg.bjfxy.top

[R15] while 逐行读文件
来源：http://xso.cashguo.top


<!-- 参考信息 -->