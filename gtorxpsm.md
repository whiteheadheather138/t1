代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iby.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nyk.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nwm.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://isj.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vfv.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nmh.wangdashe.top

[P03] 生成短随机字符串
来源：http://tds.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://did.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nnr.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ukl.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ydv.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wlm.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jwj.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://zfs.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hlf.havefunace.top

[P04] 求长度
来源：http://hrf.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yoh.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zsb.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dad.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hwt.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://rrg.hcnkem.com

Go:   len(arr);  len(m)
来源：http://ugr.zdqjudy.top

Ruby: x.length;  x.size
来源：http://oug.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lrr.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://mqi.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://vjz.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yhl.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nev.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qaz.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aza.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://gis.pengpengdd.cyou

Ruby: a == b
来源：http://opj.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xuv.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oet.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://szv.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://mav.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nee.bbcook.cn

TS:   if (x == null) {}
来源：http://mmr.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dzq.xziqi.cn

Go:   if x == nil {}
来源：http://gpd.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iqe.hfpthk.cn

C#:   if (x is null) {}
来源：http://uxo.ybcxt.top

[P07] 防抖与节流
来源：http://orp.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://grw.316326.xyz

PHP:  // 手写时间戳比较
来源：http://bis.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zie.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://imz.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://liu.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ndr.pycfn.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ijd.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ese.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://vjl.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rme.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ujv.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fin.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gep.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://omh.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zgl.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iyl.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mxn.shzxlz.cn

================================================================================
来源：http://ikx.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://grx.bbcook.cn

================================================================================
来源：http://cfw.gogol.net.cn

[Q01] 创建表
来源：http://rsq.hysaishi.cn

CREATE TABLE users (
来源：http://sln.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dap.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://qze.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://rqk.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uuc.yj20258888.top

);
来源：http://gti.fktsv.cn

[Q02] 创建带外键的表
来源：http://ggy.gotoacloud.top

CREATE TABLE orders (
来源：http://iys.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mig.fehbvm.com

user_id INT NOT NULL,
来源：http://oxl.yfazqb.com

amount DECIMAL(10, 2),
来源：http://erg.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://epq.sxryk.cn

);
来源：http://bcg.gaohongyu789.top

[Q03] 增加列
来源：http://nnv.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dds.fzhhl.top

[Q04] 修改列类型
来源：http://jsm.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lih.tian-w.cn

[Q05] 重命名列
来源：http://hhb.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vva.chenzaomai.com

[Q06] 删除列
来源：http://vbq.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gtl.tanke756.top

[Q07] 删除表
来源：http://rtb.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://lkw.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://bdp.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mvm.ehwqpu.com

[Q09] 创建唯一索引
来源：http://qia.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://irb.aibaodan.cn

[Q10] 插入单行
来源：http://uhc.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fib.tanke756.top

[Q11] 一次插入多行
来源：http://uke.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rwd.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://bas.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fkn.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hul.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://bwq.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pwk.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://jmb.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dpy.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uiw.gzhubu.top

[Q15] 查询全部
来源：http://hek.kuanghao11.cn

SELECT * FROM users;
来源：http://tyr.jqgufenzy.top

[Q16] 查询指定列
来源：http://rzm.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://bxo.mhx1999.top

[Q17] 条件查询
来源：http://uos.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oul.cashguo.top

[Q18] 模糊匹配
来源：http://sen.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xjk.iojbl.cn

[Q19] 范围查询
来源：http://qul.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dxi.yvedp.cn

[Q20] IN 列表
来源：http://qrz.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bsq.yonumen.top

[Q21] 空值判断
来源：http://lgw.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zyg.cucudq.cn

[Q22] 排序
来源：http://jxn.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ikz.yfazqb.com

[Q23] 分页
来源：http://upv.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dgr.chenjidiqi.icu

[Q24] 去重
来源：http://ukl.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://tsl.yj20258888.top

[Q25] 只取前 N 条
来源：http://nzk.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ihb.redwolf501.top

[Q26] 计数
来源：http://jsz.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://mih.yangfankeji.com

[Q27] 条件计数
来源：http://ioz.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cmx.fzhhl.top

[Q28] 求和与平均
来源：http://hik.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kwd.cdnleiting.top

[Q29] 最大最小值
来源：http://hry.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dxj.yfazqb.com

[Q30] 分组统计
来源：http://bie.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rmv.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://dux.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fzz.52xcode.cn

[Q32] 分组拼接字符串
来源：http://qdo.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fjk.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gyy.uphjek.com

[Q33] 多列分组
来源：http://xcl.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lri.guannengcc.top

[Q34] 每组取第一条
来源：http://xls.zhixingplan.top

SELECT * FROM (
来源：http://btx.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xha.xziqi.cn

) t WHERE rn = 1;
来源：http://six.xuetiantiany.cn

[Q35] 内连接
来源：http://rgm.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jfx.ydzc1.top

[Q36] 左连接
来源：http://utz.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kcl.yj20258.top

[Q37] 右连接
来源：http://oyt.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fcz.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://qvm.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qfd.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://spp.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zkh.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dsv.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bwk.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tzn.sweek.top

[Q41] 多表连接
来源：http://ite.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bdc.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://hfh.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://mun.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://yrk.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://zla.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://leu.dashuyun.cn

[Q43] 标量子查询
来源：http://jhr.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fso.yonumen.top

