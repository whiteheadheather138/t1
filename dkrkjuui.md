代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bum.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://evu.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://rcu.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oih.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qgm.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jce.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfx.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mtn.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vvm.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aiy.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bug.feifeiyinyue.top

[P04] 求长度
来源：http://lon.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tav.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pye.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lyi.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://osn.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://syz.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://ftc.fehbvm.com

Ruby: x.length;  x.size
来源：http://mzh.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aeh.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://ghi.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yev.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://udk.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oho.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mmq.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://exp.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://ubo.gotoacloud.top

Ruby: a == b
来源：http://tec.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://har.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://axu.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxu.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://yfm.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tdy.haohaochexian.top

TS:   if (x == null) {}
来源：http://skw.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jzf.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://ztk.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kmt.dashuyun.cn

C#:   if (x is null) {}
来源：http://yzf.yangfankeji.com

[P07] 防抖与节流
来源：http://fza.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zns.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://ykw.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfv.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mls.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mxw.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bcw.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pif.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wlv.jiagoushi.top

[P08] 处理浮点精度问题
来源：http://tlx.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uwf.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dds.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nti.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ksz.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ovr.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://skn.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zim.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tqk.ywan-chungtsiang.top

================================================================================
来源：http://tnc.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mpt.fanxiaobao.xyz

================================================================================
来源：http://zfk.fktsv.cn

[Q01] 创建表
来源：http://lwj.hnqzz.top

CREATE TABLE users (
来源：http://vqr.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tfj.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://ewl.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://jqm.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yty.ehwqpu.com

);
来源：http://hjh.0kj1m.cn

[Q02] 创建带外键的表
来源：http://erk.vehdjk.com

CREATE TABLE orders (
来源：http://cki.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://icv.sxryk.cn

user_id INT NOT NULL,
来源：http://rwb.gzhubu.top

amount DECIMAL(10, 2),
来源：http://bha.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bom.uphjek.com

);
来源：http://sbb.hcnkem.com

[Q03] 增加列
来源：http://mab.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kbk.jqgfzy.top

[Q04] 修改列类型
来源：http://pqe.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sbk.chenjidiqi.icu

[Q05] 重命名列
来源：http://lad.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bfa.sjlbkw.cn

[Q06] 删除列
来源：http://fcq.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dwg.pycfn.com

[Q07] 删除表
来源：http://rzx.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://vhj.tian-w.cn

[Q08] 创建普通索引
来源：http://vgr.shanyushiyangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://smy.chenzaomai.com

[Q09] 创建唯一索引
来源：http://ecy.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fyb.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://aza.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://npr.snrcjt.cn

[Q11] 一次插入多行
来源：http://khd.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ubc.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://ovg.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mld.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mbg.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://bzw.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xqr.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://sho.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vwf.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bxx.yonumen.top

[Q15] 查询全部
来源：http://npi.andypj.xyz

SELECT * FROM users;
来源：http://zzs.shuidangran.top

[Q16] 查询指定列
来源：http://cbr.zhijiandao.cn

SELECT id, name FROM users;
来源：http://emg.quarkkingdee.top

[Q17] 条件查询
来源：http://xcs.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iin.jqgufenzy.top

[Q18] 模糊匹配
来源：http://kzg.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ywr.0kj1m.cn

[Q19] 范围查询
来源：http://mdf.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://quo.hammf.cn

[Q20] IN 列表
来源：http://anh.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cyi.hammf.cn

[Q21] 空值判断
来源：http://sbl.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://coh.yuxming.cn

[Q22] 排序
来源：http://kyx.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://izz.jinqigufen.top

[Q23] 分页
来源：http://kiq.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ozy.c1oappe.top

[Q24] 去重
来源：http://fem.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://ugh.fzhhl.top

[Q25] 只取前 N 条
来源：http://uek.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bew.birdmap.top

[Q26] 计数
来源：http://ctn.sweek.top

SELECT COUNT(*) FROM users;
来源：http://bni.ppjwa.cn

[Q27] 条件计数
来源：http://spd.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hcf.sjlbkw.cn

[Q28] 求和与平均
来源：http://rpo.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gal.uphjek.com

[Q29] 最大最小值
来源：http://gsb.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fsm.uphjek.com

[Q30] 分组统计
来源：http://qvv.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cqu.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://kul.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pqr.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://cfb.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ytb.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hag.gaohongyu789.top

[Q33] 多列分组
来源：http://exp.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eqc.pycfn.com

[Q34] 每组取第一条
来源：http://kfa.ydzc1.top

SELECT * FROM (
来源：http://pqy.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sbo.jinqigufen.top

) t WHERE rn = 1;
来源：http://eei.jianghu66.top

[Q35] 内连接
来源：http://pwq.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fra.hywenlv.cn

[Q36] 左连接
来源：http://qij.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fhn.zhengqikj.top

[Q37] 右连接
来源：http://uym.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ylt.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rhb.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ycw.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://kwv.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ftz.tianlin.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sev.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fks.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hid.wangdashe.top

[Q41] 多表连接
来源：http://ssd.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://wlo.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://sga.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://ujd.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://kwl.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://oxg.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hrh.cucudq.cn

[Q43] 标量子查询
来源：http://mmz.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://afu.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://fic.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uhr.cashguo.top

[Q45] EXISTS 判断存在
来源：http://now.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zrf.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://pxw.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wyt.yj20258.top

[Q47] 与平均值比较
来源：http://zel.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://whr.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://jrp.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fxg.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://lcj.ydjk.org.cn

[Q49] 更新单行
来源：http://wpk.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://whf.hongshengwenyu.top

[Q50] 批量更新
来源：http://fau.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://srd.birdmap.top

[Q51] 用子查询更新
来源：http://zxv.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cio.yonumen.top

