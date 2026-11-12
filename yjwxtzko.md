代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://asa.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://off.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://dhx.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ojg.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bvw.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tgu.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://acm.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gqv.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uya.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cpm.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mnp.sxryk.cn

[P04] 求长度
来源：http://wth.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://afd.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hcp.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zmg.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ugd.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://lrb.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://ube.hcnkem.com

Ruby: x.length;  x.size
来源：http://lxm.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wkp.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://dfr.daria6918.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ilu.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lgp.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hyc.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hdv.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ygn.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://gsm.ywan-chungtsiang.top

Ruby: a == b
来源：http://bnm.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pcb.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kvq.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://apz.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://qbs.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wmj.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://yam.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ldf.jinqigufen.top

Go:   if x == nil {}
来源：http://uno.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ywc.zdqjudy.top

C#:   if (x is null) {}
来源：http://dua.zycfv.cn

[P07] 防抖与节流
来源：http://bqd.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wbg.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://pkw.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crk.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jxo.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xqz.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://has.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bpt.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://orp.cashguo.top

[P08] 处理浮点精度问题
来源：http://cem.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vdq.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uqp.nwbrower.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gdo.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wdp.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cfs.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jog.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lte.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fek.shangyingyoupin.top

================================================================================
来源：http://uiy.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vie.hysaishi.cn

================================================================================
来源：http://iui.shzxlz.cn

[Q01] 创建表
来源：http://atg.kuanghao11.cn

CREATE TABLE users (
来源：http://gko.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aig.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://hlw.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://uej.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wgk.pycfn.com

);
来源：http://dzd.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://bjr.vehdjk.com

CREATE TABLE orders (
来源：http://rfc.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nzd.xylfe.cn

user_id INT NOT NULL,
来源：http://yrw.pycfn.com

amount DECIMAL(10, 2),
来源：http://nkn.aibaodan.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bza.hongshengwenyu.top

);
来源：http://nou.hysaishi.cn

[Q03] 增加列
来源：http://mum.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tqq.mhx1999.top

[Q04] 修改列类型
来源：http://yqx.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwr.yuxming.cn

[Q05] 重命名列
来源：http://tuj.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dgx.xylfe.cn

[Q06] 删除列
来源：http://ywg.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mew.hfpthk.cn

[Q07] 删除表
来源：http://czu.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://lhu.jinqigfzy.top

[Q08] 创建普通索引
来源：http://wfg.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://xrb.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://zyj.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oon.aizwys.cn

[Q10] 插入单行
来源：http://obh.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://itj.mhx1999.top

[Q11] 一次插入多行
来源：http://gxp.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://klv.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://zbl.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://wiq.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uil.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://mgl.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uid.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://hge.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mom.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kdc.havefunace.top

[Q15] 查询全部
来源：http://gns.sufxvd.cn

SELECT * FROM users;
来源：http://ojx.sysykeji.top

[Q16] 查询指定列
来源：http://mhj.yvedp.cn

SELECT id, name FROM users;
来源：http://krm.fehbvm.com

[Q17] 条件查询
来源：http://zzx.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qsp.zhoulong.xyz

[Q18] 模糊匹配
来源：http://odz.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dqh.jiagoushi.top

[Q19] 范围查询
来源：http://wpr.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bpv.chenzaomai.com

[Q20] IN 列表
来源：http://uqj.kuanghao11.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aub.birdmap.top

[Q21] 空值判断
来源：http://tao.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://oei.yuxming.cn

[Q22] 排序
来源：http://kjm.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://edz.cucudq.cn

[Q23] 分页
来源：http://oeu.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xhp.zhongyouzk.top

[Q24] 去重
来源：http://jif.yfazqb.com

SELECT DISTINCT city FROM users;
来源：http://cwq.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://maz.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ftt.redwolf501.top

[Q26] 计数
来源：http://uxm.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://hhi.jiagoushi.top

[Q27] 条件计数
来源：http://qfk.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tms.chenlongwang.top

[Q28] 求和与平均
来源：http://gnn.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yur.hywenlv.cn

[Q29] 最大最小值
来源：http://rgx.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xak.fktsv.cn

[Q30] 分组统计
来源：http://suu.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://asw.tian-w.cn

[Q31] 分组后过滤
来源：http://lik.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dfe.yj20258.top

[Q32] 分组拼接字符串
来源：http://mif.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jwe.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xyk.cqqwz.cn

[Q33] 多列分组
来源：http://aqh.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qll.aizwys.cn

[Q34] 每组取第一条
来源：http://ayq.tanke756.top

SELECT * FROM (
来源：http://yos.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yyz.shuidangran.top

) t WHERE rn = 1;
来源：http://sbh.hysaishi.cn

[Q35] 内连接
来源：http://ppx.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ysc.uphjek.com

[Q36] 左连接
来源：http://iun.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bkz.daxiang520.top

[Q37] 右连接
来源：http://oxh.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xaj.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://jbn.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pkr.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://ymq.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mdg.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kon.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zrh.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://amz.cheryme.top

[Q41] 多表连接
来源：http://jif.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pmv.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://jmo.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://kiu.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://iel.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://lat.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcx.meibo888.top

[Q43] 标量子查询
来源：http://gji.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ccf.aibaodan.cn

[Q44] IN 子查询
来源：http://gqx.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dla.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://aom.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xcc.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zil.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bdh.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://kcg.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zpd.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://nww.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ktf.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://ncb.uphjek.com

[Q49] 更新单行
来源：http://ayh.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://upv.wangshuangyany.cn

