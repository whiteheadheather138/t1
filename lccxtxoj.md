代发 wailian999

C#:   Parallel.For
来源：http://ysz.zhixingplan.top

================================================================================
来源：http://wzo.yuanzhike.top

P. 常用工具函数
来源：http://uwf.hywenlv.cn

================================================================================
来源：http://elr.xuetiantiany.cn

[P01] 生成 UUID
来源：http://izz.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://jft.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gae.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://omh.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://ikd.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://bxo.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://zcm.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://wcx.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://nqk.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://uvj.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dvt.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://feb.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vla.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yfj.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://szn.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iyb.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wnu.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gbj.chenzaomai.com

[P03] 生成短随机字符串
来源：http://ddc.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mdh.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fmb.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://exj.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wrd.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xua.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ezu.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wba.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xlu.xuetiantiany.cn

[P04] 求长度
来源：http://pye.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://txt.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nkd.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shz.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wdz.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://htg.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://ebi.fzhhl.top

Ruby: x.length;  x.size
来源：http://yuk.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rkk.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://twy.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oir.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vil.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kei.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qas.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qvu.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xdh.c1oappe.top

Ruby: a == b
来源：http://cml.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kim.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nkc.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dva.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://pjy.gogol.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bqk.c1oappe.top

TS:   if (x == null) {}
来源：http://yiy.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hdo.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://jlp.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jxx.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://ehj.jyoumei.cn

[P07] 防抖与节流
来源：http://oei.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rtv.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://jbl.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://amz.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dia.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ivp.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://frz.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mpv.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bxg.cashguo.top

[P08] 处理浮点精度问题
来源：http://msg.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bbi.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jzc.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sxy.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kfk.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zxm.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iai.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://prp.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cek.0kj1m.cn

================================================================================
来源：http://xys.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cym.ctjpmb.com

================================================================================
来源：http://bsk.hfpthk.cn

[Q01] 创建表
来源：http://ucp.fktsv.cn

CREATE TABLE users (
来源：http://qyp.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fua.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://sjc.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://ofg.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://klt.tianlin.xyz

);
来源：http://xaf.jianghu66.top

[Q02] 创建带外键的表
来源：http://dwq.zhiwuduotai.top

CREATE TABLE orders (
来源：http://huj.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ikd.gogol.net.cn

user_id INT NOT NULL,
来源：http://jfp.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://gbg.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://joj.9152youxi.cn

);
来源：http://jgo.zhiwuduotai.top

[Q03] 增加列
来源：http://bir.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pec.zdqjudy.top

[Q04] 修改列类型
来源：http://jtx.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ies.yongpay.top

[Q05] 重命名列
来源：http://nub.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqq.tarul.cn

[Q06] 删除列
来源：http://jsv.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kek.hnxiangtu.top

[Q07] 删除表
来源：http://trv.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://iup.andypj.xyz

[Q08] 创建普通索引
来源：http://mry.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://edq.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://nxs.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xdz.chenjidiqi.icu

[Q10] 插入单行
来源：http://ftj.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://afo.cheryme.top

[Q11] 一次插入多行
来源：http://ilk.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://akv.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://sms.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://mvx.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ecl.sufxvd.cn

[Q13] 忽略重复插入
来源：http://vyc.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bsy.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://xih.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pan.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nef.feifeiyinyue.top

[Q15] 查询全部
来源：http://nzp.fanxiaobao.xyz

SELECT * FROM users;
来源：http://afd.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://jnw.ehwqpu.com

SELECT id, name FROM users;
来源：http://syz.zdqjudy.top

[Q17] 条件查询
来源：http://grz.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ubm.tian-w.cn

[Q18] 模糊匹配
来源：http://kxn.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ykd.jqgufenzy.top

[Q19] 范围查询
来源：http://vdj.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dpx.sxryk.cn

[Q20] IN 列表
来源：http://bii.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lqx.fehbvm.com

[Q21] 空值判断
来源：http://iry.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hdb.yuanzhike.top

[Q22] 排序
来源：http://pnd.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mza.yanxiufei.cn

[Q23] 分页
来源：http://aar.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gqn.316326.xyz

[Q24] 去重
来源：http://fsf.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://hbz.aibaodan.cn

[Q25] 只取前 N 条
来源：http://xqa.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ibv.hysaishi.cn

[Q26] 计数
来源：http://ewo.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://pcn.iojbl.cn

[Q27] 条件计数
来源：http://sct.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rgx.jqgufenzy.top

[Q28] 求和与平均
来源：http://qun.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tig.cashguo.top

[Q29] 最大最小值
来源：http://kkx.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://whc.yueranfly.top

[Q30] 分组统计
来源：http://cfu.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sxj.hnxiangtu.top

[Q31] 分组后过滤
来源：http://eyu.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://unn.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://zzb.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lci.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bvc.epnwcf.com

[Q33] 多列分组
来源：http://woa.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://orh.bbcook.cn

[Q34] 每组取第一条
来源：http://bin.meibo888.top

SELECT * FROM (
来源：http://apv.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lco.fengsongda.top

) t WHERE rn = 1;
来源：http://wcq.wangdashe.top

[Q35] 内连接
来源：http://kjy.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mcv.yj20258.top

[Q36] 左连接
来源：http://fez.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lzv.yongpay.top

[Q37] 右连接
来源：http://aow.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qyr.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://hfo.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vcn.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://epp.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vah.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://efa.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vzx.vqdsnc.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wbh.cqqwz.cn

