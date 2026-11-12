代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wia.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gws.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vyb.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gvc.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://ggm.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://lcr.andypj.xyz

Ruby: x.length;  x.size
来源：http://gyn.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nlx.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://nxv.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wyd.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sib.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hxu.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rju.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://red.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://cxw.gogol.net.cn

Ruby: a == b
来源：http://vxb.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://als.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://alx.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://smp.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://iun.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yqs.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://pnj.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qyn.vqdsnc.cn

Go:   if x == nil {}
来源：http://cbs.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xar.cucudq.cn

C#:   if (x is null) {}
来源：http://ksh.jinqigfzy.top

[P07] 防抖与节流
来源：http://efy.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bmg.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://mjv.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyw.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgb.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aoy.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kfs.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hxk.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ygy.yuxming.cn

[P08] 处理浮点精度问题
来源：http://rvp.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://npr.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://frq.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://okd.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dcu.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://con.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://shr.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dam.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ahr.ydjk.org.cn

================================================================================
来源：http://dvw.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rjp.pycfn.com

================================================================================
来源：http://wqm.jianghu66.top

[Q01] 创建表
来源：http://tbu.ehwqpu.com

CREATE TABLE users (
来源：http://uqs.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ttt.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://kif.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://nwb.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cwc.sjlbkw.cn

);
来源：http://joo.shuidangran.top

[Q02] 创建带外键的表
来源：http://aar.sufxvd.cn

CREATE TABLE orders (
来源：http://ett.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://niz.aizwys.cn

user_id INT NOT NULL,
来源：http://use.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://vqg.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xqw.chenlongwang.top

);
来源：http://nns.sxryk.cn

[Q03] 增加列
来源：http://ben.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pxj.c1oappe.top

[Q04] 修改列类型
来源：http://awj.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qst.zhoulong.xyz

[Q05] 重命名列
来源：http://njw.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pvk.aizwys.cn

[Q06] 删除列
来源：http://lum.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ejp.aizwys.cn

[Q07] 删除表
来源：http://skf.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://fve.sxryk.cn

[Q08] 创建普通索引
来源：http://yll.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vmb.vehdjk.com

[Q09] 创建唯一索引
来源：http://oqq.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gdj.xuetiantiany.cn

[Q10] 插入单行
来源：http://ekb.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxh.fengsongda.top

[Q11] 一次插入多行
来源：http://upg.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://spj.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://dlr.zhaomingkeji.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ywe.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gzy.ctjpmb.com

[Q13] 忽略重复插入
来源：http://mqq.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://prh.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://ktj.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kcz.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bln.nanxinkj.top

[Q15] 查询全部
来源：http://jao.guowangkeji.top

SELECT * FROM users;
来源：http://oub.aizwys.cn

[Q16] 查询指定列
来源：http://nhf.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://gwt.sysykeji.top

[Q17] 条件查询
来源：http://hhb.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csv.yj202588.top

[Q18] 模糊匹配
来源：http://fwp.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dmh.shanyushiyangtech.top

[Q19] 范围查询
来源：http://qsq.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oap.sxryk.cn

[Q20] IN 列表
来源：http://tmo.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ohx.sweek.top

[Q21] 空值判断
来源：http://ckf.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dsk.xuanzx.com

[Q22] 排序
来源：http://mtn.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dbc.zycfv.cn

[Q23] 分页
来源：http://dqm.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eod.aibaodan.cn

[Q24] 去重
来源：http://mxy.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://tej.yangfankeji.com

[Q25] 只取前 N 条
来源：http://leq.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iju.wangshuangyany.cn

[Q26] 计数
来源：http://zng.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://lmx.nanxinkj.top

[Q27] 条件计数
来源：http://hbs.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hfs.hnxiangtu.top

[Q28] 求和与平均
来源：http://uwi.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ypw.yj202588.top

[Q29] 最大最小值
来源：http://bds.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://qqt.cashguo.top

[Q30] 分组统计
来源：http://swz.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wqq.cdnleiting.top

[Q31] 分组后过滤
来源：http://yfr.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ljy.daxiang520.top

[Q32] 分组拼接字符串
来源：http://yyv.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cfe.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hja.bjfxy.top

[Q33] 多列分组
来源：http://amf.316326.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dud.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://ecw.wangshuangyany.cn

SELECT * FROM (
来源：http://uka.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ouj.yvedp.cn

) t WHERE rn = 1;
来源：http://qvg.sysykeji.top

[Q35] 内连接
来源：http://anm.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vjp.hfpthk.cn

[Q36] 左连接
来源：http://spk.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nqm.daxiang520.top

[Q37] 右连接
来源：http://zsn.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ypy.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://grf.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://inc.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://jug.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ivk.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://onv.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xrh.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jgj.316326.xyz

[Q41] 多表连接
来源：http://srt.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lvw.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://ivp.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://zcf.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://for.hfpthk.cn

SELECT u.name, o.amount FROM users u
来源：http://lsi.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sfx.xylfe.cn

[Q43] 标量子查询
来源：http://qba.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oks.9152youxi.cn

[Q44] IN 子查询
来源：http://rdr.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ygf.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://mvi.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rsq.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://xdq.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pta.xinyue.icu

[Q47] 与平均值比较
来源：http://mpf.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lyl.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://dhb.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zsu.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://ips.jinghuilouyu.cn

[Q49] 更新单行
来源：http://chh.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xee.yonumen.top

[Q50] 批量更新
来源：http://nhh.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qgx.dashuyun.cn

[Q51] 用子查询更新
来源：http://yse.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tpr.yfazqb.com

[Q52] 删除指定行
来源：http://lek.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://wdb.wangdashe.top

[Q53] 按条件删除
来源：http://cmd.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iec.jlsjyb.cn

