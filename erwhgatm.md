代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cyd.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pez.gotoacloud.top

[P03] 生成短随机字符串
来源：http://lax.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wlm.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vjo.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vij.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ejm.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bsf.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gli.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tpe.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dij.sjlbkw.cn

[P04] 求长度
来源：http://yiz.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fum.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://stj.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bgz.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vfq.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://ctb.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://woo.sysykeji.top

Ruby: x.length;  x.size
来源：http://sti.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ifx.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://zpf.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nhu.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lur.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://epa.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bwp.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vwx.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://mtn.svipenyu.cn

Ruby: a == b
来源：http://atz.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vkt.gogol.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jud.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ymx.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://qcy.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cai.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://rfr.c1oappe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lyf.svipenyu.cn

Go:   if x == nil {}
来源：http://nbk.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://asg.316326.xyz

C#:   if (x is null) {}
来源：http://qyl.gogol.net.cn

[P07] 防抖与节流
来源：http://ggi.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jbe.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://ebj.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wig.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqu.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wqs.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rii.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxf.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jcs.hammf.cn

[P08] 处理浮点精度问题
来源：http://xvb.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fzg.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gck.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rsn.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zmp.bjfxy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zku.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://otg.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kbl.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oyq.ehwqpu.com

================================================================================
来源：http://squ.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://keg.jinghuilouyu.cn

================================================================================
来源：http://edm.redwolf501.top

[Q01] 创建表
来源：http://nzh.xziqi.cn

CREATE TABLE users (
来源：http://zti.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://idt.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://xbt.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://ywe.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://igy.yj202588.top

);
来源：http://lht.uphjek.com

[Q02] 创建带外键的表
来源：http://fwq.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://yss.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvk.iojbl.cn

user_id INT NOT NULL,
来源：http://agb.c1oappe.top

amount DECIMAL(10, 2),
来源：http://vbl.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://amb.sweek.top

);
来源：http://jeb.zycfv.cn

[Q03] 增加列
来源：http://dzi.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qng.gaohongyu789.top

[Q04] 修改列类型
来源：http://blv.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cui.yonumen.top

[Q05] 重命名列
来源：http://mnq.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sfp.jqgfzy.top

[Q06] 删除列
来源：http://iqp.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://kzs.shanyushiyangtech.top

[Q07] 删除表
来源：http://xnc.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://vqi.tarul.cn

[Q08] 创建普通索引
来源：http://ytq.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dbr.hywenlv.cn

[Q09] 创建唯一索引
来源：http://qnn.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ege.smart0.xyz

[Q10] 插入单行
来源：http://iuv.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vhd.aizwys.cn

[Q11] 一次插入多行
来源：http://ruv.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wyu.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://tix.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://pft.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jcz.jqgfzy.top

[Q13] 忽略重复插入
来源：http://oar.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sts.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://yrl.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://koz.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ues.sjlbkw.cn

[Q15] 查询全部
来源：http://tga.xylfe.cn

SELECT * FROM users;
来源：http://lla.zhijiandao.cn

[Q16] 查询指定列
来源：http://noh.cheryme.top

SELECT id, name FROM users;
来源：http://jku.birdmap.top

[Q17] 条件查询
来源：http://hlg.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mnl.yongpay.top

[Q18] 模糊匹配
来源：http://axk.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wjd.gogol.net.cn

[Q19] 范围查询
来源：http://zde.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://enb.cheryme.top

[Q20] IN 列表
来源：http://slu.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qsm.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://unp.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aqk.fengsongda.top

[Q22] 排序
来源：http://afd.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vgr.yj20258.top

[Q23] 分页
来源：http://xiu.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hig.jyoumei.cn

[Q24] 去重
来源：http://vcw.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://zws.guannengcc.top

[Q25] 只取前 N 条
来源：http://edz.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wfa.jianghu66.top

[Q26] 计数
来源：http://jor.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://rjv.ivvv.top

[Q27] 条件计数
来源：http://lyq.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tng.bjfxy.top

[Q28] 求和与平均
来源：http://jlp.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wus.jlsjyb.cn

[Q29] 最大最小值
来源：http://hjh.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gqv.nwbrower.top

[Q30] 分组统计
来源：http://mzt.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yrw.cdnleiting.top

[Q31] 分组后过滤
来源：http://csr.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uuf.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://xfq.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dyg.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zkg.jinqigfzy.top

[Q33] 多列分组
来源：http://uwo.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ayh.jlsjyb.cn

[Q34] 每组取第一条
来源：http://liy.jqgfzy.top

SELECT * FROM (
来源：http://avv.smart0.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ubl.c1oappe.top

) t WHERE rn = 1;
来源：http://fsn.fengsongda.top

[Q35] 内连接
来源：http://uin.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wix.ctjpmb.com

[Q36] 左连接
来源：http://dpt.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jkd.gaohongyu789.top

[Q37] 右连接
来源：http://ryy.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://szx.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hom.dashuyun.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qku.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://wks.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jnh.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://btk.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rcu.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tgx.jlsjyb.cn

[Q41] 多表连接
来源：http://iph.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pux.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://kpc.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://xpy.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://pnw.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://kqc.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mlh.sysykeji.top

[Q43] 标量子查询
来源：http://wev.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rvj.jinqigfzy.top

[Q44] IN 子查询
来源：http://dcb.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kwu.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://ibf.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ybi.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://fdn.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gcq.dashuyun.cn

[Q47] 与平均值比较
来源：http://huh.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qnp.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://rai.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oyl.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://ast.cashguo.top