[Q41] 多表连接
来源：http://twk.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iwv.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://bje.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://rxs.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://qez.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://rsc.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://brf.hysaishi.cn

[Q43] 标量子查询
来源：http://nbp.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tyo.jinqigufen.top

[Q44] IN 子查询
来源：http://fka.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lul.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://qag.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yiz.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://oer.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://naz.nanxinkj.top

[Q47] 与平均值比较
来源：http://xmg.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nma.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://uhs.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wgk.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://wwt.vehdjk.com

[Q49] 更新单行
来源：http://fgb.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zyx.svipenyu.cn

[Q50] 批量更新
来源：http://jdk.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lxv.sjlbkw.cn

[Q51] 用子查询更新
来源：http://nhl.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jzn.tianlin.xyz

[Q52] 删除指定行
来源：http://ysg.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://zlz.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://czu.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://btj.chenzaomai.com

[Q54] 清空表
来源：http://rcp.ehwqpu.com

TRUNCATE TABLE logs;
来源：http://qbe.tanke756.top

[Q55] 排名（并列占位）
来源：http://ycm.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pqt.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://jmh.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zga.sweek.top

[Q57] 行号
来源：http://hxm.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://huj.guannengcc.top

[Q58] 累计求和
来源：http://ozf.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://unt.hcnkem.com

[Q59] 分组内累计
来源：http://kdy.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fam.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://oyf.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ols.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hmn.nanxinkj.top

[Q61] 移动平均
来源：http://sgg.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bxp.tian-w.cn

[Q62] 分组占比
来源：http://iru.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ums.epnwcf.com

[Q63] 开启事务
来源：http://kro.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rps.sjlbkw.cn

[Q64] 提交事务
来源：http://uvs.chenlongwang.top

COMMIT;
来源：http://xzd.guowangkeji.top

[Q65] 回滚事务
来源：http://agh.xingfuxueyuan.xyz

ROLLBACK;
来源：http://ywi.yj20258888.top

[Q66] 行锁查询
来源：http://eff.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vys.yongpay.top

[Q67] 设置隔离级别
来源：http://xhv.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jph.fanxiaobao.xyz

[Q68] 保存点
来源：http://vxx.jqgfzy.top

SAVEPOINT sp1;
来源：http://myx.gogol.net.cn

ROLLBACK TO sp1;
来源：http://akw.mhx1999.top

[Q69] 查看执行计划
来源：http://cyk.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gdb.316326.xyz

[Q70] 更新统计信息
来源：http://ssm.gaohongyu789.top

ANALYZE TABLE users;
来源：http://tqn.xuanzx.com

[Q71] 查看建表语句
来源：http://sfl.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wgn.hesvh.cn

[Q72] 查看索引
来源：http://hcm.daria6918.cn

SHOW INDEX FROM users;
来源：http://gnq.jinqigufen.top

[Q73] 查看表状态
来源：http://vkg.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tyl.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://bdx.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sfa.gogol.net.cn

[Q75] 日期格式化
来源：http://zli.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xnt.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mxh.xuanzx.com

[Q76] 按天统计
来源：http://dqp.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wel.yanxiufei.cn

[Q77] 时间加减
来源：http://php.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mmn.epnwcf.com

[Q78] 当前时间
来源：http://pbm.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://osu.andypj.xyz

[Q79] 字符串拼接
来源：http://tgd.ehwqpu.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jmg.gzhubu.top

[Q80] 字符串截取
来源：http://iee.hongshengwenyu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dpr.zhengqikj.top

[Q81] 字符串替换
来源：http://uyl.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wbl.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://efi.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fdd.yvedp.cn

[Q83] 大小写转换
来源：http://vzc.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://opg.316326.xyz

[Q84] 去除首尾空格
来源：http://bvf.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://wgb.ydzc1.top

[Q85] 数值取整
来源：http://aya.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ila.yj20258.top

[Q86] 读取 JSON 字段
来源：http://jps.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kce.cashguo.top

[Q87] JSON 字段做条件
来源：http://zry.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pqn.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://ykk.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ptv.yj20258.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://byu.meibo888.top

[Q89] 判断表是否存在
来源：http://lut.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mmg.zycfv.cn

[Q90] 生成序号列
来源：http://nnq.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fil.pengpengdd.cyou

================================================================================
来源：http://iru.sweek.top

R. Bash 专题
来源：http://iof.chenlongwang.top

================================================================================
来源：http://vgt.9152youxi.cn

[R01] shebang 与严格模式
来源：http://otg.zycfv.cn

#!/usr/bin/env bash
来源：http://giw.tian-w.cn

set -euo pipefail
来源：http://bqf.yj20258.top

[R02] 变量赋值与使用
来源：http://cps.guannengcc.top

name="Tom"; echo "$name"
来源：http://bur.hywenlv.cn

[R03] 只读变量
来源：http://tmy.pengpengdd.cyou

readonly PI=3.14
来源：http://yqc.dianchejie.cn

[R04] 位置参数
来源：http://nzi.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://krn.chenjidiqi.icu

[R05] 参数默认值
来源：http://ord.meibo888.top

name="${1:-default}"
来源：http://yqy.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://gyi.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kek.cdnleiting.top

[R07] if 判断文件
来源：http://ais.fehbvm.com


<!-- 参考信息 -->