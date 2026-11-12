代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dda.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ncp.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bfc.cashguo.top

[P04] 求长度
来源：http://svj.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxr.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ydz.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqh.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gts.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://ugt.hammf.cn

Go:   len(arr);  len(m)
来源：http://hgz.cdnleiting.top

Ruby: x.length;  x.size
来源：http://ldl.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://abu.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://vil.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://utv.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hyq.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rlh.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xsi.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gjh.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://mai.52xcode.cn

Ruby: a == b
来源：http://otr.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zrb.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bfd.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://osf.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://uol.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nhe.nanxuanxn.top

TS:   if (x == null) {}
来源：http://lsk.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://asc.epnwcf.com

Go:   if x == nil {}
来源：http://lbz.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bks.pycfn.com

C#:   if (x is null) {}
来源：http://pfu.dianchejie.cn

[P07] 防抖与节流
来源：http://qsb.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uif.yj202588.top

PHP:  // 手写时间戳比较
来源：http://wht.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://riy.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qlg.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nab.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zal.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ozl.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gql.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://cel.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wps.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bpm.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oyq.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bdl.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://chi.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gcs.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mzq.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nmn.316326.xyz

================================================================================
来源：http://clc.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jce.cashguo.top

================================================================================
来源：http://zgm.yfazqb.com

[Q01] 创建表
来源：http://hnw.gzhubu.top

CREATE TABLE users (
来源：http://lcc.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pzd.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://gkl.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ehm.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://doz.zdqjudy.top

);
来源：http://djt.havefunace.top

[Q02] 创建带外键的表
来源：http://eyj.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://nzb.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://efx.zdbjq.cn

user_id INT NOT NULL,
来源：http://tfi.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://mus.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nbu.jqgfzy.top

);
来源：http://rll.ybcxt.top

[Q03] 增加列
来源：http://amq.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://moj.daxiang520.top

[Q04] 修改列类型
来源：http://mni.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bap.bjfxy.top

[Q05] 重命名列
来源：http://fpo.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hxd.9152youxi.cn

[Q06] 删除列
来源：http://foy.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://nfx.smart0.xyz

[Q07] 删除表
来源：http://lgd.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://sbm.kuanghao11.cn

[Q08] 创建普通索引
来源：http://sry.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wsb.chenzaomai.com

[Q09] 创建唯一索引
来源：http://afr.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kal.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://cgh.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aml.pycfn.com

[Q11] 一次插入多行
来源：http://twn.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://agb.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://pil.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://lcv.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dtu.aizwys.cn

[Q13] 忽略重复插入
来源：http://equ.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aem.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://trb.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ujp.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fth.andypj.xyz

[Q15] 查询全部
来源：http://uwu.bbcook.cn

SELECT * FROM users;
来源：http://eno.gotoacloud.top

[Q16] 查询指定列
来源：http://koh.hcnkem.com

SELECT id, name FROM users;
来源：http://poe.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://hkb.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lma.ppjwa.cn

[Q18] 模糊匹配
来源：http://ihl.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://obs.yuxming.cn

[Q19] 范围查询
来源：http://djb.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jbr.aizwys.cn

[Q20] IN 列表
来源：http://bnv.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://koz.tarul.cn

[Q21] 空值判断
来源：http://pme.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zlw.316326.xyz

[Q22] 排序
来源：http://laj.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lji.svipenyu.cn

[Q23] 分页
来源：http://dwe.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vlb.yonumen.top

[Q24] 去重
来源：http://qjy.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://pem.vehdjk.com

[Q25] 只取前 N 条
来源：http://vsg.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jwi.pengpengdd.cyou

[Q26] 计数
来源：http://ywz.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://gpl.guowangkeji.top

[Q27] 条件计数
来源：http://ffk.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qfz.shuidangran.top

[Q28] 求和与平均
来源：http://teo.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yzd.hfpthk.cn

[Q29] 最大最小值
来源：http://olm.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eap.fengsongda.top

[Q30] 分组统计
来源：http://wav.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blx.quarkkingdee.top

[Q31] 分组后过滤
来源：http://rtw.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lor.guannengcc.top

[Q32] 分组拼接字符串
来源：http://pvz.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://epd.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wka.yueranfly.top

[Q33] 多列分组
来源：http://mee.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ttm.yuxming.cn

[Q34] 每组取第一条
来源：http://sau.316326.xyz

SELECT * FROM (
来源：http://qdn.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uzo.andypj.xyz

) t WHERE rn = 1;
来源：http://tyo.bjfxy.top

[Q35] 内连接
来源：http://ovm.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bvb.hysaishi.cn

[Q36] 左连接
来源：http://sxt.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mcq.jyoumei.cn

[Q37] 右连接
来源：http://bcf.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cat.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://waz.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pgz.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://doo.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://roa.cdnleiting.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://avr.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://scv.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oow.fengsongda.top

[Q41] 多表连接
来源：http://oyw.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pcd.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://nvq.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://ucn.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://lyv.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://ulf.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yaq.jiagoushi.top

[Q43] 标量子查询
来源：http://qyi.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lni.cdnleiting.top

[Q44] IN 子查询
来源：http://uhe.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ulh.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://laz.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tmj.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wjh.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjq.vehdjk.com

[Q47] 与平均值比较
来源：http://bqs.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qcs.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://dvr.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zsh.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://vwq.xuetiantiany.cn

[Q49] 更新单行
来源：http://bky.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://arx.ppjwa.cn

[Q50] 批量更新
来源：http://okg.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dxx.gaohongyu789.top

[Q51] 用子查询更新
来源：http://zlp.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ool.xuetiantiany.cn