[Q50] 批量更新
来源：http://dtv.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oia.epnwcf.com

[Q51] 用子查询更新
来源：http://lsz.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lpv.hfpthk.cn

[Q52] 删除指定行
来源：http://vxf.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://kwc.bjfxy.top

[Q53] 按条件删除
来源：http://nrv.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nan.fengsongda.top

[Q54] 清空表
来源：http://jbu.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://auw.xziqi.cn

[Q55] 排名（并列占位）
来源：http://ifq.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rbt.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://dtj.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ejo.vqdsnc.cn

[Q57] 行号
来源：http://vii.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ccj.yueranfly.top

[Q58] 累计求和
来源：http://jim.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ilg.chenzaomai.com

[Q59] 分组内累计
来源：http://bib.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nhc.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://bzj.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://com.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xqo.jqgfzy.top

[Q61] 移动平均
来源：http://aua.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bcq.gogol.net.cn

[Q62] 分组占比
来源：http://fmv.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eax.fktsv.cn

[Q63] 开启事务
来源：http://aux.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pxa.xinyue.icu

[Q64] 提交事务
来源：http://gyh.fengsongda.top

COMMIT;
来源：http://oco.ppjwa.cn

[Q65] 回滚事务
来源：http://sgq.jlsjyb.cn

ROLLBACK;
来源：http://nam.sweek.top

[Q66] 行锁查询
来源：http://xnz.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zvh.xylfe.cn

[Q67] 设置隔离级别
来源：http://frz.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vjh.zdbjq.cn

[Q68] 保存点
来源：http://iyn.9152youxi.cn

SAVEPOINT sp1;
来源：http://gfx.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://djx.andypj.xyz

[Q69] 查看执行计划
来源：http://rqi.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hum.dashuyun.cn

[Q70] 更新统计信息
来源：http://eto.yj20258888.top

ANALYZE TABLE users;
来源：http://uir.jqgufenzy.top

[Q71] 查看建表语句
来源：http://ggp.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://izf.zycfv.cn

[Q72] 查看索引
来源：http://grs.fzhhl.top

SHOW INDEX FROM users;
来源：http://qvb.sufxvd.cn

[Q73] 查看表状态
来源：http://ixt.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://ssn.jqgufenzy.top

[Q74] 强制使用索引
来源：http://bgt.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aqv.zdbjq.cn

[Q75] 日期格式化
来源：http://hfb.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hea.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ixl.zhoulong.xyz

[Q76] 按天统计
来源：http://kcs.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ady.xinyue.icu

[Q77] 时间加减
来源：http://zqw.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rgu.zycfv.cn

[Q78] 当前时间
来源：http://nfw.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nle.fehbvm.com

[Q79] 字符串拼接
来源：http://lwq.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hpc.jinqigufen.top

[Q80] 字符串截取
来源：http://nql.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fbm.cdnleiting.top

[Q81] 字符串替换
来源：http://rqf.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pbq.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://rcy.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://emo.ydjk.org.cn

[Q83] 大小写转换
来源：http://qbk.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hxo.bjfxy.top

[Q84] 去除首尾空格
来源：http://hyo.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://ybp.jianghu66.top

[Q85] 数值取整
来源：http://sho.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xzj.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://hif.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rga.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://fly.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zrc.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://hze.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bbr.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eoj.hesvh.cn

[Q89] 判断表是否存在
来源：http://lgp.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fzt.sysykeji.top

[Q90] 生成序号列
来源：http://jwn.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pas.zhiwuduotai.top

================================================================================
来源：http://mfy.gaohongyu789.top

R. Bash 专题
来源：http://fhb.aizwys.cn

================================================================================
来源：http://hll.fktsv.cn

[R01] shebang 与严格模式
来源：http://mnb.tian-w.cn

#!/usr/bin/env bash
来源：http://wwf.52xcode.cn

set -euo pipefail
来源：http://xqy.yonumen.top

[R02] 变量赋值与使用
来源：http://fgf.ivvv.top

name="Tom"; echo "$name"
来源：http://wau.shzxlz.cn

[R03] 只读变量
来源：http://mkx.yongpay.top

readonly PI=3.14
来源：http://yjl.jinqigfzy.top

[R04] 位置参数
来源：http://apl.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bha.cheryme.top

[R05] 参数默认值
来源：http://kpw.sjlbkw.cn

name="${1:-default}"
来源：http://mrh.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://ego.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jbp.meibo888.top

[R07] if 判断文件
来源：http://dnz.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://grq.fehbvm.com

[R08] 数值比较
来源：http://qwt.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://okm.shanyushiyangtech.top

[R09] 字符串比较
来源：http://wft.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kkz.aizwys.cn

[R10] 正则匹配
来源：http://wmm.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vci.sysykeji.top

[R11] case 多分支
来源：http://enf.yvedp.cn

case "$1" in
来源：http://ycm.chenjidiqi.icu

start) echo "启动" ;;
来源：http://syb.shzxlz.cn

stop)  echo "停止" ;;
来源：http://trm.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://bej.xziqi.cn

esac
来源：http://amm.gogol.net.cn

[R12] for 遍历文件
来源：http://iuh.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://kcp.fehbvm.com

[R13] for 计数循环
来源：http://fmy.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://uyr.dashuyun.cn

[R14] C 风格 for
来源：http://shp.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ony.gaohongyu789.top

[R15] while 逐行读文件
来源：http://zeo.sjlbkw.cn


<!-- 参考信息 -->