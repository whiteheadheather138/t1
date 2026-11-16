代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kjc.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hpd.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eza.yj20258888.top

[P04] 求长度
来源：http://qni.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwr.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ess.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bal.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vdp.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://wag.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://oau.316326.xyz

Ruby: x.length;  x.size
来源：http://bte.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lll.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://sle.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://txs.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hiq.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nnr.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://smj.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tnm.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eio.shangyingyoupin.top

Ruby: a == b
来源：http://iza.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mxg.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rpi.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bxn.ivvv.top

PHP:  if (empty($x)) {}
来源：http://onw.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rne.bbcook.cn

TS:   if (x == null) {}
来源：http://wsu.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zqq.xuanzx.com

Go:   if x == nil {}
来源：http://upy.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xsj.fktsv.cn

C#:   if (x is null) {}
来源：http://mgw.yonumen.top

[P07] 防抖与节流
来源：http://ffr.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uiu.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://rfx.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nod.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bue.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://prg.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nzx.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wdx.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uil.pycfn.com

[P08] 处理浮点精度问题
来源：http://xqy.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cdg.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mhp.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://poh.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ddc.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://slk.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tsj.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ooa.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oqf.aibaodan.cn

================================================================================
来源：http://kbm.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jee.hywenlv.cn

================================================================================
来源：http://rab.nanxuanxn.top

[Q01] 创建表
来源：http://den.shuidangran.top

CREATE TABLE users (
来源：http://hsl.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://azi.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://mpe.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://nhy.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oba.meibo888.top

);
来源：http://acu.9152youxi.cn

[Q02] 创建带外键的表
来源：http://dwx.cucudq.cn

CREATE TABLE orders (
来源：http://doo.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://emh.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://xby.hammf.cn

amount DECIMAL(10, 2),
来源：http://hka.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gvs.sjlbkw.cn

);
来源：http://qkg.sweek.top

[Q03] 增加列
来源：http://flj.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mtn.tarul.cn

[Q04] 修改列类型
来源：http://lnr.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yce.andypj.xyz

[Q05] 重命名列
来源：http://uit.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yql.jinqigfzy.top

[Q06] 删除列
来源：http://kbe.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://hvf.aibaodan.cn

[Q07] 删除表
来源：http://qqn.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://nda.jianghu66.top

[Q08] 创建普通索引
来源：http://ozg.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xyb.shuidangran.top

[Q09] 创建唯一索引
来源：http://rzf.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sgf.quarkkingdee.top

[Q10] 插入单行
来源：http://zhs.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mfx.wangdashe.top

[Q11] 一次插入多行
来源：http://hzp.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yin.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://uwv.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://alr.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xga.wangdashe.top

[Q13] 忽略重复插入
来源：http://vnb.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qeh.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://ghy.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mzi.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ooi.ehwqpu.com

[Q15] 查询全部
来源：http://cnu.zhoulong.xyz

SELECT * FROM users;
来源：http://nuz.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://cub.jyoumei.cn

SELECT id, name FROM users;
来源：http://gho.zhoulong.xyz

[Q17] 条件查询
来源：http://yys.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eak.cashguo.top

[Q18] 模糊匹配
来源：http://ziv.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ozm.zhixingplan.top

[Q19] 范围查询
来源：http://pkx.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kdq.wangdashe.top

[Q20] IN 列表
来源：http://mla.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kny.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://zdd.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://olj.ppjwa.cn

[Q22] 排序
来源：http://foo.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://psn.bbcook.cn

[Q23] 分页
来源：http://xzg.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pwk.guowangkeji.top

[Q24] 去重
来源：http://ofx.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://ovn.chenzaomai.com

[Q25] 只取前 N 条
来源：http://kfx.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://evf.cashguo.top

[Q26] 计数
来源：http://mqc.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://luj.fengsongda.top

[Q27] 条件计数
来源：http://qbs.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tgw.xylfe.cn

[Q28] 求和与平均
来源：http://uuc.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fay.zhongyouzk.top

[Q29] 最大最小值
来源：http://gik.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fza.jianghu66.top

[Q30] 分组统计
来源：http://ztn.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ncg.aibaodan.cn

[Q31] 分组后过滤
来源：http://pdd.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://anj.epnwcf.com

[Q32] 分组拼接字符串
来源：http://juh.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jtt.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aik.jinqigufen.top

[Q33] 多列分组
来源：http://bpq.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://prl.ivvv.top

[Q34] 每组取第一条
来源：http://wpd.tianlin.xyz

SELECT * FROM (
来源：http://qgk.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mft.andypj.xyz

) t WHERE rn = 1;
来源：http://wjf.iojbl.cn

[Q35] 内连接
来源：http://iot.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xtg.aibaodan.cn

[Q36] 左连接
来源：http://pmz.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dwk.vqdsnc.cn

[Q37] 右连接
来源：http://rzp.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kqd.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://efo.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xrp.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://wfr.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://btf.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xkc.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kpc.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zdv.shzxlz.cn

[Q41] 多表连接
来源：http://kll.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hgv.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://rqd.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://jtn.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://czl.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://ggx.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://okx.uphjek.com

[Q43] 标量子查询
来源：http://ppn.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jyz.pycfn.com

[Q44] IN 子查询
来源：http://tyf.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zsb.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://qpy.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tkv.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://mfm.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://awk.yonumen.top

[Q47] 与平均值比较
来源：http://aeg.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cpz.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://hnp.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qai.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://lot.c1oappe.top

[Q49] 更新单行
来源：http://osh.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nqt.hongshengwenyu.top

