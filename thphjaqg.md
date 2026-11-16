代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ubj.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xhk.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wvu.yj20258888.top

[P04] 求长度
来源：http://kwq.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://thp.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qro.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvz.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyc.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://jhk.daxiang520.top

Go:   len(arr);  len(m)
来源：http://xjp.shzxlz.cn

Ruby: x.length;  x.size
来源：http://dxo.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxt.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://zoj.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vtv.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://adf.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ckb.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://slg.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xus.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://wvw.jiagoushi.top

Ruby: a == b
来源：http://rxx.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pgc.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hbt.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tpy.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://efr.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lop.yj202588.top

TS:   if (x == null) {}
来源：http://xqg.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nej.cucudq.cn

Go:   if x == nil {}
来源：http://ept.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://akr.fzhhl.top

C#:   if (x is null) {}
来源：http://chc.jiagoushi.top

[P07] 防抖与节流
来源：http://sow.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ftd.tarul.cn

PHP:  // 手写时间戳比较
来源：http://xbu.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rba.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://atl.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kfu.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dzp.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xns.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ozw.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://dxj.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://chw.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jvw.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jfk.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ayi.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://len.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://btu.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fef.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iwx.ydjk.org.cn

================================================================================
来源：http://kff.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uet.pycfn.com

================================================================================
来源：http://xuh.nanxuanxn.top

[Q01] 创建表
来源：http://dou.mhx1999.top

CREATE TABLE users (
来源：http://riv.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://liz.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://juc.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://uxc.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ksv.nanxinkj.top

);
来源：http://nal.sweek.top

[Q02] 创建带外键的表
来源：http://jef.ydzc1.top

CREATE TABLE orders (
来源：http://kjt.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsp.jianghu66.top

user_id INT NOT NULL,
来源：http://hzq.fehbvm.com

amount DECIMAL(10, 2),
来源：http://lah.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xof.zhixingplan.top

);
来源：http://mqc.meibo888.top

[Q03] 增加列
来源：http://qah.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jce.bbcook.cn

[Q04] 修改列类型
来源：http://hkq.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pic.ehwqpu.com

[Q05] 重命名列
来源：http://bsa.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mdf.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://ebz.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xgf.yueranfly.top

[Q07] 删除表
来源：http://iad.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://cbt.aizwys.cn

[Q08] 创建普通索引
来源：http://tyk.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ojp.yonumen.top

[Q09] 创建唯一索引
来源：http://sem.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wsv.pengpengdd.cyou

[Q10] 插入单行
来源：http://lmw.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jyt.yuanzhike.top

[Q11] 一次插入多行
来源：http://gcs.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tec.yj202588.top

[Q12] 插入后取自增 ID
来源：http://liu.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://uqf.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fje.zdqjudy.top

[Q13] 忽略重复插入
来源：http://knr.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kgx.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://spn.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://izf.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dav.xziqi.cn

[Q15] 查询全部
来源：http://bds.nanxinkj.top

SELECT * FROM users;
来源：http://udb.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://wsw.wangdashe.top

SELECT id, name FROM users;
来源：http://nir.havefunace.top

[Q17] 条件查询
来源：http://zpc.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mju.cqqwz.cn

[Q18] 模糊匹配
来源：http://olh.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pmn.pycfn.com

[Q19] 范围查询
来源：http://gsx.hnqzz.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qyr.zhiwuduotai.top

[Q20] IN 列表
来源：http://ene.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xee.cqqwz.cn

[Q21] 空值判断
来源：http://rug.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wgz.yfazqb.com

[Q22] 排序
来源：http://wsw.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qzc.hongshengwenyu.top

[Q23] 分页
来源：http://jxw.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://adn.sysykeji.top

[Q24] 去重
来源：http://kyr.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://bzx.yuxming.cn

[Q25] 只取前 N 条
来源：http://dtw.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://npu.yuxming.cn

[Q26] 计数
来源：http://jje.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://lmu.zhixingplan.top

[Q27] 条件计数
来源：http://qag.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mdz.hywenlv.cn

[Q28] 求和与平均
来源：http://wrh.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dra.sufxvd.cn

[Q29] 最大最小值
来源：http://hop.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vhh.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://plm.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qzl.jqgufenzy.top

[Q31] 分组后过滤
来源：http://jho.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fin.shangyingyoupin.top

[Q32] 分组拼接字符串
来源：http://xda.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kgr.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gvf.fengsongda.top

[Q33] 多列分组
来源：http://vkr.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zqa.jianghu66.top

[Q34] 每组取第一条
来源：http://bcf.redwolf501.top

SELECT * FROM (
来源：http://kgh.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bbp.guannengcc.top

) t WHERE rn = 1;
来源：http://lfy.gotoacloud.top

[Q35] 内连接
来源：http://gdc.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://llz.yuxming.cn

[Q36] 左连接
来源：http://feh.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aks.meibo888.top

[Q37] 右连接
来源：http://emj.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lxt.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://qqk.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tyv.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://shz.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zax.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eoj.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zpd.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rfu.tanke756.top

[Q41] 多表连接
来源：http://mhg.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eoc.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://tce.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://rpm.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://hzy.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://qpz.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://knl.xylfe.cn

[Q43] 标量子查询
来源：http://sra.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://abq.yvedp.cn

[Q44] IN 子查询
来源：http://pze.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dqo.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://kpw.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aon.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://oso.bbcook.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://idp.yueranfly.top

[Q47] 与平均值比较
来源：http://dux.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qdz.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://gto.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ggv.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://ehi.epnwcf.com

[Q49] 更新单行
来源：http://mlm.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eap.vehdjk.com

[Q50] 批量更新
来源：http://hsf.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aen.zdbjq.cn

