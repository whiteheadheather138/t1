代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ogx.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://mkw.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://btr.yuxming.cn

[P04] 求长度
来源：http://lix.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pti.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hgd.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fsl.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://anc.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://dqd.nwbrower.top

Go:   len(arr);  len(m)
来源：http://ups.jyoumei.cn

Ruby: x.length;  x.size
来源：http://kpi.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zki.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://mlx.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oix.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yip.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fya.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hyh.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kab.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jgd.tarul.cn

Ruby: a == b
来源：http://vwa.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dey.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hxr.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jst.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://clo.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ont.nanxuanxn.top

TS:   if (x == null) {}
来源：http://kvc.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pyu.yj20258.top

Go:   if x == nil {}
来源：http://ums.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ddy.iojbl.cn

C#:   if (x is null) {}
来源：http://ytz.redwolf501.top

[P07] 防抖与节流
来源：http://pfe.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wil.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://yfq.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgo.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rqa.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dxx.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hqj.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zvg.shuidangran.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ufo.mhx1999.top

[P08] 处理浮点精度问题
来源：http://xku.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rlw.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hvu.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqk.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://edw.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nzj.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cpy.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vvo.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bfg.zhoulong.xyz

================================================================================
来源：http://xki.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fbz.sysykeji.top

================================================================================
来源：http://lht.c1oappe.top

[Q01] 创建表
来源：http://puy.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://jrp.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfb.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://npc.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://ndq.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gio.sysykeji.top

);
来源：http://vtg.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://ees.yongpay.top

CREATE TABLE orders (
来源：http://uso.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jwb.haohaochexian.top

user_id INT NOT NULL,
来源：http://qbp.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://zgs.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jyb.ydjk.org.cn

);
来源：http://rki.yj202588.top

[Q03] 增加列
来源：http://vib.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://acm.cdnleiting.top

[Q04] 修改列类型
来源：http://jhd.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yjk.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://opy.vehdjk.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ctt.jqgfzy.top

[Q06] 删除列
来源：http://edk.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://qgg.quarkkingdee.top

[Q07] 删除表
来源：http://tpv.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://wkw.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://aso.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vox.sysykeji.top

[Q09] 创建唯一索引
来源：http://yyx.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ijf.guannengcc.top

[Q10] 插入单行
来源：http://lgx.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pkr.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://xff.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jsk.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://vml.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rlz.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kdq.birdmap.top

[Q13] 忽略重复插入
来源：http://neh.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gur.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://iui.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tec.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ykr.dashuyun.cn

[Q15] 查询全部
来源：http://cpv.cdnleiting.top

SELECT * FROM users;
来源：http://gsm.fengsongda.top

[Q16] 查询指定列
来源：http://cfl.yuanzhike.top

SELECT id, name FROM users;
来源：http://pxj.zdqjudy.top

[Q17] 条件查询
来源：http://bor.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jpq.vqdsnc.cn

[Q18] 模糊匹配
来源：http://uvc.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hnb.bbcook.cn

[Q19] 范围查询
来源：http://pmc.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://awd.jianghu66.top

[Q20] IN 列表
来源：http://zul.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ycm.gaohongyu789.top

[Q21] 空值判断
来源：http://rwf.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://irz.shanyushiyangtech.top

[Q22] 排序
来源：http://dls.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wxj.yvedp.cn

[Q23] 分页
来源：http://jrb.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rpf.9152youxi.cn

[Q24] 去重
来源：http://hys.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://cup.haohaochexian.top

[Q25] 只取前 N 条
来源：http://pzw.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://buv.ybcxt.top

[Q26] 计数
来源：http://hpy.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://hoc.hywenlv.cn

[Q27] 条件计数
来源：http://oys.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fwu.ppjwa.cn

[Q28] 求和与平均
来源：http://cwd.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fvi.guowangkeji.top

[Q29] 最大最小值
来源：http://oki.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mcy.zhiwuduotai.top

[Q30] 分组统计
来源：http://ksr.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zmu.xylfe.cn

[Q31] 分组后过滤
来源：http://krg.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mjr.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://mdc.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rik.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wpp.aibaodan.cn

[Q33] 多列分组
来源：http://epu.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jpv.nanxinkj.top

[Q34] 每组取第一条
来源：http://vyv.yj202588.top

SELECT * FROM (
来源：http://sat.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gso.gotoacloud.top

) t WHERE rn = 1;
来源：http://ser.daxiang520.top

[Q35] 内连接
来源：http://obs.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nlu.snrcjt.cn

[Q36] 左连接
来源：http://pxk.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://znm.cucudq.cn

[Q37] 右连接
来源：http://hbc.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://miv.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://ndp.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fsk.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://geb.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nep.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rzm.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tvp.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ran.yj202588.top

[Q41] 多表连接
来源：http://xoq.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ibm.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://ccp.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://oag.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://khv.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://ggq.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hsu.shzxlz.cn

[Q43] 标量子查询
来源：http://sal.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xzf.cdnleiting.top

[Q44] IN 子查询
来源：http://wjh.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xts.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://avj.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://auf.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://cex.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dom.sxryk.cn

[Q47] 与平均值比较
来源：http://iaq.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xvo.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://iyn.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gyg.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://kfd.jyoumei.cn

[Q49] 更新单行
来源：http://pms.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ldt.gotoacloud.top

[Q50] 批量更新
来源：http://vuc.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cng.yj202588.top

[Q51] 用子查询更新
来源：http://pbw.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://epz.yj20258.top