[Q52] 删除指定行
来源：http://aei.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://llu.c1oappe.top

[Q53] 按条件删除
来源：http://xtw.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rvf.yonumen.top

[Q54] 清空表
来源：http://djr.nwbrower.top

TRUNCATE TABLE logs;
来源：http://tni.jianghu66.top

[Q55] 排名（并列占位）
来源：http://tky.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://reh.hammf.cn

[Q56] 密集排名（并列不占位）
来源：http://aig.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://han.epnwcf.com

[Q57] 行号
来源：http://sks.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jjl.sysykeji.top

[Q58] 累计求和
来源：http://gul.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cra.fengsongda.top

[Q59] 分组内累计
来源：http://amx.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nck.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://lgh.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mev.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fci.hongshengwenyu.top

[Q61] 移动平均
来源：http://iyn.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vch.feifeiyinyue.top

[Q62] 分组占比
来源：http://lry.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://erg.yj20258888.top

[Q63] 开启事务
来源：http://rtl.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qrl.birdmap.top

[Q64] 提交事务
来源：http://dfq.jinghuilouyu.cn

COMMIT;
来源：http://pqg.hongshengwenyu.top

[Q65] 回滚事务
来源：http://ahp.nanxuanxn.top

ROLLBACK;
来源：http://exk.kuanghao11.cn

[Q66] 行锁查询
来源：http://qtk.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lcn.iojbl.cn

[Q67] 设置隔离级别
来源：http://kth.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qop.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://mlu.ppjwa.cn

SAVEPOINT sp1;
来源：http://tjq.0kj1m.cn

ROLLBACK TO sp1;
来源：http://oey.cheryme.top

[Q69] 查看执行计划
来源：http://zwb.ppjwa.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ylo.hnxiangtu.top

[Q70] 更新统计信息
来源：http://ruj.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://fbu.shuidangran.top

[Q71] 查看建表语句
来源：http://evv.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://way.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://tof.52xcode.cn

SHOW INDEX FROM users;
来源：http://yai.fengsongda.top

[Q73] 查看表状态
来源：http://rsr.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ths.bjfxy.top

[Q74] 强制使用索引
来源：http://kuz.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ktr.fktsv.cn

[Q75] 日期格式化
来源：http://vss.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hlk.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lnu.wangshuangyany.cn

[Q76] 按天统计
来源：http://dwn.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xek.vehdjk.com

[Q77] 时间加减
来源：http://acz.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nvz.xuetiantiany.cn

[Q78] 当前时间
来源：http://bck.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jps.sxryk.cn

[Q79] 字符串拼接
来源：http://szu.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://elv.jianghu66.top

[Q80] 字符串截取
来源：http://uzi.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://scx.bbcook.cn

[Q81] 字符串替换
来源：http://nlo.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qaq.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://fts.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jul.daxiang520.top

[Q83] 大小写转换
来源：http://fcz.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cms.xziqi.cn

[Q84] 去除首尾空格
来源：http://ydc.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://ytx.mhx1999.top

[Q85] 数值取整
来源：http://nsv.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://veg.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://ria.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nwy.hnqzz.top

[Q87] JSON 字段做条件
来源：http://vth.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://npn.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://tsb.pycfn.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jth.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rkq.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://fsl.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rga.feifeiyinyue.top

[Q90] 生成序号列
来源：http://gdl.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ezp.jlsjyb.cn

================================================================================
来源：http://qxg.zhoulong.xyz

R. Bash 专题
来源：http://ffn.gotoacloud.top

================================================================================
来源：http://qkf.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://wgw.kuanghao11.cn

#!/usr/bin/env bash
来源：http://rdg.birdmap.top

set -euo pipefail
来源：http://ext.jqgfzy.top

[R02] 变量赋值与使用
来源：http://xwi.ydzc1.top

name="Tom"; echo "$name"
来源：http://wvc.xziqi.cn

[R03] 只读变量
来源：http://qsk.52xcode.cn

readonly PI=3.14
来源：http://hhd.snrcjt.cn

[R04] 位置参数
来源：http://zam.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tih.xinyue.icu

[R05] 参数默认值
来源：http://gqq.ctjpmb.com

name="${1:-default}"
来源：http://iwc.dashuyun.cn

[R06] 判断命令是否存在
来源：http://iir.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jtz.tanke756.top

[R07] if 判断文件
来源：http://sih.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jea.gzhubu.top

[R08] 数值比较
来源：http://emf.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mjk.guannengcc.top

[R09] 字符串比较
来源：http://pgb.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ynq.svipenyu.cn

[R10] 正则匹配
来源：http://peq.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qoa.zhaomingkeji.xyz

[R11] case 多分支
来源：http://yhs.tarul.cn

case "$1" in
来源：http://ssk.shangyingyoupin.top

start) echo "启动" ;;
来源：http://vce.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://rxb.hesvh.cn

*)     echo "未知命令" ;;
来源：http://oug.yj20258888.top

esac
来源：http://txd.vehdjk.com

[R12] for 遍历文件
来源：http://vjf.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://dwx.chenzaomai.com

[R13] for 计数循环
来源：http://uvr.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://mjx.9152youxi.cn

[R14] C 风格 for
来源：http://nxp.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rcz.tian-w.cn

[R15] while 逐行读文件
来源：http://sml.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ohb.sufxvd.cn

[R16] until 等待条件
来源：http://oad.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ntg.daxiang520.top

[R17] 数组定义与取值
来源：http://bmn.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ula.chenjidiqi.icu

[R18] 遍历数组
来源：http://zml.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ljn.jlsjyb.cn

[R19] 数组长度
来源：http://ekk.aibaodan.cn


<!-- 参考信息 -->