[Q51] 用子查询更新
来源：http://xmi.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wal.cucudq.cn

[Q52] 删除指定行
来源：http://ehf.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://tip.ehwqpu.com

[Q53] 按条件删除
来源：http://rdq.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gee.aibaodan.cn

[Q54] 清空表
来源：http://vqa.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://lhk.birdmap.top

[Q55] 排名（并列占位）
来源：http://sah.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vvt.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://aqo.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dop.yvedp.cn

[Q57] 行号
来源：http://rgr.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oak.ehwqpu.com

[Q58] 累计求和
来源：http://zco.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cpp.andypj.xyz

[Q59] 分组内累计
来源：http://pov.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hta.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://uok.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bom.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rlr.jlsjyb.cn

[Q61] 移动平均
来源：http://fam.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pju.vehdjk.com

[Q62] 分组占比
来源：http://bme.xuetiantiany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vkp.pycfn.com

[Q63] 开启事务
来源：http://jwz.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://dlt.xziqi.cn

[Q64] 提交事务
来源：http://gwj.birdmap.top

COMMIT;
来源：http://scx.birdmap.top

[Q65] 回滚事务
来源：http://ljo.tianlin.xyz

ROLLBACK;
来源：http://ghi.ivvv.top

[Q66] 行锁查询
来源：http://hgh.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vdo.uphjek.com

[Q67] 设置隔离级别
来源：http://jwl.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://awq.jinqigufen.top

[Q68] 保存点
来源：http://juj.sxryk.cn

SAVEPOINT sp1;
来源：http://npw.tanke756.top

ROLLBACK TO sp1;
来源：http://prx.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://syj.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wok.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://tnb.epnwcf.com

ANALYZE TABLE users;
来源：http://tqu.gaohongyu789.top

[Q71] 查看建表语句
来源：http://ofs.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lgf.epnwcf.com

[Q72] 查看索引
来源：http://wnv.smart0.xyz

SHOW INDEX FROM users;
来源：http://vuj.sufxvd.cn

[Q73] 查看表状态
来源：http://zft.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nyb.xziqi.cn

[Q74] 强制使用索引
来源：http://ori.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xng.aizwys.cn

[Q75] 日期格式化
来源：http://aoz.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rrk.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://owd.zhoulong.xyz

[Q76] 按天统计
来源：http://vxe.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aaz.jqgufenzy.top

[Q77] 时间加减
来源：http://olf.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pwx.shangyingyoupin.top

[Q78] 当前时间
来源：http://aky.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fkk.gogol.net.cn

[Q79] 字符串拼接
来源：http://yfp.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yjt.hcnkem.com

[Q80] 字符串截取
来源：http://lbc.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sjd.daxiang520.top

[Q81] 字符串替换
来源：http://mwd.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fod.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://fjp.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yuy.jqgufenzy.top

[Q83] 大小写转换
来源：http://vwf.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qof.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://enu.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://exp.shuidangran.top

[Q85] 数值取整
来源：http://aep.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://adl.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://leg.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jtk.xuanzx.com

[Q87] JSON 字段做条件
来源：http://qrs.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bop.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://din.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://emn.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://idd.hnqzz.top

[Q89] 判断表是否存在
来源：http://jpf.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://teh.yueranfly.top

[Q90] 生成序号列
来源：http://uwd.yanxiufei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vik.yanxiufei.cn

================================================================================
来源：http://yrw.gogol.net.cn

R. Bash 专题
来源：http://moc.guowangkeji.top

================================================================================
来源：http://rov.uphjek.com

[R01] shebang 与严格模式
来源：http://qgx.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://luw.snrcjt.cn

set -euo pipefail
来源：http://zok.aizwys.cn

[R02] 变量赋值与使用
来源：http://jqj.guowangkeji.top

name="Tom"; echo "$name"
来源：http://gyn.sufxvd.cn

[R03] 只读变量
来源：http://pey.zhaomingkeji.xyz

readonly PI=3.14
来源：http://bxo.pycfn.com

[R04] 位置参数
来源：http://cts.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bda.hongshengwenyu.top

[R05] 参数默认值
来源：http://iua.bbcook.cn

name="${1:-default}"
来源：http://ljt.redwolf501.top

[R06] 判断命令是否存在
来源：http://ktx.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://thd.chenzaomai.com

[R07] if 判断文件
来源：http://rbr.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bkh.zhaomingkeji.xyz

[R08] 数值比较
来源：http://tft.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ngr.yj202588.top

[R09] 字符串比较
来源：http://ceo.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dti.sysykeji.top

[R10] 正则匹配
来源：http://jby.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://owd.zhongyouzk.top

[R11] case 多分支
来源：http://cak.sysykeji.top

case "$1" in
来源：http://hcb.xuanzx.com

start) echo "启动" ;;
来源：http://uvc.hfpthk.cn

stop)  echo "停止" ;;
来源：http://zqk.fktsv.cn

*)     echo "未知命令" ;;
来源：http://djo.c1oappe.top

esac
来源：http://iko.zhoulong.xyz

[R12] for 遍历文件
来源：http://jpv.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://zzs.yfazqb.com

[R13] for 计数循环
来源：http://ude.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://lnd.yfazqb.com

[R14] C 风格 for
来源：http://nwz.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zqp.kuanghao11.cn

[R15] while 逐行读文件
来源：http://ahw.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vdx.yj20258.top

[R16] until 等待条件
来源：http://bhs.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gsc.yfazqb.com

[R17] 数组定义与取值
来源：http://xec.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://twy.hysaishi.cn

[R18] 遍历数组
来源：http://htd.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dhz.yongpay.top

[R19] 数组长度
来源：http://dbh.chenlongwang.top


<!-- 参考信息 -->