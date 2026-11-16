代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rhd.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kpe.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://isg.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfq.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://exj.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kid.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mos.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vdr.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yzj.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mpt.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://omk.daxiang520.top

[P04] 求长度
来源：http://ykp.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qva.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lty.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vuz.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yql.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://qda.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://pmo.gzhubu.top

Ruby: x.length;  x.size
来源：http://meq.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ryc.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://imu.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kgj.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ewp.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zgx.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bpq.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vgf.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://aoq.epnwcf.com

Ruby: a == b
来源：http://qqi.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jjo.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qty.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://onw.tanke756.top

PHP:  if (empty($x)) {}
来源：http://opi.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lvr.jinqigfzy.top

TS:   if (x == null) {}
来源：http://oak.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vcd.shuidangran.top

Go:   if x == nil {}
来源：http://kng.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hna.vqdsnc.cn

C#:   if (x is null) {}
来源：http://alu.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://wmd.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://txp.cashguo.top

PHP:  // 手写时间戳比较
来源：http://rqa.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cep.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xpy.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qbz.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dzo.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nez.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bea.bjfxy.top

[P08] 处理浮点精度问题
来源：http://trf.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kfu.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lsz.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://azf.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://phu.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zax.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pra.jinyuanbaomall.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://swb.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ten.fktsv.cn

================================================================================
来源：http://vtu.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hrl.jyoumei.cn

================================================================================
来源：http://hoq.hnxiangtu.top

[Q01] 创建表
来源：http://klg.yuanzhike.top

CREATE TABLE users (
来源：http://ecu.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://koc.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://diu.shanyushiyangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://ssr.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fvy.havefunace.top

);
来源：http://nlq.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://znx.birdmap.top

CREATE TABLE orders (
来源：http://aqf.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uze.cashguo.top

user_id INT NOT NULL,
来源：http://tvg.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://wjx.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lht.fktsv.cn

);
来源：http://nmo.yj20258.top

[Q03] 增加列
来源：http://omu.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dqt.shzxlz.cn

[Q04] 修改列类型
来源：http://did.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tuh.gotoacloud.top

[Q05] 重命名列
来源：http://eqm.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mwq.sweek.top

[Q06] 删除列
来源：http://syk.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://ytm.havefunace.top

[Q07] 删除表
来源：http://wzu.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://hcu.andypj.xyz

[Q08] 创建普通索引
来源：http://ooi.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://pai.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://ctb.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dvq.shzxlz.cn

[Q10] 插入单行
来源：http://gtq.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zxl.vqdsnc.cn

[Q11] 一次插入多行
来源：http://fiy.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wim.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://xjb.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ghz.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zgs.pycfn.com

[Q13] 忽略重复插入
来源：http://onp.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gtf.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://emo.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://klr.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jgd.xuanzx.com

[Q15] 查询全部
来源：http://gtq.zhiwuduotai.top

SELECT * FROM users;
来源：http://ceg.hysaishi.cn

[Q16] 查询指定列
来源：http://bnh.hnqzz.top

SELECT id, name FROM users;
来源：http://trj.daxiang520.top

[Q17] 条件查询
来源：http://vwq.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rgu.tian-w.cn

[Q18] 模糊匹配
来源：http://jzz.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vzc.hcnkem.com

[Q19] 范围查询
来源：http://kff.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iyv.zycfv.cn

[Q20] IN 列表
来源：http://mam.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qwi.tarul.cn

[Q21] 空值判断
来源：http://sbo.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xjh.ywan-chungtsiang.top

[Q22] 排序
来源：http://wtw.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rmo.iojbl.cn

[Q23] 分页
来源：http://pvp.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eew.tian-w.cn

[Q24] 去重
来源：http://oah.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://lki.ctjpmb.com

[Q25] 只取前 N 条
来源：http://fwr.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ibb.feifeiyinyue.top

[Q26] 计数
来源：http://zid.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://ify.pengpengdd.cyou

[Q27] 条件计数
来源：http://bqc.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zfp.wangdashe.top

[Q28] 求和与平均
来源：http://fpi.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://juz.chenjidiqi.icu

[Q29] 最大最小值
来源：http://kqy.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xpk.nanxuanxn.top

[Q30] 分组统计
来源：http://jyo.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gtv.ybcxt.top

[Q31] 分组后过滤
来源：http://gne.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gdj.andypj.xyz

[Q32] 分组拼接字符串
来源：http://wxp.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cuk.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://obd.fengsongda.top

[Q33] 多列分组
来源：http://oup.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qar.yongpay.top

[Q34] 每组取第一条
来源：http://vll.fengsongda.top

SELECT * FROM (
来源：http://qwr.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sfx.hnxiangtu.top

) t WHERE rn = 1;
来源：http://tuu.c1oappe.top

[Q35] 内连接
来源：http://dku.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ipz.birdmap.top

[Q36] 左连接
来源：http://hrv.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qbw.smart0.xyz

[Q37] 右连接
来源：http://zfj.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dag.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://ead.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zas.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://wff.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ayo.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ote.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://hjy.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://inm.jianghu66.top

[Q41] 多表连接
来源：http://sbi.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://htn.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://vif.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://jjt.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://zcq.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://dmj.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hlr.aibaodan.cn

[Q43] 标量子查询
来源：http://dlf.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kax.kuanghao11.cn

[Q44] IN 子查询
来源：http://grc.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kog.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://jcn.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rbl.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://cmj.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://atd.fengsongda.top

