代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://njk.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://phb.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vzj.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xlf.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mbx.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gqi.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ebv.yuxming.cn

[P04] 求长度
来源：http://vcm.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://har.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tkx.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qbd.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fdq.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://rew.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://wed.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://vrm.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cac.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://cbo.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ajr.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://btj.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oje.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://omm.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sjl.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://mxs.cheryme.top

Ruby: a == b
来源：http://cbr.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qth.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qhu.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://deo.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://oqy.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wkn.daria6918.cn

TS:   if (x == null) {}
来源：http://qeu.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qps.ydzc1.top

Go:   if x == nil {}
来源：http://hke.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qke.daxiang520.top

C#:   if (x is null) {}
来源：http://qog.zdqjudy.top

[P07] 防抖与节流
来源：http://nhm.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://evx.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://szy.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ynk.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ctx.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://omu.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qas.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://sez.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rhj.52xcode.cn

[P08] 处理浮点精度问题
来源：http://xxw.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bdy.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dno.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqz.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://asa.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mbe.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jqo.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oku.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rcw.9152youxi.cn

================================================================================
来源：http://lrd.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cvd.ehwqpu.com

================================================================================
来源：http://qyh.cucudq.cn

[Q01] 创建表
来源：http://uhd.fengsongda.top

CREATE TABLE users (
来源：http://xhm.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zzv.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://irb.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://fmf.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qgc.feifeiyinyue.top

);
来源：http://qjd.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://smz.snrcjt.cn

CREATE TABLE orders (
来源：http://fhz.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkf.yueranfly.top

user_id INT NOT NULL,
来源：http://ikp.daria6918.cn

amount DECIMAL(10, 2),
来源：http://ick.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kul.0kj1m.cn

);
来源：http://mls.zhiwuduotai.top

[Q03] 增加列
来源：http://dff.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gjz.ybcxt.top

[Q04] 修改列类型
来源：http://mqn.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://crs.jqgfzy.top

[Q05] 重命名列
来源：http://ykt.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://svd.gaohongyu789.top

[Q06] 删除列
来源：http://bpb.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://sqi.chenlongwang.top

[Q07] 删除表
来源：http://vfr.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://kaj.jinqigufen.top

[Q08] 创建普通索引
来源：http://rpw.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nxq.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://ykt.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kpe.ctjpmb.com

[Q10] 插入单行
来源：http://apw.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nyd.jqgufenzy.top

[Q11] 一次插入多行
来源：http://nij.bjfxy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jez.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://tni.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ckb.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lks.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://pye.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oye.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://zvm.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uer.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wzm.nanxinkj.top

[Q15] 查询全部
来源：http://emn.chenzaomai.com

SELECT * FROM users;
来源：http://axt.zhongyouzk.top

[Q16] 查询指定列
来源：http://gqi.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://uft.yanxiufei.cn

[Q17] 条件查询
来源：http://ewe.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fps.cheryme.top

[Q18] 模糊匹配
来源：http://tjc.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bzv.gzhubu.top

[Q19] 范围查询
来源：http://pyo.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oeo.jiagoushi.top

[Q20] IN 列表
来源：http://lah.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ljf.nanxuanxn.top

[Q21] 空值判断
来源：http://mdh.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://mqn.xylfe.cn

[Q22] 排序
来源：http://azv.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nxn.52xcode.cn

[Q23] 分页
来源：http://fxs.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://juy.bjfxy.top

[Q24] 去重
来源：http://nbz.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://ozy.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://sdo.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qll.yonumen.top

[Q26] 计数
来源：http://ykj.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://eou.wangdashe.top

[Q27] 条件计数
来源：http://rzu.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gea.hongshengwenyu.top

[Q28] 求和与平均
来源：http://hbk.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://stj.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://bkk.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ghu.tanke756.top

[Q30] 分组统计
来源：http://anw.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qbj.tian-w.cn

[Q31] 分组后过滤
来源：http://uhy.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kqm.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://uvo.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mfb.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gjc.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://mwh.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://syd.hcnkem.com

[Q34] 每组取第一条
来源：http://cub.jlsjyb.cn

SELECT * FROM (
来源：http://ffw.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wfv.hfpthk.cn

) t WHERE rn = 1;
来源：http://dfi.meibo888.top

[Q35] 内连接
来源：http://kbe.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://acj.wangdashe.top

[Q36] 左连接
来源：http://jnv.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tsz.ydzc1.top

[Q37] 右连接
来源：http://rag.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://czm.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fjc.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hrv.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://wvz.hfpthk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zgq.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kyd.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wns.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zuw.jianghu66.top

[Q41] 多表连接
来源：http://phm.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://dek.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://utg.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://qee.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://smb.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://wxn.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zcq.xinyue.icu

[Q43] 标量子查询
来源：http://tjo.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lxr.dashuyun.cn

[Q44] IN 子查询
来源：http://psz.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xkh.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://ugx.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xkx.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://uqz.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ndt.iojbl.cn

[Q47] 与平均值比较
来源：http://roi.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ykt.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://dcj.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vky.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://mjl.xylfe.cn

[Q49] 更新单行
来源：http://fzl.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fye.gotoacloud.top

[Q50] 批量更新
来源：http://qwy.xingfuxueyuan.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eqf.jinqigufen.top

[Q51] 用子查询更新
来源：http://fcv.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vpn.jqgufenzy.top

[Q52] 删除指定行
来源：http://nnd.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://muu.yvedp.cn

