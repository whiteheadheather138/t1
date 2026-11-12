代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xzy.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kiu.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vqe.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hho.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vlg.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xwq.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://apn.xinyue.icu

[P04] 求长度
来源：http://cnq.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bly.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zlq.zhongyouzk.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://koo.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xoi.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://vtc.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://ukx.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://nbt.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://lek.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://xtm.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nuf.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://emi.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dpk.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://veh.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dzt.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lie.sufxvd.cn

Ruby: a == b
来源：http://rxs.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggt.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vrl.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nkx.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://vzu.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qdl.mhx1999.top

TS:   if (x == null) {}
来源：http://tin.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://foh.yonumen.top

Go:   if x == nil {}
来源：http://azk.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tpk.gaohongyu789.top

C#:   if (x is null) {}
来源：http://cyd.chenlongwang.top

[P07] 防抖与节流
来源：http://psr.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ghl.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://cbq.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irl.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvs.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sjk.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jkt.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zpo.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://saw.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://jip.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ocd.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lwm.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ucf.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://edd.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tky.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uui.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jky.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vtr.ivvv.top

================================================================================
来源：http://ici.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dgn.svipenyu.cn

================================================================================
来源：http://wtk.wangshuangyany.cn

[Q01] 创建表
来源：http://sge.ydjk.org.cn

CREATE TABLE users (
来源：http://eif.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://afl.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://meq.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://gjc.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sjd.gotoacloud.top

);
来源：http://gou.daxiang520.top

[Q02] 创建带外键的表
来源：http://zpn.xuanzx.com

CREATE TABLE orders (
来源：http://bbl.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yxy.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://vkh.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://tne.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kwu.shanyushiyangtech.top

);
来源：http://mkq.zhongyouzk.top

[Q03] 增加列
来源：http://ntj.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sdl.uphjek.com

[Q04] 修改列类型
来源：http://dpd.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://duw.havefunace.top

[Q05] 重命名列
来源：http://mlw.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rqe.jinyuanbaomall.cn

[Q06] 删除列
来源：http://uwy.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://ibj.zhengqikj.top

[Q07] 删除表
来源：http://hft.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://tct.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://fiw.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cnn.bbcook.cn

[Q09] 创建唯一索引
来源：http://wrw.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gxy.epnwcf.com

[Q10] 插入单行
来源：http://pfi.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ueb.cdnleiting.top

[Q11] 一次插入多行
来源：http://hoq.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qbq.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://dln.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jcs.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wju.chenlongwang.top

[Q13] 忽略重复插入
来源：http://vic.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rkt.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://vlf.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pbb.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ypr.hywenlv.cn

[Q15] 查询全部
来源：http://uhg.jyoumei.cn

SELECT * FROM users;
来源：http://eea.hywenlv.cn

[Q16] 查询指定列
来源：http://uwe.nwbrower.top

SELECT id, name FROM users;
来源：http://cbj.chenjidiqi.icu

[Q17] 条件查询
来源：http://wzo.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oto.dashuyun.cn

[Q18] 模糊匹配
来源：http://afv.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iuc.pengpengdd.cyou

[Q19] 范围查询
来源：http://amx.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://som.xinyue.icu

[Q20] IN 列表
来源：http://jdp.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kjg.tarul.cn

[Q21] 空值判断
来源：http://nvo.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wxn.jlsjyb.cn

[Q22] 排序
来源：http://qmz.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bcx.gotoacloud.top

[Q23] 分页
来源：http://ocp.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vyj.snrcjt.cn

[Q24] 去重
来源：http://vqn.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://rxz.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://dgj.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jmm.guannengcc.top

[Q26] 计数
来源：http://qge.sweek.top

SELECT COUNT(*) FROM users;
来源：http://xbk.fktsv.cn

[Q27] 条件计数
来源：http://kng.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kxb.vehdjk.com

[Q28] 求和与平均
来源：http://dfd.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hou.hcnkem.com

[Q29] 最大最小值
来源：http://rsx.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rhx.chenjidiqi.icu

[Q30] 分组统计
来源：http://tyv.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://inj.gaohongyu789.top

[Q31] 分组后过滤
来源：http://abu.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bts.smart0.xyz

[Q32] 分组拼接字符串
来源：http://hfb.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bxr.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pqe.guowangkeji.top

[Q33] 多列分组
来源：http://wkt.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://buh.fengsongda.top

[Q34] 每组取第一条
来源：http://kge.birdmap.top