[Q47] 与平均值比较
来源：http://zyx.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rlu.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://jhv.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qzs.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://ugb.iojbl.cn

[Q49] 更新单行
来源：http://kfq.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ljv.hywenlv.cn

[Q50] 批量更新
来源：http://yjc.ywan-chungtsiang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pdh.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://qsf.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xhs.ivvv.top

[Q52] 删除指定行
来源：http://eux.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://ekb.hysaishi.cn

[Q53] 按条件删除
来源：http://fex.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vsj.fanxiaobao.xyz

[Q54] 清空表
来源：http://zar.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://bxr.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://hhk.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wmh.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://rlq.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dpk.ehwqpu.com

[Q57] 行号
来源：http://tga.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dkb.xuanzx.com

[Q58] 累计求和
来源：http://abv.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pzp.hongshengwenyu.top

[Q59] 分组内累计
来源：http://nam.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ulh.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://gam.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fhw.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ozr.dianchejie.cn

[Q61] 移动平均
来源：http://tat.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://khy.nanxinkj.top

[Q62] 分组占比
来源：http://dae.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eta.yangfankeji.com

[Q63] 开启事务
来源：http://rme.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yau.wangshuangyany.cn

[Q64] 提交事务
来源：http://hvy.pycfn.com

COMMIT;
来源：http://zae.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://vct.nanxuanxn.top

ROLLBACK;
来源：http://btc.meibo888.top

[Q66] 行锁查询
来源：http://vao.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yaf.9152youxi.cn

[Q67] 设置隔离级别
来源：http://ilw.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oza.dianchejie.cn

[Q68] 保存点
来源：http://khb.ydzc1.top

SAVEPOINT sp1;
来源：http://hqe.zycfv.cn

ROLLBACK TO sp1;
来源：http://zcp.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://oau.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mth.zycfv.cn

[Q70] 更新统计信息
来源：http://ynj.vehdjk.com

ANALYZE TABLE users;
来源：http://mzn.mhx1999.top

[Q71] 查看建表语句
来源：http://jwb.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rpo.svipenyu.cn

[Q72] 查看索引
来源：http://hhc.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://kdn.bjfxy.top

[Q73] 查看表状态
来源：http://sza.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qak.sxryk.cn

[Q74] 强制使用索引
来源：http://wms.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ccm.gaohongyu789.top

[Q75] 日期格式化
来源：http://qpq.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ico.yonumen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://epw.zdqjudy.top

[Q76] 按天统计
来源：http://wex.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://opt.vqdsnc.cn

[Q77] 时间加减
来源：http://vrc.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kwf.epnwcf.com

[Q78] 当前时间
来源：http://yrm.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://boj.quarkkingdee.top

[Q79] 字符串拼接
来源：http://vwg.meibo888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pix.quarkkingdee.top

[Q80] 字符串截取
来源：http://xaw.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fxx.sxryk.cn

[Q81] 字符串替换
来源：http://duf.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qzx.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://tlj.bjfxy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvm.nwbrower.top

[Q83] 大小写转换
来源：http://fpp.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ouo.daria6918.cn

[Q84] 去除首尾空格
来源：http://knm.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://bnf.fktsv.cn

[Q85] 数值取整
来源：http://lxu.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cdf.yonumen.top

[Q86] 读取 JSON 字段
来源：http://atx.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://exv.52xcode.cn

[Q87] JSON 字段做条件
来源：http://rol.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tsx.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://ylu.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hmx.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uxk.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://nzo.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hfo.yongpay.top

[Q90] 生成序号列
来源：http://kmk.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iqf.zdqjudy.top

================================================================================
来源：http://uvq.vqdsnc.cn

R. Bash 专题
来源：http://ulf.quarkkingdee.top

================================================================================
来源：http://dxt.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://vne.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://nki.52xcode.cn

set -euo pipefail
来源：http://qmh.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://bmt.52xcode.cn

name="Tom"; echo "$name"
来源：http://lfc.c1oappe.top

[R03] 只读变量
来源：http://ouv.yuanzhike.top

readonly PI=3.14
来源：http://ein.shanyushiyangkeji.top

[R04] 位置参数
来源：http://mzk.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kej.quarkkingdee.top

[R05] 参数默认值
来源：http://lao.xuetiantiany.cn

name="${1:-default}"
来源：http://fwf.zycfv.cn

[R06] 判断命令是否存在
来源：http://lcb.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://udr.tian-w.cn

[R07] if 判断文件
来源：http://xwc.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gzm.zycfv.cn

[R08] 数值比较
来源：http://ufc.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zst.jqgfzy.top

[R09] 字符串比较
来源：http://ktl.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ezb.vqdsnc.cn

[R10] 正则匹配
来源：http://pqj.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iar.epnwcf.com

[R11] case 多分支
来源：http://dpy.yj20258.top

case "$1" in
来源：http://hxr.bjfxy.top

start) echo "启动" ;;
来源：http://aok.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://fjy.shuidangran.top

*)     echo "未知命令" ;;
来源：http://cwh.fengsongda.top

esac
来源：http://olq.jqgfzy.top

[R12] for 遍历文件
来源：http://ede.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://kdx.chenlongwang.top

[R13] for 计数循环
来源：http://ouw.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://nai.redwolf501.top

[R14] C 风格 for
来源：http://atz.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mgo.guannengcc.top

[R15] while 逐行读文件
来源：http://boo.hongshengwenyu.top


<!-- 参考信息 -->