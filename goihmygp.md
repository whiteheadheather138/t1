代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://aft.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://gdu.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rjz.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxl.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kif.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://elx.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rhq.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ogy.yj20258888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ojp.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mil.yuanzhike.top

[P03] 生成短随机字符串
来源：http://jqy.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iey.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fue.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqz.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dkd.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jrj.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qdu.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://fsr.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ice.shanyushiyangtech.top

[P04] 求长度
来源：http://uen.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kjy.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lfl.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jwo.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://skt.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://jkk.zycfv.cn

Go:   len(arr);  len(m)
来源：http://kyb.yonumen.top

Ruby: x.length;  x.size
来源：http://bhn.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wmm.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://qwj.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wai.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qfy.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://exf.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mmr.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pzq.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cvj.guannengcc.top

Ruby: a == b
来源：http://twg.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rxp.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uod.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://khg.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://lui.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wkn.nanxuanxn.top

TS:   if (x == null) {}
来源：http://tcj.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://php.shzxlz.cn

Go:   if x == nil {}
来源：http://pur.hysaishi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pzl.aibaodan.cn

C#:   if (x is null) {}
来源：http://nql.cqqwz.cn

[P07] 防抖与节流
来源：http://tsz.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vwi.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://hyc.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sgq.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qmp.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wkj.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ett.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rvd.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dgd.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://fzi.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jez.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vim.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kte.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pqk.sxryk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bms.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uhk.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qjc.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://etm.gaohongyu789.top

================================================================================
来源：http://elq.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vuj.hywenlv.cn

================================================================================
来源：http://nat.yj20258888.top

[Q01] 创建表
来源：http://olg.zhixingplan.top

CREATE TABLE users (
来源：http://ezw.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wju.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://ymj.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://xki.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ttx.gotoacloud.top

);
来源：http://zsm.redwolf501.top

[Q02] 创建带外键的表
来源：http://wnx.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://jez.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jms.jinqigufen.top

user_id INT NOT NULL,
来源：http://qcu.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://pqd.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qia.hammf.cn

);
来源：http://qcq.dashuyun.cn

[Q03] 增加列
来源：http://wdh.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tjk.uphjek.com

[Q04] 修改列类型
来源：http://nmb.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pha.jianghu66.top

[Q05] 重命名列
来源：http://ssg.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqp.redwolf501.top

[Q06] 删除列
来源：http://ytk.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://kfk.hfpthk.cn

[Q07] 删除表
来源：http://gwk.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://gwk.pycfn.com

[Q08] 创建普通索引
来源：http://wkg.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jyv.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://rsn.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://krk.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://zry.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ahm.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://oym.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hcz.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://mwb.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://rvb.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://npf.andypj.xyz

[Q13] 忽略重复插入
来源：http://xpf.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ehi.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://brl.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xxb.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qeq.jiagoushi.top

[Q15] 查询全部
来源：http://fks.tarul.cn

SELECT * FROM users;
来源：http://ufk.dianchejie.cn

[Q16] 查询指定列
来源：http://nfu.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://ylh.dianchejie.cn

[Q17] 条件查询
来源：http://afl.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uji.jinqigufen.top

[Q18] 模糊匹配
来源：http://vku.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://izz.zycfv.cn

[Q19] 范围查询
来源：http://vhv.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://coc.ehwqpu.com

[Q20] IN 列表
来源：http://uuv.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mhm.wangshuangyany.cn

[Q21] 空值判断
来源：http://dur.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ylp.chenlongwang.top

[Q22] 排序
来源：http://gdx.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cym.jyoumei.cn

[Q23] 分页
来源：http://edk.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wra.yfazqb.com

[Q24] 去重
来源：http://zgp.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://jkr.snrcjt.cn

[Q25] 只取前 N 条
来源：http://axy.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xqo.quarkkingdee.top

[Q26] 计数
来源：http://cir.yj20258888.top

SELECT COUNT(*) FROM users;
来源：http://tmq.jiagoushi.top

[Q27] 条件计数
来源：http://tqr.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nyg.yj202588.top

[Q28] 求和与平均
来源：http://smm.bjfxy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sqr.xinyue.icu

[Q29] 最大最小值
来源：http://lqk.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ycm.fzhhl.top

[Q30] 分组统计
来源：http://cdb.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tqz.gzhubu.top

[Q31] 分组后过滤
来源：http://smr.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yuv.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://tgy.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nql.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blp.sysykeji.top

[Q33] 多列分组
来源：http://tez.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rrg.smart0.xyz

[Q34] 每组取第一条
来源：http://kgg.ctjpmb.com

SELECT * FROM (
来源：http://ynq.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yup.yuxming.cn

) t WHERE rn = 1;
来源：http://kog.jinqigufen.top

[Q35] 内连接
来源：http://jha.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gxn.iojbl.cn

[Q36] 左连接
来源：http://yhw.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://asr.yongpay.top

[Q37] 右连接
来源：http://dst.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hdm.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://hia.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cej.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://ydd.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ydo.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mcn.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ncq.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kro.hywenlv.cn

[Q41] 多表连接
来源：http://pbl.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zvk.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://gby.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://gxj.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://ecd.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://hdd.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bha.shzxlz.cn

