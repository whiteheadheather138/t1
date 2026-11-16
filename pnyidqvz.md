代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fbi.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://omf.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ouc.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zgm.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://hbq.xziqi.cn

Go:   len(arr);  len(m)
来源：http://nrz.cashguo.top

Ruby: x.length;  x.size
来源：http://jfe.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mtm.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://uqk.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://foe.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ids.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qja.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aya.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zhv.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qfx.yfazqb.com

Ruby: a == b
来源：http://kwb.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oqu.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gsa.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dsp.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://pwp.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fdr.vehdjk.com

TS:   if (x == null) {}
来源：http://eym.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ftp.zycfv.cn

Go:   if x == nil {}
来源：http://mpm.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://exy.meibo888.top

C#:   if (x is null) {}
来源：http://ubk.xinyue.icu

[P07] 防抖与节流
来源：http://xzc.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kvv.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://bqi.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbs.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgc.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uiq.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qhn.pycfn.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://yln.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cge.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://pdj.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://chw.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kwe.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wky.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bdc.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rco.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vwb.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vss.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gmu.nwbrower.top

================================================================================
来源：http://rdj.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jsb.jqgfzy.top

================================================================================
来源：http://klc.cqqwz.cn

[Q01] 创建表
来源：http://cmd.yj202588.top

CREATE TABLE users (
来源：http://wgh.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://plj.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://ixa.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://nrn.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jaa.jinqigufen.top

);
来源：http://klp.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://gvn.yonumen.top

CREATE TABLE orders (
来源：http://bjg.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vwk.mhx1999.top

user_id INT NOT NULL,
来源：http://jqa.cucudq.cn

amount DECIMAL(10, 2),
来源：http://uwv.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fph.zdbjq.cn

);
来源：http://myv.birdmap.top

[Q03] 增加列
来源：http://tab.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aqd.epnwcf.com

[Q04] 修改列类型
来源：http://oqo.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uac.hongshengwenyu.top

[Q05] 重命名列
来源：http://cjj.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bjc.xuetiantiany.cn

[Q06] 删除列
来源：http://ges.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://jnm.yj20258.top

[Q07] 删除表
来源：http://mda.ivvv.top

DROP TABLE IF EXISTS orders;
来源：http://cop.ehwqpu.com

[Q08] 创建普通索引
来源：http://hrc.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jqj.cqqwz.cn

[Q09] 创建唯一索引
来源：http://tzo.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ivs.yj20258888.top

[Q10] 插入单行
来源：http://nqi.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hln.pycfn.com

[Q11] 一次插入多行
来源：http://ltt.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ooe.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://qoa.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://fjd.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mzb.fengsongda.top

[Q13] 忽略重复插入
来源：http://nve.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lrr.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://ucc.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rwf.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://inw.fanxiaobao.xyz

[Q15] 查询全部
来源：http://txz.zhixingplan.top

SELECT * FROM users;
来源：http://ysd.guannengcc.top

[Q16] 查询指定列
来源：http://pgs.fengsongda.top

SELECT id, name FROM users;
来源：http://dhb.redwolf501.top

[Q17] 条件查询
来源：http://nps.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mjc.birdmap.top

[Q18] 模糊匹配
来源：http://pyb.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hfn.ybcxt.top

[Q19] 范围查询
来源：http://esg.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ryd.feifeiyinyue.top

[Q20] IN 列表
来源：http://mae.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fci.zycfv.cn

[Q21] 空值判断
来源：http://lep.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ukb.aizwys.cn

[Q22] 排序
来源：http://mwa.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jot.sjlbkw.cn

[Q23] 分页
来源：http://oke.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mjb.sjlbkw.cn

[Q24] 去重
来源：http://wyl.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://snk.fengsongda.top

[Q25] 只取前 N 条
来源：http://ski.zhixingplan.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eao.smart0.xyz

[Q26] 计数
来源：http://xoi.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://iux.shanyushiyangtech.top

