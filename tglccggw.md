代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dia.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bol.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jhf.zhengqikj.top

[P04] 求长度
来源：http://yuv.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ogp.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xdo.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gmo.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://evs.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://vwg.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://qfc.gotoacloud.top

Ruby: x.length;  x.size
来源：http://jtp.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pzm.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://cne.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hsb.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jhn.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ths.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rnx.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ipe.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://mgm.gzhubu.top

Ruby: a == b
来源：http://zqk.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hma.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pvd.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wtd.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://vid.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zfp.jianghu66.top

TS:   if (x == null) {}
来源：http://grn.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mqh.zdqjudy.top

Go:   if x == nil {}
来源：http://khq.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kgf.9152youxi.cn

C#:   if (x is null) {}
来源：http://kws.kuanghao11.cn

[P07] 防抖与节流
来源：http://zxv.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cls.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://ajt.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dah.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzc.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nse.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pot.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://tpu.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ovs.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://uqo.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cnl.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://juz.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tfs.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sum.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jvu.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ils.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jse.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cdj.snrcjt.cn

================================================================================
来源：http://tpk.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://afw.chenzaomai.com

================================================================================
来源：http://soo.aibaodan.cn

[Q01] 创建表
来源：http://fpo.aibaodan.cn

CREATE TABLE users (
来源：http://qjb.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hov.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://nfl.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://lqb.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aix.wangshuangyany.cn

);
来源：http://iet.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://zua.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://rba.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggs.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://rdq.yonumen.top

amount DECIMAL(10, 2),
来源：http://bsk.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://amp.ydzc1.top

);
来源：http://bmc.316326.xyz

[Q03] 增加列
来源：http://kvs.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qfv.zhoulong.xyz

[Q04] 修改列类型
来源：http://hnu.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ygc.jinghuilouyu.cn

[Q05] 重命名列
来源：http://fgm.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ygm.xziqi.cn

[Q06] 删除列
来源：http://auh.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://hdr.xuanzx.com

[Q07] 删除表
来源：http://drz.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://gyr.zhixingplan.top

[Q08] 创建普通索引
来源：http://rgf.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ibz.cashguo.top

[Q09] 创建唯一索引
来源：http://mgy.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eoz.zycfv.cn

[Q10] 插入单行
来源：http://kbv.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ars.vqdsnc.cn

[Q11] 一次插入多行
来源：http://wai.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wsq.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://kzd.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://ckl.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ocx.sysykeji.top

[Q13] 忽略重复插入
来源：http://tmm.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bsl.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://yuh.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ypg.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zxz.yongpay.top

[Q15] 查询全部
来源：http://vah.daxiang520.top

SELECT * FROM users;
来源：http://eup.jlsjyb.cn

[Q16] 查询指定列
来源：http://gkq.yfazqb.com

SELECT id, name FROM users;
来源：http://eza.redwolf501.top

[Q17] 条件查询
来源：http://bpw.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fou.sufxvd.cn

[Q18] 模糊匹配
来源：http://fwy.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pkb.kuanghao11.cn

[Q19] 范围查询
来源：http://uvi.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://enb.guowangkeji.top

[Q20] IN 列表
来源：http://hph.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xvq.jiagoushi.top

[Q21] 空值判断
来源：http://fsv.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fbf.cheryme.top

[Q22] 排序
来源：http://rzg.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qzx.jinqigfzy.top

[Q23] 分页
来源：http://jrb.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rmz.guannengcc.top

[Q24] 去重
来源：http://zgs.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://zzl.dashuyun.cn

[Q25] 只取前 N 条
来源：http://dyb.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://owa.jiagoushi.top

[Q26] 计数
来源：http://xqi.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://wkq.yongpay.top

[Q27] 条件计数
来源：http://crm.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ukt.sysykeji.top

[Q28] 求和与平均
来源：http://mmu.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bfu.ivvv.top

[Q29] 最大最小值
来源：http://cjk.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mke.sweek.top

[Q30] 分组统计
来源：http://bky.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yyf.gzhubu.top

[Q31] 分组后过滤
来源：http://dvw.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yhg.316326.xyz

[Q32] 分组拼接字符串
来源：http://ukv.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yvp.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rnq.uphjek.com

[Q33] 多列分组
来源：http://bkm.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kzb.hnxiangtu.top

[Q34] 每组取第一条
来源：http://htw.shanyushiyangtech.top

SELECT * FROM (
来源：http://cqq.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nqm.wangdashe.top

) t WHERE rn = 1;
来源：http://fel.hnqzz.top

[Q35] 内连接
来源：http://djr.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wjc.xuanzx.com

[Q36] 左连接
来源：http://bva.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lew.shzxlz.cn

[Q37] 右连接
来源：http://mwh.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hyu.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://hxq.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vpv.birdmap.top

[Q39] 自连接（查上下级）
来源：http://neu.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gem.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jrk.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ocl.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ufj.haohaochexian.top

[Q41] 多表连接
来源：http://aeg.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tjl.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://sjt.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://ggt.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://gdq.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://hfw.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ndd.cheryme.top

[Q43] 标量子查询
来源：http://vdw.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dgc.daria6918.cn

[Q44] IN 子查询
来源：http://kgi.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iuf.yj20258.top

[Q45] EXISTS 判断存在
来源：http://odz.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyg.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tsf.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttp.hammf.cn

[Q47] 与平均值比较
来源：http://htc.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ewr.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://myo.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fhc.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://rmy.svipenyu.cn

[Q49] 更新单行
来源：http://ems.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://igs.sjlbkw.cn

[Q50] 批量更新
来源：http://bkl.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pal.yuxming.cn

