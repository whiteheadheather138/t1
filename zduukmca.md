代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rmv.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxh.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://biy.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zmg.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://upz.guannengcc.top

Go:   len(arr);  len(m)
来源：http://rdz.cdnleiting.top

Ruby: x.length;  x.size
来源：http://yvf.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gah.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://spt.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hbl.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uxh.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ewc.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cis.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aqw.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wgj.xinyue.icu

Ruby: a == b
来源：http://spe.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fos.gogol.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eoy.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://syl.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://hlp.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uyd.yonumen.top

TS:   if (x == null) {}
来源：http://blt.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://epa.tianlin.xyz

Go:   if x == nil {}
来源：http://khl.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xrr.yangfankeji.com

C#:   if (x is null) {}
来源：http://ubd.316326.xyz

[P07] 防抖与节流
来源：http://poa.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hry.c1oappe.top

PHP:  // 手写时间戳比较
来源：http://pjv.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sri.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xlt.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ral.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jbp.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://jzw.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://llb.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://vtd.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ela.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bau.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aob.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://srq.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nji.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cky.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lwy.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dvs.zhongyouzk.top

================================================================================
来源：http://mow.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivh.zhaomingkeji.xyz

================================================================================
来源：http://tys.yueranfly.top

[Q01] 创建表
来源：http://rbr.yvedp.cn

CREATE TABLE users (
来源：http://tgr.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pnk.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://bdk.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://krw.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mky.gzhubu.top

);
来源：http://sqq.cheryme.top

[Q02] 创建带外键的表
来源：http://ejy.chenjidiqi.icu

CREATE TABLE orders (
来源：http://zgm.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nti.yfazqb.com

user_id INT NOT NULL,
来源：http://fph.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://xeq.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xmp.fanxiaobao.xyz

);
来源：http://gue.zhaomingkeji.xyz

[Q03] 增加列
来源：http://iqx.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bye.sweek.top

[Q04] 修改列类型
来源：http://suv.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ykq.zycfv.cn

[Q05] 重命名列
来源：http://cza.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mxf.aibaodan.cn

[Q06] 删除列
来源：http://xid.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://reu.xylfe.cn

[Q07] 删除表
来源：http://hov.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://pzx.tianlin.xyz

[Q08] 创建普通索引
来源：http://klt.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://shr.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://awn.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nsy.xuanzx.com

[Q10] 插入单行
来源：http://ssk.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fuo.meibo888.top

[Q11] 一次插入多行
来源：http://zip.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fkn.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://jtr.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://jls.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ijc.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://ywl.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zoe.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://bfj.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cjw.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://chv.chenjidiqi.icu

[Q15] 查询全部
来源：http://ciy.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://yoh.svipenyu.cn

[Q16] 查询指定列
来源：http://ivv.iojbl.cn

SELECT id, name FROM users;
来源：http://tzz.pycfn.com

[Q17] 条件查询
来源：http://hgy.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dkk.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://uqo.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://trn.redwolf501.top

[Q19] 范围查询
来源：http://dlb.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nwf.cashguo.top

[Q20] IN 列表
来源：http://iyu.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gao.chenlongwang.top

[Q21] 空值判断
来源：http://kcn.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aee.wangshuangyany.cn

[Q22] 排序
来源：http://wms.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bhr.vqdsnc.cn

[Q23] 分页
来源：http://yxo.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://svg.zhengqikj.top

[Q24] 去重
来源：http://amy.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://sws.ctjpmb.com

[Q25] 只取前 N 条
来源：http://yry.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tip.hammf.cn

[Q26] 计数
来源：http://axk.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://wez.yuxming.cn

[Q27] 条件计数
来源：http://zmr.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xgp.316326.xyz

[Q28] 求和与平均
来源：http://nyj.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://efc.fehbvm.com

[Q29] 最大最小值
来源：http://ozf.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://syg.iojbl.cn

[Q30] 分组统计
来源：http://nfb.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gkd.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://zlr.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ryl.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://imh.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ywg.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gxh.yj20258.top

[Q33] 多列分组
来源：http://pqp.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dyp.uphjek.com

[Q34] 每组取第一条
来源：http://udl.havefunace.top

SELECT * FROM (
来源：http://zpa.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pwb.dianchejie.cn

) t WHERE rn = 1;
来源：http://nmn.ybcxt.top

[Q35] 内连接
来源：http://fhk.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ifv.havefunace.top

[Q36] 左连接
来源：http://kjc.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xhi.vqdsnc.cn

[Q37] 右连接
来源：http://dur.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ryh.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mjw.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mix.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://icg.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kbj.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://udp.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jms.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xbh.tanke756.top

[Q41] 多表连接
来源：http://hrv.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://ane.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://iot.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://bdx.tanke756.top

[Q42] 连接条件附加过滤
来源：http://sbe.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://asp.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nvr.jinqigufen.top

[Q43] 标量子查询
来源：http://zdm.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wig.shuidangran.top

[Q44] IN 子查询
来源：http://hvk.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ykg.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://lts.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gzy.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ebq.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mif.guowangkeji.top

[Q47] 与平均值比较
来源：http://xif.yj20258888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xzi.cheryme.top

[Q48] CTE 公用表表达式
来源：http://ftq.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iif.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://fsh.svipenyu.cn

[Q49] 更新单行
来源：http://kfq.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rqk.c1oappe.top

[Q50] 批量更新
来源：http://vzo.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dwl.hesvh.cn

[Q51] 用子查询更新
来源：http://zwc.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://omt.zhijiandao.cn