[Q49] 更新单行
来源：http://yzs.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nmy.ivvv.top

[Q50] 批量更新
来源：http://muq.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://unz.dianchejie.cn

[Q51] 用子查询更新
来源：http://yol.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pav.jinqigfzy.top

[Q52] 删除指定行
来源：http://azz.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://loe.wangdashe.top

[Q53] 按条件删除
来源：http://wku.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vgz.sysykeji.top

[Q54] 清空表
来源：http://jql.yvedp.cn

TRUNCATE TABLE logs;
来源：http://gkx.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://sfs.shanyushiyangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://quv.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://rkr.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hxm.shanyushiyangtech.top

[Q57] 行号
来源：http://ats.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yei.feifeiyinyue.top

[Q58] 累计求和
来源：http://pkx.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dwf.yonumen.top

[Q59] 分组内累计
来源：http://ows.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lhz.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://cfn.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yux.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://imi.jqgufenzy.top

[Q61] 移动平均
来源：http://vxt.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cdf.shuidangran.top

[Q62] 分组占比
来源：http://wuu.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tgo.yanxiufei.cn

[Q63] 开启事务
来源：http://air.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ytd.ppjwa.cn

[Q64] 提交事务
来源：http://lpq.nanxuanxn.top

COMMIT;
来源：http://dli.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://khs.jiagoushi.top

ROLLBACK;
来源：http://vxp.havefunace.top

[Q66] 行锁查询
来源：http://thm.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fht.hammf.cn

[Q67] 设置隔离级别
来源：http://fmh.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://btb.hywenlv.cn

[Q68] 保存点
来源：http://zky.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://rfh.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://fep.vehdjk.com

[Q69] 查看执行计划
来源：http://qkv.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ikd.tianlin.xyz

[Q70] 更新统计信息
来源：http://vdt.hywenlv.cn

ANALYZE TABLE users;
来源：http://eax.cheryme.top

[Q71] 查看建表语句
来源：http://gap.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ugm.yuxming.cn

[Q72] 查看索引
来源：http://sec.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://kgs.cucudq.cn

[Q73] 查看表状态
来源：http://qth.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://emy.fengsongda.top

[Q74] 强制使用索引
来源：http://svl.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdy.fzhhl.top

[Q75] 日期格式化
来源：http://kmc.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ueb.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mzv.yueranfly.top

[Q76] 按天统计
来源：http://ihl.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pmo.sysykeji.top

[Q77] 时间加减
来源：http://avv.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kba.fzhhl.top

[Q78] 当前时间
来源：http://nxl.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://any.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://yre.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cwa.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://zak.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yex.dianchejie.cn

[Q81] 字符串替换
来源：http://ium.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dos.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://xoi.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qpu.aibaodan.cn

[Q83] 大小写转换
来源：http://zmh.xylfe.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jnh.tianlin.xyz

[Q84] 去除首尾空格
来源：http://xcu.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://bjm.shuidangran.top

[Q85] 数值取整
来源：http://jnb.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aco.316326.xyz

[Q86] 读取 JSON 字段
来源：http://zbk.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://crx.wangdashe.top

[Q87] JSON 字段做条件
来源：http://iol.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jnt.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://djg.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hfo.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aqp.dashuyun.cn

[Q89] 判断表是否存在
来源：http://avs.fengsongda.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://diz.jqgufenzy.top

[Q90] 生成序号列
来源：http://msd.birdmap.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ark.smart0.xyz

================================================================================
来源：http://vox.dashuyun.cn

R. Bash 专题
来源：http://hcm.zhijiandao.cn

================================================================================
来源：http://xdx.dianchejie.cn

[R01] shebang 与严格模式
来源：http://jdh.tianlin.xyz

#!/usr/bin/env bash
来源：http://muh.zhiwuduotai.top

set -euo pipefail
来源：http://mzh.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://gjz.yj20258.top

name="Tom"; echo "$name"
来源：http://bma.wangdashe.top

[R03] 只读变量
来源：http://ntf.pengpengdd.cyou

readonly PI=3.14
来源：http://aax.316326.xyz

[R04] 位置参数
来源：http://arr.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvs.316326.xyz

[R05] 参数默认值
来源：http://meb.yueranfly.top

name="${1:-default}"
来源：http://skv.yongpay.top

[R06] 判断命令是否存在
来源：http://ktc.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ogr.zhoulong.xyz

[R07] if 判断文件
来源：http://bnx.daxiang520.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fcv.nanxuanxn.top

[R08] 数值比较
来源：http://rvz.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cwq.nanxinkj.top

[R09] 字符串比较
来源：http://zaq.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jxh.dianchejie.cn

[R10] 正则匹配
来源：http://gbd.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://epe.jinqigfzy.top

[R11] case 多分支
来源：http://dlw.fehbvm.com

case "$1" in
来源：http://mqo.feifeiyinyue.top

start) echo "启动" ;;
来源：http://qeg.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://dpy.hongshengwenyu.top

*)     echo "未知命令" ;;
来源：http://wmn.bbcook.cn

esac
来源：http://kzu.snrcjt.cn

[R12] for 遍历文件
来源：http://oml.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://ixl.zhiwuduotai.top

[R13] for 计数循环
来源：http://zaz.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://xlx.sufxvd.cn

[R14] C 风格 for
来源：http://hzl.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sfs.9152youxi.cn

[R15] while 逐行读文件
来源：http://qzu.snrcjt.cn


<!-- 参考信息 -->