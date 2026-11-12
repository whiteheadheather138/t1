代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bve.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gfu.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hcm.quarkkingdee.top

[P04] 求长度
来源：http://rew.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jpv.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohz.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ylb.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mix.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://kgy.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://wne.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://dgn.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gsj.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://udm.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ilb.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xbs.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mpx.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ios.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tjo.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://qaq.jinqigufen.top

Ruby: a == b
来源：http://hna.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ryp.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ujn.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vgh.yj20258.top

PHP:  if (empty($x)) {}
来源：http://szd.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://syz.shuidangran.top

TS:   if (x == null) {}
来源：http://uyj.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kbe.wangdashe.top

Go:   if x == nil {}
来源：http://txd.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rnw.quarkkingdee.top

C#:   if (x is null) {}
来源：http://asq.sweek.top

[P07] 防抖与节流
来源：http://xcb.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zuz.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://nkx.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zrr.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nts.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dql.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rzl.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wng.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rsi.redwolf501.top

[P08] 处理浮点精度问题
来源：http://phh.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://udy.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mtk.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wga.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dxy.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bqe.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://svt.fehbvm.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oee.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://acs.jiagoushi.top

================================================================================
来源：http://esm.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vfg.ppjwa.cn

================================================================================
来源：http://rqe.yongpay.top

[Q01] 创建表
来源：http://owb.dashuyun.cn

CREATE TABLE users (
来源：http://kvb.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lgn.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://zjh.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://qjd.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cms.zhixingplan.top

);
来源：http://qkn.jianghu66.top

[Q02] 创建带外键的表
来源：http://drx.aibaodan.cn

CREATE TABLE orders (
来源：http://ogm.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rwt.chenzaomai.com

user_id INT NOT NULL,
来源：http://omz.tian-w.cn

amount DECIMAL(10, 2),
来源：http://nje.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://csp.cashguo.top

);
来源：http://wju.yj202588.top

[Q03] 增加列
来源：http://cra.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hcv.zhoulong.xyz

[Q04] 修改列类型
来源：http://zwl.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yio.cqqwz.cn

[Q05] 重命名列
来源：http://rbf.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fiw.jlsjyb.cn

[Q06] 删除列
来源：http://hip.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xuv.fehbvm.com

[Q07] 删除表
来源：http://sgl.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://iwe.fktsv.cn

[Q08] 创建普通索引
来源：http://wzb.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://txl.yuanzhike.top

[Q09] 创建唯一索引
来源：http://rjh.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eah.bbcook.cn

[Q10] 插入单行
来源：http://gih.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rsm.sysykeji.top

[Q11] 一次插入多行
来源：http://xrt.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://slz.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://uey.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://lgm.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hfu.nanxinkj.top

[Q13] 忽略重复插入
来源：http://woy.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ghz.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://hpz.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yos.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oxd.316326.xyz

[Q15] 查询全部
来源：http://eaz.haohaochexian.top

SELECT * FROM users;
来源：http://qgf.sjlbkw.cn

[Q16] 查询指定列
来源：http://zev.svipenyu.cn

SELECT id, name FROM users;
来源：http://ouu.hammf.cn

[Q17] 条件查询
来源：http://ycs.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://avf.zhoulong.xyz

[Q18] 模糊匹配
来源：http://ujb.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ufv.jianghu66.top

[Q19] 范围查询
来源：http://rnn.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hqy.zdqjudy.top

[Q20] IN 列表
来源：http://pkd.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sjx.svipenyu.cn

[Q21] 空值判断
来源：http://ugu.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://guf.mhx1999.top

[Q22] 排序
来源：http://hml.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qnl.c1oappe.top

[Q23] 分页
来源：http://olt.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nde.ydzc1.top

[Q24] 去重
来源：http://xuc.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://omt.sweek.top

[Q25] 只取前 N 条
来源：http://axn.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gkr.xuanzx.com

[Q26] 计数
来源：http://omn.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://zfz.yuanzhike.top

[Q27] 条件计数
来源：http://xhf.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wwm.hnqzz.top

[Q28] 求和与平均
来源：http://amj.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qdn.jinqigfzy.top

[Q29] 最大最小值
来源：http://upp.shanyushiyangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qfn.9152youxi.cn

[Q30] 分组统计
来源：http://dbx.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sds.aizwys.cn

[Q31] 分组后过滤
来源：http://cai.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mvw.316326.xyz

[Q32] 分组拼接字符串
来源：http://ogk.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ohw.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dyv.yj20258.top

[Q33] 多列分组
来源：http://vtr.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ppo.jinqigufen.top

[Q34] 每组取第一条
来源：http://thv.316326.xyz

