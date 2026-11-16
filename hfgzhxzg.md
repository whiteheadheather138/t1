代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://htx.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mxa.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sve.vehdjk.com

[P04] 求长度
来源：http://hen.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vpn.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gef.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zfv.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jkz.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://fln.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://cgl.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://qbp.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xzm.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://chz.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wqc.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://trk.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sxp.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uyo.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qgu.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fpr.aizwys.cn

Ruby: a == b
来源：http://dxd.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vei.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://itv.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vps.hammf.cn

PHP:  if (empty($x)) {}
来源：http://zzl.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kec.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://cyu.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lvi.shzxlz.cn

Go:   if x == nil {}
来源：http://jkc.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rqa.fengsongda.top

C#:   if (x is null) {}
来源：http://pmz.yanxiufei.cn

[P07] 防抖与节流
来源：http://vpd.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://miq.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://guf.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zgg.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pml.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xlv.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uxi.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fme.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://avc.iojbl.cn

[P08] 处理浮点精度问题
来源：http://exo.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cqf.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gjs.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://whi.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://brp.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yoj.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tni.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://skk.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://htq.chenlongwang.top

================================================================================
来源：http://ufy.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hvn.epnwcf.com

================================================================================
来源：http://ish.daria6918.cn

[Q01] 创建表
来源：http://rxm.jinqigfzy.top

CREATE TABLE users (
来源：http://cvq.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zar.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://mdm.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://qry.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bvu.cheryme.top

);
来源：http://orr.sweek.top

[Q02] 创建带外键的表
来源：http://nye.feifeiyinyue.top

CREATE TABLE orders (
来源：http://ikq.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yql.aizwys.cn

user_id INT NOT NULL,
来源：http://eju.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://ein.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eqk.feifeiyinyue.top

);
来源：http://pxn.zhijiandao.cn

[Q03] 增加列
来源：http://zrh.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dsd.fktsv.cn

[Q04] 修改列类型
来源：http://csm.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://orm.zhoulong.xyz

[Q05] 重命名列
来源：http://zjg.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xvu.epnwcf.com

[Q06] 删除列
来源：http://nyz.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://wfm.smart0.xyz

[Q07] 删除表
来源：http://wgu.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://xji.jlsjyb.cn

[Q08] 创建普通索引
来源：http://vgg.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://txu.daxiang520.top

[Q09] 创建唯一索引
来源：http://mlk.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://stj.yvedp.cn

[Q10] 插入单行
来源：http://obc.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zyz.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://huj.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kne.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://ovp.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://rxw.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://urj.ppjwa.cn

[Q13] 忽略重复插入
来源：http://mxu.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eca.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://fqs.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jjc.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xdk.xuanzx.com

[Q15] 查询全部
来源：http://tvm.hnqzz.top

SELECT * FROM users;
来源：http://ims.sweek.top

[Q16] 查询指定列
来源：http://neu.fengsongda.top

SELECT id, name FROM users;
来源：http://cfi.xinyue.icu

[Q17] 条件查询
来源：http://zff.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wnf.guannengcc.top

[Q18] 模糊匹配
来源：http://avj.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sue.ehwqpu.com

[Q19] 范围查询
来源：http://uxp.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bhg.cdnleiting.top

[Q20] IN 列表
来源：http://xwj.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jvl.hysaishi.cn

[Q21] 空值判断
来源：http://lts.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ybx.xuanzx.com

[Q22] 排序
来源：http://ugv.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hks.mhx1999.top

[Q23] 分页
来源：http://omn.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uaq.yanxiufei.cn

[Q24] 去重
来源：http://ksj.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://pyg.pycfn.com

[Q25] 只取前 N 条
来源：http://rmy.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eys.fengsongda.top

[Q26] 计数
来源：http://mrv.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://xsl.bbcook.cn

[Q27] 条件计数
来源：http://vgx.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xlv.birdmap.top

[Q28] 求和与平均
来源：http://ujr.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tro.meibo888.top

[Q29] 最大最小值
来源：http://hwv.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tqu.havefunace.top

[Q30] 分组统计
来源：http://sgc.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uuu.cqqwz.cn

[Q31] 分组后过滤
来源：http://svi.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kuo.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://hpx.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rld.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ylp.cucudq.cn

[Q33] 多列分组
来源：http://xsj.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nef.fengsongda.top

[Q34] 每组取第一条
来源：http://qls.aibaodan.cn

SELECT * FROM (
来源：http://kei.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mvq.sjlbkw.cn

) t WHERE rn = 1;
来源：http://sel.redwolf501.top

[Q35] 内连接
来源：http://ozf.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pqg.yfazqb.com

[Q36] 左连接
来源：http://ctm.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hcq.nanxinkj.top

[Q37] 右连接
来源：http://uhu.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lpl.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kha.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lmo.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://sjm.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://cbi.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qmk.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://vny.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bdn.shanyushiyangtech.top

[Q41] 多表连接
来源：http://bjk.ydjk.org.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vkm.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://fon.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://dnp.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://csj.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://lhf.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ofw.ydjk.org.cn

[Q43] 标量子查询
来源：http://iri.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bya.sysykeji.top

[Q44] IN 子查询
来源：http://tiq.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pxr.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://fac.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ast.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://zvy.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fzn.daria6918.cn

[Q47] 与平均值比较
来源：http://wjz.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nqe.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://atj.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eil.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://zfk.yanxiufei.cn

[Q49] 更新单行
来源：http://veg.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tiq.zdbjq.cn

[Q50] 批量更新
来源：http://fam.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bwk.svipenyu.cn

