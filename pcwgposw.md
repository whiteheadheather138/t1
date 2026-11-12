代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dxf.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://atn.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nhc.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wex.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qdh.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://btp.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ypq.wangdashe.top

[P04] 求长度
来源：http://mfi.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kiq.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dvz.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pjk.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://val.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://cto.hcnkem.com

Go:   len(arr);  len(m)
来源：http://ghs.tanke756.top

Ruby: x.length;  x.size
来源：http://syy.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vmu.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://vaa.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ddl.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iul.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sgl.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uio.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://syu.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://qhu.jinghuilouyu.cn

Ruby: a == b
来源：http://pip.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hwt.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ocy.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pvq.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://bge.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jux.fktsv.cn

TS:   if (x == null) {}
来源：http://npq.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vhu.cqqwz.cn

Go:   if x == nil {}
来源：http://nxd.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zny.yueranfly.top

C#:   if (x is null) {}
来源：http://yww.hfpthk.cn

[P07] 防抖与节流
来源：http://gue.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lmf.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://jli.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbm.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://key.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uit.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sqo.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dvh.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pgp.bjfxy.top

[P08] 处理浮点精度问题
来源：http://qfl.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pxh.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pxr.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fdu.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eps.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://znt.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iig.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zbl.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oho.fanxiaobao.xyz

================================================================================
来源：http://otg.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gau.yonumen.top

================================================================================
来源：http://tat.yfazqb.com

[Q01] 创建表
来源：http://agf.yonumen.top

CREATE TABLE users (
来源：http://zmz.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mqb.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://ucr.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://mku.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xwz.zhixingplan.top

);
来源：http://htf.ydzc1.top

[Q02] 创建带外键的表
来源：http://sdw.wangshuangyany.cn

CREATE TABLE orders (
来源：http://fvs.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzd.sjlbkw.cn

user_id INT NOT NULL,
来源：http://ead.ydzc1.top

amount DECIMAL(10, 2),
来源：http://xkf.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ccy.yongpay.top

);
来源：http://mzt.fengsongda.top

[Q03] 增加列
来源：http://txl.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bao.guowangkeji.top

[Q04] 修改列类型
来源：http://qji.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pbx.wangdashe.top

[Q05] 重命名列
来源：http://srg.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hak.dashuyun.cn

[Q06] 删除列
来源：http://jtv.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://ugh.52xcode.cn

[Q07] 删除表
来源：http://ghe.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://kca.tian-w.cn

[Q08] 创建普通索引
来源：http://cef.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sjr.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://ybn.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cfa.jianghu66.top

[Q10] 插入单行
来源：http://mdz.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wbf.gzhubu.top

[Q11] 一次插入多行
来源：http://gew.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rbw.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://hht.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://ghw.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bhk.0kj1m.cn

[Q13] 忽略重复插入
来源：http://get.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mic.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://hvp.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yfl.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dtx.andypj.xyz

[Q15] 查询全部
来源：http://vjg.birdmap.top

SELECT * FROM users;
来源：http://lub.hysaishi.cn

[Q16] 查询指定列
来源：http://qbc.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://vwc.haohaochexian.top

[Q17] 条件查询
来源：http://wky.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wrv.redwolf501.top

[Q18] 模糊匹配
来源：http://bsw.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xpp.meibo888.top

[Q19] 范围查询
来源：http://mgn.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bzd.wangdashe.top

[Q20] IN 列表
来源：http://kww.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hsg.52xcode.cn

[Q21] 空值判断
来源：http://loc.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cqk.jinyuanbaomall.cn

[Q22] 排序
来源：http://tkx.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dhp.zhengqikj.top

[Q23] 分页
来源：http://yrn.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dny.bbcook.cn

[Q24] 去重
来源：http://dtk.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://qpk.hfpthk.cn

[Q25] 只取前 N 条
来源：http://bdb.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zhl.wangshuangyany.cn

[Q26] 计数
来源：http://ubw.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://cxj.xuetiantiany.cn

[Q27] 条件计数
来源：http://cza.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://awf.guowangkeji.top

[Q28] 求和与平均
来源：http://ysr.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dxi.mhx1999.top

[Q29] 最大最小值
来源：http://nst.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://moi.bjfxy.top

[Q30] 分组统计
来源：http://mak.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iww.jinqigufen.top

[Q31] 分组后过滤
来源：http://kfj.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jww.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://kdz.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dpp.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pyb.fktsv.cn

[Q33] 多列分组
来源：http://cje.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nzi.bbcook.cn

[Q34] 每组取第一条
来源：http://ibp.wangdashe.top

SELECT * FROM (
来源：http://pqy.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wbj.hnxiangtu.top

) t WHERE rn = 1;
来源：http://pjm.c1oappe.top

[Q35] 内连接
来源：http://shs.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jix.gotoacloud.top

[Q36] 左连接
来源：http://rpv.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nad.redwolf501.top

[Q37] 右连接
来源：http://ycy.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kka.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://rxb.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://flw.gaohongyu789.top

[Q39] 自连接（查上下级）
来源：http://nge.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jnw.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ukc.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iyb.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pto.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://grz.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://raa.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://iuk.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://yym.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://nyj.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://nuq.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ewz.guannengcc.top

[Q43] 标量子查询
来源：http://qdx.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xfh.xuetiantiany.cn

[Q44] IN 子查询
来源：http://aaz.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yqi.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://gve.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zva.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://win.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dhd.zhengqikj.top

[Q47] 与平均值比较
来源：http://ana.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ogs.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://ffu.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://naw.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://kpo.jlsjyb.cn

[Q49] 更新单行
来源：http://sjt.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jru.ctjpmb.com

