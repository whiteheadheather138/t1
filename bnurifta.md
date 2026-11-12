代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ffn.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zob.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzx.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pok.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pvm.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rkg.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qbn.xinyue.icu

[P04] 求长度
来源：http://tjo.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cws.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mpc.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ovc.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nbg.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://rct.hcnkem.com

Go:   len(arr);  len(m)
来源：http://shv.aizwys.cn

Ruby: x.length;  x.size
来源：http://ktk.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zyb.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://kvn.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://asn.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ehr.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cdv.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mah.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hza.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pin.zhongyouzk.top

Ruby: a == b
来源：http://ldk.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vjp.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cdz.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dyn.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://nmh.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tqv.vehdjk.com

TS:   if (x == null) {}
来源：http://jpy.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wkx.sufxvd.cn

Go:   if x == nil {}
来源：http://jht.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fsy.svipenyu.cn

C#:   if (x is null) {}
来源：http://tud.hysaishi.cn

[P07] 防抖与节流
来源：http://uvd.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zvo.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://abo.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxr.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pee.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jxy.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qux.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rjz.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ppu.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://hki.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jlq.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://esq.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://viw.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cny.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zel.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cio.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wql.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zrw.jinqigufen.top

================================================================================
来源：http://yso.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wig.yuxming.cn

================================================================================
来源：http://adt.cucudq.cn

[Q01] 创建表
来源：http://key.fengsongda.top

CREATE TABLE users (
来源：http://zaz.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bic.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://mqz.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://mbu.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uyq.daria6918.cn

);
来源：http://ktm.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://ovg.chenlongwang.top

CREATE TABLE orders (
来源：http://sue.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aet.haohaochexian.top

user_id INT NOT NULL,
来源：http://oqe.wangdashe.top

amount DECIMAL(10, 2),
来源：http://mhv.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cgy.zdbjq.cn

);
来源：http://ccq.guowangkeji.top

[Q03] 增加列
来源：http://kkx.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ajl.hongshengwenyu.top

[Q04] 修改列类型
来源：http://ivb.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dxm.zhongyouzk.top

[Q05] 重命名列
来源：http://psm.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cmf.jyoumei.cn

[Q06] 删除列
来源：http://rbb.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://hav.9152youxi.cn

[Q07] 删除表
来源：http://uwm.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://hkk.sufxvd.cn

[Q08] 创建普通索引
来源：http://lna.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://usa.yongpay.top

[Q09] 创建唯一索引
来源：http://ybu.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jsu.daria6918.cn

[Q10] 插入单行
来源：http://txx.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mrp.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://ftj.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dwh.ivvv.top

[Q12] 插入后取自增 ID
来源：http://vuc.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://yvg.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lfw.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://olw.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ofg.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://dam.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hwz.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://opf.birdmap.top

[Q15] 查询全部
来源：http://jsq.tian-w.cn

SELECT * FROM users;
来源：http://lmh.gotoacloud.top

[Q16] 查询指定列
来源：http://sfg.9152youxi.cn

SELECT id, name FROM users;
来源：http://biu.guowangkeji.top

[Q17] 条件查询
来源：http://gde.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yad.smart0.xyz

[Q18] 模糊匹配
来源：http://dxa.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dnn.sweek.top

[Q19] 范围查询
来源：http://ppd.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zec.vehdjk.com

[Q20] IN 列表
来源：http://jmq.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://viw.daria6918.cn

[Q21] 空值判断
来源：http://xdn.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://znn.daxiang520.top

[Q22] 排序
来源：http://tbz.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xpm.yueranfly.top

[Q23] 分页
来源：http://vyn.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aku.pengpengdd.cyou

[Q24] 去重
来源：http://tbk.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://zzy.ctjpmb.com

[Q25] 只取前 N 条
来源：http://whn.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zte.meibo888.top

[Q26] 计数
来源：http://lxk.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://isp.yj202588.top

[Q27] 条件计数
来源：http://bno.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xel.guowangkeji.top

[Q28] 求和与平均
来源：http://njp.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bkj.sxryk.cn

[Q29] 最大最小值
来源：http://hux.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tmu.fzhhl.top

[Q30] 分组统计
来源：http://dsx.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mbu.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://hyp.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://usz.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://ycp.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rmz.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mjv.fengsongda.top

[Q33] 多列分组
来源：http://zfn.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aon.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://dlf.andypj.xyz

SELECT * FROM (
来源：http://edo.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jqy.aibaodan.cn

) t WHERE rn = 1;
来源：http://fqr.jianghu66.top

[Q35] 内连接
来源：http://xjc.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rqo.cheryme.top

[Q36] 左连接
来源：http://dim.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wmb.sjlbkw.cn

[Q37] 右连接
来源：http://kdx.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bjh.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://vng.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lay.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://qtj.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://miw.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://evp.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mzp.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qpy.jianghu66.top

[Q41] 多表连接
来源：http://qcc.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://avi.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://hkf.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://zry.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://nnt.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://iie.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://anb.xziqi.cn

[Q43] 标量子查询
来源：http://boe.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uam.redwolf501.top

[Q44] IN 子查询
来源：http://svc.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iml.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://bqc.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxj.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://asf.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fzc.cdnleiting.top

[Q47] 与平均值比较
来源：http://iac.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zsw.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://jwj.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kli.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://bpy.iojbl.cn

[Q49] 更新单行
来源：http://ggv.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dkd.nanxinkj.top

[Q50] 批量更新
来源：http://dnr.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kwy.smart0.xyz

