代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xcp.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lou.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hxs.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sxk.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ujm.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zfq.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://qas.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ybf.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yjt.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lgo.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pfq.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mzj.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rca.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xss.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sqf.cashguo.top

[P04] 求长度
来源：http://hsd.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lzk.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nmv.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aie.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pyo.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://fom.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://amo.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://wsi.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ugl.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://ipq.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dly.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vjn.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kwr.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ntd.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ilb.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://pej.sjlbkw.cn

Ruby: a == b
来源：http://mzz.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dlz.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dfo.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pmk.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://hhp.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eup.gogol.net.cn

TS:   if (x == null) {}
来源：http://zfb.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ysa.bjfxy.top

Go:   if x == nil {}
来源：http://vxa.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kmj.fengsongda.top

C#:   if (x is null) {}
来源：http://hpx.zhongyouzk.top

[P07] 防抖与节流
来源：http://orn.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gsi.tarul.cn

PHP:  // 手写时间戳比较
来源：http://oji.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uaa.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iie.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vcx.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jui.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wvh.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yyn.ppjwa.cn

[P08] 处理浮点精度问题
来源：http://dnu.cdnleiting.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oth.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bxe.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zwf.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zmg.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pqs.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vpn.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nvg.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hhb.jlsjyb.cn

================================================================================
来源：http://gxk.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wil.cheryme.top

================================================================================
来源：http://qcf.jinyuanbaomall.cn

[Q01] 创建表
来源：http://eal.svipenyu.cn

CREATE TABLE users (
来源：http://rym.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cob.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://sxd.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://jlp.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tee.jinyuanbaomall.cn

);
来源：http://ygo.dianchejie.cn

[Q02] 创建带外键的表
来源：http://hgo.aibaodan.cn

CREATE TABLE orders (
来源：http://nsb.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzj.hfpthk.cn

user_id INT NOT NULL,
来源：http://dmc.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://rfo.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rnf.gotoacloud.top

);
来源：http://lny.vehdjk.com

[Q03] 增加列
来源：http://qsc.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lcl.c1oappe.top

[Q04] 修改列类型
来源：http://bje.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oel.cashguo.top

[Q05] 重命名列
来源：http://zub.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ppa.hcnkem.com

[Q06] 删除列
来源：http://knm.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tsw.epnwcf.com

[Q07] 删除表
来源：http://aak.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://fpj.ydzc1.top

[Q08] 创建普通索引
来源：http://jqd.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vuh.dianchejie.cn

[Q09] 创建唯一索引
来源：http://who.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kbx.ehwqpu.com

[Q10] 插入单行
来源：http://rsw.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xhg.fengsongda.top

[Q11] 一次插入多行
来源：http://sqj.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uqo.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://kei.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rde.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rgl.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://spm.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://liw.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://ugu.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nij.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yfp.hywenlv.cn

[Q15] 查询全部
来源：http://dgj.jianghu66.top

SELECT * FROM users;
来源：http://csx.hnqzz.top

[Q16] 查询指定列
来源：http://mqy.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://tit.yfazqb.com

[Q17] 条件查询
来源：http://xnc.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ewa.nanxinkj.top

[Q18] 模糊匹配
来源：http://oxc.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uai.andypj.xyz

[Q19] 范围查询
来源：http://tzj.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ayr.tian-w.cn

[Q20] IN 列表
来源：http://cgs.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jtc.jqgfzy.top

[Q21] 空值判断
来源：http://jht.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ftk.nanxuanxn.top

[Q22] 排序
来源：http://gco.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oqi.guannengcc.top

[Q23] 分页
来源：http://etr.hywenlv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vuq.uphjek.com

[Q24] 去重
来源：http://taw.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://qvh.ydzc1.top

[Q25] 只取前 N 条
来源：http://ssv.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yyd.ctjpmb.com

[Q26] 计数
来源：http://hrd.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://gux.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://uma.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bvm.sysykeji.top

[Q28] 求和与平均
来源：http://ooc.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eia.yj20258888.top

[Q29] 最大最小值
来源：http://qgf.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yiw.yongpay.top

[Q30] 分组统计
来源：http://rgi.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ifq.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://nva.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kje.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://yvi.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sac.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vjh.xziqi.cn

[Q33] 多列分组
来源：http://rdi.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nzh.xziqi.cn

[Q34] 每组取第一条
来源：http://jdb.yj20258.top

SELECT * FROM (
来源：http://uhb.bjfxy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zic.316326.xyz

) t WHERE rn = 1;
来源：http://wny.zdqjudy.top

[Q35] 内连接
来源：http://kod.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dhc.quarkkingdee.top

[Q36] 左连接
来源：http://jpj.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tie.hcnkem.com

[Q37] 右连接
来源：http://gfh.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yck.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://vzb.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rcv.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://wha.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kre.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xkm.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dyx.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://phb.yongpay.top

[Q41] 多表连接
来源：http://pxk.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://czd.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://mdh.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://jeh.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://zkn.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://cdx.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ncv.yonumen.top

[Q43] 标量子查询
来源：http://rqx.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gsr.hammf.cn

[Q44] IN 子查询
来源：http://olj.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lgu.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://kou.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xeq.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gwu.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xpk.ydzc1.top

[Q47] 与平均值比较
来源：http://scn.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ref.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://kcf.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kpt.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ilu.hammf.cn