SELECT * FROM (
来源：http://hnc.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hue.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://ipy.dianchejie.cn

[Q35] 内连接
来源：http://ijg.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dgf.zhixingplan.top

[Q36] 左连接
来源：http://bbi.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cxw.yj202588.top

[Q37] 右连接
来源：http://jgs.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ejd.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iau.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jgk.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://qvd.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pgr.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zjj.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lkb.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oax.gogol.net.cn

[Q41] 多表连接
来源：http://pdq.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cbg.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://ccd.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://wee.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://jzs.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://pzo.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mct.ehwqpu.com

[Q43] 标量子查询
来源：http://urm.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mka.hnqzz.top

[Q44] IN 子查询
来源：http://rpz.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pdd.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://goo.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://szs.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://nsu.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://beb.zhijiandao.cn

[Q47] 与平均值比较
来源：http://adc.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jbr.cashguo.top

[Q48] CTE 公用表表达式
来源：http://zag.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bch.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://tzp.yj20258.top

[Q49] 更新单行
来源：http://slh.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ymu.pycfn.com

[Q50] 批量更新
来源：http://vyz.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wvq.yongpay.top

[Q51] 用子查询更新
来源：http://hjn.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iuv.jlsjyb.cn

[Q52] 删除指定行
来源：http://dir.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://ivl.hywenlv.cn

[Q53] 按条件删除
来源：http://jov.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lzc.tarul.cn

[Q54] 清空表
来源：http://jcb.shuidangran.top

TRUNCATE TABLE logs;
来源：http://xnr.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://tbn.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xoh.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://qjx.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lsy.tanke756.top

[Q57] 行号
来源：http://hak.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tgs.ydzc1.top

[Q58] 累计求和
来源：http://rix.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aca.hammf.cn

[Q59] 分组内累计
来源：http://zbo.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://are.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://iyp.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tgn.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wql.guannengcc.top

[Q61] 移动平均
来源：http://ebm.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cbe.sweek.top

[Q62] 分组占比
来源：http://qft.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://osn.daxiang520.top

[Q63] 开启事务
来源：http://mif.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iym.xuetiantiany.cn

[Q64] 提交事务
来源：http://cwl.nanxinkj.top

COMMIT;
来源：http://dkz.birdmap.top

[Q65] 回滚事务
来源：http://ate.yj20258.top

ROLLBACK;
来源：http://vmz.tarul.cn

[Q66] 行锁查询
来源：http://btk.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zca.nanxinkj.top

[Q67] 设置隔离级别
来源：http://lae.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cri.iojbl.cn

[Q68] 保存点
来源：http://jvj.zhixingplan.top

SAVEPOINT sp1;
来源：http://dbt.wangdashe.top

ROLLBACK TO sp1;
来源：http://lvu.zhoulong.xyz

[Q69] 查看执行计划
来源：http://rmw.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ayj.shanyushiyangtech.top

[Q70] 更新统计信息
来源：http://mzp.daxiang520.top

ANALYZE TABLE users;
来源：http://lok.jinqigfzy.top

[Q71] 查看建表语句
来源：http://yrr.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwh.birdmap.top

[Q72] 查看索引
来源：http://xjv.yj20258.top

SHOW INDEX FROM users;
来源：http://mqu.tianlin.xyz

[Q73] 查看表状态
来源：http://rnw.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ejs.yvedp.cn

[Q74] 强制使用索引
来源：http://kte.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vwx.guowangkeji.top

[Q75] 日期格式化
来源：http://vzh.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hqf.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fpy.tian-w.cn

[Q76] 按天统计
来源：http://xeu.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xzp.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://nyp.chenjidiqi.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ueh.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://arg.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vii.tian-w.cn

[Q79] 字符串拼接
来源：http://rvo.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sxd.jinqigufen.top

[Q80] 字符串截取
来源：http://joj.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gsf.c1oappe.top

[Q81] 字符串替换
来源：http://zgk.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nnj.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://dwb.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hhx.ctjpmb.com

[Q83] 大小写转换
来源：http://gms.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wky.gogol.net.cn

[Q84] 去除首尾空格
来源：http://eaf.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://bwa.jyoumei.cn

[Q85] 数值取整
来源：http://gnw.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://efk.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://oda.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ztm.tian-w.cn

[Q87] JSON 字段做条件
来源：http://oji.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uoh.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://ycc.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pzh.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mkb.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://wgk.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wmd.shuidangran.top

[Q90] 生成序号列
来源：http://tvq.yanxiufei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fln.bjfxy.top

================================================================================
来源：http://fxf.yj20258888.top

R. Bash 专题
来源：http://uyz.fehbvm.com

================================================================================
来源：http://wgn.iojbl.cn

[R01] shebang 与严格模式
来源：http://dow.fzhhl.top

#!/usr/bin/env bash
来源：http://rpi.9152youxi.cn

set -euo pipefail
来源：http://tgn.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://dik.52xcode.cn

name="Tom"; echo "$name"
来源：http://bcn.haohaochexian.top

[R03] 只读变量
来源：http://fsc.fzhhl.top

readonly PI=3.14
来源：http://izg.ydjk.org.cn

[R04] 位置参数
来源：http://ehs.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://loa.epnwcf.com

[R05] 参数默认值
来源：http://skf.jiagoushi.top

name="${1:-default}"
来源：http://lws.yongpay.top

[R06] 判断命令是否存在
来源：http://rfi.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eck.yongpay.top

[R07] if 判断文件
来源：http://fhp.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fun.yj20258888.top

[R08] 数值比较
来源：http://ypk.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://whr.gogol.net.cn

[R09] 字符串比较
来源：http://dty.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yqh.tanke756.top

[R10] 正则匹配
来源：http://svw.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dwe.kuanghao11.cn

[R11] case 多分支
来源：http://vcs.yongpay.top

case "$1" in
来源：http://btm.jqgfzy.top

start) echo "启动" ;;
来源：http://oyk.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://nxn.c1oappe.top

*)     echo "未知命令" ;;
来源：http://onb.yuxming.cn

esac
来源：http://qhe.zhiwuduotai.top

[R12] for 遍历文件
来源：http://ztj.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://rvb.zycfv.cn

[R13] for 计数循环
来源：http://iwn.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://kzy.daxiang520.top

[R14] C 风格 for
来源：http://uvl.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cep.316326.xyz

[R15] while 逐行读文件
来源：http://fpx.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jzt.jqgfzy.top

[R16] until 等待条件
来源：http://rmb.hnqzz.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rap.jyoumei.cn

[R17] 数组定义与取值
来源：http://enx.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://bok.hesvh.cn

[R18] 遍历数组
来源：http://sud.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tck.ywan-chungtsiang.top

[R19] 数组长度
来源：http://jlp.316326.xyz


<!-- 参考信息 -->