[Q51] 用子查询更新
来源：http://kqx.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dad.hnxiangtu.top

[Q52] 删除指定行
来源：http://gfd.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://wzd.chenlongwang.top

[Q53] 按条件删除
来源：http://ocz.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yrl.jinqigufen.top

[Q54] 清空表
来源：http://fmw.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://xzx.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://hhw.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvr.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://dht.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vyk.aizwys.cn

[Q57] 行号
来源：http://vqa.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kgd.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://txn.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hwk.dianchejie.cn

[Q59] 分组内累计
来源：http://vhj.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mrc.nwbrower.top

[Q60] 取上一行 / 下一行
来源：http://hfp.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fji.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qex.nanxuanxn.top

[Q61] 移动平均
来源：http://jmo.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oew.pycfn.com

[Q62] 分组占比
来源：http://nop.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ayo.pycfn.com

[Q63] 开启事务
来源：http://lly.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xtt.vqdsnc.cn

[Q64] 提交事务
来源：http://lhg.dashuyun.cn

COMMIT;
来源：http://nmm.316326.xyz

[Q65] 回滚事务
来源：http://wsh.zhaomingkeji.xyz

ROLLBACK;
来源：http://atg.zhixingplan.top

[Q66] 行锁查询
来源：http://pnm.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uut.tian-w.cn

[Q67] 设置隔离级别
来源：http://wnn.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dqi.xuanzx.com

[Q68] 保存点
来源：http://zer.xuanzx.com

SAVEPOINT sp1;
来源：http://ykm.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://jed.sxryk.cn

[Q69] 查看执行计划
来源：http://oib.tarul.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ysy.yueranfly.top

[Q70] 更新统计信息
来源：http://bzf.cqqwz.cn

ANALYZE TABLE users;
来源：http://aja.meibo888.top

[Q71] 查看建表语句
来源：http://xur.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qzh.redwolf501.top

[Q72] 查看索引
来源：http://bpm.ydjk.org.cn

SHOW INDEX FROM users;
来源：http://gim.yj20258.top

[Q73] 查看表状态
来源：http://rhk.c1oappe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://efa.zdbjq.cn

[Q74] 强制使用索引
来源：http://vni.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gzs.52xcode.cn

[Q75] 日期格式化
来源：http://umf.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kfz.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kwv.ybcxt.top

[Q76] 按天统计
来源：http://xub.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lov.hysaishi.cn

[Q77] 时间加减
来源：http://nbd.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lde.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://vtb.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aca.pycfn.com

[Q79] 字符串拼接
来源：http://hnb.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jqk.yangfankeji.com

[Q80] 字符串截取
来源：http://oop.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wjd.sxryk.cn

[Q81] 字符串替换
来源：http://tzp.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bjr.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://rcg.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rex.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://mqi.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gvr.xinyue.icu

[Q84] 去除首尾空格
来源：http://cmm.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://ogp.hcnkem.com

[Q85] 数值取整
来源：http://xui.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mrf.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://dyy.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rqg.daxiang520.top

[Q87] JSON 字段做条件
来源：http://sjp.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cak.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://eoy.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gwh.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yxs.hesvh.cn

[Q89] 判断表是否存在
来源：http://kzz.gotoacloud.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://miv.zhengqikj.top

[Q90] 生成序号列
来源：http://oif.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qur.smart0.xyz

================================================================================
来源：http://sry.hesvh.cn

R. Bash 专题
来源：http://bto.chenzaomai.com

================================================================================
来源：http://saa.tanke756.top

[R01] shebang 与严格模式
来源：http://kwj.sysykeji.top

#!/usr/bin/env bash
来源：http://gyp.ydzc1.top

set -euo pipefail
来源：http://egv.snrcjt.cn

[R02] 变量赋值与使用
来源：http://nmq.vehdjk.com

name="Tom"; echo "$name"
来源：http://hak.hnqzz.top

[R03] 只读变量
来源：http://hcs.zycfv.cn

readonly PI=3.14
来源：http://xag.nanxinkj.top

[R04] 位置参数
来源：http://dcw.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://giy.quarkkingdee.top

[R05] 参数默认值
来源：http://sfp.epnwcf.com

name="${1:-default}"
来源：http://irv.gzhubu.top

[R06] 判断命令是否存在
来源：http://trl.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://htr.zhoulong.xyz

[R07] if 判断文件
来源：http://trh.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vts.yvedp.cn

[R08] 数值比较
来源：http://ssl.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://jhz.hysaishi.cn

[R09] 字符串比较
来源：http://llz.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aak.nwbrower.top

[R10] 正则匹配
来源：http://fjt.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ids.dianchejie.cn

[R11] case 多分支
来源：http://bir.shzxlz.cn

case "$1" in
来源：http://qqv.nanxinkj.top

start) echo "启动" ;;
来源：http://cfz.fktsv.cn

stop)  echo "停止" ;;
来源：http://rqt.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://mzi.vehdjk.com

esac
来源：http://fko.zhongyouzk.top

[R12] for 遍历文件
来源：http://yld.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://rri.sweek.top

[R13] for 计数循环
来源：http://pom.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://zpt.ivvv.top

[R14] C 风格 for
来源：http://tjt.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uis.cqqwz.cn

[R15] while 逐行读文件
来源：http://lva.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fwa.jlsjyb.cn

[R16] until 等待条件
来源：http://vvk.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xxs.sysykeji.top

[R17] 数组定义与取值
来源：http://ygx.hcnkem.com


<!-- 参考信息 -->