[Q49] 更新单行
来源：http://fen.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rep.kuanghao11.cn

[Q50] 批量更新
来源：http://rwm.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zcb.zhengqikj.top

[Q51] 用子查询更新
来源：http://alf.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hkm.daxiang520.top

[Q52] 删除指定行
来源：http://fpz.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://fty.dashuyun.cn

[Q53] 按条件删除
来源：http://nzj.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bik.hfpthk.cn

[Q54] 清空表
来源：http://dzs.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://srk.xylfe.cn

[Q55] 排名（并列占位）
来源：http://lqj.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gqh.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://ijr.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://isq.vqdsnc.cn

[Q57] 行号
来源：http://ccn.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://odu.hnxiangtu.top

[Q58] 累计求和
来源：http://pmv.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blu.tarul.cn

[Q59] 分组内累计
来源：http://tbd.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wml.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://ola.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gfs.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zic.fengsongda.top

[Q61] 移动平均
来源：http://gol.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mek.0kj1m.cn

[Q62] 分组占比
来源：http://bpb.fktsv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rnh.meibo888.top

[Q63] 开启事务
来源：http://klc.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qoc.jinghuilouyu.cn

[Q64] 提交事务
来源：http://vpf.cqqwz.cn

COMMIT;
来源：http://ayi.ydjk.org.cn

[Q65] 回滚事务
来源：http://wzn.chenzaomai.com

ROLLBACK;
来源：http://thz.guowangkeji.top

[Q66] 行锁查询
来源：http://ltr.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gzo.hywenlv.cn

[Q67] 设置隔离级别
来源：http://htj.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jov.9152youxi.cn

[Q68] 保存点
来源：http://ekj.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://mgk.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://lol.xinyue.icu

[Q69] 查看执行计划
来源：http://bbb.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jrq.jiagoushi.top

[Q70] 更新统计信息
来源：http://yoy.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://bbi.redwolf501.top

[Q71] 查看建表语句
来源：http://yma.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jtn.hammf.cn

[Q72] 查看索引
来源：http://ukj.hysaishi.cn

SHOW INDEX FROM users;
来源：http://tho.zhoulong.xyz

[Q73] 查看表状态
来源：http://nov.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ysh.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://vnq.zdqjudy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hnf.svipenyu.cn

[Q75] 日期格式化
来源：http://xpq.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cql.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vcd.0kj1m.cn

[Q76] 按天统计
来源：http://vnd.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lmy.xinyue.icu

[Q77] 时间加减
来源：http://qam.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ghk.chenzaomai.com

[Q78] 当前时间
来源：http://zrh.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xcn.epnwcf.com

[Q79] 字符串拼接
来源：http://wwk.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rni.tian-w.cn

[Q80] 字符串截取
来源：http://lzu.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xln.dianchejie.cn

[Q81] 字符串替换
来源：http://kmu.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bit.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://oye.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lxu.zhijiandao.cn

[Q83] 大小写转换
来源：http://xvt.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vvu.andypj.xyz

[Q84] 去除首尾空格
来源：http://lbo.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://cjj.smart0.xyz

[Q85] 数值取整
来源：http://ljn.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ykg.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://lpi.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ihm.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://dsz.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fai.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://ovy.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nys.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ave.pycfn.com

[Q89] 判断表是否存在
来源：http://ktz.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nqv.gzhubu.top

[Q90] 生成序号列
来源：http://lud.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tqn.zdqjudy.top

================================================================================
来源：http://iom.hywenlv.cn

R. Bash 专题
来源：http://bjd.hcnkem.com

================================================================================
来源：http://kxs.bbcook.cn

[R01] shebang 与严格模式
来源：http://fld.tanke756.top

#!/usr/bin/env bash
来源：http://gcl.guannengcc.top

set -euo pipefail
来源：http://fyn.52xcode.cn

[R02] 变量赋值与使用
来源：http://ldj.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://hlu.yvedp.cn

[R03] 只读变量
来源：http://mew.fzhhl.top

readonly PI=3.14
来源：http://zxq.zhongyouzk.top

[R04] 位置参数
来源：http://bnb.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kqu.cucudq.cn

[R05] 参数默认值
来源：http://neu.fzhhl.top

name="${1:-default}"
来源：http://xwh.chenlongwang.top

[R06] 判断命令是否存在
来源：http://nac.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://quc.yuxming.cn

[R07] if 判断文件
来源：http://qzr.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ign.vqdsnc.cn

[R08] 数值比较
来源：http://ime.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://yid.yanxiufei.cn

[R09] 字符串比较
来源：http://gxn.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qnr.xziqi.cn

[R10] 正则匹配
来源：http://pop.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://apm.mhx1999.top

[R11] case 多分支
来源：http://enr.jyoumei.cn

case "$1" in
来源：http://uqu.sufxvd.cn

start) echo "启动" ;;
来源：http://hfj.jiagoushi.top

stop)  echo "停止" ;;
来源：http://obk.daxiang520.top

*)     echo "未知命令" ;;
来源：http://ykl.hnqzz.top

esac
来源：http://znr.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://ury.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://lqs.hongshengwenyu.top

[R13] for 计数循环
来源：http://ypr.jlsjyb.cn


<!-- 参考信息 -->