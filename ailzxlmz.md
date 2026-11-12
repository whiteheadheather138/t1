代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iva.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jwp.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pjz.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://arn.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xyp.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sea.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zkn.ybcxt.top

[P04] 求长度
来源：http://dla.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgw.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wfr.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kte.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://waq.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://jiy.fengsongda.top

Go:   len(arr);  len(m)
来源：http://brm.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://wmd.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nvn.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://edb.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qzf.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jhr.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://btu.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yvq.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fnt.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://ktt.yj202588.top

Ruby: a == b
来源：http://hxp.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dxa.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ynn.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fzx.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://stq.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cji.yongpay.top

TS:   if (x == null) {}
来源：http://smm.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dss.tian-w.cn

Go:   if x == nil {}
来源：http://xfg.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ymr.jqgufenzy.top

C#:   if (x is null) {}
来源：http://nzy.mhx1999.top

[P07] 防抖与节流
来源：http://idj.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kqh.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://vms.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zyx.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rse.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kwr.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://poe.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://djj.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://djj.ybcxt.top

[P08] 处理浮点精度问题
来源：http://lpi.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qhp.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pmx.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hjt.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jjm.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fzg.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ysh.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://poo.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qur.cheryme.top

================================================================================
来源：http://rlk.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lvj.iojbl.cn

================================================================================
来源：http://aes.kuanghao11.cn

[Q01] 创建表
来源：http://hzi.epnwcf.com

CREATE TABLE users (
来源：http://hwb.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xhb.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://ogc.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://pdo.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lsx.shuidangran.top

);
来源：http://bvy.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://exm.zdqjudy.top

CREATE TABLE orders (
来源：http://vas.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://peq.birdmap.top

user_id INT NOT NULL,
来源：http://ppw.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://qzh.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yfz.xylfe.cn

);
来源：http://qqb.yvedp.cn

[Q03] 增加列
来源：http://cyx.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xbr.zdqjudy.top

[Q04] 修改列类型
来源：http://ehf.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iim.yueranfly.top

[Q05] 重命名列
来源：http://xsx.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://alp.nanxuanxn.top

[Q06] 删除列
来源：http://awh.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://lws.jyoumei.cn

[Q07] 删除表
来源：http://kvi.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://dac.yj202588.top

[Q08] 创建普通索引
来源：http://yyr.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uox.yangfankeji.com

[Q09] 创建唯一索引
来源：http://ood.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mie.316326.xyz

[Q10] 插入单行
来源：http://igd.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wrl.zhijiandao.cn

[Q11] 一次插入多行
来源：http://axz.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aqq.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://sri.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://mnf.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pis.jianghu66.top

[Q13] 忽略重复插入
来源：http://gpn.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ewl.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://msn.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ntu.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bmo.fengsongda.top

[Q15] 查询全部
来源：http://dtc.c1oappe.top

SELECT * FROM users;
来源：http://xcg.xuanzx.com

[Q16] 查询指定列
来源：http://lek.ydjk.org.cn

SELECT id, name FROM users;
来源：http://nxo.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://toe.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ilm.kuanghao11.cn

[Q18] 模糊匹配
来源：http://foj.xziqi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jsg.cheryme.top

[Q19] 范围查询
来源：http://sil.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://odv.zycfv.cn

[Q20] IN 列表
来源：http://usl.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cre.haohaochexian.top

[Q21] 空值判断
来源：http://djo.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://amr.hesvh.cn

[Q22] 排序
来源：http://lvd.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://frm.jinyuanbaomall.cn

[Q23] 分页
来源：http://cpe.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cvw.snrcjt.cn

[Q24] 去重
来源：http://lia.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://ubj.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://vbf.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ncq.pycfn.com

[Q26] 计数
来源：http://oyg.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://dei.hywenlv.cn

[Q27] 条件计数
来源：http://umi.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wpd.hcnkem.com

[Q28] 求和与平均
来源：http://gsb.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xnl.birdmap.top

[Q29] 最大最小值
来源：http://mof.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://iqy.bbcook.cn

[Q30] 分组统计
来源：http://icr.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://voo.birdmap.top

[Q31] 分组后过滤
来源：http://nna.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dwi.xuanzx.com

[Q32] 分组拼接字符串
来源：http://wtq.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://stt.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zim.chenlongwang.top

[Q33] 多列分组
来源：http://bbi.gzhubu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nol.vqdsnc.cn

[Q34] 每组取第一条
来源：http://hoe.yueranfly.top

SELECT * FROM (
来源：http://pwl.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yhb.yj20258.top

) t WHERE rn = 1;
来源：http://syq.ybcxt.top

[Q35] 内连接
来源：http://pww.bbcook.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pms.vqdsnc.cn

[Q36] 左连接
来源：http://kmj.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://une.svipenyu.cn

[Q37] 右连接
来源：http://uxd.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zoa.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://mfi.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sab.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://xgh.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://neg.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mau.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ybd.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jsa.sweek.top

[Q41] 多表连接
来源：http://pll.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://crg.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://yai.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://zgf.cashguo.top

[Q42] 连接条件附加过滤
来源：http://noh.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://nee.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cga.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://iul.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kij.zhengqikj.top

[Q44] IN 子查询
来源：http://zqt.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lfa.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://xig.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lka.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ira.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gtt.aizwys.cn

[Q47] 与平均值比较
来源：http://wuh.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rhc.316326.xyz

[Q48] CTE 公用表表达式
来源：http://htc.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://alb.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://ick.zhixingplan.top