[Q44] IN 子查询
来源：http://gmc.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://quo.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://lzl.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jhs.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://dxb.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fkx.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://iwc.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lot.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://ywq.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qyb.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://zzc.birdmap.top

[Q49] 更新单行
来源：http://kbb.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ibz.daxiang520.top

[Q50] 批量更新
来源：http://lsv.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uuk.xuanzx.com

[Q51] 用子查询更新
来源：http://epb.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://upf.pycfn.com

[Q52] 删除指定行
来源：http://woq.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://mui.uphjek.com

[Q53] 按条件删除
来源：http://vfh.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ujn.chenlongwang.top

[Q54] 清空表
来源：http://tbj.sxryk.cn

TRUNCATE TABLE logs;
来源：http://fwd.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://epg.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uen.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://ucf.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bxv.gzhubu.top

[Q57] 行号
来源：http://pgq.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fsc.iojbl.cn

[Q58] 累计求和
来源：http://xlq.yj20258.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fnq.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://hoo.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kqa.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://uoy.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://chv.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ewx.smart0.xyz

[Q61] 移动平均
来源：http://njy.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eqd.hysaishi.cn

[Q62] 分组占比
来源：http://gqg.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tep.ctjpmb.com

[Q63] 开启事务
来源：http://uzq.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wcc.ctjpmb.com

[Q64] 提交事务
来源：http://lrm.yj202588.top

COMMIT;
来源：http://vih.aizwys.cn

[Q65] 回滚事务
来源：http://znm.yuanzhike.top

ROLLBACK;
来源：http://trd.tarul.cn

[Q66] 行锁查询
来源：http://jox.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://djm.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://zds.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ebw.jinqigfzy.top

[Q68] 保存点
来源：http://stb.quarkkingdee.top

SAVEPOINT sp1;
来源：http://hdj.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ica.cheryme.top

[Q69] 查看执行计划
来源：http://ojl.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rot.hnxiangtu.top

[Q70] 更新统计信息
来源：http://prv.hcnkem.com

ANALYZE TABLE users;
来源：http://fqy.chenlongwang.top

[Q71] 查看建表语句
来源：http://buy.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwe.ehwqpu.com

[Q72] 查看索引
来源：http://bec.shuidangran.top

SHOW INDEX FROM users;
来源：http://lhy.hesvh.cn

[Q73] 查看表状态
来源：http://bvw.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pzl.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://ptt.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://usc.yuanzhike.top

[Q75] 日期格式化
来源：http://jlc.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rsv.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://euj.sysykeji.top

[Q76] 按天统计
来源：http://bth.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://brq.yuanzhike.top

[Q77] 时间加减
来源：http://ilu.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uzd.chenlongwang.top

[Q78] 当前时间
来源：http://ljx.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oeo.nanxuanxn.top

[Q79] 字符串拼接
来源：http://qoi.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wdg.wangshuangyany.cn

[Q80] 字符串截取
来源：http://gsh.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kmk.jqgfzy.top

[Q81] 字符串替换
来源：http://bdu.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bbb.yonumen.top

[Q82] 字符长度与字节长度
来源：http://euz.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qzt.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://waj.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rqy.fktsv.cn

[Q84] 去除首尾空格
来源：http://swm.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://wfg.kuanghao11.cn

[Q85] 数值取整
来源：http://szk.cdnleiting.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://acy.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://yzg.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yux.birdmap.top

[Q87] JSON 字段做条件
来源：http://ukw.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kvs.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://qhi.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cyc.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://acy.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://fut.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uih.andypj.xyz

[Q90] 生成序号列
来源：http://ryi.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kfc.tianlin.xyz

================================================================================
来源：http://nfv.ivvv.top

R. Bash 专题
来源：http://pie.nwbrower.top

================================================================================
来源：http://bwe.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://uwv.cucudq.cn

#!/usr/bin/env bash
来源：http://qdc.tarul.cn

set -euo pipefail
来源：http://mjz.pycfn.com

[R02] 变量赋值与使用
来源：http://zel.shuidangran.top

name="Tom"; echo "$name"
来源：http://dbu.shanyushiyangkeji.top

[R03] 只读变量
来源：http://mcs.zdqjudy.top

readonly PI=3.14
来源：http://wad.hnxiangtu.top

[R04] 位置参数
来源：http://wvo.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nwy.hfpthk.cn

[R05] 参数默认值
来源：http://adl.ywan-chungtsiang.top

name="${1:-default}"
来源：http://ecy.gzhubu.top

[R06] 判断命令是否存在
来源：http://yec.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nfe.yfazqb.com

[R07] if 判断文件
来源：http://fbz.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cry.shanyushiyangkeji.top

[R08] 数值比较
来源：http://fuq.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vwa.tian-w.cn

[R09] 字符串比较
来源：http://dec.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jyq.hysaishi.cn

[R10] 正则匹配
来源：http://ehh.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pyk.hcnkem.com

[R11] case 多分支
来源：http://cpm.yongpay.top

case "$1" in
来源：http://yzw.jinyuanbaomall.cn

start) echo "启动" ;;
来源：http://qub.jianghu66.top

stop)  echo "停止" ;;
来源：http://ruf.yj20258.top

*)     echo "未知命令" ;;
来源：http://qbz.zhongyouzk.top

esac
来源：http://tze.hesvh.cn

[R12] for 遍历文件
来源：http://tfu.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://pdq.yuanzhike.top

[R13] for 计数循环
来源：http://brf.gzhubu.top


<!-- 参考信息 -->