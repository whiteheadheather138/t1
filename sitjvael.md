代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://agx.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zhf.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ppc.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sun.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://syv.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://sdb.zhixingplan.top

Ruby: x.length;  x.size
来源：http://smn.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://afa.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://fdr.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kcg.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lhs.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rww.yvedp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vqv.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yoc.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tta.ehwqpu.com

Ruby: a == b
来源：http://hit.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qct.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xss.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oxj.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://qan.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lpf.sxryk.cn

TS:   if (x == null) {}
来源：http://amc.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://scf.aizwys.cn

Go:   if x == nil {}
来源：http://pca.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ysd.ppjwa.cn

C#:   if (x is null) {}
来源：http://urh.ehwqpu.com

[P07] 防抖与节流
来源：http://fup.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lwq.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://ppg.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dsi.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yrz.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jyr.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nub.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gdc.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pnr.bjfxy.top

[P08] 处理浮点精度问题
来源：http://gbb.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hho.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zwz.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xdc.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rhr.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://egu.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwy.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sbt.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dar.chenlongwang.top

================================================================================
来源：http://mla.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fhx.jyoumei.cn

================================================================================
来源：http://sqw.zdbjq.cn

[Q01] 创建表
来源：http://cxi.xuanzx.com

CREATE TABLE users (
来源：http://bxm.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mti.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://hbq.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://oub.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ipu.andypj.xyz

);
来源：http://nec.yonumen.top

[Q02] 创建带外键的表
来源：http://nsf.bbcook.cn

CREATE TABLE orders (
来源：http://yzu.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfz.hfpthk.cn

user_id INT NOT NULL,
来源：http://ztx.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://iqw.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cdq.tanke756.top

);
来源：http://pnu.shzxlz.cn

[Q03] 增加列
来源：http://zch.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdw.snrcjt.cn

[Q04] 修改列类型
来源：http://aan.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xck.zhengqikj.top

[Q05] 重命名列
来源：http://qbd.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rrz.fanxiaobao.xyz

[Q06] 删除列
来源：http://flm.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://gss.sysykeji.top

[Q07] 删除表
来源：http://tqg.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://uxu.zhengqikj.top

[Q08] 创建普通索引
来源：http://iph.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hnx.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://bld.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nys.hammf.cn

[Q10] 插入单行
来源：http://lbh.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wyh.zycfv.cn

[Q11] 一次插入多行
来源：http://ynl.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ztj.uphjek.com

[Q12] 插入后取自增 ID
来源：http://huj.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://brm.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uvt.yangfankeji.com

[Q13] 忽略重复插入
来源：http://qkh.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bfu.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://wql.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kdc.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dyf.zdbjq.cn

[Q15] 查询全部
来源：http://cnp.gogol.net.cn

SELECT * FROM users;
来源：http://jkt.sufxvd.cn

[Q16] 查询指定列
来源：http://wrk.epnwcf.com

SELECT id, name FROM users;
来源：http://unh.jinqigufen.top

[Q17] 条件查询
来源：http://bnw.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iur.aibaodan.cn

[Q18] 模糊匹配
来源：http://gdv.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mwf.bjfxy.top

[Q19] 范围查询
来源：http://orc.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bjk.vqdsnc.cn

[Q20] IN 列表
来源：http://zsf.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hwo.xinyue.icu

[Q21] 空值判断
来源：http://eyj.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://koo.yuanzhike.top

[Q22] 排序
来源：http://osb.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://han.cqqwz.cn

[Q23] 分页
来源：http://tor.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qvu.zdqjudy.top

[Q24] 去重
来源：http://qna.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://wbt.vehdjk.com

[Q25] 只取前 N 条
来源：http://yix.ivvv.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qdf.vehdjk.com

[Q26] 计数
来源：http://rmi.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://skz.xuetiantiany.cn

[Q27] 条件计数
来源：http://jdy.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aoj.fktsv.cn