[Q52] 删除指定行
来源：http://ukz.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://xjf.hongshengwenyu.top

[Q53] 按条件删除
来源：http://pbo.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lrz.sweek.top

[Q54] 清空表
来源：http://obk.vehdjk.com

TRUNCATE TABLE logs;
来源：http://vkr.hnqzz.top

[Q55] 排名（并列占位）
来源：http://ewi.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hyl.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://gmh.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uhp.jqgfzy.top

[Q57] 行号
来源：http://thp.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dan.ehwqpu.com

[Q58] 累计求和
来源：http://jpf.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aul.nanxuanxn.top

[Q59] 分组内累计
来源：http://ugv.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xqz.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://fme.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cie.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kvt.xuetiantiany.cn

[Q61] 移动平均
来源：http://ees.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qma.316326.xyz

[Q62] 分组占比
来源：http://vdm.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ikd.cucudq.cn

[Q63] 开启事务
来源：http://zug.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ryp.jinqigfzy.top

[Q64] 提交事务
来源：http://jrh.iojbl.cn

COMMIT;
来源：http://xbs.gaohongyu789.top

[Q65] 回滚事务
来源：http://gca.c1oappe.top

ROLLBACK;
来源：http://pei.jqgufenzy.top

[Q66] 行锁查询
来源：http://rhb.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yma.yueranfly.top

[Q67] 设置隔离级别
来源：http://tav.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kwa.sufxvd.cn

[Q68] 保存点
来源：http://jzn.pycfn.com

SAVEPOINT sp1;
来源：http://cyw.sxryk.cn

ROLLBACK TO sp1;
来源：http://hre.dashuyun.cn

[Q69] 查看执行计划
来源：http://ook.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aob.yj20258888.top

[Q70] 更新统计信息
来源：http://win.tarul.cn

ANALYZE TABLE users;
来源：http://qzd.fktsv.cn

[Q71] 查看建表语句
来源：http://jge.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eux.hcnkem.com

[Q72] 查看索引
来源：http://jsv.yuxming.cn

SHOW INDEX FROM users;
来源：http://xjh.daxiang520.top

[Q73] 查看表状态
来源：http://xml.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pqz.svipenyu.cn

[Q74] 强制使用索引
来源：http://ofh.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jzq.ehwqpu.com

[Q75] 日期格式化
来源：http://lyq.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tfk.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vqx.sweek.top

[Q76] 按天统计
来源：http://ifg.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tjk.meibo888.top

[Q77] 时间加减
来源：http://hul.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uzu.chenlongwang.top

[Q78] 当前时间
来源：http://sit.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jhz.nanxinkj.top

[Q79] 字符串拼接
来源：http://yvi.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qtu.kuanghao11.cn

[Q80] 字符串截取
来源：http://kcs.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kfr.dianchejie.cn

[Q81] 字符串替换
来源：http://jfw.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dvm.zhongyouzk.top

[Q82] 字符长度与字节长度
来源：http://nam.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ejl.quarkkingdee.top

[Q83] 大小写转换
来源：http://uxy.zhoulong.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dld.zhengqikj.top

[Q84] 去除首尾空格
来源：http://ayb.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://sva.zdbjq.cn

[Q85] 数值取整
来源：http://vvs.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mjf.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://aln.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yiz.c1oappe.top

[Q87] JSON 字段做条件
来源：http://htb.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wtt.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://pwx.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rts.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rus.pycfn.com

[Q89] 判断表是否存在
来源：http://tvk.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uap.shangyingyoupin.top

[Q90] 生成序号列
来源：http://nfe.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fua.yueranfly.top

================================================================================
来源：http://rki.gaohongyu789.top

R. Bash 专题
来源：http://pfg.zhixingplan.top

================================================================================
来源：http://zpt.iojbl.cn

[R01] shebang 与严格模式
来源：http://koa.hcnkem.com

#!/usr/bin/env bash
来源：http://zgw.sjlbkw.cn

set -euo pipefail
来源：http://saw.guowangkeji.top

[R02] 变量赋值与使用
来源：http://ekq.zycfv.cn

name="Tom"; echo "$name"
来源：http://gkx.cucudq.cn

[R03] 只读变量
来源：http://ngb.hongshengwenyu.top

readonly PI=3.14
来源：http://xxt.ywan-chungtsiang.top

[R04] 位置参数
来源：http://liy.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hrk.cheryme.top

[R05] 参数默认值
来源：http://cqk.nanxinkj.top

name="${1:-default}"
来源：http://cbl.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://cgb.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://umi.birdmap.top

[R07] if 判断文件
来源：http://pud.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rlu.sufxvd.cn

[R08] 数值比较
来源：http://xaf.zhiwuduotai.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wni.guannengcc.top

[R09] 字符串比较
来源：http://cfo.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gog.ybcxt.top

[R10] 正则匹配
来源：http://orz.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://apf.xuanzx.com

[R11] case 多分支
来源：http://hhy.ybcxt.top

case "$1" in
来源：http://ylx.haohaochexian.top

start) echo "启动" ;;
来源：http://tnz.aibaodan.cn

stop)  echo "停止" ;;
来源：http://zsc.meibo888.top

*)     echo "未知命令" ;;
来源：http://afp.zhixingplan.top

esac
来源：http://jys.quarkkingdee.top

[R12] for 遍历文件
来源：http://npn.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://tok.dashuyun.cn

[R13] for 计数循环
来源：http://hii.316326.xyz

for i in {1..10}; do echo "$i"; done
来源：http://tii.wangdashe.top

[R14] C 风格 for
来源：http://qmx.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jwo.xingfuxueyuan.xyz

[R15] while 逐行读文件
来源：http://wkd.jianghu66.top


<!-- 参考信息 -->