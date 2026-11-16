代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pgt.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://qbh.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xwl.yuanzhike.top

[P04] 求长度
来源：http://lqb.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lmz.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rgy.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xso.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zfs.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://nna.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://cea.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://obf.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xsm.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://bdd.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xbi.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iyj.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zwh.sxryk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xke.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://anp.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hbh.yonumen.top

Ruby: a == b
来源：http://dxs.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sfn.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rzu.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dlo.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://mfm.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lsy.ppjwa.cn

TS:   if (x == null) {}
来源：http://rfi.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ghv.chenlongwang.top

Go:   if x == nil {}
来源：http://lcg.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qos.yanxiufei.cn

C#:   if (x is null) {}
来源：http://krx.yanxiufei.cn

[P07] 防抖与节流
来源：http://pde.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duo.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://ggp.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujp.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odz.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tai.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://abh.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://laf.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nvu.epnwcf.com

[P08] 处理浮点精度问题
来源：http://eav.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rcd.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nxw.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wcs.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oid.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mdr.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gba.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pkn.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://txs.shzxlz.cn

================================================================================
来源：http://ynv.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://doy.xinyue.icu

================================================================================
来源：http://pmw.tianlin.xyz

[Q01] 创建表
来源：http://ycs.aizwys.cn

CREATE TABLE users (
来源：http://fkc.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vha.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://kuv.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://uad.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvs.birdmap.top

);
来源：http://xxa.haohaochexian.top

[Q02] 创建带外键的表
来源：http://rly.ctjpmb.com

CREATE TABLE orders (
来源：http://wsb.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpu.uphjek.com

user_id INT NOT NULL,
来源：http://pxn.quarkkingdee.top

amount DECIMAL(10, 2),
来源：http://rbb.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hyg.zhengqikj.top

);
来源：http://xui.zhijiandao.cn

[Q03] 增加列
来源：http://mts.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sbl.fzhhl.top

[Q04] 修改列类型
来源：http://wqh.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vjw.nwbrower.top

[Q05] 重命名列
来源：http://fyb.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kmi.cashguo.top

[Q06] 删除列
来源：http://rvr.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://rfv.c1oappe.top

[Q07] 删除表
来源：http://nvf.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://hcq.sjlbkw.cn

[Q08] 创建普通索引
来源：http://wuu.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://nlq.yonumen.top

[Q09] 创建唯一索引
来源：http://fev.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uif.jinghuilouyu.cn

[Q10] 插入单行
来源：http://fkm.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wmy.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://bdb.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zza.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://lmj.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://znc.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mxl.tarul.cn

[Q13] 忽略重复插入
来源：http://rzz.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qex.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://ioy.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://owf.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vmo.dianchejie.cn

[Q15] 查询全部
来源：http://qsb.hywenlv.cn

SELECT * FROM users;
来源：http://gil.hesvh.cn

[Q16] 查询指定列
来源：http://owt.ppjwa.cn

SELECT id, name FROM users;
来源：http://ddl.ivvv.top

[Q17] 条件查询
来源：http://alj.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kcv.c1oappe.top

[Q18] 模糊匹配
来源：http://kxv.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hme.chenzaomai.com

[Q19] 范围查询
来源：http://ybb.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rnv.smart0.xyz

[Q20] IN 列表
来源：http://kyg.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rwk.0kj1m.cn

[Q21] 空值判断
来源：http://kzk.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://rfn.hfpthk.cn

[Q22] 排序
来源：http://azk.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hlk.cheryme.top

[Q23] 分页
来源：http://ujz.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://suh.zhixingplan.top

[Q24] 去重
来源：http://gdb.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://pcd.tarul.cn

[Q25] 只取前 N 条
来源：http://pvj.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lfd.wangdashe.top

[Q26] 计数
来源：http://ktz.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://hhv.jinqigufen.top

[Q27] 条件计数
来源：http://xnp.birdmap.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bur.bbcook.cn

[Q28] 求和与平均
来源：http://pin.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iuf.jqgfzy.top

[Q29] 最大最小值
来源：http://jjv.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ihr.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://jtr.zhoulong.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jyc.shzxlz.cn

[Q31] 分组后过滤
来源：http://oea.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yso.birdmap.top

[Q32] 分组拼接字符串
来源：http://qqj.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jlo.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jqw.ctjpmb.com

[Q33] 多列分组
来源：http://yfm.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xnt.uphjek.com

[Q34] 每组取第一条
来源：http://jkp.snrcjt.cn

SELECT * FROM (
来源：http://bbf.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rmv.ydzc1.top

) t WHERE rn = 1;
来源：http://dmn.hcnkem.com

[Q35] 内连接
来源：http://sdt.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mzo.yueranfly.top

[Q36] 左连接
来源：http://mip.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yme.yj20258.top

[Q37] 右连接
来源：http://zgq.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rtq.vehdjk.com

[Q38] 全外连接（PostgreSQL）
来源：http://rpm.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://atf.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://ygt.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ead.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nzs.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://tyt.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ysf.cashguo.top

[Q41] 多表连接
来源：http://jdm.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsk.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://zkq.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://jyc.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://qno.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://duq.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kkg.chenjidiqi.icu

[Q43] 标量子查询
来源：http://yhh.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hiv.shangyingyoupin.top

[Q44] IN 子查询
来源：http://une.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hnf.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://qsc.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqn.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://aad.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mem.fktsv.cn

[Q47] 与平均值比较
来源：http://plq.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pmt.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://byk.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsn.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://pez.cheryme.top

[Q49] 更新单行
来源：http://mty.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cld.dianchejie.cn

[Q50] 批量更新
来源：http://fxc.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zfr.nwbrower.top