[Q50] 批量更新
来源：http://qgr.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nws.cashguo.top

[Q51] 用子查询更新
来源：http://hqb.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ovo.kuanghao11.cn

[Q52] 删除指定行
来源：http://tju.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://ign.daxiang520.top

[Q53] 按条件删除
来源：http://ztu.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mnu.iojbl.cn

[Q54] 清空表
来源：http://iln.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://fhp.xziqi.cn

[Q55] 排名（并列占位）
来源：http://zus.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pcl.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://pnr.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jcc.zdbjq.cn

[Q57] 行号
来源：http://nma.xylfe.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://flx.daxiang520.top

[Q58] 累计求和
来源：http://ill.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ccw.chenjidiqi.icu

[Q59] 分组内累计
来源：http://qcp.cucudq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pnw.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://aig.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jpy.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ldv.yj20258888.top

[Q61] 移动平均
来源：http://jpz.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xht.hesvh.cn

[Q62] 分组占比
来源：http://kek.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qsu.fehbvm.com

[Q63] 开启事务
来源：http://qzu.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uah.pengpengdd.cyou

[Q64] 提交事务
来源：http://cpa.fengsongda.top

COMMIT;
来源：http://thu.0kj1m.cn

[Q65] 回滚事务
来源：http://xva.jqgfzy.top

ROLLBACK;
来源：http://wws.fzhhl.top

[Q66] 行锁查询
来源：http://azo.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nii.aibaodan.cn

[Q67] 设置隔离级别
来源：http://asl.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vrk.bjfxy.top

[Q68] 保存点
来源：http://yvp.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://ocb.fengsongda.top

ROLLBACK TO sp1;
来源：http://vqo.xuanzx.com

[Q69] 查看执行计划
来源：http://loj.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fgb.tanke756.top

[Q70] 更新统计信息
来源：http://hni.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://wyt.sjlbkw.cn

[Q71] 查看建表语句
来源：http://ryw.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dfr.mhx1999.top

[Q72] 查看索引
来源：http://wmj.redwolf501.top

SHOW INDEX FROM users;
来源：http://urw.xuetiantiany.cn

[Q73] 查看表状态
来源：http://tii.ehwqpu.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ryy.quarkkingdee.top

[Q74] 强制使用索引
来源：http://cll.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hlj.cheryme.top

[Q75] 日期格式化
来源：http://tuo.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jry.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uwy.epnwcf.com

[Q76] 按天统计
来源：http://zzo.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tyo.chenjidiqi.icu

[Q77] 时间加减
来源：http://oep.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://igh.fktsv.cn

[Q78] 当前时间
来源：http://skc.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rgl.cashguo.top

[Q79] 字符串拼接
来源：http://tzj.gzhubu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://toy.dianchejie.cn

[Q80] 字符串截取
来源：http://fou.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ijr.mhx1999.top

[Q81] 字符串替换
来源：http://bof.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nwc.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://smk.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vpq.yonumen.top

[Q83] 大小写转换
来源：http://etu.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://asj.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://ptk.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://nft.bbcook.cn

[Q85] 数值取整
来源：http://pel.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uvz.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://pri.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://odb.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://scb.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qwj.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://met.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jxu.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mlq.nanxinkj.top

[Q89] 判断表是否存在
来源：http://pdj.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hps.birdmap.top

[Q90] 生成序号列
来源：http://ubm.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jlk.dashuyun.cn

================================================================================
来源：http://lwl.yvedp.cn

R. Bash 专题
来源：http://kja.jinyuanbaomall.cn

================================================================================
来源：http://thr.zycfv.cn

[R01] shebang 与严格模式
来源：http://zsb.ehwqpu.com

#!/usr/bin/env bash
来源：http://dzv.zhiwuduotai.top

set -euo pipefail
来源：http://nsd.jyoumei.cn

[R02] 变量赋值与使用
来源：http://sww.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://nsu.hfpthk.cn

[R03] 只读变量
来源：http://ovb.hfpthk.cn

readonly PI=3.14
来源：http://eqx.vqdsnc.cn

[R04] 位置参数
来源：http://soq.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oil.yj20258.top

[R05] 参数默认值
来源：http://pku.jinqigufen.top

name="${1:-default}"
来源：http://ant.yueranfly.top

[R06] 判断命令是否存在
来源：http://kng.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blw.c1oappe.top

[R07] if 判断文件
来源：http://dij.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hfv.zhengqikj.top

[R08] 数值比较
来源：http://orr.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://doo.zhixingplan.top

[R09] 字符串比较
来源：http://qaz.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bbq.snrcjt.cn

[R10] 正则匹配
来源：http://pdp.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eph.xylfe.cn

[R11] case 多分支
来源：http://dam.yangfankeji.com

case "$1" in
来源：http://mkl.meibo888.top

start) echo "启动" ;;
来源：http://rzx.gogol.net.cn

stop)  echo "停止" ;;
来源：http://xpl.daria6918.cn

*)     echo "未知命令" ;;
来源：http://sof.shanyushiyangkeji.top

esac
来源：http://wwn.nanxuanxn.top

[R12] for 遍历文件
来源：http://byp.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://vxd.bjfxy.top

[R13] for 计数循环
来源：http://nsi.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://lyu.316326.xyz

[R14] C 风格 for
来源：http://qba.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hgq.meibo888.top

[R15] while 逐行读文件
来源：http://het.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://azu.zhongyouzk.top

[R16] until 等待条件
来源：http://bnb.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rag.ybcxt.top

[R17] 数组定义与取值
来源：http://rjr.yj20258.top


<!-- 参考信息 -->