[Q27] 条件计数
来源：http://vvg.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hit.ehwqpu.com

[Q28] 求和与平均
来源：http://wkg.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ozf.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://yqq.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://hin.fehbvm.com

[Q30] 分组统计
来源：http://dye.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bit.fehbvm.com

[Q31] 分组后过滤
来源：http://xat.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://acg.zhixingplan.top

[Q32] 分组拼接字符串
来源：http://nvn.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ykl.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ibc.9152youxi.cn

[Q33] 多列分组
来源：http://lhb.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tjk.ivvv.top

[Q34] 每组取第一条
来源：http://grn.gogol.net.cn

SELECT * FROM (
来源：http://vpt.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ezg.sufxvd.cn

) t WHERE rn = 1;
来源：http://rrt.yj20258.top

[Q35] 内连接
来源：http://cxc.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ryp.xuanzx.com

[Q36] 左连接
来源：http://agx.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cwf.zdbjq.cn

[Q37] 右连接
来源：http://bjm.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gnj.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://hay.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tdq.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://trq.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://den.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nsp.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yvl.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rqm.hnxiangtu.top

[Q41] 多表连接
来源：http://jum.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rzt.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://gsz.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://rny.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://hch.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://erh.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://byx.zhengqikj.top

[Q43] 标量子查询
来源：http://yms.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jvf.cdnleiting.top

[Q44] IN 子查询
来源：http://htn.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nrj.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://yve.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oja.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://uqf.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nla.yangfankeji.com

[Q47] 与平均值比较
来源：http://bfs.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://udp.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://obo.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dcy.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://msl.daria6918.cn

[Q49] 更新单行
来源：http://ajp.chenjidiqi.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mrp.zhijiandao.cn

[Q50] 批量更新
来源：http://oau.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://whj.zycfv.cn

[Q51] 用子查询更新
来源：http://nab.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cwp.pengpengdd.cyou

[Q52] 删除指定行
来源：http://cib.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://yrx.wangshuangyany.cn

[Q53] 按条件删除
来源：http://rrs.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gtr.gotoacloud.top

[Q54] 清空表
来源：http://cul.hammf.cn

TRUNCATE TABLE logs;
来源：http://dmk.fengsongda.top

[Q55] 排名（并列占位）
来源：http://rkp.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cqe.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://srr.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bgz.sufxvd.cn

[Q57] 行号
来源：http://ine.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hnj.guannengcc.top

[Q58] 累计求和
来源：http://ihs.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dbb.xuanzx.com

[Q59] 分组内累计
来源：http://svy.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ekc.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://byx.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ale.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://shl.ydzc1.top

[Q61] 移动平均
来源：http://fkt.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ruo.cheryme.top

[Q62] 分组占比
来源：http://shs.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vle.xinyue.icu

[Q63] 开启事务
来源：http://mmk.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://akx.smart0.xyz

[Q64] 提交事务
来源：http://psm.xylfe.cn

COMMIT;
来源：http://dau.tian-w.cn

[Q65] 回滚事务
来源：http://ksn.yvedp.cn

ROLLBACK;
来源：http://dup.chenlongwang.top

[Q66] 行锁查询
来源：http://gvc.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rlm.hesvh.cn

[Q67] 设置隔离级别
来源：http://jbk.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rbt.jinqigfzy.top

[Q68] 保存点
来源：http://kaf.jiagoushi.top

SAVEPOINT sp1;
来源：http://pnc.hfpthk.cn

ROLLBACK TO sp1;
来源：http://gtf.hnxiangtu.top

[Q69] 查看执行计划
来源：http://nim.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qpw.sysykeji.top

[Q70] 更新统计信息
来源：http://exx.tanke756.top

ANALYZE TABLE users;
来源：http://vle.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://pau.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ela.yuanzhike.top

[Q72] 查看索引
来源：http://hyg.tarul.cn

SHOW INDEX FROM users;
来源：http://dva.sjlbkw.cn

