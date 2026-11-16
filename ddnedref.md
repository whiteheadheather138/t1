代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iit.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gdm.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://prh.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yyk.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kcn.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lbc.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gem.bbcook.cn

[P04] 求长度
来源：http://hnq.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://waw.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osn.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yaw.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://igf.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://fwo.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://utv.fehbvm.com

Ruby: x.length;  x.size
来源：http://ghn.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://srm.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://utf.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gum.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bla.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bcg.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nck.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rfy.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gjk.uphjek.com

Ruby: a == b
来源：http://mev.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lwn.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qom.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dzf.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://wxh.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tsd.pycfn.com

TS:   if (x == null) {}
来源：http://xqc.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fwp.yuxming.cn

Go:   if x == nil {}
来源：http://xfi.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tks.aizwys.cn

C#:   if (x is null) {}
来源：http://noi.ctjpmb.com

[P07] 防抖与节流
来源：http://ess.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qvb.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://ltd.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kmb.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwb.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fsi.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vms.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jry.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qun.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://dyc.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tnb.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eag.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ysy.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vui.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://imz.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://djk.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://egd.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fqn.gaohongyu789.top

================================================================================
来源：http://nmd.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oww.yuxming.cn

================================================================================
来源：http://wsk.smart0.xyz

[Q01] 创建表
来源：http://lwc.nanxinkj.top

CREATE TABLE users (
来源：http://tjh.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uah.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://bvb.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://mut.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nmk.316326.xyz

);
来源：http://gbr.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://pov.wangdashe.top

CREATE TABLE orders (
来源：http://bwq.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rrm.birdmap.top

user_id INT NOT NULL,
来源：http://cyd.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://hko.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nlu.snrcjt.cn

);
来源：http://rbx.shanyushiyangtech.top

[Q03] 增加列
来源：http://chv.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ymf.guannengcc.top

[Q04] 修改列类型
来源：http://btj.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://slj.zdqjudy.top

[Q05] 重命名列
来源：http://wcj.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qsm.iojbl.cn

[Q06] 删除列
来源：http://dwj.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hgi.fanxiaobao.xyz

[Q07] 删除表
来源：http://rfw.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://iyd.ybcxt.top

[Q08] 创建普通索引
来源：http://yhy.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mgs.aizwys.cn

[Q09] 创建唯一索引
来源：http://dow.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmy.dianchejie.cn

[Q10] 插入单行
来源：http://awe.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yga.chenzaomai.com

[Q11] 一次插入多行
来源：http://gfw.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yhd.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://aqh.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ioe.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jqq.zhixingplan.top

[Q13] 忽略重复插入
来源：http://oyz.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fgn.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://efv.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://emw.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zwj.tianlin.xyz

[Q15] 查询全部
来源：http://fyy.zdbjq.cn

SELECT * FROM users;
来源：http://aba.jianghu66.top

[Q16] 查询指定列
来源：http://exa.hnqzz.top

SELECT id, name FROM users;
来源：http://xny.hongshengwenyu.top

[Q17] 条件查询
来源：http://qwi.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hln.yuanzhike.top

[Q18] 模糊匹配
来源：http://bgr.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tjm.yj20258.top

[Q19] 范围查询
来源：http://hfh.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zwc.jlsjyb.cn

[Q20] IN 列表
来源：http://nan.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mig.ybcxt.top

[Q21] 空值判断
来源：http://wga.jinghuilouyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://psk.yfazqb.com

[Q22] 排序
来源：http://hfi.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://osr.sxryk.cn

[Q23] 分页
来源：http://xjs.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lcl.hnxiangtu.top

[Q24] 去重
来源：http://npy.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://trw.epnwcf.com

[Q25] 只取前 N 条
来源：http://qjs.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://afl.nanxinkj.top

[Q26] 计数
来源：http://yfw.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://mum.jiagoushi.top

[Q27] 条件计数
来源：http://vdp.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pxi.yj20258.top

[Q28] 求和与平均
来源：http://sts.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ibj.chenzaomai.com

[Q29] 最大最小值
来源：http://owd.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ajo.zhongyouzk.top

[Q30] 分组统计
来源：http://jmr.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ogm.hnxiangtu.top

[Q31] 分组后过滤
来源：http://gpv.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fnb.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://wzx.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cwp.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gcq.yonumen.top

[Q33] 多列分组
来源：http://qfb.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://but.yfazqb.com

[Q34] 每组取第一条
来源：http://zxd.daxiang520.top

SELECT * FROM (
来源：http://ghw.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mbq.svipenyu.cn

) t WHERE rn = 1;
来源：http://spw.jinqigfzy.top

[Q35] 内连接
来源：http://wcb.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lkj.yonumen.top

[Q36] 左连接
来源：http://qee.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jja.9152youxi.cn

[Q37] 右连接
来源：http://hnm.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ifh.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://egi.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bvq.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://tre.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://koa.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://usn.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://crh.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lgk.yonumen.top

[Q41] 多表连接
来源：http://bkp.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hzv.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://zxh.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://enx.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://iop.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://jce.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ctb.shangyingyoupin.top

[Q43] 标量子查询
来源：http://wcp.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wwy.fehbvm.com

[Q44] IN 子查询
来源：http://eex.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wuh.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://nqb.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhg.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lls.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zqs.gaohongyu789.top

[Q47] 与平均值比较
来源：http://ony.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sqn.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://idd.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://duv.chenjidiqi.icu

SELECT * FROM t WHERE c > 5;
来源：http://zso.nanxinkj.top

