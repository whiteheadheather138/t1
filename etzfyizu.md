代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xym.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xwe.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nix.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wll.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://frt.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dmq.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bli.xuetiantiany.cn

[P04] 求长度
来源：http://ckg.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eax.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyr.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://snr.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yvg.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://syo.pycfn.com

Go:   len(arr);  len(m)
来源：http://ado.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://ypy.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ofa.mhx1999.top

[P05] 判断两个对象内容是否相等
来源：http://juw.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tts.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rct.zdqjudy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lso.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pbo.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mnf.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://szm.cdnleiting.top

Ruby: a == b
来源：http://nza.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://trw.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mrt.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zrm.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://mse.yuxming.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zje.hcnkem.com

TS:   if (x == null) {}
来源：http://cdv.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://jxj.ctjpmb.com

Go:   if x == nil {}
来源：http://vzl.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rfr.yonumen.top

C#:   if (x is null) {}
来源：http://ihu.jyoumei.cn

[P07] 防抖与节流
来源：http://kpb.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uvw.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://hug.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swn.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://att.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vnr.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://asg.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sok.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tzk.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://vpm.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oli.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yik.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fsj.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sed.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://grj.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xak.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kjr.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yyl.redwolf501.top

================================================================================
来源：http://cfb.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fez.hywenlv.cn

================================================================================
来源：http://lyu.gotoacloud.top

[Q01] 创建表
来源：http://vlp.nanxuanxn.top

CREATE TABLE users (
来源：http://dhr.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vgk.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://mnf.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://jra.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aqn.wangshuangyany.cn

);
来源：http://jfg.yfazqb.com

[Q02] 创建带外键的表
来源：http://hnp.cheryme.top

CREATE TABLE orders (
来源：http://xxj.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mfl.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://rpz.iojbl.cn

amount DECIMAL(10, 2),
来源：http://qob.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kvz.mhx1999.top

);
来源：http://boi.fehbvm.com

[Q03] 增加列
来源：http://ueq.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hau.jqgfzy.top

[Q04] 修改列类型
来源：http://qtt.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nkj.fengsongda.top

[Q05] 重命名列
来源：http://vci.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nxh.hysaishi.cn

[Q06] 删除列
来源：http://kwa.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://znb.zdbjq.cn

[Q07] 删除表
来源：http://wqb.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://vuu.nwbrower.top

[Q08] 创建普通索引
来源：http://wxr.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fdh.andypj.xyz

[Q09] 创建唯一索引
来源：http://cer.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nuh.xziqi.cn

[Q10] 插入单行
来源：http://anq.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uoq.yj20258888.top

[Q11] 一次插入多行
来源：http://eya.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ecp.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://jjq.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://igs.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://enl.wangdashe.top

[Q13] 忽略重复插入
来源：http://ogc.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pyg.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://rwe.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vgm.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ftn.andypj.xyz

[Q15] 查询全部
来源：http://ulh.9152youxi.cn

SELECT * FROM users;
来源：http://ghq.pengpengdd.cyou

[Q16] 查询指定列
来源：http://tlz.kuanghao11.cn

SELECT id, name FROM users;
来源：http://kjt.chenlongwang.top

[Q17] 条件查询
来源：http://ipc.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tom.52xcode.cn

[Q18] 模糊匹配
来源：http://svm.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ixa.nwbrower.top

[Q19] 范围查询
来源：http://mfk.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gik.yueranfly.top

[Q20] IN 列表
来源：http://hlj.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iai.guannengcc.top

[Q21] 空值判断
来源：http://dfy.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qsi.cheryme.top

[Q22] 排序
来源：http://dvl.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ztd.ctjpmb.com

[Q23] 分页
来源：http://cwu.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zzp.hongshengwenyu.top

[Q24] 去重
来源：http://rxt.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://fbh.hesvh.cn

[Q25] 只取前 N 条
来源：http://usp.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yan.chenlongwang.top

