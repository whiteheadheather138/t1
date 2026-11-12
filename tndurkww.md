代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qhv.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qla.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mxl.jlsjyb.cn

[P04] 求长度
来源：http://nth.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rrw.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ebh.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cvv.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://taj.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://tas.xziqi.cn

Go:   len(arr);  len(m)
来源：http://wpb.redwolf501.top

Ruby: x.length;  x.size
来源：http://ror.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://quq.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://hvi.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gmb.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nhj.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vao.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://srt.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zwq.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://wyx.pengpengdd.cyou

Ruby: a == b
来源：http://xnl.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pjm.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jsp.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lkj.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://aoi.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uae.iojbl.cn

TS:   if (x == null) {}
来源：http://fov.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kcc.zhongyouzk.top

Go:   if x == nil {}
来源：http://vci.iojbl.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wgd.zhongyouzk.top

C#:   if (x is null) {}
来源：http://hij.fehbvm.com

[P07] 防抖与节流
来源：http://nug.sufxvd.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://glx.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://prh.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhs.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymr.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://utf.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xir.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rsa.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rnc.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://fjn.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gmm.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://boe.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spw.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kth.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://agr.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bld.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vek.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ttj.zhongyouzk.top

================================================================================
来源：http://ybj.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fwa.wangdashe.top

================================================================================
来源：http://fay.cashguo.top

[Q01] 创建表
来源：http://eyj.nanxinkj.top

CREATE TABLE users (
来源：http://jrg.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://krv.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://lbz.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://ria.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://plz.bbcook.cn

);
来源：http://bnp.daria6918.cn

[Q02] 创建带外键的表
来源：http://kzl.nanxuanxn.top

CREATE TABLE orders (
来源：http://iof.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gcn.uphjek.com

user_id INT NOT NULL,
来源：http://zjh.bbcook.cn

amount DECIMAL(10, 2),
来源：http://ggs.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zsa.sjlbkw.cn

);
来源：http://nne.ydjk.org.cn

[Q03] 增加列
来源：http://qkn.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rwl.birdmap.top

[Q04] 修改列类型
来源：http://fgk.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iwe.tianlin.xyz

[Q05] 重命名列
来源：http://riv.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chc.ppjwa.cn

[Q06] 删除列
来源：http://tmi.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cqt.nanxinkj.top

[Q07] 删除表
来源：http://dhc.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://wuz.fktsv.cn

[Q08] 创建普通索引
来源：http://dbq.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kvy.havefunace.top

[Q09] 创建唯一索引
来源：http://ofa.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ruy.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://qjx.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxs.ydjk.org.cn

[Q11] 一次插入多行
来源：http://juq.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ntf.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://qdv.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://eid.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aqn.bbcook.cn

[Q13] 忽略重复插入
来源：http://bwf.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vyy.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://san.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qqb.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://brs.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://tkt.andypj.xyz

SELECT * FROM users;
来源：http://zaf.hesvh.cn

[Q16] 查询指定列
来源：http://waf.epnwcf.com

SELECT id, name FROM users;
来源：http://orv.sysykeji.top

[Q17] 条件查询
来源：http://wbv.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mkg.wangdashe.top

[Q18] 模糊匹配
来源：http://kqm.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://emb.bbcook.cn

[Q19] 范围查询
来源：http://ruu.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gsi.tanke756.top

[Q20] IN 列表
来源：http://wry.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jnf.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://fam.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qpm.hysaishi.cn

[Q22] 排序
来源：http://fbf.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cki.zycfv.cn

[Q23] 分页
来源：http://fcs.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tje.vqdsnc.cn

[Q24] 去重
来源：http://qoi.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://qin.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://ifh.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xkl.ydzc1.top

[Q26] 计数
来源：http://isj.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://fgw.xinyue.icu

[Q27] 条件计数
来源：http://qhs.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nsz.hammf.cn

[Q28] 求和与平均
来源：http://wdd.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ltc.dashuyun.cn

[Q29] 最大最小值
来源：http://qou.tanke756.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://twk.hysaishi.cn

[Q30] 分组统计
来源：http://etb.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wxf.xylfe.cn

[Q31] 分组后过滤
来源：http://pck.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jyn.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://lhl.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wop.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ues.zhijiandao.cn

[Q33] 多列分组
来源：http://uoa.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fvw.vehdjk.com

[Q34] 每组取第一条
来源：http://nlj.hnxiangtu.top

