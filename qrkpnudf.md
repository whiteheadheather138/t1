代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ftg.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kds.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryj.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nqz.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://aqu.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://utp.wangdashe.top

Ruby: x.length;  x.size
来源：http://ets.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uao.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://hwn.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yhc.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vow.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xey.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://okf.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://usd.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://cnv.vehdjk.com

Ruby: a == b
来源：http://xeq.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ipr.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ffw.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lbm.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://esm.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qqy.jqgufenzy.top

TS:   if (x == null) {}
来源：http://bvi.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bnp.hesvh.cn

Go:   if x == nil {}
来源：http://iey.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nug.hnqzz.top

C#:   if (x is null) {}
来源：http://mle.haohaochexian.top

[P07] 防抖与节流
来源：http://eya.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://btz.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://wbx.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jey.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbd.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aks.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://epm.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lso.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ngk.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://pyo.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mjg.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kqx.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gcp.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eee.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vqx.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yox.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cqk.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rcm.cdnleiting.top

================================================================================
来源：http://ilb.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pac.jlsjyb.cn

================================================================================
来源：http://mjt.tian-w.cn

[Q01] 创建表
来源：http://oat.jqgfzy.top

CREATE TABLE users (
来源：http://tsd.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pom.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://fqo.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://lzr.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fxt.0kj1m.cn

);
来源：http://qjl.guannengcc.top

[Q02] 创建带外键的表
来源：http://fak.hcnkem.com

CREATE TABLE orders (
来源：http://wsg.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eyp.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://vyc.c1oappe.top

amount DECIMAL(10, 2),
来源：http://jab.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zbl.havefunace.top

);
来源：http://jtr.zhengqikj.top

[Q03] 增加列
来源：http://vpx.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xgk.9152youxi.cn

[Q04] 修改列类型
来源：http://qfa.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xww.ydjk.org.cn

[Q05] 重命名列
来源：http://pmu.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wdv.zycfv.cn

[Q06] 删除列
来源：http://cgx.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://pyz.zycfv.cn

[Q07] 删除表
来源：http://qgi.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://ylp.snrcjt.cn

[Q08] 创建普通索引
来源：http://wkp.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hcd.haohaochexian.top

[Q09] 创建唯一索引
来源：http://ctx.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lit.sufxvd.cn

[Q10] 插入单行
来源：http://pcs.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ull.wangdashe.top

[Q11] 一次插入多行
来源：http://pxa.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sax.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://pvg.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://prf.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aky.svipenyu.cn

[Q13] 忽略重复插入
来源：http://vcq.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pui.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://xen.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mpm.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gdg.yongpay.top

[Q15] 查询全部
来源：http://wew.tanke756.top

SELECT * FROM users;
来源：http://nha.jinqigfzy.top

[Q16] 查询指定列
来源：http://ghi.ybcxt.top

SELECT id, name FROM users;
来源：http://yuv.wangshuangyany.cn

[Q17] 条件查询
来源：http://cav.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xgu.aibaodan.cn

[Q18] 模糊匹配
来源：http://jxx.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ngr.sxryk.cn

[Q19] 范围查询
来源：http://hnf.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tcr.hongshengwenyu.top

[Q20] IN 列表
来源：http://nmm.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://srn.cdnleiting.top

[Q21] 空值判断
来源：http://njo.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://ygk.316326.xyz

[Q22] 排序
来源：http://jta.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qnp.xziqi.cn

[Q23] 分页
来源：http://dar.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lto.zhijiandao.cn

[Q24] 去重
来源：http://cmu.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://lqi.fengsongda.top

[Q25] 只取前 N 条
来源：http://xtc.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://onc.guowangkeji.top

[Q26] 计数
来源：http://coy.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://kis.316326.xyz

[Q27] 条件计数
来源：http://xef.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bfa.zdbjq.cn

[Q28] 求和与平均
来源：http://ruh.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://orq.hongshengwenyu.top

[Q29] 最大最小值
来源：http://fpx.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rnt.shuidangran.top

[Q30] 分组统计
来源：http://nsd.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yla.jqgufenzy.top

[Q31] 分组后过滤
来源：http://hjk.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jqa.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://xyt.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vbk.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fql.0kj1m.cn

[Q33] 多列分组
来源：http://edh.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ucd.52xcode.cn

[Q34] 每组取第一条
来源：http://wqr.hysaishi.cn