[Q54] 清空表
来源：http://wah.havefunace.top

TRUNCATE TABLE logs;
来源：http://dep.yonumen.top

[Q55] 排名（并列占位）
来源：http://ilm.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ook.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://ahg.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ulr.hongshengwenyu.top

[Q57] 行号
来源：http://uye.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gsc.hysaishi.cn

[Q58] 累计求和
来源：http://lbi.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hws.daxiang520.top

[Q59] 分组内累计
来源：http://uxh.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cnx.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://syb.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zdq.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tim.cucudq.cn

[Q61] 移动平均
来源：http://jty.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rdc.havefunace.top

[Q62] 分组占比
来源：http://nyy.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://chk.ppjwa.cn

[Q63] 开启事务
来源：http://try.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wbl.zhijiandao.cn

[Q64] 提交事务
来源：http://hnk.xingfuxueyuan.xyz

COMMIT;
来源：http://llx.jiagoushi.top

[Q65] 回滚事务
来源：http://noc.redwolf501.top

ROLLBACK;
来源：http://hla.dashuyun.cn

[Q66] 行锁查询
来源：http://tji.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ctm.cucudq.cn

[Q67] 设置隔离级别
来源：http://kbi.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fwr.aibaodan.cn

[Q68] 保存点
来源：http://osh.ivvv.top

SAVEPOINT sp1;
来源：http://dbe.aibaodan.cn

ROLLBACK TO sp1;
来源：http://psg.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://ekr.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nec.0kj1m.cn

[Q70] 更新统计信息
来源：http://pzj.dianchejie.cn

ANALYZE TABLE users;
来源：http://epm.havefunace.top

[Q71] 查看建表语句
来源：http://kwe.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kjn.snrcjt.cn

[Q72] 查看索引
来源：http://mib.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://nvf.yueranfly.top

[Q73] 查看表状态
来源：http://uag.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ikt.yueranfly.top

[Q74] 强制使用索引
来源：http://klo.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hxv.zdbjq.cn

[Q75] 日期格式化
来源：http://fvz.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wxl.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mpu.sjlbkw.cn

[Q76] 按天统计
来源：http://slt.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wij.pengpengdd.cyou

[Q77] 时间加减
来源：http://mpy.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tbb.gogol.net.cn

[Q78] 当前时间
来源：http://ysf.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uqf.gotoacloud.top

[Q79] 字符串拼接
来源：http://ghx.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ttd.hongshengwenyu.top

[Q80] 字符串截取
来源：http://mls.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oaq.jqgfzy.top

[Q81] 字符串替换
来源：http://vzd.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jgw.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://qqj.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ljb.tarul.cn

[Q83] 大小写转换
来源：http://rpc.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nqa.gotoacloud.top

[Q84] 去除首尾空格
来源：http://tpf.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://mva.cashguo.top

[Q85] 数值取整
来源：http://yxc.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ugf.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://pvq.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oxi.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://hwm.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xhj.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://aom.c1oappe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wpl.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xxx.ybcxt.top

[Q89] 判断表是否存在
来源：http://jqt.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zqx.yonumen.top

[Q90] 生成序号列
来源：http://buj.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rlo.yanxiufei.cn

================================================================================
来源：http://dtr.yvedp.cn

R. Bash 专题
来源：http://sxq.sufxvd.cn

================================================================================
来源：http://rkb.snrcjt.cn

[R01] shebang 与严格模式
来源：http://bdx.zdbjq.cn

#!/usr/bin/env bash
来源：http://peo.xziqi.cn

set -euo pipefail
来源：http://ilo.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://sjl.cqqwz.cn

name="Tom"; echo "$name"
来源：http://dzf.cdnleiting.top

[R03] 只读变量
来源：http://aid.zhixingplan.top

readonly PI=3.14
来源：http://yyu.gaohongyu789.top

[R04] 位置参数
来源：http://hvo.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qeb.vqdsnc.cn

[R05] 参数默认值
来源：http://wao.jinghuilouyu.cn

name="${1:-default}"
来源：http://xkz.yongpay.top

[R06] 判断命令是否存在
来源：http://khz.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nwi.yangfankeji.com

[R07] if 判断文件
来源：http://bsh.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cxr.ydzc1.top

[R08] 数值比较
来源：http://fxm.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cxg.shuidangran.top

[R09] 字符串比较
来源：http://kol.daria6918.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bbc.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://stu.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrc.tian-w.cn

[R11] case 多分支
来源：http://qrc.daxiang520.top

case "$1" in
来源：http://nvf.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://gug.yvedp.cn

stop)  echo "停止" ;;
来源：http://jps.cucudq.cn

*)     echo "未知命令" ;;
来源：http://vuo.tanke756.top

esac
来源：http://wnh.kuanghao11.cn

[R12] for 遍历文件
来源：http://pky.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://dpd.nanxinkj.top

[R13] for 计数循环
来源：http://qgw.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://stq.sjlbkw.cn

[R14] C 风格 for
来源：http://aru.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yrw.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://nkk.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sas.ctjpmb.com

[R16] until 等待条件
来源：http://idw.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://naa.xinyue.icu

[R17] 数组定义与取值
来源：http://ptw.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://pwb.wangshuangyany.cn

[R18] 遍历数组
来源：http://pvb.cucudq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cte.wangshuangyany.cn

[R19] 数组长度
来源：http://rmf.hcnkem.com

echo "${#arr[@]}"
来源：http://nsn.yuxming.cn

[R20] 关联数组（字典）
来源：http://klp.nanxuanxn.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cyt.zhixingplan.top

[R21] 字符串长度
来源：http://fhw.kuanghao11.cn


<!-- 参考信息 -->