SELECT * FROM (
来源：http://zex.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://edo.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://txe.havefunace.top

[Q35] 内连接
来源：http://efm.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fio.zdqjudy.top

[Q36] 左连接
来源：http://rxg.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tjy.zdqjudy.top

[Q37] 右连接
来源：http://als.ydjk.org.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iwe.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://hih.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uxl.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://uxn.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://tpw.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qqr.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eul.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lou.pycfn.com

[Q41] 多表连接
来源：http://tmk.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://xty.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://plv.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://xca.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://swp.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://icq.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://obl.redwolf501.top

[Q43] 标量子查询
来源：http://gbb.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nwj.ydzc1.top

[Q44] IN 子查询
来源：http://iei.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://viz.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://jax.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nnr.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://dwj.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fiz.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://hxm.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dzp.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://kym.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jzr.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://xcu.yj202588.top

[Q49] 更新单行
来源：http://ssi.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hjx.sweek.top

[Q50] 批量更新
来源：http://nln.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://skz.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://hzd.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bvy.havefunace.top

[Q52] 删除指定行
来源：http://ugj.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://jeb.jyoumei.cn

[Q53] 按条件删除
来源：http://fgz.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kjv.jinyuanbaomall.cn

[Q54] 清空表
来源：http://ixw.ivvv.top

TRUNCATE TABLE logs;
来源：http://ynn.bjfxy.top

[Q55] 排名（并列占位）
来源：http://zfn.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://npu.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://yfv.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ojy.zhiwuduotai.top

[Q57] 行号
来源：http://saa.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fhf.ppjwa.cn

[Q58] 累计求和
来源：http://tzr.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ask.yonumen.top

[Q59] 分组内累计
来源：http://tbn.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wfa.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://sqx.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lko.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bkf.fanxiaobao.xyz

[Q61] 移动平均
来源：http://dfh.ppjwa.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ysi.pycfn.com

[Q62] 分组占比
来源：http://ssn.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hwz.fengsongda.top

[Q63] 开启事务
来源：http://erk.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rlk.iojbl.cn

[Q64] 提交事务
来源：http://gpm.chenlongwang.top

COMMIT;
来源：http://hox.yj20258.top

[Q65] 回滚事务
来源：http://ylf.fehbvm.com

ROLLBACK;
来源：http://rly.pengpengdd.cyou

[Q66] 行锁查询
来源：http://vak.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dks.zycfv.cn

[Q67] 设置隔离级别
来源：http://ofh.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jrl.316326.xyz

[Q68] 保存点
来源：http://gin.zhoulong.xyz

SAVEPOINT sp1;
来源：http://htt.shanyushiyangtech.top

ROLLBACK TO sp1;
来源：http://flr.aizwys.cn

[Q69] 查看执行计划
来源：http://omg.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gff.wangdashe.top

[Q70] 更新统计信息
来源：http://lar.jqgfzy.top

ANALYZE TABLE users;
来源：http://vva.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://dop.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wmi.hnxiangtu.top

[Q72] 查看索引
来源：http://cub.9152youxi.cn

SHOW INDEX FROM users;
来源：http://ffm.sweek.top

[Q73] 查看表状态
来源：http://xrj.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fap.bbcook.cn

[Q74] 强制使用索引
来源：http://eoh.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tnv.ybcxt.top

[Q75] 日期格式化
来源：http://gqf.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rbs.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uqw.gaohongyu789.top

[Q76] 按天统计
来源：http://dux.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fan.shuidangran.top

[Q77] 时间加减
来源：http://oao.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyu.dashuyun.cn

[Q78] 当前时间
来源：http://vaa.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fzc.jqgfzy.top

[Q79] 字符串拼接
来源：http://vis.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wms.yj20258888.top

[Q80] 字符串截取
来源：http://ikw.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ulm.yvedp.cn

[Q81] 字符串替换
来源：http://dee.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sjk.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://aav.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uyz.zhixingplan.top

[Q83] 大小写转换
来源：http://bty.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hxf.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://pke.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://kpz.ybcxt.top

[Q85] 数值取整
来源：http://uzu.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tfe.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://zlr.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iao.fzhhl.top

[Q87] JSON 字段做条件
来源：http://jsa.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qkh.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://xmc.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qqe.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jbw.c1oappe.top

[Q89] 判断表是否存在
来源：http://pok.sjlbkw.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://otd.cucudq.cn

[Q90] 生成序号列
来源：http://shy.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zly.jyoumei.cn

================================================================================
来源：http://bpn.zhengqikj.top

R. Bash 专题
来源：http://kkt.tarul.cn

================================================================================
来源：http://bkb.zhengqikj.top

[R01] shebang 与严格模式
来源：http://pvd.daria6918.cn

#!/usr/bin/env bash
来源：http://kmb.yuanzhike.top

set -euo pipefail
来源：http://hcr.bjfxy.top

[R02] 变量赋值与使用
来源：http://prq.ydzc1.top

name="Tom"; echo "$name"
来源：http://gzg.chenjidiqi.icu

[R03] 只读变量
来源：http://ytk.svipenyu.cn

readonly PI=3.14
来源：http://azx.jiagoushi.top

[R04] 位置参数
来源：http://pjn.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://olj.tianlin.xyz

[R05] 参数默认值
来源：http://kvu.ybcxt.top

name="${1:-default}"
来源：http://pke.shanyushiyangtech.top

[R06] 判断命令是否存在
来源：http://qdo.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://atz.ybcxt.top

[R07] if 判断文件
来源：http://dlo.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yvh.fehbvm.com

[R08] 数值比较
来源：http://nfi.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ons.mhx1999.top

[R09] 字符串比较
来源：http://dzz.daria6918.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://edj.quarkkingdee.top

[R10] 正则匹配
来源：http://ddq.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pjm.mhx1999.top

[R11] case 多分支
来源：http://xek.xylfe.cn

case "$1" in
来源：http://jxe.jqgufenzy.top

start) echo "启动" ;;
来源：http://gcb.xylfe.cn

stop)  echo "停止" ;;
来源：http://zgy.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://oon.yanxiufei.cn

esac
来源：http://tfo.yuanzhike.top

[R12] for 遍历文件
来源：http://pbn.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://cyi.hnxiangtu.top

[R13] for 计数循环
来源：http://qzr.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://zxy.gzhubu.top

[R14] C 风格 for
来源：http://sga.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://clq.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://ryq.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://adm.ydjk.org.cn

[R16] until 等待条件
来源：http://lig.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uys.yangfankeji.com

[R17] 数组定义与取值
来源：http://gbb.aizwys.cn


<!-- 参考信息 -->