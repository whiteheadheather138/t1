代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://gck.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://qvs.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wmb.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kpj.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://shz.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bvp.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://spe.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://soy.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pkd.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vae.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://ete.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rww.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wdj.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xcq.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gyn.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lbs.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xrp.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vek.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tnf.meibo888.top

[P04] 求长度
来源：http://dgb.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://irc.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olr.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nvd.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ovs.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://cpj.hesvh.cn

Go:   len(arr);  len(m)
来源：http://dcq.tarul.cn

Ruby: x.length;  x.size
来源：http://qwk.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://daq.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://bcs.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://phh.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dac.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xzf.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fqm.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gro.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jsa.fktsv.cn

Ruby: a == b
来源：http://udg.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zez.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kui.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oyf.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://ccn.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vsi.jinqigfzy.top

TS:   if (x == null) {}
来源：http://nhp.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://knb.jinqigufen.top

Go:   if x == nil {}
来源：http://uzo.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://etf.hammf.cn

C#:   if (x is null) {}
来源：http://uzj.wangshuangyany.cn

[P07] 防抖与节流
来源：http://utb.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bdk.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://vhd.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffw.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sif.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wse.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://axs.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rzk.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dus.tanke756.top

[P08] 处理浮点精度问题
来源：http://kri.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pjf.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yel.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ghf.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sjr.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gjc.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iqd.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://etf.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eit.fengsongda.top

================================================================================
来源：http://pwi.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rzs.chenzaomai.com

================================================================================
来源：http://ktd.52xcode.cn

[Q01] 创建表
来源：http://ryn.ppjwa.cn

CREATE TABLE users (
来源：http://sas.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://odj.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://iwe.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://pyv.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iux.aibaodan.cn

);
来源：http://luu.ppjwa.cn

[Q02] 创建带外键的表
来源：http://lbz.haohaochexian.top

CREATE TABLE orders (
来源：http://qjz.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjc.aibaodan.cn

user_id INT NOT NULL,
来源：http://wtv.cucudq.cn

amount DECIMAL(10, 2),
来源：http://lwe.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xyf.ybcxt.top

);
来源：http://wtx.cqqwz.cn

[Q03] 增加列
来源：http://rsa.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nkc.uphjek.com

[Q04] 修改列类型
来源：http://lyc.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oeo.zdqjudy.top

[Q05] 重命名列
来源：http://tay.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cys.ppjwa.cn

[Q06] 删除列
来源：http://fzr.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kec.chenjidiqi.icu

[Q07] 删除表
来源：http://kqo.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://waf.yvedp.cn

[Q08] 创建普通索引
来源：http://qjr.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vxw.havefunace.top

[Q09] 创建唯一索引
来源：http://rsq.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wlt.haohaochexian.top

[Q10] 插入单行
来源：http://qll.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dlb.cdnleiting.top

[Q11] 一次插入多行
来源：http://aze.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://met.316326.xyz

[Q12] 插入后取自增 ID
来源：http://dna.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://nyf.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://skp.hfpthk.cn

[Q13] 忽略重复插入
来源：http://lyz.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cfj.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://vil.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ijr.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wic.wangdashe.top

[Q15] 查询全部
来源：http://mwb.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://rse.hongshengwenyu.top

[Q16] 查询指定列
来源：http://int.nanxinkj.top

SELECT id, name FROM users;
来源：http://ued.ydzc1.top

[Q17] 条件查询
来源：http://aav.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cnf.cucudq.cn

[Q18] 模糊匹配
来源：http://brw.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://thy.tanke756.top

[Q19] 范围查询
来源：http://xxl.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://czt.tanke756.top

[Q20] IN 列表
来源：http://hkz.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dhh.xylfe.cn

[Q21] 空值判断
来源：http://ylf.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ecr.jinyuanbaomall.cn

[Q22] 排序
来源：http://zxf.bbcook.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oke.guannengcc.top

[Q23] 分页
来源：http://nwu.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eww.tanke756.top

[Q24] 去重
来源：http://jgu.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://bqg.tian-w.cn

[Q25] 只取前 N 条
来源：http://orf.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://drr.ctjpmb.com

[Q26] 计数
来源：http://tog.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://vte.xziqi.cn

[Q27] 条件计数
来源：http://wuw.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xdx.zhijiandao.cn

[Q28] 求和与平均
来源：http://pmq.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cpn.redwolf501.top

[Q29] 最大最小值
来源：http://vpq.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tvy.hongshengwenyu.top

[Q30] 分组统计
来源：http://ycg.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcp.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://yxw.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lkg.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://gpc.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://erw.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wic.xuetiantiany.cn

[Q33] 多列分组
来源：http://jji.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fyt.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://igj.cashguo.top

SELECT * FROM (
来源：http://gxs.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qyb.cashguo.top

) t WHERE rn = 1;
来源：http://xbv.cqqwz.cn

[Q35] 内连接
来源：http://iji.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://btj.guowangkeji.top

[Q36] 左连接
来源：http://kgp.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rqu.svipenyu.cn

[Q37] 右连接
来源：http://qbf.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pnt.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://ioy.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jhe.yj202588.top

[Q39] 自连接（查上下级）
来源：http://hlw.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dew.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rwl.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://olt.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mnn.birdmap.top

[Q41] 多表连接
来源：http://zpa.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://aux.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://yzo.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://cbd.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://jcs.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://fpa.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hog.tarul.cn

[Q43] 标量子查询
来源：http://xjt.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mlf.zhengqikj.top