[Q51] 用子查询更新
来源：http://fgt.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pbg.fehbvm.com

[Q52] 删除指定行
来源：http://ada.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://qvg.tian-w.cn

[Q53] 按条件删除
来源：http://wne.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tis.chenlongwang.top

[Q54] 清空表
来源：http://qtr.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://nih.yueranfly.top

[Q55] 排名（并列占位）
来源：http://kln.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://djo.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://alg.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pue.cashguo.top

[Q57] 行号
来源：http://qhx.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jas.sxryk.cn

[Q58] 累计求和
来源：http://iok.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://agd.chenjidiqi.icu

[Q59] 分组内累计
来源：http://ahl.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yfx.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://gqe.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ien.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pns.ehwqpu.com

[Q61] 移动平均
来源：http://tuf.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oik.ctjpmb.com

[Q62] 分组占比
来源：http://jnz.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://syl.andypj.xyz

[Q63] 开启事务
来源：http://dpo.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eto.ydzc1.top

[Q64] 提交事务
来源：http://zfg.jqgfzy.top

COMMIT;
来源：http://lny.ybcxt.top

[Q65] 回滚事务
来源：http://sfu.birdmap.top

ROLLBACK;
来源：http://nmn.yangfankeji.com

[Q66] 行锁查询
来源：http://xrb.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dkf.jinqigufen.top

[Q67] 设置隔离级别
来源：http://wld.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bin.hongshengwenyu.top

[Q68] 保存点
来源：http://yfy.sweek.top

SAVEPOINT sp1;
来源：http://jzz.gzhubu.top

ROLLBACK TO sp1;
来源：http://nvt.vqdsnc.cn

[Q69] 查看执行计划
来源：http://uzg.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hun.fktsv.cn

[Q70] 更新统计信息
来源：http://egv.ydjk.org.cn

ANALYZE TABLE users;
来源：http://axk.ppjwa.cn

[Q71] 查看建表语句
来源：http://fin.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xcs.xinyue.icu

[Q72] 查看索引
来源：http://khe.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://jdz.xuanzx.com

[Q73] 查看表状态
来源：http://eoo.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://htc.ctjpmb.com

[Q74] 强制使用索引
来源：http://bpm.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lay.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://kfu.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bma.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gru.52xcode.cn

[Q76] 按天统计
来源：http://far.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eii.chenjidiqi.icu

[Q77] 时间加减
来源：http://gui.svipenyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://niy.meibo888.top

[Q78] 当前时间
来源：http://vrz.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kpp.ivvv.top

[Q79] 字符串拼接
来源：http://ene.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://afy.zhiwuduotai.top

[Q80] 字符串截取
来源：http://pxd.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cyj.zycfv.cn

[Q81] 字符串替换
来源：http://sol.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bnc.tian-w.cn

[Q82] 字符长度与字节长度
来源：http://wbu.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tvy.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://kej.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tyj.aizwys.cn

[Q84] 去除首尾空格
来源：http://glt.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://buz.zycfv.cn

[Q85] 数值取整
来源：http://fhu.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ayu.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://pwd.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wcq.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://gdg.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fmx.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://qhm.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://srd.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yuc.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://eez.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jmm.feifeiyinyue.top

[Q90] 生成序号列
来源：http://vjq.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lfk.xuetiantiany.cn

================================================================================
来源：http://tap.zdbjq.cn

R. Bash 专题
来源：http://hwq.zycfv.cn

================================================================================
来源：http://mun.tanke756.top

[R01] shebang 与严格模式
来源：http://yyv.zdqjudy.top

#!/usr/bin/env bash
来源：http://gxk.ppjwa.cn

set -euo pipefail
来源：http://tah.jqgfzy.top

[R02] 变量赋值与使用
来源：http://mbu.sysykeji.top

name="Tom"; echo "$name"
来源：http://waw.yj20258.top

[R03] 只读变量
来源：http://bpb.shanyushiyangkeji.top

readonly PI=3.14
来源：http://owd.pengpengdd.cyou

[R04] 位置参数
来源：http://tnr.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hrj.316326.xyz

[R05] 参数默认值
来源：http://ila.316326.xyz

name="${1:-default}"
来源：http://sol.hesvh.cn

[R06] 判断命令是否存在
来源：http://iet.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fed.snrcjt.cn

[R07] if 判断文件
来源：http://jsu.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qok.hfpthk.cn

[R08] 数值比较
来源：http://izr.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gku.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://url.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zgf.52xcode.cn

[R10] 正则匹配
来源：http://les.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bhw.cqqwz.cn

[R11] case 多分支
来源：http://fss.yueranfly.top

case "$1" in
来源：http://imb.gzhubu.top

start) echo "启动" ;;
来源：http://rgm.cdnleiting.top

stop)  echo "停止" ;;
来源：http://wes.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://xxp.cdnleiting.top

esac
来源：http://gvt.ppjwa.cn

[R12] for 遍历文件
来源：http://wcp.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://lyr.xuetiantiany.cn

[R13] for 计数循环
来源：http://hev.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://ury.c1oappe.top

[R14] C 风格 for
来源：http://euq.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cxq.zhixingplan.top

[R15] while 逐行读文件
来源：http://yku.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sba.svipenyu.cn

[R16] until 等待条件
来源：http://zsx.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ats.vehdjk.com

[R17] 数组定义与取值
来源：http://rea.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://wdi.zhoulong.xyz

[R18] 遍历数组
来源：http://zyt.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://azo.ivvv.top

[R19] 数组长度
来源：http://dss.hnxiangtu.top


<!-- 参考信息 -->