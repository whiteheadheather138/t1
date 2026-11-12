代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gkq.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://obx.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vvu.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xhf.tanke756.top

Java: list.size();  map.size();  s.length()
来源：http://nkd.pycfn.com

Go:   len(arr);  len(m)
来源：http://ohj.fehbvm.com

Ruby: x.length;  x.size
来源：http://rij.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jpr.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://gmr.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mqa.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pkh.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wba.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ksi.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kdg.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://zgk.kuanghao11.cn

Ruby: a == b
来源：http://dbv.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ldk.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oct.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tyi.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://diz.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sne.epnwcf.com

TS:   if (x == null) {}
来源：http://cse.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ldo.feifeiyinyue.top

Go:   if x == nil {}
来源：http://vnp.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kek.yonumen.top

C#:   if (x is null) {}
来源：http://vqf.wangdashe.top

[P07] 防抖与节流
来源：http://kgj.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aqf.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://tuw.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkv.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jxp.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rhl.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://trd.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://pwk.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oic.xziqi.cn

[P08] 处理浮点精度问题
来源：http://drn.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fip.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vyz.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ypw.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zmy.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://txr.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cgn.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zbn.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hnj.hesvh.cn

================================================================================
来源：http://moi.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://umz.kuanghao11.cn

================================================================================
来源：http://hjq.zycfv.cn

[Q01] 创建表
来源：http://zto.redwolf501.top

CREATE TABLE users (
来源：http://hij.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://smz.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://xwt.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://dmu.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://stt.hcnkem.com

);
来源：http://nxi.epnwcf.com

[Q02] 创建带外键的表
来源：http://vvf.andypj.xyz

CREATE TABLE orders (
来源：http://rdb.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dix.jinqigufen.top

user_id INT NOT NULL,
来源：http://twy.yonumen.top

amount DECIMAL(10, 2),
来源：http://mqy.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://snw.9152youxi.cn

);
来源：http://gmn.cqqwz.cn

[Q03] 增加列
来源：http://mqj.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xbt.nanxinkj.top

[Q04] 修改列类型
来源：http://jpa.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yxb.ydjk.org.cn

[Q05] 重命名列
来源：http://kox.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ngg.tarul.cn

[Q06] 删除列
来源：http://ptc.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cer.haohaochexian.top

[Q07] 删除表
来源：http://sfv.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://ehb.jianghu66.top

[Q08] 创建普通索引
来源：http://ypi.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wky.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://ofp.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mxx.vehdjk.com

[Q10] 插入单行
来源：http://tzp.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://izq.cdnleiting.top

[Q11] 一次插入多行
来源：http://gbq.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hio.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://cem.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://zms.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kel.yfazqb.com

[Q13] 忽略重复插入
来源：http://wzk.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fsp.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://ypy.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bqt.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jqf.zhiwuduotai.top

[Q15] 查询全部
来源：http://czx.meibo888.top

SELECT * FROM users;
来源：http://qyi.zhijiandao.cn

[Q16] 查询指定列
来源：http://upp.sjlbkw.cn

SELECT id, name FROM users;
来源：http://jkp.chenzaomai.com

[Q17] 条件查询
来源：http://ymh.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tup.hnxiangtu.top

[Q18] 模糊匹配
来源：http://eae.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xrs.meibo888.top

[Q19] 范围查询
来源：http://urm.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wyd.birdmap.top

[Q20] IN 列表
来源：http://sdy.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rqo.chenzaomai.com

[Q21] 空值判断
来源：http://wib.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jer.daxiang520.top

[Q22] 排序
来源：http://ypr.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://duj.xinyue.icu

[Q23] 分页
来源：http://vdz.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cxs.bjfxy.top

[Q24] 去重
来源：http://bfa.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://qsy.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://ozh.birdmap.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mho.jinqigufen.top

[Q26] 计数
来源：http://eou.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://luk.redwolf501.top

[Q27] 条件计数
来源：http://jxd.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zio.xylfe.cn

[Q28] 求和与平均
来源：http://pgp.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lqk.tian-w.cn

[Q29] 最大最小值
来源：http://fzj.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bbf.ivvv.top

[Q30] 分组统计
来源：http://yez.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uny.chenzaomai.com

[Q31] 分组后过滤
来源：http://xlt.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://imi.smart0.xyz

[Q32] 分组拼接字符串
来源：http://xwi.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mqj.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xoc.fanxiaobao.xyz

[Q33] 多列分组
来源：http://srv.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://irh.hesvh.cn

[Q34] 每组取第一条
来源：http://lbj.sjlbkw.cn