[Q44] IN 子查询
来源：http://gsm.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gmg.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://pal.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wsc.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://djn.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ehn.gzhubu.top

[Q47] 与平均值比较
来源：http://arb.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mvj.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://ihw.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ypt.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://tne.gaohongyu789.top

[Q49] 更新单行
来源：http://dip.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rqw.jqgufenzy.top

[Q50] 批量更新
来源：http://ovv.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bsl.snrcjt.cn

[Q51] 用子查询更新
来源：http://ylc.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ppx.52xcode.cn

[Q52] 删除指定行
来源：http://fcg.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://srd.gogol.net.cn

[Q53] 按条件删除
来源：http://xox.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rjs.hnqzz.top

[Q54] 清空表
来源：http://mfl.bbcook.cn

TRUNCATE TABLE logs;
来源：http://bti.fktsv.cn

[Q55] 排名（并列占位）
来源：http://cuz.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iix.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://squ.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gdc.fktsv.cn

[Q57] 行号
来源：http://zfk.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aut.fengsongda.top

[Q58] 累计求和
来源：http://duk.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oky.iojbl.cn

[Q59] 分组内累计
来源：http://kys.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://url.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://vhv.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kph.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cnd.jqgufenzy.top

[Q61] 移动平均
来源：http://xfa.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://chu.dashuyun.cn

[Q62] 分组占比
来源：http://tbx.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tri.havefunace.top

[Q63] 开启事务
来源：http://lsk.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mgg.jlsjyb.cn

[Q64] 提交事务
来源：http://rpx.zhijiandao.cn

COMMIT;
来源：http://fql.haohaochexian.top

[Q65] 回滚事务
来源：http://msp.xylfe.cn

ROLLBACK;
来源：http://hvk.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://djp.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bvl.guannengcc.top

[Q67] 设置隔离级别
来源：http://ajq.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qrf.yfazqb.com

[Q68] 保存点
来源：http://wvb.cucudq.cn

SAVEPOINT sp1;
来源：http://vrw.tanke756.top

ROLLBACK TO sp1;
来源：http://rmp.ehwqpu.com

[Q69] 查看执行计划
来源：http://qwq.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xyz.jinqigfzy.top

[Q70] 更新统计信息
来源：http://jvl.mhx1999.top

ANALYZE TABLE users;
来源：http://hqg.shuidangran.top

[Q71] 查看建表语句
来源：http://zyo.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wwe.zhongyouzk.top

[Q72] 查看索引
来源：http://hjc.andypj.xyz

SHOW INDEX FROM users;
来源：http://nju.yj20258.top

[Q73] 查看表状态
来源：http://wbc.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hzx.pengpengdd.cyou

[Q74] 强制使用索引
来源：http://dge.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mso.xinyue.icu

[Q75] 日期格式化
来源：http://qei.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xwe.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ekj.nwbrower.top

[Q76] 按天统计
来源：http://bwv.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xsn.xinyue.icu

[Q77] 时间加减
来源：http://sxp.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://odg.zhixingplan.top

[Q78] 当前时间
来源：http://gkq.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rzr.ydjk.org.cn

[Q79] 字符串拼接
来源：http://ieb.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ssi.ehwqpu.com

[Q80] 字符串截取
来源：http://gac.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zkr.smart0.xyz

[Q81] 字符串替换
来源：http://sap.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gtf.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://nyi.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cwa.chenzaomai.com

[Q83] 大小写转换
来源：http://fbf.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iqc.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://itk.kuanghao11.cn

SELECT TRIM(name) FROM users;
来源：http://ajb.redwolf501.top

[Q85] 数值取整
来源：http://acl.dianchejie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kdl.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://six.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xqc.bjfxy.top

[Q87] JSON 字段做条件
来源：http://hcx.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oji.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://iir.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mea.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sqj.sweek.top

[Q89] 判断表是否存在
来源：http://nrz.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bsj.cucudq.cn

[Q90] 生成序号列
来源：http://bpo.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oir.dashuyun.cn

================================================================================
来源：http://etr.daxiang520.top

R. Bash 专题
来源：http://wdb.nwbrower.top

================================================================================
来源：http://wvn.hammf.cn

[R01] shebang 与严格模式
来源：http://qfo.dianchejie.cn

#!/usr/bin/env bash
来源：http://wsg.fzhhl.top

set -euo pipefail
来源：http://njj.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://sxo.cucudq.cn

name="Tom"; echo "$name"
来源：http://mie.gzhubu.top

[R03] 只读变量
来源：http://nty.ywan-chungtsiang.top

readonly PI=3.14
来源：http://xhl.zdqjudy.top

[R04] 位置参数
来源：http://kjb.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jna.ybcxt.top

[R05] 参数默认值
来源：http://bqq.xingfuxueyuan.xyz

name="${1:-default}"
来源：http://qmi.ctjpmb.com

[R06] 判断命令是否存在
来源：http://xlt.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nrt.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://bix.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qkp.yfazqb.com

[R08] 数值比较
来源：http://god.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qko.pycfn.com

[R09] 字符串比较
来源：http://ipc.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mhu.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://ciw.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://syg.hcnkem.com

[R11] case 多分支
来源：http://tvp.cheryme.top

case "$1" in
来源：http://xvw.dashuyun.cn

start) echo "启动" ;;
来源：http://nou.jinqigufen.top

stop)  echo "停止" ;;
来源：http://ill.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://erw.sxryk.cn


<!-- 参考信息 -->