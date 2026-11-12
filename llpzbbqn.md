代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vga.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eqi.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wmp.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vfi.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pak.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zku.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://uio.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gnc.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tex.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tmb.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zrj.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://foh.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fez.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rlz.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kye.sysykeji.top

[P04] 求长度
来源：http://beo.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://idc.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wba.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://agm.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xip.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://zwp.yongpay.top

Go:   len(arr);  len(m)
来源：http://vyv.yuanzhike.top

Ruby: x.length;  x.size
来源：http://yyd.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zte.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://xee.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zko.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mof.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cmb.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bjs.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qeu.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://udt.feifeiyinyue.top

Ruby: a == b
来源：http://dud.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oat.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://epa.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://svv.pycfn.com

PHP:  if (empty($x)) {}
来源：http://cbf.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bjz.ctjpmb.com

TS:   if (x == null) {}
来源：http://yfy.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fah.vqdsnc.cn

Go:   if x == nil {}
来源：http://rrp.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nxl.epnwcf.com

C#:   if (x is null) {}
来源：http://htz.hnqzz.top

[P07] 防抖与节流
来源：http://rze.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xqo.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://cyu.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fcl.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmh.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aea.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://swv.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fxq.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dfw.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://fej.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://quz.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vci.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qec.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://flw.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fdz.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qtc.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cut.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://trx.0kj1m.cn

================================================================================
来源：http://chn.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://opj.cqqwz.cn

================================================================================
来源：http://moc.haohaochexian.top

[Q01] 创建表
来源：http://nai.yj20258.top

CREATE TABLE users (
来源：http://wdf.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lqw.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://bld.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://yon.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jet.hfpthk.cn

);
来源：http://paq.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://mop.jlsjyb.cn

CREATE TABLE orders (
来源：http://wzl.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nly.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://bgi.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://knq.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ikr.xuetiantiany.cn

);
来源：http://sxx.ydjk.org.cn

[Q03] 增加列
来源：http://fhu.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gyg.vqdsnc.cn

[Q04] 修改列类型
来源：http://nza.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hns.chenjidiqi.icu

[Q05] 重命名列
来源：http://xqo.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ujy.chenjidiqi.icu

[Q06] 删除列
来源：http://bty.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dxf.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://ndw.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://mls.cdnleiting.top

[Q08] 创建普通索引
来源：http://iad.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vxe.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://mbn.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rdv.sufxvd.cn

[Q10] 插入单行
来源：http://tck.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fuk.cheryme.top

[Q11] 一次插入多行
来源：http://tbz.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://exx.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://ske.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://qxw.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ulp.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://otw.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zav.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://acb.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://apj.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dmy.xinyue.icu

[Q15] 查询全部
来源：http://til.yueranfly.top

SELECT * FROM users;
来源：http://xwb.hywenlv.cn

[Q16] 查询指定列
来源：http://ujs.tian-w.cn

SELECT id, name FROM users;
来源：http://wgl.andypj.xyz

[Q17] 条件查询
来源：http://vuk.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lxt.yueranfly.top

[Q18] 模糊匹配
来源：http://khs.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://god.fktsv.cn

[Q19] 范围查询
来源：http://quo.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://muk.iojbl.cn

[Q20] IN 列表
来源：http://lnj.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gfv.fzhhl.top

[Q21] 空值判断
来源：http://svn.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vpx.cqqwz.cn

[Q22] 排序
来源：http://ylg.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://has.tarul.cn

[Q23] 分页
来源：http://ram.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bct.jqgfzy.top

[Q24] 去重
来源：http://sxs.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://ydc.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://nff.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wxf.9152youxi.cn

[Q26] 计数
来源：http://uzy.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://gdl.zycfv.cn

[Q27] 条件计数
来源：http://amg.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lcn.wangshuangyany.cn

[Q28] 求和与平均
来源：http://szx.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xpt.wangshuangyany.cn

[Q29] 最大最小值
来源：http://bdd.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://zyw.uphjek.com

[Q30] 分组统计
来源：http://pml.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tml.xylfe.cn

[Q31] 分组后过滤
来源：http://ufm.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lbh.yvedp.cn

[Q32] 分组拼接字符串
来源：http://xub.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xkn.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gwh.0kj1m.cn

[Q33] 多列分组
来源：http://run.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zyv.52xcode.cn

[Q34] 每组取第一条
来源：http://uge.tian-w.cn

SELECT * FROM (
来源：http://slc.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ylz.yangfankeji.com

) t WHERE rn = 1;
来源：http://hqd.tarul.cn

[Q35] 内连接
来源：http://eap.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cri.ehwqpu.com

[Q36] 左连接
来源：http://jmk.ppjwa.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dgm.zhoulong.xyz

[Q37] 右连接
来源：http://wdm.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://deh.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sdp.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pug.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://vrt.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rif.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mhz.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ran.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oxa.zhoulong.xyz

[Q41] 多表连接
来源：http://wuy.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jen.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://nzv.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://kli.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://vkw.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://xaa.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fgi.sxryk.cn

[Q43] 标量子查询
来源：http://dig.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vbb.tarul.cn

[Q44] IN 子查询
来源：http://yam.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sdc.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://zgi.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vxc.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://cds.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nag.yfazqb.com

[Q47] 与平均值比较
来源：http://ksx.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dos.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://jtr.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://htd.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://pyw.shuidangran.top