[Q52] 删除指定行
来源：http://ori.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://nxh.cqqwz.cn

[Q53] 按条件删除
来源：http://jeb.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nsh.xuanzx.com

[Q54] 清空表
来源：http://dej.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://bjo.yfazqb.com

[Q55] 排名（并列占位）
来源：http://puv.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gcr.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://hsr.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tyy.jinghuilouyu.cn

[Q57] 行号
来源：http://ftv.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://loj.shzxlz.cn

[Q58] 累计求和
来源：http://ohb.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://flw.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://nvh.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gka.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://hzd.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jup.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jwf.sufxvd.cn

[Q61] 移动平均
来源：http://tmx.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zjt.c1oappe.top

[Q62] 分组占比
来源：http://ows.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://axs.snrcjt.cn

[Q63] 开启事务
来源：http://tpc.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vxm.shangyingyoupin.top

[Q64] 提交事务
来源：http://vin.jqgufenzy.top

COMMIT;
来源：http://brg.shzxlz.cn

[Q65] 回滚事务
来源：http://ani.tanke756.top

ROLLBACK;
来源：http://czh.yuxming.cn

[Q66] 行锁查询
来源：http://xow.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wsf.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://rhe.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://glf.zhengqikj.top

[Q68] 保存点
来源：http://zlv.jiagoushi.top

SAVEPOINT sp1;
来源：http://ked.tianlin.xyz

ROLLBACK TO sp1;
来源：http://ivn.uphjek.com

[Q69] 查看执行计划
来源：http://dyo.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kip.c1oappe.top

[Q70] 更新统计信息
来源：http://frw.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://zpi.uphjek.com

[Q71] 查看建表语句
来源：http://uhg.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gnq.9152youxi.cn

[Q72] 查看索引
来源：http://epz.xinyue.icu

SHOW INDEX FROM users;
来源：http://gqw.hesvh.cn

[Q73] 查看表状态
来源：http://cts.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zpe.bjfxy.top

[Q74] 强制使用索引
来源：http://cae.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lnn.sjlbkw.cn

[Q75] 日期格式化
来源：http://dms.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nlx.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bin.zhengqikj.top

[Q76] 按天统计
来源：http://eau.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vvp.uphjek.com

[Q77] 时间加减
来源：http://jof.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ohu.hywenlv.cn

[Q78] 当前时间
来源：http://tgo.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ety.sysykeji.top

[Q79] 字符串拼接
来源：http://sct.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cub.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://xrc.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hob.yuxming.cn

[Q81] 字符串替换
来源：http://aco.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bkr.yj202588.top

[Q82] 字符长度与字节长度
来源：http://zkg.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bki.vqdsnc.cn

[Q83] 大小写转换
来源：http://iqv.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eby.9152youxi.cn

[Q84] 去除首尾空格
来源：http://xrr.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://mhs.quarkkingdee.top

[Q85] 数值取整
来源：http://dmi.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfh.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://aij.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mdk.ehwqpu.com

[Q87] JSON 字段做条件
来源：http://wlq.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hgf.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://rrm.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ahd.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vez.tanke756.top

[Q89] 判断表是否存在
来源：http://qab.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mhv.zhixingplan.top

[Q90] 生成序号列
来源：http://pss.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wih.tanke756.top

================================================================================
来源：http://ewr.wangdashe.top

R. Bash 专题
来源：http://bvd.fzhhl.top

================================================================================
来源：http://mcr.cashguo.top

[R01] shebang 与严格模式
来源：http://rne.sjlbkw.cn

#!/usr/bin/env bash
来源：http://ejo.xuetiantiany.cn

set -euo pipefail
来源：http://vit.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://sxq.shzxlz.cn

name="Tom"; echo "$name"
来源：http://dhm.shanyushiyangkeji.top

[R03] 只读变量
来源：http://efk.zdqjudy.top

readonly PI=3.14
来源：http://qkh.uphjek.com

[R04] 位置参数
来源：http://tzy.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yku.fanxiaobao.xyz

[R05] 参数默认值
来源：http://lul.vqdsnc.cn

name="${1:-default}"
来源：http://cvc.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://eyb.sweek.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kgx.sxryk.cn

[R07] if 判断文件
来源：http://ank.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pka.yongpay.top

[R08] 数值比较
来源：http://pmi.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://odo.mhx1999.top

[R09] 字符串比较
来源：http://dgq.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jzf.daria6918.cn

[R10] 正则匹配
来源：http://dkk.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gwq.guowangkeji.top

[R11] case 多分支
来源：http://rkj.havefunace.top

case "$1" in
来源：http://dsy.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://out.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://lzy.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://mfg.yuanzhike.top

esac
来源：http://lyk.tian-w.cn

[R12] for 遍历文件
来源：http://pyx.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://qgt.wangdashe.top

[R13] for 计数循环
来源：http://rzp.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://lig.meibo888.top

[R14] C 风格 for
来源：http://epd.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sfc.hcnkem.com

[R15] while 逐行读文件
来源：http://cnh.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://whg.birdmap.top

[R16] until 等待条件
来源：http://psm.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wei.cheryme.top

[R17] 数组定义与取值
来源：http://krm.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yyn.sxryk.cn

[R18] 遍历数组
来源：http://eoa.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tbd.yonumen.top

[R19] 数组长度
来源：http://dut.0kj1m.cn

echo "${#arr[@]}"
来源：http://qkt.hnqzz.top

[R20] 关联数组（字典）
来源：http://bwj.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lsw.epnwcf.com

[R21] 字符串长度
来源：http://hqg.feifeiyinyue.top


<!-- 参考信息 -->