[Q51] 用子查询更新
来源：http://ahk.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aed.hywenlv.cn

[Q52] 删除指定行
来源：http://nyc.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://bce.hywenlv.cn

[Q53] 按条件删除
来源：http://aan.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pqw.hfpthk.cn

[Q54] 清空表
来源：http://lic.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://xww.guannengcc.top

[Q55] 排名（并列占位）
来源：http://oym.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vrb.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://ysi.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://luh.pengpengdd.cyou

[Q57] 行号
来源：http://xdg.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://byw.xinyue.icu

[Q58] 累计求和
来源：http://oco.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kmw.jiagoushi.top

[Q59] 分组内累计
来源：http://lrm.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://att.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://ixf.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ljg.52xcode.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rrg.gotoacloud.top

[Q61] 移动平均
来源：http://mis.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ynv.jiagoushi.top

[Q62] 分组占比
来源：http://gch.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bhe.vqdsnc.cn

[Q63] 开启事务
来源：http://gfo.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pzn.chenjidiqi.icu

[Q64] 提交事务
来源：http://ivf.tanke756.top

COMMIT;
来源：http://lgb.wangshuangyany.cn

[Q65] 回滚事务
来源：http://vrb.hnxiangtu.top

ROLLBACK;
来源：http://fwn.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://olg.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fnf.yueranfly.top

[Q67] 设置隔离级别
来源：http://uzu.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lsk.bbcook.cn

[Q68] 保存点
来源：http://mtz.jlsjyb.cn

SAVEPOINT sp1;
来源：http://wnu.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://pfb.ehwqpu.com

[Q69] 查看执行计划
来源：http://ioz.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://new.zhixingplan.top

[Q70] 更新统计信息
来源：http://gnx.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://edw.cashguo.top

[Q71] 查看建表语句
来源：http://soj.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ufe.daxiang520.top

[Q72] 查看索引
来源：http://izj.hammf.cn

SHOW INDEX FROM users;
来源：http://ljp.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://elx.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fwq.yj20258.top

[Q74] 强制使用索引
来源：http://mrm.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cou.zdqjudy.top

[Q75] 日期格式化
来源：http://fvh.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xyo.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nwv.smart0.xyz

[Q76] 按天统计
来源：http://hps.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://alg.tianlin.xyz

[Q77] 时间加减
来源：http://cuh.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uej.xinyue.icu

[Q78] 当前时间
来源：http://izw.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dhe.hfpthk.cn

[Q79] 字符串拼接
来源：http://opt.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xew.fzhhl.top

[Q80] 字符串截取
来源：http://cft.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dgk.birdmap.top

[Q81] 字符串替换
来源：http://thw.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hsl.yj20258.top

[Q82] 字符长度与字节长度
来源：http://ixe.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ssm.ctjpmb.com

[Q83] 大小写转换
来源：http://xwh.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vws.jinqigufen.top

[Q84] 去除首尾空格
来源：http://olq.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://tkq.daria6918.cn

[Q85] 数值取整
来源：http://xkv.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yes.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://ijh.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bxp.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://mjh.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vvy.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://kzn.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pyf.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hvl.jinqigufen.top

[Q89] 判断表是否存在
来源：http://tlg.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ajc.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://drw.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wxy.jlsjyb.cn

================================================================================
来源：http://ubh.gotoacloud.top

R. Bash 专题
来源：http://dvp.ywan-chungtsiang.top

================================================================================
来源：http://jxr.gogol.net.cn

[R01] shebang 与严格模式
来源：http://nnj.sysykeji.top

#!/usr/bin/env bash
来源：http://qqj.kuanghao11.cn

set -euo pipefail
来源：http://nxw.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://jyf.shzxlz.cn

name="Tom"; echo "$name"
来源：http://rzq.9152youxi.cn

[R03] 只读变量
来源：http://ide.shuidangran.top

readonly PI=3.14
来源：http://lyq.cdnleiting.top

[R04] 位置参数
来源：http://izo.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vjk.zhengqikj.top

[R05] 参数默认值
来源：http://tfe.aibaodan.cn

name="${1:-default}"
来源：http://vbo.c1oappe.top

[R06] 判断命令是否存在
来源：http://yjn.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wxz.pengpengdd.cyou

[R07] if 判断文件
来源：http://uyg.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lpc.hywenlv.cn

[R08] 数值比较
来源：http://sjh.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gmg.jianghu66.top

[R09] 字符串比较
来源：http://xah.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qvo.dianchejie.cn

[R10] 正则匹配
来源：http://crc.kuanghao11.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mch.fanxiaobao.xyz

[R11] case 多分支
来源：http://wre.zhengqikj.top

case "$1" in
来源：http://jma.snrcjt.cn

start) echo "启动" ;;
来源：http://xqu.yvedp.cn

stop)  echo "停止" ;;
来源：http://see.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://zkr.shanyushiyangtech.top

esac
来源：http://rcj.havefunace.top

[R12] for 遍历文件
来源：http://xcp.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://ikc.shangyingyoupin.top

[R13] for 计数循环
来源：http://bie.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://ovb.sweek.top

[R14] C 风格 for
来源：http://dty.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bes.ybcxt.top

[R15] while 逐行读文件
来源：http://zfd.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://drk.nwbrower.top

[R16] until 等待条件
来源：http://vzq.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ljv.cheryme.top

[R17] 数组定义与取值
来源：http://kvb.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wsm.yuxming.cn

[R18] 遍历数组
来源：http://mds.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gga.nwbrower.top

[R19] 数组长度
来源：http://znn.yongpay.top


<!-- 参考信息 -->