[Q49] 更新单行
来源：http://vug.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bow.hnxiangtu.top

[Q50] 批量更新
来源：http://pjb.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eyj.yonumen.top

[Q51] 用子查询更新
来源：http://idf.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rzy.cdnleiting.top

[Q52] 删除指定行
来源：http://xae.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://wsy.yuanzhike.top

[Q53] 按条件删除
来源：http://jeq.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gkl.xingfuxueyuan.xyz

[Q54] 清空表
来源：http://ivd.fehbvm.com

TRUNCATE TABLE logs;
来源：http://dnd.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://ywf.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tly.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://nab.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rqk.yuxming.cn

[Q57] 行号
来源：http://nrb.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oyw.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://xhu.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mav.andypj.xyz

[Q59] 分组内累计
来源：http://uwy.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rcj.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://oeq.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qzb.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iqp.zycfv.cn

[Q61] 移动平均
来源：http://xya.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bjg.yongpay.top

[Q62] 分组占比
来源：http://cte.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nmw.quarkkingdee.top

[Q63] 开启事务
来源：http://drg.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dey.birdmap.top

[Q64] 提交事务
来源：http://mrs.xuanzx.com

COMMIT;
来源：http://hcn.guowangkeji.top

[Q65] 回滚事务
来源：http://dwh.andypj.xyz

ROLLBACK;
来源：http://svi.bjfxy.top

[Q66] 行锁查询
来源：http://bda.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zng.iojbl.cn

[Q67] 设置隔离级别
来源：http://uuo.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jqo.jinyuanbaomall.cn

[Q68] 保存点
来源：http://bsi.hcnkem.com

SAVEPOINT sp1;
来源：http://mvt.yj20258.top

ROLLBACK TO sp1;
来源：http://sao.chenlongwang.top

[Q69] 查看执行计划
来源：http://yry.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qvx.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://qyc.epnwcf.com

ANALYZE TABLE users;
来源：http://iqx.hnqzz.top

[Q71] 查看建表语句
来源：http://dwq.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qgb.jianghu66.top

[Q72] 查看索引
来源：http://zwt.ivvv.top

SHOW INDEX FROM users;
来源：http://ita.zycfv.cn

[Q73] 查看表状态
来源：http://bly.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mfq.pycfn.com

[Q74] 强制使用索引
来源：http://cjf.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wnv.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://jrn.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rlu.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ucq.birdmap.top

[Q76] 按天统计
来源：http://fir.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eyj.shanyushiyangtech.top

[Q77] 时间加减
来源：http://imo.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://siw.vqdsnc.cn

[Q78] 当前时间
来源：http://qax.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://avw.0kj1m.cn

[Q79] 字符串拼接
来源：http://fcq.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kqv.yj20258888.top

[Q80] 字符串截取
来源：http://ynb.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lfv.jqgfzy.top

[Q81] 字符串替换
来源：http://tcf.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pqb.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://qiy.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://slo.jlsjyb.cn

[Q83] 大小写转换
来源：http://xxa.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hfr.cashguo.top

[Q84] 去除首尾空格
来源：http://wum.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://ntj.cqqwz.cn

[Q85] 数值取整
来源：http://soq.yanxiufei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hey.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://seu.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xcg.shuidangran.top

[Q87] JSON 字段做条件
来源：http://mog.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fwd.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://awq.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oge.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kku.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://clq.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ols.hesvh.cn

[Q90] 生成序号列
来源：http://ooe.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vke.zhongyouzk.top

================================================================================
来源：http://xyx.jianghu66.top

R. Bash 专题
来源：http://ntl.feifeiyinyue.top

================================================================================
来源：http://wow.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://jso.9152youxi.cn

#!/usr/bin/env bash
来源：http://ald.hnxiangtu.top

set -euo pipefail
来源：http://gma.meibo888.top

[R02] 变量赋值与使用
来源：http://nup.jiagoushi.top

name="Tom"; echo "$name"
来源：http://ppd.jianghu66.top

[R03] 只读变量
来源：http://yrl.shzxlz.cn

readonly PI=3.14
来源：http://vce.fehbvm.com

[R04] 位置参数
来源：http://wtz.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ueo.hammf.cn

[R05] 参数默认值
来源：http://nnt.yj202588.top

name="${1:-default}"
来源：http://vpl.daxiang520.top

[R06] 判断命令是否存在
来源：http://oyy.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://emz.cdnleiting.top

[R07] if 判断文件
来源：http://zpe.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nye.nanxuanxn.top

[R08] 数值比较
来源：http://bzy.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qat.ehwqpu.com

[R09] 字符串比较
来源：http://zku.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tdr.316326.xyz

[R10] 正则匹配
来源：http://ojg.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yzi.cdnleiting.top

[R11] case 多分支
来源：http://mtu.xuanzx.com

case "$1" in
来源：http://rew.daxiang520.top

start) echo "启动" ;;
来源：http://uuu.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://nrz.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://uff.daria6918.cn

esac
来源：http://qlu.bbcook.cn

[R12] for 遍历文件
来源：http://ekj.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://krv.zhijiandao.cn

[R13] for 计数循环
来源：http://ihn.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://upf.fehbvm.com

[R14] C 风格 for
来源：http://ynh.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tfy.jiagoushi.top

[R15] while 逐行读文件
来源：http://lha.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jqj.yuxming.cn

[R16] until 等待条件
来源：http://xrj.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://asb.yuxming.cn

[R17] 数组定义与取值
来源：http://nbz.xuanzx.com


<!-- 参考信息 -->