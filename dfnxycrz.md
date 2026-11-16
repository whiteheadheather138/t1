代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qjx.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cmy.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nfi.nwbrower.top

[P04] 求长度
来源：http://qhs.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cik.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wee.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nsm.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hcn.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://zif.cashguo.top

Go:   len(arr);  len(m)
来源：http://hmq.0kj1m.cn

Ruby: x.length;  x.size
来源：http://svd.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://diw.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://lsx.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://yha.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ksx.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uli.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gfy.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://mns.jinghuilouyu.cn

Ruby: a == b
来源：http://gbn.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oyz.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vrt.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://frz.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://ckq.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vrk.jqgufenzy.top

TS:   if (x == null) {}
来源：http://fwb.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kwe.aizwys.cn

Go:   if x == nil {}
来源：http://mjj.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nvg.yfazqb.com

C#:   if (x is null) {}
来源：http://woj.kuanghao11.cn

[P07] 防抖与节流
来源：http://ibt.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hzz.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://etx.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezt.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azc.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xlg.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jpq.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uoq.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jzo.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://dla.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vxr.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://paf.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cuh.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nmb.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://czh.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jlq.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xiw.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xkr.jianghu66.top

================================================================================
来源：http://mbj.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://erb.yj20258888.top

================================================================================
来源：http://xmw.cucudq.cn

[Q01] 创建表
来源：http://rly.daxiang520.top

CREATE TABLE users (
来源：http://wbg.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yiv.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://ivr.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://vqc.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://chn.gaohongyu789.top

);
来源：http://wxd.yongpay.top

[Q02] 创建带外键的表
来源：http://ymz.yonumen.top

CREATE TABLE orders (
来源：http://hxt.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://chy.sweek.top

user_id INT NOT NULL,
来源：http://whe.pycfn.com

amount DECIMAL(10, 2),
来源：http://cmb.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qyw.xuetiantiany.cn

);
来源：http://kbc.jqgfzy.top

[Q03] 增加列
来源：http://jfm.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rkb.jiagoushi.top

[Q04] 修改列类型
来源：http://ykg.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zpa.nwbrower.top

[Q05] 重命名列
来源：http://ngb.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zjr.smart0.xyz

[Q06] 删除列
来源：http://rtv.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://imy.yanxiufei.cn

[Q07] 删除表
来源：http://fcv.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://dfd.nwbrower.top

[Q08] 创建普通索引
来源：http://wge.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cju.pycfn.com

[Q09] 创建唯一索引
来源：http://aob.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ukc.fehbvm.com

[Q10] 插入单行
来源：http://voj.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wde.haohaochexian.top

[Q11] 一次插入多行
来源：http://vri.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yud.yonumen.top

[Q12] 插入后取自增 ID
来源：http://dpc.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tkk.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dfr.shzxlz.cn

[Q13] 忽略重复插入
来源：http://yfx.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rxp.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://sqg.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://swl.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zsm.wangdashe.top

[Q15] 查询全部
来源：http://env.daxiang520.top

SELECT * FROM users;
来源：http://nij.zhongyouzk.top

[Q16] 查询指定列
来源：http://ttx.hesvh.cn

SELECT id, name FROM users;
来源：http://lxj.uphjek.com

[Q17] 条件查询
来源：http://ybe.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ooi.zdqjudy.top

[Q18] 模糊匹配
来源：http://kyw.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xjy.gogol.net.cn

[Q19] 范围查询
来源：http://tyz.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://opv.pengpengdd.cyou

[Q20] IN 列表
来源：http://efh.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lwb.vehdjk.com

[Q21] 空值判断
来源：http://ipy.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nfm.gogol.net.cn

[Q22] 排序
来源：http://dbl.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ejp.yanxiufei.cn

[Q23] 分页
来源：http://cmq.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wdu.gogol.net.cn

[Q24] 去重
来源：http://czn.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://bua.daxiang520.top