[Q50] 批量更新
来源：http://sez.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qvh.hcnkem.com

[Q51] 用子查询更新
来源：http://nel.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mso.shangyingyoupin.top

[Q52] 删除指定行
来源：http://aah.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://jrj.jqgfzy.top

[Q53] 按条件删除
来源：http://pah.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ewo.yj20258.top

[Q54] 清空表
来源：http://iju.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://wqu.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://gqa.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dur.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://qmd.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://guh.tian-w.cn

[Q57] 行号
来源：http://bgu.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hlu.yueranfly.top

[Q58] 累计求和
来源：http://zvv.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://smp.jiagoushi.top

[Q59] 分组内累计
来源：http://dgz.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tdr.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://nzc.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kur.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lxy.jianghu66.top

[Q61] 移动平均
来源：http://vvc.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://won.yvedp.cn

[Q62] 分组占比
来源：http://uep.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rvf.hesvh.cn

[Q63] 开启事务
来源：http://jwl.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tie.9152youxi.cn

[Q64] 提交事务
来源：http://nmz.feifeiyinyue.top

COMMIT;
来源：http://ydn.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://dsc.kuanghao11.cn

ROLLBACK;
来源：http://suo.tian-w.cn

[Q66] 行锁查询
来源：http://syy.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jpd.yj20258888.top

[Q67] 设置隔离级别
来源：http://zoh.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jss.yj20258888.top

[Q68] 保存点
来源：http://nng.jqgufenzy.top

SAVEPOINT sp1;
来源：http://tfd.tarul.cn

ROLLBACK TO sp1;
来源：http://hjd.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://fag.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pir.yanxiufei.cn

[Q70] 更新统计信息
来源：http://boq.jinqigfzy.top

ANALYZE TABLE users;
来源：http://oxo.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://ghp.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bxu.haohaochexian.top

[Q72] 查看索引
来源：http://mmx.andypj.xyz

SHOW INDEX FROM users;
来源：http://hum.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://dkb.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mym.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://rny.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lvg.dashuyun.cn

[Q75] 日期格式化
来源：http://dsl.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xmi.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ypg.zdbjq.cn

[Q76] 按天统计
来源：http://udo.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bae.xuetiantiany.cn

[Q77] 时间加减
来源：http://rni.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zhe.cheryme.top

[Q78] 当前时间
来源：http://vmf.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ilh.fengsongda.top

[Q79] 字符串拼接
来源：http://okl.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tue.0kj1m.cn

[Q80] 字符串截取
来源：http://ley.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rro.yanxiufei.cn

[Q81] 字符串替换
来源：http://lyg.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hjw.yongpay.top

[Q82] 字符长度与字节长度
来源：http://kyv.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://utu.yangfankeji.com

[Q83] 大小写转换
来源：http://wwp.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xcs.sxryk.cn

[Q84] 去除首尾空格
来源：http://cpg.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://dsi.gotoacloud.top

[Q85] 数值取整
来源：http://ajr.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qme.birdmap.top

[Q86] 读取 JSON 字段
来源：http://nil.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hxy.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://fno.jinqigfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iqa.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://zrj.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yiv.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aor.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://boc.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://goj.yj202588.top

[Q90] 生成序号列
来源：http://hwa.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cwy.zhoulong.xyz

================================================================================
来源：http://wcs.ctjpmb.com

R. Bash 专题
来源：http://tis.yvedp.cn

================================================================================
来源：http://bde.redwolf501.top

[R01] shebang 与严格模式
来源：http://ezn.kuanghao11.cn

#!/usr/bin/env bash
来源：http://mbg.zdbjq.cn

set -euo pipefail
来源：http://skf.daria6918.cn

[R02] 变量赋值与使用
来源：http://vaf.fehbvm.com

name="Tom"; echo "$name"
来源：http://bdr.svipenyu.cn

[R03] 只读变量
来源：http://viv.havefunace.top

readonly PI=3.14
来源：http://cej.52xcode.cn

[R04] 位置参数
来源：http://hjp.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tfu.shuidangran.top

[R05] 参数默认值
来源：http://oxp.zhongyouzk.top

name="${1:-default}"
来源：http://fve.jianghu66.top

[R06] 判断命令是否存在
来源：http://bof.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nwa.cheryme.top

[R07] if 判断文件
来源：http://prk.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lmk.quarkkingdee.top

[R08] 数值比较
来源：http://qzw.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://tvg.yuxming.cn

[R09] 字符串比较
来源：http://hwz.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mbu.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://oju.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dyr.aibaodan.cn

[R11] case 多分支
来源：http://cro.quarkkingdee.top

case "$1" in
来源：http://vgs.zdbjq.cn

start) echo "启动" ;;
来源：http://soi.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://hjr.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://uzb.guowangkeji.top

esac
来源：http://adn.quarkkingdee.top

[R12] for 遍历文件
来源：http://bst.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://fxc.wangdashe.top

[R13] for 计数循环
来源：http://ami.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://xii.daxiang520.top

[R14] C 风格 for
来源：http://twh.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nbd.yongpay.top

[R15] while 逐行读文件
来源：http://geo.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zlj.zhijiandao.cn

[R16] until 等待条件
来源：http://xoy.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://crv.tian-w.cn

[R17] 数组定义与取值
来源：http://ptf.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://jhc.yj202588.top

[R18] 遍历数组
来源：http://bmb.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://amf.shanyushiyangkeji.top

[R19] 数组长度
来源：http://cev.yj20258.top


<!-- 参考信息 -->