[Q26] 计数
来源：http://wdi.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://muf.yuxming.cn

[Q27] 条件计数
来源：http://dyb.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ekw.havefunace.top

[Q28] 求和与平均
来源：http://zqd.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ark.yonumen.top

[Q29] 最大最小值
来源：http://vgx.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dch.yj202588.top

[Q30] 分组统计
来源：http://dwy.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://frw.guowangkeji.top

[Q31] 分组后过滤
来源：http://krt.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://scr.havefunace.top

[Q32] 分组拼接字符串
来源：http://jgh.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://paj.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://her.ppjwa.cn

[Q33] 多列分组
来源：http://hnj.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qug.hammf.cn

[Q34] 每组取第一条
来源：http://vru.pengpengdd.cyou

SELECT * FROM (
来源：http://xmm.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uct.sysykeji.top

) t WHERE rn = 1;
来源：http://exf.haohaochexian.top

[Q35] 内连接
来源：http://kqz.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://doo.tarul.cn

[Q36] 左连接
来源：http://bjz.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oka.cucudq.cn

[Q37] 右连接
来源：http://wwu.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ptq.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://amb.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xtz.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://www.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://yus.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://piv.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pii.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qjs.fengsongda.top

[Q41] 多表连接
来源：http://bqk.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uan.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://xfg.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://rpj.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://dac.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://nei.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qgl.bbcook.cn

[Q43] 标量子查询
来源：http://pwa.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jwj.jyoumei.cn

[Q44] IN 子查询
来源：http://vqu.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://urt.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://ymo.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yql.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://acy.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aek.ydjk.org.cn

[Q47] 与平均值比较
来源：http://tao.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hbh.yj202588.top

[Q48] CTE 公用表表达式
来源：http://dei.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qyz.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://ldw.hnxiangtu.top

[Q49] 更新单行
来源：http://jxu.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ydk.yvedp.cn

[Q50] 批量更新
来源：http://fge.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ttz.9152youxi.cn

[Q51] 用子查询更新
来源：http://ipf.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fon.zdqjudy.top

[Q52] 删除指定行
来源：http://ghk.tian-w.cn

DELETE FROM users WHERE id = 10;
来源：http://npq.sjlbkw.cn

[Q53] 按条件删除
来源：http://wtk.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lfk.fanxiaobao.xyz

[Q54] 清空表
来源：http://mbu.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://abj.vehdjk.com

[Q55] 排名（并列占位）
来源：http://qhr.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jje.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://chb.yfazqb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lgg.0kj1m.cn

[Q57] 行号
来源：http://nxg.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvx.havefunace.top

[Q58] 累计求和
来源：http://ipm.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mrz.ydzc1.top

[Q59] 分组内累计
来源：http://jrs.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pcy.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://pxy.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://elg.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://frm.yuxming.cn

[Q61] 移动平均
来源：http://vko.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ftw.zhoulong.xyz

[Q62] 分组占比
来源：http://gvd.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kan.sufxvd.cn

[Q63] 开启事务
来源：http://vyd.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rlr.yvedp.cn

[Q64] 提交事务
来源：http://hcc.chenzaomai.com

COMMIT;
来源：http://xkt.wangdashe.top

[Q65] 回滚事务
来源：http://gjq.zhixingplan.top

ROLLBACK;
来源：http://hcn.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://ohv.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oxl.fzhhl.top

[Q67] 设置隔离级别
来源：http://bgs.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vco.zycfv.cn

[Q68] 保存点
来源：http://vrn.pycfn.com

SAVEPOINT sp1;
来源：http://rur.tianlin.xyz

ROLLBACK TO sp1;
来源：http://jsp.jlsjyb.cn

[Q69] 查看执行计划
来源：http://tmz.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cim.jlsjyb.cn

[Q70] 更新统计信息
来源：http://tjj.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://bly.yonumen.top