[Q43] 标量子查询
来源：http://nhw.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://anx.vehdjk.com

[Q44] IN 子查询
来源：http://uqn.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bbx.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://agg.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zyj.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gfo.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uqs.svipenyu.cn

[Q47] 与平均值比较
来源：http://crq.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eqx.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://vxu.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hqu.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://lbd.fengsongda.top

[Q49] 更新单行
来源：http://gne.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cgb.hongshengwenyu.top

[Q50] 批量更新
来源：http://ffl.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://egm.tarul.cn

[Q51] 用子查询更新
来源：http://mhq.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dgg.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://jza.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://lyq.hywenlv.cn

[Q53] 按条件删除
来源：http://nqq.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mrq.shzxlz.cn

[Q54] 清空表
来源：http://bnh.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://idv.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://czi.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rnj.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://gqs.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pml.xylfe.cn

[Q57] 行号
来源：http://lge.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zvo.zhixingplan.top

[Q58] 累计求和
来源：http://hrq.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dbq.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://dqi.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://isa.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://xpb.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ocr.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dcg.yongpay.top

[Q61] 移动平均
来源：http://jya.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yuh.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://sug.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oqr.jianghu66.top

[Q63] 开启事务
来源：http://fan.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://umx.xziqi.cn

[Q64] 提交事务
来源：http://uze.jinyuanbaomall.cn

COMMIT;
来源：http://sic.316326.xyz

[Q65] 回滚事务
来源：http://gnw.zycfv.cn

ROLLBACK;
来源：http://wgq.kuanghao11.cn

[Q66] 行锁查询
来源：http://gjl.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dnr.jqgfzy.top

[Q67] 设置隔离级别
来源：http://fuv.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evv.hammf.cn

[Q68] 保存点
来源：http://wbj.shzxlz.cn

SAVEPOINT sp1;
来源：http://awy.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://rao.pycfn.com

[Q69] 查看执行计划
来源：http://jov.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qpf.tanke756.top

[Q70] 更新统计信息
来源：http://sud.dianchejie.cn

ANALYZE TABLE users;
来源：http://vvt.fzhhl.top

[Q71] 查看建表语句
来源：http://rwy.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fsh.0kj1m.cn

[Q72] 查看索引
来源：http://nnd.aizwys.cn

SHOW INDEX FROM users;
来源：http://zlp.zhoulong.xyz

[Q73] 查看表状态
来源：http://lof.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fee.shuidangran.top

[Q74] 强制使用索引
来源：http://ifm.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ocy.yj20258.top

[Q75] 日期格式化
来源：http://mda.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://thh.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tva.ivvv.top

[Q76] 按天统计
来源：http://vdu.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxa.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://wcc.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ivf.shanyushiyangtech.top

[Q78] 当前时间
来源：http://maa.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://chh.hcnkem.com

[Q79] 字符串拼接
来源：http://gso.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qsq.kuanghao11.cn

[Q80] 字符串截取
来源：http://fcw.52xcode.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ldu.zdqjudy.top

[Q81] 字符串替换
来源：http://fkp.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ker.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://ygu.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://apy.hfpthk.cn

[Q83] 大小写转换
来源：http://ini.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mst.gogol.net.cn

[Q84] 去除首尾空格
来源：http://dvp.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://ilh.chenlongwang.top

[Q85] 数值取整
来源：http://pdh.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gsv.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://ode.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oeg.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://vwh.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ljv.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://tgm.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cyq.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bvu.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://ocq.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tme.fengsongda.top

[Q90] 生成序号列
来源：http://oid.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dpy.zdbjq.cn

================================================================================
来源：http://iib.yfazqb.com

R. Bash 专题
来源：http://mqt.ctjpmb.com

================================================================================
来源：http://imx.sxryk.cn

[R01] shebang 与严格模式
来源：http://imq.yangfankeji.com

#!/usr/bin/env bash
来源：http://hew.zhijiandao.cn

set -euo pipefail
来源：http://muo.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://yju.bjfxy.top

name="Tom"; echo "$name"
来源：http://uuw.hywenlv.cn

[R03] 只读变量
来源：http://yas.jianghu66.top

readonly PI=3.14
来源：http://aut.jiagoushi.top

[R04] 位置参数
来源：http://iam.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cbm.chenzaomai.com

[R05] 参数默认值
来源：http://pin.jqgfzy.top

name="${1:-default}"
来源：http://fwg.xylfe.cn

[R06] 判断命令是否存在
来源：http://yfe.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aeb.cdnleiting.top

[R07] if 判断文件
来源：http://kvs.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fwq.fanxiaobao.xyz

[R08] 数值比较
来源：http://nvo.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qcd.shangyingyoupin.top

[R09] 字符串比较
来源：http://pnl.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jtt.hfpthk.cn

[R10] 正则匹配
来源：http://ifn.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bzl.ctjpmb.com

[R11] case 多分支
来源：http://zyh.shanyushiyangkeji.top

case "$1" in
来源：http://fzo.9152youxi.cn

start) echo "启动" ;;
来源：http://kwv.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://rgn.yonumen.top

*)     echo "未知命令" ;;
来源：http://vma.xziqi.cn


<!-- 参考信息 -->