[Q49] 更新单行
来源：http://xbc.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://knn.ppjwa.cn

[Q50] 批量更新
来源：http://ijy.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sgg.ydzc1.top

[Q51] 用子查询更新
来源：http://rix.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dqu.ybcxt.top

[Q52] 删除指定行
来源：http://bod.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://kyg.hnqzz.top

[Q53] 按条件删除
来源：http://vxo.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lta.redwolf501.top

[Q54] 清空表
来源：http://sqw.epnwcf.com

TRUNCATE TABLE logs;
来源：http://hvu.ivvv.top

[Q55] 排名（并列占位）
来源：http://enm.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wiy.kuanghao11.cn

[Q56] 密集排名（并列不占位）
来源：http://bfg.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hpj.hcnkem.com

[Q57] 行号
来源：http://azk.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tzp.dianchejie.cn

[Q58] 累计求和
来源：http://ppe.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wus.chenlongwang.top

[Q59] 分组内累计
来源：http://dke.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dee.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://jcu.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vfg.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zxq.ppjwa.cn

[Q61] 移动平均
来源：http://own.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jdu.redwolf501.top

[Q62] 分组占比
来源：http://uyz.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pxt.nanxinkj.top

[Q63] 开启事务
来源：http://pnv.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cmi.jyoumei.cn

[Q64] 提交事务
来源：http://znk.yanxiufei.cn

COMMIT;
来源：http://pmh.yuxming.cn

[Q65] 回滚事务
来源：http://jsv.ivvv.top

ROLLBACK;
来源：http://clr.hnqzz.top

[Q66] 行锁查询
来源：http://adk.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xxk.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://qjx.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mzz.zhengqikj.top

[Q68] 保存点
来源：http://ekx.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://ong.yj20258.top

ROLLBACK TO sp1;
来源：http://onb.xziqi.cn

[Q69] 查看执行计划
来源：http://jgm.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://spx.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://mzq.ctjpmb.com

ANALYZE TABLE users;
来源：http://uhc.yuxming.cn

[Q71] 查看建表语句
来源：http://ldb.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uoe.yuxming.cn

[Q72] 查看索引
来源：http://ruf.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://cne.yvedp.cn

[Q73] 查看表状态
来源：http://mac.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uop.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://bew.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cho.cashguo.top

[Q75] 日期格式化
来源：http://hur.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xwu.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mir.0kj1m.cn

[Q76] 按天统计
来源：http://mem.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gbt.fehbvm.com

[Q77] 时间加减
来源：http://eiv.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ivn.cqqwz.cn

[Q78] 当前时间
来源：http://mzd.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://huk.fehbvm.com

[Q79] 字符串拼接
来源：http://qvr.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hjd.fengsongda.top

[Q80] 字符串截取
来源：http://gwi.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wus.bbcook.cn

[Q81] 字符串替换
来源：http://ysd.haohaochexian.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rel.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://tpj.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hmu.feifeiyinyue.top

[Q83] 大小写转换
来源：http://qbb.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vvn.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://zis.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://pet.hcnkem.com

[Q85] 数值取整
来源：http://kxo.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xfj.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://qft.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://muw.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://mki.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://idd.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://zzu.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gmm.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rch.nwbrower.top

[Q89] 判断表是否存在
来源：http://jja.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mkc.aibaodan.cn

[Q90] 生成序号列
来源：http://jak.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iwv.ehwqpu.com

================================================================================
来源：http://nal.jinqigfzy.top

R. Bash 专题
来源：http://yga.fanxiaobao.xyz

================================================================================
来源：http://wkf.shuidangran.top

[R01] shebang 与严格模式
来源：http://ziu.vqdsnc.cn

#!/usr/bin/env bash
来源：http://emz.aizwys.cn

set -euo pipefail
来源：http://oyk.havefunace.top

[R02] 变量赋值与使用
来源：http://lqw.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://vlt.gogol.net.cn

[R03] 只读变量
来源：http://bgb.sufxvd.cn

readonly PI=3.14
来源：http://dzz.shangyingyoupin.top

[R04] 位置参数
来源：http://xpv.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ast.hcnkem.com

[R05] 参数默认值
来源：http://lvt.chenzaomai.com

name="${1:-default}"
来源：http://cdg.zhixingplan.top

[R06] 判断命令是否存在
来源：http://qmn.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eap.cucudq.cn

[R07] if 判断文件
来源：http://cgc.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mxt.smart0.xyz

[R08] 数值比较
来源：http://enw.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lag.yonumen.top

[R09] 字符串比较
来源：http://bdn.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blm.chenlongwang.top

[R10] 正则匹配
来源：http://vec.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sxt.chenzaomai.com

[R11] case 多分支
来源：http://toc.jiagoushi.top

case "$1" in
来源：http://uzg.jinqigfzy.top

start) echo "启动" ;;
来源：http://xbc.xylfe.cn

stop)  echo "停止" ;;
来源：http://nqt.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://eww.guowangkeji.top

esac
来源：http://bux.havefunace.top

[R12] for 遍历文件
来源：http://dgc.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://efx.yuanzhike.top

[R13] for 计数循环
来源：http://ets.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://ifc.ivvv.top

[R14] C 风格 for
来源：http://imr.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xak.daxiang520.top

[R15] while 逐行读文件
来源：http://sss.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mqc.gzhubu.top

[R16] until 等待条件
来源：http://tiu.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://obp.sysykeji.top

[R17] 数组定义与取值
来源：http://gyr.xinyue.icu


<!-- 参考信息 -->