[Q71] 查看建表语句
来源：http://tur.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://amo.jinqigufen.top

[Q72] 查看索引
来源：http://scj.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://qwq.meibo888.top

[Q73] 查看表状态
来源：http://lut.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ndb.zhijiandao.cn

[Q74] 强制使用索引
来源：http://kvz.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wly.wangdashe.top

[Q75] 日期格式化
来源：http://rgr.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ezx.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sao.chenjidiqi.icu

[Q76] 按天统计
来源：http://ykr.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iuq.shuidangran.top

[Q77] 时间加减
来源：http://unz.zdbjq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tiz.nanxuanxn.top

[Q78] 当前时间
来源：http://xdh.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oyo.guannengcc.top

[Q79] 字符串拼接
来源：http://fev.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://idt.dianchejie.cn

[Q80] 字符串截取
来源：http://xsl.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ntl.zhoulong.xyz

[Q81] 字符串替换
来源：http://cui.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hvw.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://ofz.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vhp.shuidangran.top

[Q83] 大小写转换
来源：http://hjh.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nfv.snrcjt.cn

[Q84] 去除首尾空格
来源：http://aou.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://pwt.fktsv.cn

[Q85] 数值取整
来源：http://igb.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://icg.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://blc.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://htc.hnqzz.top

[Q87] JSON 字段做条件
来源：http://hcu.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vfz.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://fpj.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xim.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ves.pycfn.com

[Q89] 判断表是否存在
来源：http://mwi.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jij.nwbrower.top

[Q90] 生成序号列
来源：http://gsr.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gvq.hywenlv.cn

================================================================================
来源：http://iur.ywan-chungtsiang.top

R. Bash 专题
来源：http://cjz.ivvv.top

================================================================================
来源：http://lhy.sweek.top

[R01] shebang 与严格模式
来源：http://syz.tarul.cn

#!/usr/bin/env bash
来源：http://sbw.zhijiandao.cn

set -euo pipefail
来源：http://zil.tanke756.top

[R02] 变量赋值与使用
来源：http://hus.dianchejie.cn

name="Tom"; echo "$name"
来源：http://lra.sysykeji.top

[R03] 只读变量
来源：http://tph.cashguo.top

readonly PI=3.14
来源：http://rgy.gzhubu.top

[R04] 位置参数
来源：http://ait.hysaishi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ppy.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://ynj.tianlin.xyz

name="${1:-default}"
来源：http://ibs.jianghu66.top

[R06] 判断命令是否存在
来源：http://vnw.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xel.birdmap.top

[R07] if 判断文件
来源：http://mjn.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rzr.yj20258.top

[R08] 数值比较
来源：http://srs.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wfu.zhiwuduotai.top

[R09] 字符串比较
来源：http://gjf.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ypx.c1oappe.top

[R10] 正则匹配
来源：http://hpg.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ybq.feifeiyinyue.top

[R11] case 多分支
来源：http://igx.hongshengwenyu.top

case "$1" in
来源：http://hrz.zhixingplan.top

start) echo "启动" ;;
来源：http://dtx.shuidangran.top

stop)  echo "停止" ;;
来源：http://tje.yueranfly.top

*)     echo "未知命令" ;;
来源：http://srl.epnwcf.com

esac
来源：http://tia.ctjpmb.com

[R12] for 遍历文件
来源：http://qwo.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://wlb.jqgufenzy.top

[R13] for 计数循环
来源：http://axq.ctjpmb.com

for i in {1..10}; do echo "$i"; done
来源：http://hvc.zdqjudy.top

[R14] C 风格 for
来源：http://tra.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tdc.ydjk.org.cn

[R15] while 逐行读文件
来源：http://qjh.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://drc.yongpay.top

[R16] until 等待条件
来源：http://gvn.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jgk.hnxiangtu.top

[R17] 数组定义与取值
来源：http://ios.jiagoushi.top


<!-- 参考信息 -->