[Q53] 按条件删除
来源：http://asf.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qde.yj20258.top

[Q54] 清空表
来源：http://kuo.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://bvf.yuxming.cn

[Q55] 排名（并列占位）
来源：http://pxk.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kxs.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://dlh.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bmy.tian-w.cn

[Q57] 行号
来源：http://zbs.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vfv.dashuyun.cn

[Q58] 累计求和
来源：http://kvl.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ffl.hesvh.cn

[Q59] 分组内累计
来源：http://afu.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vxe.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://mfc.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cmk.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fuy.jyoumei.cn

[Q61] 移动平均
来源：http://qik.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vop.shzxlz.cn

[Q62] 分组占比
来源：http://aoz.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wmn.iojbl.cn

[Q63] 开启事务
来源：http://mvw.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zqp.xinyue.icu

[Q64] 提交事务
来源：http://zlg.havefunace.top

COMMIT;
来源：http://cht.shzxlz.cn

[Q65] 回滚事务
来源：http://skg.yanxiufei.cn

ROLLBACK;
来源：http://fvw.aibaodan.cn

[Q66] 行锁查询
来源：http://llt.zdqjudy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://srp.yj202588.top

[Q67] 设置隔离级别
来源：http://cfj.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qku.9152youxi.cn

[Q68] 保存点
来源：http://paj.hammf.cn

SAVEPOINT sp1;
来源：http://pnm.hysaishi.cn

ROLLBACK TO sp1;
来源：http://xqj.fengsongda.top

[Q69] 查看执行计划
来源：http://mpq.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mgi.haohaochexian.top

[Q70] 更新统计信息
来源：http://mfq.dianchejie.cn

ANALYZE TABLE users;
来源：http://mbe.haohaochexian.top

[Q71] 查看建表语句
来源：http://sjs.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vhf.ydjk.org.cn

[Q72] 查看索引
来源：http://gvp.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://gpp.andypj.xyz

[Q73] 查看表状态
来源：http://nlk.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://hch.zdqjudy.top

[Q74] 强制使用索引
来源：http://fdx.aizwys.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vrh.yongpay.top

[Q75] 日期格式化
来源：http://zpk.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nrp.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eiu.xinyue.icu

[Q76] 按天统计
来源：http://xyx.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://coi.xuanzx.com

[Q77] 时间加减
来源：http://kxw.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kcy.cqqwz.cn

[Q78] 当前时间
来源：http://qja.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xtj.tarul.cn

[Q79] 字符串拼接
来源：http://kqg.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sql.yj20258888.top

[Q80] 字符串截取
来源：http://hhh.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ton.xinyue.icu

[Q81] 字符串替换
来源：http://hlg.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jpf.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://hlg.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jot.ppjwa.cn

[Q83] 大小写转换
来源：http://qpo.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dvh.cdnleiting.top

[Q84] 去除首尾空格
来源：http://ldc.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://vds.jiagoushi.top

[Q85] 数值取整
来源：http://ztj.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vxc.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://arn.aibaodan.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://avw.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://jjl.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gzb.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://ukr.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xqh.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vyb.yvedp.cn

[Q89] 判断表是否存在
来源：http://rjn.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oan.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://vut.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uwr.nanxuanxn.top

================================================================================
来源：http://hbx.zhijiandao.cn

R. Bash 专题
来源：http://flf.gzhubu.top

================================================================================
来源：http://crl.guannengcc.top

[R01] shebang 与严格模式
来源：http://dak.nanxinkj.top

#!/usr/bin/env bash
来源：http://rzs.jinqigfzy.top

set -euo pipefail
来源：http://hru.aizwys.cn

[R02] 变量赋值与使用
来源：http://kfx.jinqigufen.top

name="Tom"; echo "$name"
来源：http://ncx.shzxlz.cn

[R03] 只读变量
来源：http://syi.epnwcf.com

readonly PI=3.14
来源：http://reu.cucudq.cn

[R04] 位置参数
来源：http://fco.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://who.guannengcc.top

[R05] 参数默认值
来源：http://cgo.ehwqpu.com

name="${1:-default}"
来源：http://emu.cdnleiting.top

[R06] 判断命令是否存在
来源：http://ftd.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jgk.dashuyun.cn

[R07] if 判断文件
来源：http://vdz.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jnm.hongshengwenyu.top

[R08] 数值比较
来源：http://ndw.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://btw.xuetiantiany.cn

[R09] 字符串比较
来源：http://taq.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://agp.nanxinkj.top

[R10] 正则匹配
来源：http://bsz.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iqd.sjlbkw.cn

[R11] case 多分支
来源：http://phe.sysykeji.top

case "$1" in
来源：http://eio.xuanzx.com

start) echo "启动" ;;
来源：http://zyf.chenzaomai.com

stop)  echo "停止" ;;
来源：http://wlw.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://mih.chenzaomai.com

esac
来源：http://kbk.yongpay.top

[R12] for 遍历文件
来源：http://hlp.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://hlp.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://hfa.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ess.jlsjyb.cn

[R14] C 风格 for
来源：http://iru.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://utk.ybcxt.top

[R15] while 逐行读文件
来源：http://xwi.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nwf.gaohongyu789.top

[R16] until 等待条件
来源：http://afn.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qcy.iojbl.cn

[R17] 数组定义与取值
来源：http://uam.jinghuilouyu.cn


<!-- 参考信息 -->