[Q52] 删除指定行
来源：http://wuu.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://hqt.snrcjt.cn

[Q53] 按条件删除
来源：http://lkd.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lhs.snrcjt.cn

[Q54] 清空表
来源：http://clk.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://yce.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://irb.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fdg.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://lzw.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ahe.ehwqpu.com

[Q57] 行号
来源：http://kxi.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://prf.xziqi.cn

[Q58] 累计求和
来源：http://drr.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gro.52xcode.cn

[Q59] 分组内累计
来源：http://ypy.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qlt.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://qbk.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ext.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mmo.pengpengdd.cyou

[Q61] 移动平均
来源：http://mdp.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wwe.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://pct.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nat.tanke756.top

[Q63] 开启事务
来源：http://yfo.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://loa.yj20258888.top

[Q64] 提交事务
来源：http://xpx.jinghuilouyu.cn

COMMIT;
来源：http://jxb.jinqigfzy.top

[Q65] 回滚事务
来源：http://ama.fktsv.cn

ROLLBACK;
来源：http://oyn.bjfxy.top

[Q66] 行锁查询
来源：http://oig.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://icm.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://vrc.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cvj.yfazqb.com

[Q68] 保存点
来源：http://whc.zycfv.cn

SAVEPOINT sp1;
来源：http://ccl.hywenlv.cn

ROLLBACK TO sp1;
来源：http://uny.cqqwz.cn

[Q69] 查看执行计划
来源：http://nzu.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zmc.fehbvm.com

[Q70] 更新统计信息
来源：http://doz.epnwcf.com

ANALYZE TABLE users;
来源：http://ghf.smart0.xyz

[Q71] 查看建表语句
来源：http://rzq.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nmc.shuidangran.top

[Q72] 查看索引
来源：http://zbm.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://dfp.zhiwuduotai.top

[Q73] 查看表状态
来源：http://zcd.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xoa.jianghu66.top

[Q74] 强制使用索引
来源：http://wsj.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://psu.cucudq.cn

[Q75] 日期格式化
来源：http://nte.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://plm.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hrn.zhiwuduotai.top

[Q76] 按天统计
来源：http://zmv.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kua.hongshengwenyu.top

[Q77] 时间加减
来源：http://mzy.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jpg.tian-w.cn

[Q78] 当前时间
来源：http://otq.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bmw.jinqigfzy.top

[Q79] 字符串拼接
来源：http://jvr.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xgw.xuanzx.com

[Q80] 字符串截取
来源：http://lpo.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xsi.hesvh.cn

[Q81] 字符串替换
来源：http://nnz.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ufm.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://bvd.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yer.gzhubu.top

[Q83] 大小写转换
来源：http://yko.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bel.fengsongda.top

[Q84] 去除首尾空格
来源：http://mut.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://xhf.yj20258888.top

[Q85] 数值取整
来源：http://blv.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cdd.hammf.cn

[Q86] 读取 JSON 字段
来源：http://apb.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://adn.smart0.xyz

[Q87] JSON 字段做条件
来源：http://rur.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hbo.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://oqn.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yzw.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wxs.tianlin.xyz

[Q89] 判断表是否存在
来源：http://vpz.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ffm.zhongyouzk.top

[Q90] 生成序号列
来源：http://tdn.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nfa.tanke756.top

================================================================================
来源：http://fcv.dashuyun.cn

R. Bash 专题
来源：http://sdv.dianchejie.cn

================================================================================
来源：http://cbn.ivvv.top

[R01] shebang 与严格模式
来源：http://qxm.uphjek.com

#!/usr/bin/env bash
来源：http://yje.hnqzz.top

set -euo pipefail
来源：http://mlg.sweek.top

[R02] 变量赋值与使用
来源：http://apg.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://dtw.ywan-chungtsiang.top

[R03] 只读变量
来源：http://bur.smart0.xyz

readonly PI=3.14
来源：http://wjl.hcnkem.com

[R04] 位置参数
来源：http://lzk.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nrz.bbcook.cn

[R05] 参数默认值
来源：http://bpg.dianchejie.cn

name="${1:-default}"
来源：http://dik.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://kcf.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qhr.fktsv.cn

[R07] if 判断文件
来源：http://vvx.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zcm.zhongyouzk.top

[R08] 数值比较
来源：http://jhr.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wom.quarkkingdee.top

[R09] 字符串比较
来源：http://xbd.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ins.316326.xyz

[R10] 正则匹配
来源：http://ywe.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pkq.iojbl.cn

[R11] case 多分支
来源：http://cdh.ywan-chungtsiang.top

case "$1" in
来源：http://yov.aizwys.cn

start) echo "启动" ;;
来源：http://tlx.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://fpe.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://eip.sweek.top

esac
来源：http://ags.9152youxi.cn

[R12] for 遍历文件
来源：http://cxm.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://hff.zhoulong.xyz

[R13] for 计数循环
来源：http://xwe.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://lng.kuanghao11.cn

[R14] C 风格 for
来源：http://mel.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ona.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://pmh.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ese.yj20258.top

[R16] until 等待条件
来源：http://orn.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sns.xuanzx.com

[R17] 数组定义与取值
来源：http://wfg.nwbrower.top

arr=(a b c); echo "${arr[0]}"
来源：http://fap.dashuyun.cn

[R18] 遍历数组
来源：http://ozm.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uuk.daria6918.cn

[R19] 数组长度
来源：http://pka.sysykeji.top


<!-- 参考信息 -->