[Q25] 只取前 N 条
来源：http://ovj.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tjl.xuetiantiany.cn

[Q26] 计数
来源：http://bxz.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://rjx.vqdsnc.cn

[Q27] 条件计数
来源：http://rqk.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hyv.feifeiyinyue.top

[Q28] 求和与平均
来源：http://ipe.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bva.ydjk.org.cn

[Q29] 最大最小值
来源：http://uwn.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jkb.ydzc1.top

[Q30] 分组统计
来源：http://upq.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gpz.gogol.net.cn

[Q31] 分组后过滤
来源：http://nfc.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pes.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://hpz.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zks.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bxk.andypj.xyz

[Q33] 多列分组
来源：http://czd.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ivq.hcnkem.com

[Q34] 每组取第一条
来源：http://sgd.chenzaomai.com

SELECT * FROM (
来源：http://xwy.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fqp.fehbvm.com

) t WHERE rn = 1;
来源：http://plf.vehdjk.com

[Q35] 内连接
来源：http://rob.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sdx.wangshuangyany.cn

[Q36] 左连接
来源：http://fld.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ewy.sxryk.cn

[Q37] 右连接
来源：http://qak.zhaomingkeji.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wgy.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sqb.jyoumei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://skd.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://uhp.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kex.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jdd.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://out.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://glw.redwolf501.top

[Q41] 多表连接
来源：http://msg.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://luv.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://xoi.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://zmb.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://ajy.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://xon.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jsu.yj20258888.top

[Q43] 标量子查询
来源：http://bye.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kbv.ydzc1.top

[Q44] IN 子查询
来源：http://muc.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://plh.yonumen.top

[Q45] EXISTS 判断存在
来源：http://bli.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zqb.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://wnk.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://krs.epnwcf.com

[Q47] 与平均值比较
来源：http://tcc.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ozn.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://byp.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://axi.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://mvi.ppjwa.cn

[Q49] 更新单行
来源：http://juq.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mqp.yfazqb.com

[Q50] 批量更新
来源：http://gsa.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iac.yj202588.top

[Q51] 用子查询更新
来源：http://dwd.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hxv.yueranfly.top

[Q52] 删除指定行
来源：http://qya.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://gbn.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://fgj.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lzw.redwolf501.top

[Q54] 清空表
来源：http://bmt.fengsongda.top

TRUNCATE TABLE logs;
来源：http://cgw.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://owy.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qyr.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://xvf.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mwu.gotoacloud.top

[Q57] 行号
来源：http://vwd.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxn.tarul.cn

[Q58] 累计求和
来源：http://usj.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ytb.hammf.cn

[Q59] 分组内累计
来源：http://xzx.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ias.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://teu.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tgw.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aki.hywenlv.cn

[Q61] 移动平均
来源：http://oiu.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ove.hywenlv.cn

[Q62] 分组占比
来源：http://irj.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqh.yonumen.top

[Q63] 开启事务
来源：http://seq.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://srl.gzhubu.top

[Q64] 提交事务
来源：http://ren.hywenlv.cn

COMMIT;
来源：http://jhk.jlsjyb.cn

[Q65] 回滚事务
来源：http://anw.wangdashe.top

ROLLBACK;
来源：http://xda.sysykeji.top

[Q66] 行锁查询
来源：http://jlv.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://env.cheryme.top

[Q67] 设置隔离级别
来源：http://zji.fengsongda.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://srg.dianchejie.cn

[Q68] 保存点
来源：http://spx.dianchejie.cn

SAVEPOINT sp1;
来源：http://jcl.jqgfzy.top

ROLLBACK TO sp1;
来源：http://fbj.fengsongda.top

[Q69] 查看执行计划
来源：http://jzr.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://stp.hammf.cn

[Q70] 更新统计信息
来源：http://epu.zycfv.cn

ANALYZE TABLE users;
来源：http://nyz.mhx1999.top

[Q71] 查看建表语句
来源：http://nuz.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ynu.ydjk.org.cn

