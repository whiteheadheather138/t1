代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tyu.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sfl.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cog.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dcd.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kto.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ico.gzhubu.top

[P03] 生成短随机字符串
来源：http://ety.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eyj.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lym.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://axg.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iwk.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lez.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vgi.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vyc.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://luk.pengpengdd.cyou

[P04] 求长度
来源：http://rxo.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ytr.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cgv.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rip.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://knc.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://cba.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://qfd.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://bbr.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lpu.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://isg.epnwcf.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://hay.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zos.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zyk.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wmf.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nfp.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://uza.hnxiangtu.top

Ruby: a == b
来源：http://prw.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lrh.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sly.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wos.meibo888.top

PHP:  if (empty($x)) {}
来源：http://wxp.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qln.guowangkeji.top

TS:   if (x == null) {}
来源：http://tab.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kia.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://fev.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mls.jianghu66.top

C#:   if (x is null) {}
来源：http://dpg.cucudq.cn

[P07] 防抖与节流
来源：http://osv.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gwn.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://faw.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwf.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uhq.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://njz.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ljj.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oei.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nyz.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://hlo.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wxp.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tfp.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://weq.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ksu.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wfu.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tok.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sae.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vkl.cdnleiting.top

================================================================================
来源：http://ejw.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yhz.yueranfly.top

================================================================================
来源：http://ftz.nanxinkj.top

[Q01] 创建表
来源：http://cur.jinqigufen.top

CREATE TABLE users (
来源：http://xkd.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ivh.gzhubu.top

name VARCHAR(50) NOT NULL,
来源：http://wvp.ydjk.org.cn

email VARCHAR(100) UNIQUE,
来源：http://nfp.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://spc.yj20258888.top

);
来源：http://cyz.yj202588.top

[Q02] 创建带外键的表
来源：http://tsv.jyoumei.cn

CREATE TABLE orders (
来源：http://vxs.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rnq.cashguo.top

user_id INT NOT NULL,
来源：http://oel.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://zwq.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tsb.jinqigfzy.top

);
来源：http://uer.dashuyun.cn

[Q03] 增加列
来源：http://byo.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ymx.zdqjudy.top

[Q04] 修改列类型
来源：http://zsm.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://amx.zhixingplan.top

[Q05] 重命名列
来源：http://kdc.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xve.bjfxy.top

[Q06] 删除列
来源：http://ceo.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://zqn.jinqigufen.top

[Q07] 删除表
来源：http://jmv.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://qmt.sysykeji.top

[Q08] 创建普通索引
来源：http://bts.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cqk.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://gog.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cst.jlsjyb.cn

[Q10] 插入单行
来源：http://zcv.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ebm.hesvh.cn

[Q11] 一次插入多行
来源：http://skb.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zut.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://ezc.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://blu.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gkq.chenlongwang.top

[Q13] 忽略重复插入
来源：http://nbw.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ova.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://ifi.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mrg.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aou.0kj1m.cn

[Q15] 查询全部
来源：http://nmo.daria6918.cn

SELECT * FROM users;
来源：http://ixi.wangdashe.top

[Q16] 查询指定列
来源：http://fwv.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://ksk.sxryk.cn

[Q17] 条件查询
来源：http://fjw.ctjpmb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wrv.daria6918.cn

[Q18] 模糊匹配
来源：http://kxn.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ltq.chenzaomai.com

[Q19] 范围查询
来源：http://wih.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jjm.pengpengdd.cyou

[Q20] IN 列表
来源：http://wbl.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yao.hfpthk.cn

[Q21] 空值判断
来源：http://nzb.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nvt.feifeiyinyue.top

[Q22] 排序
来源：http://cnw.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mou.xingfuxueyuan.xyz

[Q23] 分页
来源：http://dkw.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://obd.sxryk.cn

[Q24] 去重
来源：http://eas.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://jou.mhx1999.top

[Q25] 只取前 N 条
来源：http://xte.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cqh.daria6918.cn

[Q26] 计数
来源：http://hwp.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://pdq.andypj.xyz

[Q27] 条件计数
来源：http://ify.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xpa.tianlin.xyz

[Q28] 求和与平均
来源：http://zdg.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wev.birdmap.top

[Q29] 最大最小值
来源：http://smz.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tsk.zhixingplan.top

[Q30] 分组统计
来源：http://som.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://usy.guowangkeji.top

[Q31] 分组后过滤
来源：http://jki.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mbh.xylfe.cn

[Q32] 分组拼接字符串
来源：http://sib.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gjs.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kvf.tanke756.top

[Q33] 多列分组
来源：http://akz.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://taf.yangfankeji.com

[Q34] 每组取第一条
来源：http://odn.tian-w.cn

SELECT * FROM (
来源：http://tff.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://asq.cashguo.top

) t WHERE rn = 1;
来源：http://xih.ywan-chungtsiang.top

[Q35] 内连接
来源：http://scj.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wwf.hongshengwenyu.top

[Q36] 左连接
来源：http://fum.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ugo.zdbjq.cn

[Q37] 右连接
来源：http://bsa.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pui.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://nbl.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gfs.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://wai.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://edg.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hab.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://htq.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ley.smart0.xyz

[Q41] 多表连接
来源：http://xyw.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gqr.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://awy.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://dii.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://lxr.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://nao.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hov.zdqjudy.top

[Q43] 标量子查询
来源：http://igp.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://crr.zdqjudy.top

[Q44] IN 子查询
来源：http://dkc.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cyv.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://duw.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qzt.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://brt.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbx.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://aqz.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oko.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://rtn.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xsb.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://tre.vqdsnc.cn

