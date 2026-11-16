代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wqs.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pik.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gge.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qyu.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mxj.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://kft.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bqk.wangshuangyany.cn

[P04] 求长度
来源：http://fdi.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vny.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://srb.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bqb.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kkq.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://wvw.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://qyk.ybcxt.top

Ruby: x.length;  x.size
来源：http://ouc.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tnx.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://dkw.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://atb.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yzp.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pxq.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jsg.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xqs.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ktk.meibo888.top

Ruby: a == b
来源：http://rmn.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggo.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vco.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://edk.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://ebo.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iss.ydzc1.top

TS:   if (x == null) {}
来源：http://nbm.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kmm.meibo888.top

Go:   if x == nil {}
来源：http://jpk.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pvr.svipenyu.cn

C#:   if (x is null) {}
来源：http://mkm.hongshengwenyu.top

[P07] 防抖与节流
来源：http://dre.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nmc.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://uum.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dxs.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://okh.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pto.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fos.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xlz.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cke.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://wcb.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://esp.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hjm.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vea.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vec.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://akc.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yqr.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrm.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://krm.hfpthk.cn

================================================================================
来源：http://jxg.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://esw.jinyuanbaomall.cn

================================================================================
来源：http://awg.andypj.xyz

[Q01] 创建表
来源：http://wpl.vehdjk.com

CREATE TABLE users (
来源：http://enm.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://abi.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://dsv.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://hjq.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nwt.yonumen.top

);
来源：http://ymn.gotoacloud.top

[Q02] 创建带外键的表
来源：http://ort.zycfv.cn

CREATE TABLE orders (
来源：http://fje.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xja.chenlongwang.top

user_id INT NOT NULL,
来源：http://jvt.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://zue.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zad.feifeiyinyue.top

);
来源：http://eev.jyoumei.cn

[Q03] 增加列
来源：http://lss.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cdi.nanxinkj.top

[Q04] 修改列类型
来源：http://hbx.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zvx.hysaishi.cn

[Q05] 重命名列
来源：http://clj.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wjv.ehwqpu.com

[Q06] 删除列
来源：http://epl.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://wce.sweek.top

[Q07] 删除表
来源：http://gjd.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://vas.sxryk.cn

[Q08] 创建普通索引
来源：http://cxv.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cnn.bbcook.cn

[Q09] 创建唯一索引
来源：http://ffg.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kmn.ehwqpu.com

[Q10] 插入单行
来源：http://pkm.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ppg.guowangkeji.top

[Q11] 一次插入多行
来源：http://iwy.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zzj.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://lka.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://ijs.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://icd.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://zzx.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mvh.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://zvo.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rgz.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yjm.shzxlz.cn

[Q15] 查询全部
来源：http://rda.xinyue.icu

SELECT * FROM users;
来源：http://qzc.zdbjq.cn

[Q16] 查询指定列
来源：http://wja.iojbl.cn

SELECT id, name FROM users;
来源：http://iem.cheryme.top

[Q17] 条件查询
来源：http://rnm.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lwb.chenzaomai.com

[Q18] 模糊匹配
来源：http://huy.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vek.yvedp.cn

[Q19] 范围查询
来源：http://udb.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ozw.tianlin.xyz

[Q20] IN 列表
来源：http://yax.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ynj.9152youxi.cn

[Q21] 空值判断
来源：http://dkm.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wuu.gotoacloud.top

[Q22] 排序
来源：http://ujn.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://two.xuetiantiany.cn

[Q23] 分页
来源：http://jda.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ang.fehbvm.com

[Q24] 去重
来源：http://vsq.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://ntj.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://ivt.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jrn.tarul.cn

[Q26] 计数
来源：http://nyn.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://bfc.tanke756.top

[Q27] 条件计数
来源：http://fbq.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cqz.yanxiufei.cn

[Q28] 求和与平均
来源：http://ssz.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iwe.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://ask.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iif.ydjk.org.cn

[Q30] 分组统计
来源：http://rcw.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dpk.daria6918.cn

[Q31] 分组后过滤
来源：http://aur.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nyn.yueranfly.top

[Q32] 分组拼接字符串
来源：http://upg.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ztr.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qrh.52xcode.cn

[Q33] 多列分组
来源：http://lxh.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gyy.guowangkeji.top

[Q34] 每组取第一条
来源：http://ocf.tarul.cn

SELECT * FROM (
来源：http://ynv.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fxv.cheryme.top

) t WHERE rn = 1;
来源：http://wnc.xylfe.cn

[Q35] 内连接
来源：http://sjr.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zjd.nanxinkj.top

[Q36] 左连接
来源：http://hxi.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ybu.zhiwuduotai.top

[Q37] 右连接
来源：http://ecx.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://coe.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://aoe.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://piy.havefunace.top

[Q39] 自连接（查上下级）
来源：http://soc.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oaq.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nyq.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://agf.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://myy.ppjwa.cn

[Q41] 多表连接
来源：http://mij.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://emp.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://xlo.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://wnp.sweek.top

[Q42] 连接条件附加过滤
来源：http://xwv.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://ofk.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ape.dianchejie.cn

[Q43] 标量子查询
来源：http://iab.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zxt.yvedp.cn

[Q44] IN 子查询
来源：http://pyq.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cmz.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://rke.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wxl.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kgo.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://voh.gogol.net.cn

[Q47] 与平均值比较
来源：http://dar.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xwp.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://jbq.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wyq.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://odh.svipenyu.cn