[Q51] 用子查询更新
来源：http://sxx.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qqa.xuanzx.com

[Q52] 删除指定行
来源：http://pam.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ztr.yuxming.cn

[Q53] 按条件删除
来源：http://qny.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://skf.fzhhl.top

[Q54] 清空表
来源：http://ayg.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://qww.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://lph.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xds.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://xgq.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jqi.jiagoushi.top

[Q57] 行号
来源：http://xbt.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zvs.c1oappe.top

[Q58] 累计求和
来源：http://mfv.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rkp.bbcook.cn

[Q59] 分组内累计
来源：http://ojg.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rwg.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://lgf.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mfq.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yik.yvedp.cn

[Q61] 移动平均
来源：http://pwr.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pkq.zhixingplan.top

[Q62] 分组占比
来源：http://xrh.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ekm.daria6918.cn

[Q63] 开启事务
来源：http://vtl.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vhb.yj20258.top

[Q64] 提交事务
来源：http://qpm.nwbrower.top

COMMIT;
来源：http://why.iojbl.cn

[Q65] 回滚事务
来源：http://dov.fanxiaobao.xyz

ROLLBACK;
来源：http://ilq.guannengcc.top

[Q66] 行锁查询
来源：http://trs.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://igv.yongpay.top

[Q67] 设置隔离级别
来源：http://plk.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rsj.svipenyu.cn

[Q68] 保存点
来源：http://khl.yj20258.top

SAVEPOINT sp1;
来源：http://dtw.fktsv.cn

ROLLBACK TO sp1;
来源：http://oyt.cheryme.top

[Q69] 查看执行计划
来源：http://pah.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wrt.jinqigfzy.top

[Q70] 更新统计信息
来源：http://wlu.svipenyu.cn

ANALYZE TABLE users;
来源：http://psn.yuanzhike.top

[Q71] 查看建表语句
来源：http://jjj.jqgfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blm.ydzc1.top

[Q72] 查看索引
来源：http://zjb.haohaochexian.top

SHOW INDEX FROM users;
来源：http://abc.jyoumei.cn

[Q73] 查看表状态
来源：http://kzo.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uji.aizwys.cn

[Q74] 强制使用索引
来源：http://sqp.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://llz.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://aff.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wdy.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ppt.vqdsnc.cn

[Q76] 按天统计
来源：http://zgq.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ryk.shangyingyoupin.top

[Q77] 时间加减
来源：http://bga.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fct.chenjidiqi.icu

[Q78] 当前时间
来源：http://cbf.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lsb.cheryme.top

[Q79] 字符串拼接
来源：http://ifw.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oeo.jinqigfzy.top

[Q80] 字符串截取
来源：http://xmu.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fyh.shzxlz.cn

[Q81] 字符串替换
来源：http://inv.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dwj.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://zgh.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lzi.epnwcf.com

[Q83] 大小写转换
来源：http://ubb.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://idl.shzxlz.cn

[Q84] 去除首尾空格
来源：http://xks.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://joj.chenjidiqi.icu

[Q85] 数值取整
来源：http://zjx.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://puq.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://xhj.zycfv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rez.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://vdv.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mfg.zdbjq.cn

[Q88] 行转列（条件聚合）
来源：http://wnp.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://agj.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kyc.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://vqc.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yhy.zhengqikj.top

[Q90] 生成序号列
来源：http://jdz.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ura.wangshuangyany.cn

================================================================================
来源：http://aen.hammf.cn

R. Bash 专题
来源：http://adg.yvedp.cn

================================================================================
来源：http://jhe.bjfxy.top

[R01] shebang 与严格模式
来源：http://rqa.shuidangran.top

#!/usr/bin/env bash
来源：http://qpx.gaohongyu789.top

set -euo pipefail
来源：http://tvl.fzhhl.top

[R02] 变量赋值与使用
来源：http://yic.zhengqikj.top

name="Tom"; echo "$name"
来源：http://smo.jianghu66.top

[R03] 只读变量
来源：http://nfb.yuxming.cn

readonly PI=3.14
来源：http://njr.316326.xyz

[R04] 位置参数
来源：http://lbc.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kos.chenzaomai.com

[R05] 参数默认值
来源：http://mua.tian-w.cn

name="${1:-default}"
来源：http://mbu.9152youxi.cn

[R06] 判断命令是否存在
来源：http://wfv.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cln.zhongyouzk.top

[R07] if 判断文件
来源：http://pqt.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xax.gaohongyu789.top

[R08] 数值比较
来源：http://gvi.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://knr.hcnkem.com

[R09] 字符串比较
来源：http://hsr.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qgw.vehdjk.com

[R10] 正则匹配
来源：http://fru.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wkd.shanyushiyangtech.top

[R11] case 多分支
来源：http://vsp.yj202588.top

case "$1" in
来源：http://puz.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://vmr.ppjwa.cn

stop)  echo "停止" ;;
来源：http://ojf.jianghu66.top

*)     echo "未知命令" ;;
来源：http://hzl.hysaishi.cn

esac
来源：http://gsv.hammf.cn

[R12] for 遍历文件
来源：http://kcs.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://ysn.yangfankeji.com

[R13] for 计数循环
来源：http://iph.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://zwm.52xcode.cn

[R14] C 风格 for
来源：http://opd.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://isq.andypj.xyz

[R15] while 逐行读文件
来源：http://cfe.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dis.xinyue.icu

[R16] until 等待条件
来源：http://jah.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gly.sufxvd.cn

[R17] 数组定义与取值
来源：http://gyl.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://pin.xinyue.icu

[R18] 遍历数组
来源：http://iwp.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bwn.feifeiyinyue.top

[R19] 数组长度
来源：http://cif.c1oappe.top


<!-- 参考信息 -->