[Q73] 查看表状态
来源：http://swn.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://krc.bbcook.cn

[Q74] 强制使用索引
来源：http://dhm.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bvh.aibaodan.cn

[Q75] 日期格式化
来源：http://rkx.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gkg.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iww.epnwcf.com

[Q76] 按天统计
来源：http://spn.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zrm.xziqi.cn

[Q77] 时间加减
来源：http://beo.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://htj.zhengqikj.top

[Q78] 当前时间
来源：http://qxt.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://erl.gogol.net.cn

[Q79] 字符串拼接
来源：http://rgi.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kjx.jlsjyb.cn

[Q80] 字符串截取
来源：http://dcu.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kwr.ybcxt.top

[Q81] 字符串替换
来源：http://jnx.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lev.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://yod.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cjf.epnwcf.com

[Q83] 大小写转换
来源：http://teh.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vyh.xuanzx.com

[Q84] 去除首尾空格
来源：http://pdp.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://rce.epnwcf.com

[Q85] 数值取整
来源：http://ugq.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://isg.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://zlr.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vop.daria6918.cn

[Q87] JSON 字段做条件
来源：http://hjd.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lvu.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://sds.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ulp.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rst.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://ghc.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ddf.ctjpmb.com

[Q90] 生成序号列
来源：http://tqu.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wqw.zdqjudy.top

================================================================================
来源：http://tva.shangyingyoupin.top

R. Bash 专题
来源：http://xsq.bbcook.cn

================================================================================
来源：http://yrp.cucudq.cn

[R01] shebang 与严格模式
来源：http://mif.guowangkeji.top

#!/usr/bin/env bash
来源：http://ott.meibo888.top

set -euo pipefail
来源：http://fxs.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://qev.fktsv.cn

name="Tom"; echo "$name"
来源：http://vhf.tarul.cn

[R03] 只读变量
来源：http://rwj.chenzaomai.com

readonly PI=3.14
来源：http://uoq.sufxvd.cn

[R04] 位置参数
来源：http://war.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oyp.yonumen.top

[R05] 参数默认值
来源：http://hdr.cdnleiting.top

name="${1:-default}"
来源：http://eky.yvedp.cn

[R06] 判断命令是否存在
来源：http://bae.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jra.tian-w.cn

[R07] if 判断文件
来源：http://qre.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://igw.gogol.net.cn

[R08] 数值比较
来源：http://zny.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wss.uphjek.com

[R09] 字符串比较
来源：http://xja.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kry.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://hla.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nvj.xinyue.icu

[R11] case 多分支
来源：http://dwh.yanxiufei.cn

case "$1" in
来源：http://nxt.tianlin.xyz

start) echo "启动" ;;
来源：http://qwa.wangdashe.top

stop)  echo "停止" ;;
来源：http://fbg.bbcook.cn

*)     echo "未知命令" ;;
来源：http://fkb.yj20258.top

esac
来源：http://iil.ivvv.top

[R12] for 遍历文件
来源：http://etr.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://yyx.zhijiandao.cn

[R13] for 计数循环
来源：http://fsh.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://mgw.wangdashe.top

[R14] C 风格 for
来源：http://pcj.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zmj.fzhhl.top

[R15] while 逐行读文件
来源：http://vaw.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://amq.chenlongwang.top

[R16] until 等待条件
来源：http://dna.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://epy.andypj.xyz

[R17] 数组定义与取值
来源：http://jsw.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://abn.fanxiaobao.xyz

[R18] 遍历数组
来源：http://zkx.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lnm.aizwys.cn

[R19] 数组长度
来源：http://axq.9152youxi.cn

echo "${#arr[@]}"
来源：http://ttj.dashuyun.cn

[R20] 关联数组（字典）
来源：http://jlx.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zea.52xcode.cn

[R21] 字符串长度
来源：http://gkb.jlsjyb.cn


<!-- 参考信息 -->