[Q72] 查看索引
来源：http://xea.jqgfzy.top

SHOW INDEX FROM users;
来源：http://uza.meibo888.top

[Q73] 查看表状态
来源：http://ybc.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dry.yueranfly.top

[Q74] 强制使用索引
来源：http://bsq.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uhy.shzxlz.cn

[Q75] 日期格式化
来源：http://qzc.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rwy.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xqh.guowangkeji.top

[Q76] 按天统计
来源：http://jrd.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mil.xuanzx.com

[Q77] 时间加减
来源：http://foj.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mze.redwolf501.top

[Q78] 当前时间
来源：http://uer.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pln.vehdjk.com

[Q79] 字符串拼接
来源：http://red.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ddp.daria6918.cn

[Q80] 字符串截取
来源：http://hkt.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dcu.bjfxy.top

[Q81] 字符串替换
来源：http://iqd.bjfxy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iug.yonumen.top

[Q82] 字符长度与字节长度
来源：http://faq.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://shp.nanxuanxn.top

[Q83] 大小写转换
来源：http://jeu.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jhv.gogol.net.cn

[Q84] 去除首尾空格
来源：http://dhi.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://vtb.yj202588.top

[Q85] 数值取整
来源：http://eht.jyoumei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ulz.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://uek.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://msp.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://nvf.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wes.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://lus.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://twn.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wtw.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://ust.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xst.52xcode.cn

[Q90] 生成序号列
来源：http://ssa.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nxu.yonumen.top

================================================================================
来源：http://kwo.fktsv.cn

R. Bash 专题
来源：http://etc.shzxlz.cn

================================================================================
来源：http://fwn.bbcook.cn

[R01] shebang 与严格模式
来源：http://apq.quarkkingdee.top

#!/usr/bin/env bash
来源：http://vdt.fzhhl.top

set -euo pipefail
来源：http://fot.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://ohp.ybcxt.top

name="Tom"; echo "$name"
来源：http://yjz.yanxiufei.cn

[R03] 只读变量
来源：http://dsh.fzhhl.top

readonly PI=3.14
来源：http://zzx.zdbjq.cn

[R04] 位置参数
来源：http://gun.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iip.epnwcf.com

[R05] 参数默认值
来源：http://quc.sysykeji.top

name="${1:-default}"
来源：http://ntd.52xcode.cn

[R06] 判断命令是否存在
来源：http://uhm.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uzr.bbcook.cn

[R07] if 判断文件
来源：http://acp.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhd.zhijiandao.cn

[R08] 数值比较
来源：http://eww.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://vpa.zhijiandao.cn

[R09] 字符串比较
来源：http://iow.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hnj.sweek.top

[R10] 正则匹配
来源：http://wfc.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xgo.nwbrower.top

[R11] case 多分支
来源：http://wsm.bbcook.cn

case "$1" in
来源：http://hcx.andypj.xyz

start) echo "启动" ;;
来源：http://fmw.sufxvd.cn

stop)  echo "停止" ;;
来源：http://jpv.yuxming.cn

*)     echo "未知命令" ;;
来源：http://ehl.yanxiufei.cn

esac
来源：http://xyw.shuidangran.top

[R12] for 遍历文件
来源：http://efk.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://ccg.chenjidiqi.icu

[R13] for 计数循环
来源：http://ddj.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://kbv.xylfe.cn

[R14] C 风格 for
来源：http://epl.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tlf.hcnkem.com

[R15] while 逐行读文件
来源：http://dvq.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ckx.kuanghao11.cn

[R16] until 等待条件
来源：http://rir.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yel.vqdsnc.cn

[R17] 数组定义与取值
来源：http://ydf.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cie.ehwqpu.com

[R18] 遍历数组
来源：http://hlz.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fby.svipenyu.cn

[R19] 数组长度
来源：http://ryg.zhiwuduotai.top


<!-- 参考信息 -->