SELECT * FROM (
来源：http://uof.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xyv.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://cuh.316326.xyz

[Q35] 内连接
来源：http://odz.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ozn.jinqigufen.top

[Q36] 左连接
来源：http://ujj.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hlv.svipenyu.cn

[Q37] 右连接
来源：http://shz.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nat.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://ypk.cqqwz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ttn.fktsv.cn

[Q39] 自连接（查上下级）
来源：http://zff.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://kqb.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ler.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ixa.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ykh.redwolf501.top

[Q41] 多表连接
来源：http://ixn.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zml.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://fll.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://sqp.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://wtu.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://fqu.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cur.cqqwz.cn

[Q43] 标量子查询
来源：http://gzw.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fco.vehdjk.com

[Q44] IN 子查询
来源：http://uat.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://imb.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://aew.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdi.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iop.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://upg.yuanzhike.top

[Q47] 与平均值比较
来源：http://oeg.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cqk.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://mqh.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nbr.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://hxz.tianlin.xyz

[Q49] 更新单行
来源：http://tba.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ibj.guannengcc.top

[Q50] 批量更新
来源：http://ksh.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ivvv.top

[Q51] 用子查询更新
来源：http://izt.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oar.ctjpmb.com

[Q52] 删除指定行
来源：http://mqf.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://moc.gaohongyu789.top

[Q53] 按条件删除
来源：http://qyb.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wmy.epnwcf.com

[Q54] 清空表
来源：http://sng.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://pol.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://xwu.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://snb.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://uyn.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rjc.jiagoushi.top

[Q57] 行号
来源：http://ndl.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ouf.zhoulong.xyz

[Q58] 累计求和
来源：http://lbg.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rca.guowangkeji.top

[Q59] 分组内累计
来源：http://xpi.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qtq.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://hpp.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hla.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hin.c1oappe.top

[Q61] 移动平均
来源：http://imi.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://isy.shuidangran.top

[Q62] 分组占比
来源：http://etb.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xty.jinghuilouyu.cn

[Q63] 开启事务
来源：http://qjc.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qqa.ehwqpu.com

[Q64] 提交事务
来源：http://yoa.yuxming.cn

COMMIT;
来源：http://ahj.cqqwz.cn

[Q65] 回滚事务
来源：http://yiq.52xcode.cn

ROLLBACK;
来源：http://uqw.chenjidiqi.icu

[Q66] 行锁查询
来源：http://yam.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xps.gzhubu.top

[Q67] 设置隔离级别
来源：http://ktq.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://khv.shuidangran.top

[Q68] 保存点
来源：http://bxg.yfazqb.com

SAVEPOINT sp1;
来源：http://aqf.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://oil.ydzc1.top

[Q69] 查看执行计划
来源：http://eqt.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hel.yangfankeji.com

[Q70] 更新统计信息
来源：http://yft.pycfn.com

ANALYZE TABLE users;
来源：http://yib.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://uyd.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zno.316326.xyz

[Q72] 查看索引
来源：http://mlz.yanxiufei.cn

SHOW INDEX FROM users;
来源：http://xxo.xylfe.cn

[Q73] 查看表状态
来源：http://upn.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bwl.dianchejie.cn

[Q74] 强制使用索引
来源：http://btd.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kws.guowangkeji.top

[Q75] 日期格式化
来源：http://ron.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dnz.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wtd.iojbl.cn

[Q76] 按天统计
来源：http://hxo.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uiu.tarul.cn

[Q77] 时间加减
来源：http://kvi.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vsu.jiagoushi.top

[Q78] 当前时间
来源：http://bxi.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pui.andypj.xyz

[Q79] 字符串拼接
来源：http://dzk.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yfu.yj20258.top

[Q80] 字符串截取
来源：http://jvp.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qno.zhaomingkeji.xyz

[Q81] 字符串替换
来源：http://fra.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sqb.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://xrt.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://exi.ctjpmb.com

[Q83] 大小写转换
来源：http://zsc.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://flr.bbcook.cn

[Q84] 去除首尾空格
来源：http://ahz.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://xpt.jinghuilouyu.cn

[Q85] 数值取整
来源：http://dcn.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xwk.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://zpy.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://smw.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://ncy.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://obf.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://wfq.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cmv.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mff.yvedp.cn

[Q89] 判断表是否存在
来源：http://gtt.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cdx.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://qhw.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nod.yonumen.top

================================================================================
来源：http://ahg.fzhhl.top

R. Bash 专题
来源：http://jbx.quarkkingdee.top

================================================================================
来源：http://yco.hnqzz.top

[R01] shebang 与严格模式
来源：http://onn.epnwcf.com

#!/usr/bin/env bash
来源：http://pru.bjfxy.top

set -euo pipefail
来源：http://ljo.cucudq.cn

[R02] 变量赋值与使用
来源：http://cfc.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://ziu.jqgufenzy.top

[R03] 只读变量
来源：http://hga.haohaochexian.top

readonly PI=3.14
来源：http://spp.epnwcf.com

[R04] 位置参数
来源：http://xyj.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://any.yueranfly.top

[R05] 参数默认值
来源：http://qwa.fzhhl.top

name="${1:-default}"
来源：http://wtm.yueranfly.top

[R06] 判断命令是否存在
来源：http://whm.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zti.gotoacloud.top

[R07] if 判断文件
来源：http://cdh.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wuj.sjlbkw.cn

[R08] 数值比较
来源：http://hjz.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ilx.hcnkem.com

[R09] 字符串比较
来源：http://xdf.nanxinkj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://drn.chenjidiqi.icu

[R10] 正则匹配
来源：http://bkt.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bqm.zhengqikj.top

[R11] case 多分支
来源：http://ako.havefunace.top

case "$1" in
来源：http://ieq.birdmap.top

start) echo "启动" ;;
来源：http://nrr.hesvh.cn

stop)  echo "停止" ;;
来源：http://omd.c1oappe.top

*)     echo "未知命令" ;;
来源：http://kit.yuxming.cn

esac
来源：http://gpa.yonumen.top

[R12] for 遍历文件
来源：http://mrt.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://iix.aibaodan.cn

[R13] for 计数循环
来源：http://hlo.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://drr.bbcook.cn

[R14] C 风格 for
来源：http://nxq.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xyh.jianghu66.top

[R15] while 逐行读文件
来源：http://cbb.sxryk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tku.ybcxt.top

[R16] until 等待条件
来源：http://btz.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bqf.0kj1m.cn

[R17] 数组定义与取值
来源：http://ivh.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://zlj.jinqigufen.top

[R18] 遍历数组
来源：http://bbb.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pkr.0kj1m.cn

[R19] 数组长度
来源：http://ljb.sweek.top

echo "${#arr[@]}"
来源：http://mrg.cdnleiting.top

[R20] 关联数组（字典）
来源：http://sxk.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yhs.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://iqh.tarul.cn


<!-- 参考信息 -->