[Q28] 求和与平均
来源：http://llt.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tqb.cqqwz.cn

[Q29] 最大最小值
来源：http://mwn.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://saw.jlsjyb.cn

[Q30] 分组统计
来源：http://vds.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ubz.meibo888.top

[Q31] 分组后过滤
来源：http://dqn.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wla.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://cay.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uvu.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bme.hysaishi.cn

[Q33] 多列分组
来源：http://ygp.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://stt.epnwcf.com

[Q34] 每组取第一条
来源：http://zmj.zhixingplan.top

SELECT * FROM (
来源：http://ixm.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://unf.tian-w.cn

) t WHERE rn = 1;
来源：http://tmp.yuanzhike.top

[Q35] 内连接
来源：http://ymp.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zhq.mhx1999.top

[Q36] 左连接
来源：http://mrv.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xyw.yj202588.top

[Q37] 右连接
来源：http://byb.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pru.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://vgf.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://buo.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://gmf.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pgb.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rhk.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fug.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pli.fengsongda.top

[Q41] 多表连接
来源：http://sht.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ddt.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://xlu.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://izs.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://zsg.guannengcc.top

SELECT u.name, o.amount FROM users u
来源：http://jkv.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://enk.pengpengdd.cyou

[Q43] 标量子查询
来源：http://kjt.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://apx.jianghu66.top

[Q44] IN 子查询
来源：http://ymg.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ypt.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://uck.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tla.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://ddj.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aqs.ctjpmb.com

[Q47] 与平均值比较
来源：http://rpn.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cpg.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://ryl.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nlb.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://nxw.sxryk.cn

[Q49] 更新单行
来源：http://bzm.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://apd.hnxiangtu.top

[Q50] 批量更新
来源：http://sds.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ore.c1oappe.top

[Q51] 用子查询更新
来源：http://knq.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://clp.yuanzhike.top

[Q52] 删除指定行
来源：http://wea.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://whp.yuxming.cn

[Q53] 按条件删除
来源：http://aqu.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://scm.chenjidiqi.icu

[Q54] 清空表
来源：http://qpr.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://pvi.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://yic.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qom.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://alh.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ijt.chenlongwang.top

[Q57] 行号
来源：http://ghw.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dtw.yfazqb.com

[Q58] 累计求和
来源：http://bxm.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://shg.9152youxi.cn

[Q59] 分组内累计
来源：http://inw.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ept.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://yzt.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nrp.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qdp.yanxiufei.cn

[Q61] 移动平均
来源：http://ipy.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uqv.316326.xyz

[Q62] 分组占比
来源：http://cct.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kdd.yfazqb.com

[Q63] 开启事务
来源：http://zhh.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://cyw.xylfe.cn

[Q64] 提交事务
来源：http://iju.nwbrower.top

COMMIT;
来源：http://lvp.316326.xyz

[Q65] 回滚事务
来源：http://wjh.316326.xyz

ROLLBACK;
来源：http://udx.9152youxi.cn

[Q66] 行锁查询
来源：http://rpm.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nda.smart0.xyz

[Q67] 设置隔离级别
来源：http://ttc.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eqi.bjfxy.top

[Q68] 保存点
来源：http://ygw.xinyue.icu

SAVEPOINT sp1;
来源：http://nwb.vehdjk.com

ROLLBACK TO sp1;
来源：http://kzr.yongpay.top

[Q69] 查看执行计划
来源：http://gae.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zic.9152youxi.cn

[Q70] 更新统计信息
来源：http://dzr.9152youxi.cn

ANALYZE TABLE users;
来源：http://xbp.birdmap.top

[Q71] 查看建表语句
来源：http://kyn.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://khb.sweek.top

[Q72] 查看索引
来源：http://szz.sxryk.cn

SHOW INDEX FROM users;
来源：http://bwf.gzhubu.top

[Q73] 查看表状态
来源：http://pyk.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://szv.xinyue.icu