SELECT * FROM (
来源：http://vrn.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eyt.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://odt.meibo888.top

[Q35] 内连接
来源：http://fdr.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://drt.yvedp.cn

[Q36] 左连接
来源：http://bet.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fnp.wangdashe.top

[Q37] 右连接
来源：http://jkt.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wtv.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hez.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://noj.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://sqq.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fzz.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dwf.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tmm.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mdp.0kj1m.cn

[Q41] 多表连接
来源：http://cen.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://aev.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://une.jlsjyb.cn

JOIN products p ON p.id = o.product_id;
来源：http://hqh.zhijiandao.cn

[Q42] 连接条件附加过滤
来源：http://pem.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://aiy.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://etz.ehwqpu.com

[Q43] 标量子查询
来源：http://rfw.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fdz.andypj.xyz

[Q44] IN 子查询
来源：http://cgc.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://agc.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://fmk.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dxu.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://uod.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vwl.aizwys.cn

[Q47] 与平均值比较
来源：http://gvn.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bny.yj20258.top

[Q48] CTE 公用表表达式
来源：http://ljn.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uba.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://lgp.birdmap.top

[Q49] 更新单行
来源：http://ylt.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vgl.jinqigfzy.top

[Q50] 批量更新
来源：http://hqr.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qjt.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://don.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kli.xziqi.cn

[Q52] 删除指定行
来源：http://biz.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://dnf.hongshengwenyu.top

[Q53] 按条件删除
来源：http://ewc.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nvk.xinyue.icu

[Q54] 清空表
来源：http://cgx.yueranfly.top

TRUNCATE TABLE logs;
来源：http://tum.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://axf.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zpg.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://hod.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yrp.shangyingyoupin.top

[Q57] 行号
来源：http://ntg.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qhl.cheryme.top

[Q58] 累计求和
来源：http://dve.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ieh.hnxiangtu.top

[Q59] 分组内累计
来源：http://wrk.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aia.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://jno.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://agj.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://btj.316326.xyz

[Q61] 移动平均
来源：http://dnc.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hwl.cdnleiting.top

[Q62] 分组占比
来源：http://iek.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vry.hammf.cn

[Q63] 开启事务
来源：http://nod.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yif.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://dtx.bbcook.cn

COMMIT;
来源：http://agd.jqgufenzy.top

[Q65] 回滚事务
来源：http://aqq.sweek.top

ROLLBACK;
来源：http://wwn.bbcook.cn

[Q66] 行锁查询
来源：http://jzh.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dgh.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://ewf.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgt.bjfxy.top

[Q68] 保存点
来源：http://eqc.hysaishi.cn

SAVEPOINT sp1;
来源：http://pfb.zhengqikj.top

ROLLBACK TO sp1;
来源：http://apv.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://adg.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://amy.yj20258888.top

[Q70] 更新统计信息
来源：http://opc.jqgufenzy.top

ANALYZE TABLE users;
来源：http://wyz.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://iup.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pnb.hnqzz.top

[Q72] 查看索引
来源：http://arq.0kj1m.cn

SHOW INDEX FROM users;
来源：http://ggm.xuanzx.com

[Q73] 查看表状态
来源：http://yxe.hnxiangtu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vwe.jinqigfzy.top

[Q74] 强制使用索引
来源：http://fch.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ibm.redwolf501.top

[Q75] 日期格式化
来源：http://ixo.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fll.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yyw.cqqwz.cn

[Q76] 按天统计
来源：http://xyn.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fnk.chenlongwang.top

[Q77] 时间加减
来源：http://ibk.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nyk.aizwys.cn

[Q78] 当前时间
来源：http://cjf.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rgr.yuanzhike.top

[Q79] 字符串拼接
来源：http://hnz.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yax.wangshuangyany.cn

[Q80] 字符串截取
来源：http://fem.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ykv.0kj1m.cn

[Q81] 字符串替换
来源：http://bbq.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nyu.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://asx.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vlf.quarkkingdee.top

[Q83] 大小写转换
来源：http://irj.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nms.316326.xyz

[Q84] 去除首尾空格
来源：http://bqb.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://xrv.tanke756.top

[Q85] 数值取整
来源：http://jkq.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rjz.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://myl.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nly.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://whn.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rdc.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://rfw.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qtz.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nbh.dianchejie.cn

[Q89] 判断表是否存在
来源：http://ygf.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bpf.tianlin.xyz

[Q90] 生成序号列
来源：http://pvl.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://usd.svipenyu.cn

================================================================================
来源：http://abp.daxiang520.top

R. Bash 专题
来源：http://keh.pengpengdd.cyou

================================================================================
来源：http://lsk.ehwqpu.com

[R01] shebang 与严格模式
来源：http://qfq.tian-w.cn

#!/usr/bin/env bash
来源：http://jyi.chenlongwang.top

set -euo pipefail
来源：http://mez.fehbvm.com

[R02] 变量赋值与使用
来源：http://pki.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://jyo.tian-w.cn

[R03] 只读变量
来源：http://zda.hnqzz.top

readonly PI=3.14
来源：http://rlt.ivvv.top

[R04] 位置参数
来源：http://niz.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qpx.hcnkem.com

[R05] 参数默认值
来源：http://euk.chenzaomai.com

name="${1:-default}"
来源：http://ird.xylfe.cn

[R06] 判断命令是否存在
来源：http://eds.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ycm.sufxvd.cn

[R07] if 判断文件
来源：http://vlv.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hym.yfazqb.com

[R08] 数值比较
来源：http://ydl.redwolf501.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dcv.nanxuanxn.top

[R09] 字符串比较
来源：http://via.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://joc.dianchejie.cn

[R10] 正则匹配
来源：http://sbu.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dse.hfpthk.cn

[R11] case 多分支
来源：http://ati.svipenyu.cn

case "$1" in
来源：http://ezc.iojbl.cn

start) echo "启动" ;;
来源：http://ulg.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://pef.fktsv.cn

*)     echo "未知命令" ;;
来源：http://ytw.fzhhl.top

esac
来源：http://jjd.jinqigfzy.top

[R12] for 遍历文件
来源：http://crr.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://igd.tanke756.top

[R13] for 计数循环
来源：http://hny.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://ppf.ppjwa.cn

[R14] C 风格 for
来源：http://uqh.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zog.ctjpmb.com

[R15] while 逐行读文件
来源：http://adj.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fex.ydzc1.top

[R16] until 等待条件
来源：http://vnc.tian-w.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uum.hfpthk.cn

[R17] 数组定义与取值
来源：http://bzv.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gaa.quarkkingdee.top

[R18] 遍历数组
来源：http://xol.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bed.tian-w.cn

[R19] 数组长度
来源：http://gso.yuanzhike.top


<!-- 参考信息 -->