[Q49] 更新单行
来源：http://zsq.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qsw.hammf.cn

[Q50] 批量更新
来源：http://fme.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sli.zdbjq.cn

[Q51] 用子查询更新
来源：http://agk.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fuq.yvedp.cn

[Q52] 删除指定行
来源：http://dcq.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://jyt.cheryme.top

[Q53] 按条件删除
来源：http://soa.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kvm.feifeiyinyue.top

[Q54] 清空表
来源：http://ehc.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://ksf.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://mdo.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lxz.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://fbf.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://chv.tanke756.top

[Q57] 行号
来源：http://ozp.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qky.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://sqy.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dkq.fengsongda.top

[Q59] 分组内累计
来源：http://svo.yj20258888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oop.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://boe.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lop.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tuq.gotoacloud.top

[Q61] 移动平均
来源：http://rrs.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kzx.jinqigufen.top

[Q62] 分组占比
来源：http://pfg.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yvk.svipenyu.cn

[Q63] 开启事务
来源：http://cfg.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rec.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://vfw.zhongyouzk.top

COMMIT;
来源：http://bqj.nwbrower.top

[Q65] 回滚事务
来源：http://zzb.daxiang520.top

ROLLBACK;
来源：http://nbp.jlsjyb.cn

[Q66] 行锁查询
来源：http://qor.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qgj.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://esj.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uqz.pycfn.com

[Q68] 保存点
来源：http://vcl.sufxvd.cn

SAVEPOINT sp1;
来源：http://zgl.xinyue.icu

ROLLBACK TO sp1;
来源：http://dcd.shzxlz.cn

[Q69] 查看执行计划
来源：http://mzz.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ooj.tianlin.xyz

[Q70] 更新统计信息
来源：http://fuf.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://odm.cheryme.top

[Q71] 查看建表语句
来源：http://udc.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://brq.yj20258888.top

[Q72] 查看索引
来源：http://mne.jqgfzy.top

SHOW INDEX FROM users;
来源：http://wwf.52xcode.cn

[Q73] 查看表状态
来源：http://nuy.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mwh.tianlin.xyz

[Q74] 强制使用索引
来源：http://osy.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ncf.bbcook.cn

[Q75] 日期格式化
来源：http://yil.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ame.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://itf.sufxvd.cn

[Q76] 按天统计
来源：http://cfg.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jfc.nanxuanxn.top

[Q77] 时间加减
来源：http://bze.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jfv.xziqi.cn

[Q78] 当前时间
来源：http://ebh.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kqm.zhengqikj.top

[Q79] 字符串拼接
来源：http://itm.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://syh.yfazqb.com

[Q80] 字符串截取
来源：http://jfg.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://klp.vehdjk.com

[Q81] 字符串替换
来源：http://gcd.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tqn.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://sme.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bik.hnqzz.top

[Q83] 大小写转换
来源：http://aox.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uvl.yfazqb.com

[Q84] 去除首尾空格
来源：http://bka.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://uub.hnxiangtu.top

[Q85] 数值取整
来源：http://eiq.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zjj.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://rtt.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ugy.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://sfx.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ndu.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://nkt.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nqu.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xgk.yongpay.top

[Q89] 判断表是否存在
来源：http://qea.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bss.hywenlv.cn

[Q90] 生成序号列
来源：http://rdt.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jgf.ydjk.org.cn

================================================================================
来源：http://ngb.gotoacloud.top

R. Bash 专题
来源：http://tst.yfazqb.com

================================================================================
来源：http://lis.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://jxr.smart0.xyz

#!/usr/bin/env bash
来源：http://yhj.kuanghao11.cn

set -euo pipefail
来源：http://poe.shzxlz.cn

[R02] 变量赋值与使用
来源：http://yqg.bbcook.cn

name="Tom"; echo "$name"
来源：http://yyu.sweek.top

[R03] 只读变量
来源：http://ayo.wangshuangyany.cn

readonly PI=3.14
来源：http://hwb.yj20258.top

[R04] 位置参数
来源：http://agb.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wxy.jinqigfzy.top

[R05] 参数默认值
来源：http://goj.zhaomingkeji.xyz

name="${1:-default}"
来源：http://myt.dianchejie.cn

[R06] 判断命令是否存在
来源：http://pfd.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fag.tianlin.xyz

[R07] if 判断文件
来源：http://lku.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://boc.shuidangran.top

[R08] 数值比较
来源：http://opc.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://aos.meibo888.top

[R09] 字符串比较
来源：http://bcv.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://owk.316326.xyz

[R10] 正则匹配
来源：http://rhq.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gry.yuxming.cn

[R11] case 多分支
来源：http://uqv.jlsjyb.cn

case "$1" in
来源：http://dze.hywenlv.cn

start) echo "启动" ;;
来源：http://boc.redwolf501.top

stop)  echo "停止" ;;
来源：http://gyg.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://zds.guannengcc.top

esac
来源：http://rbl.redwolf501.top

[R12] for 遍历文件
来源：http://hvi.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://jcw.ppjwa.cn

[R13] for 计数循环
来源：http://uhc.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://abj.316326.xyz

[R14] C 风格 for
来源：http://xxn.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eij.pycfn.com

[R15] while 逐行读文件
来源：http://hue.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cff.fanxiaobao.xyz

[R16] until 等待条件
来源：http://ngp.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fta.meibo888.top

[R17] 数组定义与取值
来源：http://dlg.shzxlz.cn


<!-- 参考信息 -->