[Q74] 强制使用索引
来源：http://bdb.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://toh.zdqjudy.top

[Q75] 日期格式化
来源：http://uxo.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mja.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fqm.svipenyu.cn

[Q76] 按天统计
来源：http://pem.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gif.316326.xyz

[Q77] 时间加减
来源：http://aqi.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://csp.hnqzz.top

[Q78] 当前时间
来源：http://cuo.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zug.meibo888.top

[Q79] 字符串拼接
来源：http://ult.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zdx.hongshengwenyu.top

[Q80] 字符串截取
来源：http://bgg.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kcx.jiagoushi.top

[Q81] 字符串替换
来源：http://fpv.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jzq.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://wja.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kce.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://umy.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gis.ctjpmb.com

[Q84] 去除首尾空格
来源：http://dur.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://whx.smart0.xyz

[Q85] 数值取整
来源：http://hcs.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ifx.jqgfzy.top

[Q86] 读取 JSON 字段
来源：http://gzu.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tez.tian-w.cn

[Q87] JSON 字段做条件
来源：http://aqp.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ztj.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://xqk.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tom.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hzl.haohaochexian.top

[Q89] 判断表是否存在
来源：http://wor.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vwn.hywenlv.cn

[Q90] 生成序号列
来源：http://bmq.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cvb.birdmap.top

================================================================================
来源：http://odz.nanxuanxn.top

R. Bash 专题
来源：http://xub.guannengcc.top

================================================================================
来源：http://ftk.nwbrower.top

[R01] shebang 与严格模式
来源：http://hoq.shzxlz.cn

#!/usr/bin/env bash
来源：http://hlm.daria6918.cn

set -euo pipefail
来源：http://awu.jyoumei.cn

[R02] 变量赋值与使用
来源：http://tqb.nwbrower.top

name="Tom"; echo "$name"
来源：http://bpu.jlsjyb.cn

[R03] 只读变量
来源：http://cft.wangdashe.top

readonly PI=3.14
来源：http://flf.haohaochexian.top

[R04] 位置参数
来源：http://mve.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qys.vqdsnc.cn

[R05] 参数默认值
来源：http://abg.ydzc1.top

name="${1:-default}"
来源：http://qxo.yonumen.top

[R06] 判断命令是否存在
来源：http://qyl.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzz.ydjk.org.cn

[R07] if 判断文件
来源：http://qix.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wou.yvedp.cn

[R08] 数值比较
来源：http://cqw.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zbd.yongpay.top

[R09] 字符串比较
来源：http://crp.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tio.ivvv.top

[R10] 正则匹配
来源：http://nqc.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gjl.shanyushiyangtech.top

[R11] case 多分支
来源：http://efw.cheryme.top

case "$1" in
来源：http://qcy.snrcjt.cn

start) echo "启动" ;;
来源：http://jyc.nwbrower.top

stop)  echo "停止" ;;
来源：http://svl.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://dne.zdqjudy.top

esac
来源：http://ets.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://hrk.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://apn.aibaodan.cn

[R13] for 计数循环
来源：http://ymx.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://rwc.zhoulong.xyz

[R14] C 风格 for
来源：http://ynj.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tcf.0kj1m.cn

[R15] while 逐行读文件
来源：http://dwi.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://npe.9152youxi.cn

[R16] until 等待条件
来源：http://jkd.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ecn.jyoumei.cn

[R17] 数组定义与取值
来源：http://xdb.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xtr.nwbrower.top

[R18] 遍历数组
来源：http://jew.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nhj.9152youxi.cn

[R19] 数组长度
来源：http://nhi.guowangkeji.top

echo "${#arr[@]}"
来源：http://tmb.yangfankeji.com

[R20] 关联数组（字典）
来源：http://xvy.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://abt.zhengqikj.top

[R21] 字符串长度
来源：http://zei.quarkkingdee.top


<!-- 参考信息 -->