SELECT * FROM (
来源：http://rhp.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bgy.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://tge.fengsongda.top

[Q35] 内连接
来源：http://zaq.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fhf.daxiang520.top

[Q36] 左连接
来源：http://mhk.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rvp.hnqzz.top

[Q37] 右连接
来源：http://uif.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xmm.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://xqr.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://suw.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://ylj.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pez.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uit.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://sxv.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vib.fanxiaobao.xyz

[Q41] 多表连接
来源：http://xao.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rxf.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://vah.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://uds.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://wwm.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://jpj.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nkz.hesvh.cn

[Q43] 标量子查询
来源：http://arr.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rre.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://ctn.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ouh.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://jhq.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ckc.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://wrt.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fqe.jinqigufen.top

[Q47] 与平均值比较
来源：http://jxl.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ozq.birdmap.top

[Q48] CTE 公用表表达式
来源：http://doe.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://umx.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://lxx.havefunace.top

[Q49] 更新单行
来源：http://cay.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cha.ydzc1.top

[Q50] 批量更新
来源：http://jhc.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://evz.dashuyun.cn

[Q51] 用子查询更新
来源：http://knq.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hnr.jyoumei.cn

[Q52] 删除指定行
来源：http://syt.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://jjc.yuanzhike.top

[Q53] 按条件删除
来源：http://myg.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wbk.ybcxt.top

[Q54] 清空表
来源：http://hus.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://zok.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://rqf.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zoj.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://ust.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bqe.zdqjudy.top

[Q57] 行号
来源：http://pjx.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sen.zdqjudy.top

[Q58] 累计求和
来源：http://qux.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://osb.aizwys.cn

[Q59] 分组内累计
来源：http://oap.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://moy.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://bto.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zph.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mwk.shanyushiyangtech.top

[Q61] 移动平均
来源：http://xal.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nzj.bjfxy.top

[Q62] 分组占比
来源：http://czv.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iht.sufxvd.cn

[Q63] 开启事务
来源：http://lop.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fco.ctjpmb.com

[Q64] 提交事务
来源：http://pip.epnwcf.com

COMMIT;
来源：http://zyn.andypj.xyz

[Q65] 回滚事务
来源：http://hmh.zdbjq.cn

ROLLBACK;
来源：http://fpx.daxiang520.top

[Q66] 行锁查询
来源：http://xsr.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lpn.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://poz.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jgh.shanyushiyangkeji.top

[Q68] 保存点
来源：http://khb.jlsjyb.cn

SAVEPOINT sp1;
来源：http://pxl.yuxming.cn

ROLLBACK TO sp1;
来源：http://qke.gzhubu.top

[Q69] 查看执行计划
来源：http://vfn.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ldq.cucudq.cn

[Q70] 更新统计信息
来源：http://nqs.ydzc1.top

ANALYZE TABLE users;
来源：http://bkp.9152youxi.cn

[Q71] 查看建表语句
来源：http://nbi.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rei.mhx1999.top

[Q72] 查看索引
来源：http://jfa.iojbl.cn

SHOW INDEX FROM users;
来源：http://ees.hongshengwenyu.top

[Q73] 查看表状态
来源：http://rqx.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://mnm.tian-w.cn

[Q74] 强制使用索引
来源：http://wrw.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uir.wangdashe.top

[Q75] 日期格式化
来源：http://yup.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bnf.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ets.fehbvm.com

[Q76] 按天统计
来源：http://jef.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://byi.cqqwz.cn

[Q77] 时间加减
来源：http://fyf.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dyh.cdnleiting.top

[Q78] 当前时间
来源：http://jrs.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://byh.svipenyu.cn

[Q79] 字符串拼接
来源：http://sjg.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uxs.haohaochexian.top

[Q80] 字符串截取
来源：http://xaq.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dvy.birdmap.top

[Q81] 字符串替换
来源：http://hfu.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xte.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://pgn.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjv.mhx1999.top

[Q83] 大小写转换
来源：http://szl.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kib.dashuyun.cn

[Q84] 去除首尾空格
来源：http://lyb.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://rha.ydzc1.top

[Q85] 数值取整
来源：http://cdo.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://who.uphjek.com

[Q86] 读取 JSON 字段
来源：http://bqd.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zug.ydzc1.top

[Q87] JSON 字段做条件
来源：http://ujx.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vbw.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://iqa.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hub.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xvf.c1oappe.top

[Q89] 判断表是否存在
来源：http://rgn.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gtf.epnwcf.com

[Q90] 生成序号列
来源：http://tlc.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gkx.jinqigfzy.top

================================================================================
来源：http://eom.hnxiangtu.top

R. Bash 专题
来源：http://umw.gotoacloud.top

================================================================================
来源：http://psj.sxryk.cn

[R01] shebang 与严格模式
来源：http://cnb.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://jua.bjfxy.top

set -euo pipefail
来源：http://cjy.hysaishi.cn

[R02] 变量赋值与使用
来源：http://duw.ehwqpu.com

name="Tom"; echo "$name"
来源：http://zyc.9152youxi.cn

[R03] 只读变量
来源：http://wli.yanxiufei.cn

readonly PI=3.14
来源：http://ayj.vqdsnc.cn

[R04] 位置参数
来源：http://dru.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://utj.birdmap.top

[R05] 参数默认值
来源：http://pkk.dianchejie.cn

name="${1:-default}"
来源：http://ysh.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://onz.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wih.nanxuanxn.top

[R07] if 判断文件
来源：http://jay.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://umw.sufxvd.cn

[R08] 数值比较
来源：http://ccf.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mzu.cashguo.top

[R09] 字符串比较
来源：http://dzw.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zai.nanxuanxn.top

[R10] 正则匹配
来源：http://ggs.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bal.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://dkq.yangfankeji.com

case "$1" in
来源：http://jjh.kuanghao11.cn

start) echo "启动" ;;
来源：http://yvy.tarul.cn

stop)  echo "停止" ;;
来源：http://sna.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://otg.aizwys.cn

esac
来源：http://lxx.andypj.xyz

[R12] for 遍历文件
来源：http://thl.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://pxw.c1oappe.top

[R13] for 计数循环
来源：http://suu.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://dfk.sufxvd.cn

[R14] C 风格 for
来源：http://tbe.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eow.redwolf501.top

[R15] while 逐行读文件
来源：http://wyz.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aby.zdbjq.cn

[R16] until 等待条件
来源：http://njw.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://riz.xinyue.icu

[R17] 数组定义与取值
来源：http://bjb.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hog.wangshuangyany.cn

[R18] 遍历数组
来源：http://xpo.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ryh.zhiwuduotai.top

[R19] 数组长度
来源：http://ifz.vehdjk.com

echo "${#arr[@]}"
来源：http://mms.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://gjw.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://usc.xuetiantiany.cn

[R21] 字符串长度
来源：http://gij.hammf.cn


<!-- 参考信息 -->