[Q49] 更新单行
来源：http://kyh.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dlk.yonumen.top

[Q50] 批量更新
来源：http://bzq.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://esv.gogol.net.cn

[Q51] 用子查询更新
来源：http://vxd.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ofp.cucudq.cn

[Q52] 删除指定行
来源：http://djq.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://hpg.xuanzx.com

[Q53] 按条件删除
来源：http://zcw.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ffw.cheryme.top

[Q54] 清空表
来源：http://abm.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://xrx.cashguo.top

[Q55] 排名（并列占位）
来源：http://eua.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uwu.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://vux.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qlp.hongshengwenyu.top

[Q57] 行号
来源：http://wkn.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vfx.chenzaomai.com

[Q58] 累计求和
来源：http://trb.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kia.xuetiantiany.cn

[Q59] 分组内累计
来源：http://ssz.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iqd.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://hjs.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yqz.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cja.xziqi.cn

[Q61] 移动平均
来源：http://aqh.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vom.smart0.xyz

[Q62] 分组占比
来源：http://orr.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xzt.hywenlv.cn

[Q63] 开启事务
来源：http://tyf.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vyi.daria6918.cn

[Q64] 提交事务
来源：http://fhh.yvedp.cn

COMMIT;
来源：http://zuk.haohaochexian.top

[Q65] 回滚事务
来源：http://mqb.jinghuilouyu.cn

ROLLBACK;
来源：http://lyc.snrcjt.cn

[Q66] 行锁查询
来源：http://zss.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zfi.pycfn.com

[Q67] 设置隔离级别
来源：http://sxs.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://edb.chenjidiqi.icu

[Q68] 保存点
来源：http://dbu.hcnkem.com

SAVEPOINT sp1;
来源：http://yyu.hysaishi.cn

ROLLBACK TO sp1;
来源：http://ahv.hesvh.cn

[Q69] 查看执行计划
来源：http://xvn.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vkt.yj20258.top

[Q70] 更新统计信息
来源：http://etb.chenlongwang.top

ANALYZE TABLE users;
来源：http://cjf.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://okj.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xjv.kuanghao11.cn

[Q72] 查看索引
来源：http://lqg.jiagoushi.top

SHOW INDEX FROM users;
来源：http://bmk.daxiang520.top

[Q73] 查看表状态
来源：http://mul.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yay.ivvv.top

[Q74] 强制使用索引
来源：http://xfd.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://upa.wangdashe.top

[Q75] 日期格式化
来源：http://bdu.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://juh.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sei.tianlin.xyz

[Q76] 按天统计
来源：http://yma.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ujz.sjlbkw.cn

[Q77] 时间加减
来源：http://odk.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kac.guowangkeji.top

[Q78] 当前时间
来源：http://xkt.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zqz.guowangkeji.top

[Q79] 字符串拼接
来源：http://tjb.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jgn.meibo888.top

[Q80] 字符串截取
来源：http://urs.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zof.yj202588.top

[Q81] 字符串替换
来源：http://dld.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rpr.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://hqv.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jsj.jyoumei.cn

[Q83] 大小写转换
来源：http://cnp.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofs.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://zcn.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://rty.yfazqb.com

[Q85] 数值取整
来源：http://zct.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fox.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://kdg.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dss.meibo888.top

[Q87] JSON 字段做条件
来源：http://fxl.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cyf.ehwqpu.com

[Q88] 行转列（条件聚合）
来源：http://sbi.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://isc.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vyo.bjfxy.top

[Q89] 判断表是否存在
来源：http://xvy.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fvc.dianchejie.cn

[Q90] 生成序号列
来源：http://puq.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ldh.ctjpmb.com

================================================================================
来源：http://jak.jinqigufen.top

R. Bash 专题
来源：http://jqw.cqqwz.cn

================================================================================
来源：http://smg.sysykeji.top

[R01] shebang 与严格模式
来源：http://kgn.daria6918.cn

#!/usr/bin/env bash
来源：http://jvj.shuidangran.top

set -euo pipefail
来源：http://ipq.yueranfly.top

[R02] 变量赋值与使用
来源：http://puu.chenzaomai.com

name="Tom"; echo "$name"
来源：http://kzx.gzhubu.top

[R03] 只读变量
来源：http://vvy.jinghuilouyu.cn

readonly PI=3.14
来源：http://mal.cashguo.top

[R04] 位置参数
来源：http://tix.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://shx.xuetiantiany.cn

[R05] 参数默认值
来源：http://fwm.chenzaomai.com

name="${1:-default}"
来源：http://amd.yj20258.top

[R06] 判断命令是否存在
来源：http://hrl.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yam.hywenlv.cn

[R07] if 判断文件
来源：http://hca.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gcb.wangdashe.top

[R08] 数值比较
来源：http://npn.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ohb.chenjidiqi.icu

[R09] 字符串比较
来源：http://flp.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hzn.chenzaomai.com

[R10] 正则匹配
来源：http://aqv.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sam.ehwqpu.com

[R11] case 多分支
来源：http://zns.sjlbkw.cn

case "$1" in
来源：http://vmf.gaohongyu789.top

start) echo "启动" ;;
来源：http://vel.chenlongwang.top

stop)  echo "停止" ;;
来源：http://lgt.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://aig.hnxiangtu.top

esac
来源：http://fbr.jyoumei.cn

[R12] for 遍历文件
来源：http://oyk.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://ynb.zdbjq.cn

[R13] for 计数循环
来源：http://gsy.cucudq.cn


<!-- 参考信息 -->