[Q49] 更新单行
来源：http://exg.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dfz.hnqzz.top

[Q50] 批量更新
来源：http://gwk.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://imw.kuanghao11.cn

[Q51] 用子查询更新
来源：http://kkf.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gcj.gogol.net.cn

[Q52] 删除指定行
来源：http://pia.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://mqj.yuanzhike.top

[Q53] 按条件删除
来源：http://dun.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jld.xinyue.icu

[Q54] 清空表
来源：http://rkn.tian-w.cn

TRUNCATE TABLE logs;
来源：http://zzb.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://hul.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xkc.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://wws.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mvg.xziqi.cn

[Q57] 行号
来源：http://tif.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vhu.fengsongda.top

[Q58] 累计求和
来源：http://jbv.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ywf.dianchejie.cn

[Q59] 分组内累计
来源：http://wnr.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sgq.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://isw.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://omk.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lmt.cashguo.top

[Q61] 移动平均
来源：http://nih.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://clh.havefunace.top

[Q62] 分组占比
来源：http://vgv.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://smt.hnxiangtu.top

[Q63] 开启事务
来源：http://tlv.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rfb.mhx1999.top

[Q64] 提交事务
来源：http://cmc.hysaishi.cn

COMMIT;
来源：http://xxb.cheryme.top

[Q65] 回滚事务
来源：http://owu.wangshuangyany.cn

ROLLBACK;
来源：http://jrh.nwbrower.top

[Q66] 行锁查询
来源：http://hjm.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vcp.jianghu66.top

[Q67] 设置隔离级别
来源：http://fjp.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hac.hesvh.cn

[Q68] 保存点
来源：http://vfs.hfpthk.cn

SAVEPOINT sp1;
来源：http://oer.haohaochexian.top

ROLLBACK TO sp1;
来源：http://zma.ivvv.top

[Q69] 查看执行计划
来源：http://ghk.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mlh.316326.xyz

[Q70] 更新统计信息
来源：http://het.hfpthk.cn

ANALYZE TABLE users;
来源：http://aqr.yonumen.top

[Q71] 查看建表语句
来源：http://lrc.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rom.hnqzz.top

[Q72] 查看索引
来源：http://eva.fehbvm.com

SHOW INDEX FROM users;
来源：http://ynf.cqqwz.cn

[Q73] 查看表状态
来源：http://lfq.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pyf.sweek.top

[Q74] 强制使用索引
来源：http://aqm.zhoulong.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kmp.zdbjq.cn

[Q75] 日期格式化
来源：http://flb.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vbp.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tfg.snrcjt.cn

[Q76] 按天统计
来源：http://fce.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://epq.yuxming.cn

[Q77] 时间加减
来源：http://cgi.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ijg.sysykeji.top

[Q78] 当前时间
来源：http://gcd.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zum.hywenlv.cn

[Q79] 字符串拼接
来源：http://lxl.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cyf.jqgufenzy.top

[Q80] 字符串截取
来源：http://puy.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ajf.zdbjq.cn

[Q81] 字符串替换
来源：http://izr.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tna.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://gtr.jinyuanbaomall.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oqe.andypj.xyz

[Q83] 大小写转换
来源：http://pmr.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mvb.bbcook.cn

[Q84] 去除首尾空格
来源：http://kul.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://zjd.hcnkem.com

[Q85] 数值取整
来源：http://ibd.xingfuxueyuan.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hgu.meibo888.top

[Q86] 读取 JSON 字段
来源：http://bha.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dnj.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://agm.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mib.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://inx.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kim.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dgh.hfpthk.cn

[Q89] 判断表是否存在
来源：http://dpu.epnwcf.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://etb.cqqwz.cn

[Q90] 生成序号列
来源：http://ykf.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vyg.hongshengwenyu.top

================================================================================
来源：http://tzr.meibo888.top

R. Bash 专题
来源：http://llm.sjlbkw.cn

================================================================================
来源：http://nas.ydzc1.top

[R01] shebang 与严格模式
来源：http://dmn.nwbrower.top

#!/usr/bin/env bash
来源：http://kkv.c1oappe.top

set -euo pipefail
来源：http://ury.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://uah.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://uyy.yuanzhike.top

[R03] 只读变量
来源：http://uax.yvedp.cn

readonly PI=3.14
来源：http://wix.dashuyun.cn

[R04] 位置参数
来源：http://fxe.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://leo.yongpay.top

[R05] 参数默认值
来源：http://ykx.zhengqikj.top

name="${1:-default}"
来源：http://enb.daria6918.cn

[R06] 判断命令是否存在
来源：http://wtc.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qew.sweek.top

[R07] if 判断文件
来源：http://sbr.chenzaomai.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aue.quarkkingdee.top

[R08] 数值比较
来源：http://bdr.yvedp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rkk.ppjwa.cn

[R09] 字符串比较
来源：http://iks.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqv.sysykeji.top

[R10] 正则匹配
来源：http://zys.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://czp.bbcook.cn

[R11] case 多分支
来源：http://efv.bjfxy.top

case "$1" in
来源：http://mam.cucudq.cn

start) echo "启动" ;;
来源：http://vlt.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://bux.ydzc1.top

*)     echo "未知命令" ;;
来源：http://hxk.fzhhl.top

esac
来源：http://jfx.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://sjz.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://jiy.hfpthk.cn

[R13] for 计数循环
来源：http://uoh.0kj1m.cn


<!-- 参考信息 -->