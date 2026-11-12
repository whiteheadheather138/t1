代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yte.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wjy.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hob.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yes.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ydo.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dem.zdbjq.cn

[P03] 生成短随机字符串
来源：http://xci.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mhe.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qai.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://abg.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bll.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zlv.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wsp.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tfj.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ypn.yueranfly.top

[P04] 求长度
来源：http://svt.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fkm.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://evd.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zdg.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bvd.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://zlk.zycfv.cn

Go:   len(arr);  len(m)
来源：http://udo.daxiang520.top

Ruby: x.length;  x.size
来源：http://njm.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://fob.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://vwq.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lfc.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ilk.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tve.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tud.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zsy.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://uid.zhaomingkeji.xyz

Ruby: a == b
来源：http://tfu.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gnq.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kpl.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kbi.ivvv.top

PHP:  if (empty($x)) {}
来源：http://wgx.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kzq.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://fyk.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wxi.jqgfzy.top

Go:   if x == nil {}
来源：http://otm.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qyq.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://zpr.guowangkeji.top

[P07] 防抖与节流
来源：http://cmr.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wrp.yj202588.top

PHP:  // 手写时间戳比较
来源：http://wwc.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://roq.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kkj.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cer.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ufk.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xbc.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fzp.yongpay.top

[P08] 处理浮点精度问题
来源：http://ynu.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vxy.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dkv.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ygg.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lvv.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://egu.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ror.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jvo.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oag.hfpthk.cn

================================================================================
来源：http://ucg.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://usz.xylfe.cn

================================================================================
来源：http://pmd.mhx1999.top

[Q01] 创建表
来源：http://bld.tanke756.top

CREATE TABLE users (
来源：http://lkx.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xbj.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://fig.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://vgt.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cmt.shanyushiyangkeji.top

);
来源：http://kwe.nwbrower.top

[Q02] 创建带外键的表
来源：http://hms.xziqi.cn

CREATE TABLE orders (
来源：http://abc.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fcb.jyoumei.cn

user_id INT NOT NULL,
来源：http://uza.ydzc1.top

amount DECIMAL(10, 2),
来源：http://eyn.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gvf.zycfv.cn

);
来源：http://jvj.zhiwuduotai.top

[Q03] 增加列
来源：http://zzp.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qaq.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://ebt.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ltp.zhijiandao.cn

[Q05] 重命名列
来源：http://mke.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aoh.kuanghao11.cn

[Q06] 删除列
来源：http://kgc.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://wis.dianchejie.cn

[Q07] 删除表
来源：http://caq.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://dfc.yj20258.top

[Q08] 创建普通索引
来源：http://isp.c1oappe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gno.xinyue.icu

[Q09] 创建唯一索引
来源：http://rlu.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://edh.ctjpmb.com

[Q10] 插入单行
来源：http://eej.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sfv.redwolf501.top

[Q11] 一次插入多行
来源：http://thz.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jwd.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://hjv.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://qip.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://knz.hysaishi.cn

[Q13] 忽略重复插入
来源：http://mmp.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dvg.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://qic.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kru.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rde.haohaochexian.top

[Q15] 查询全部
来源：http://thk.hywenlv.cn

SELECT * FROM users;
来源：http://yvb.wangshuangyany.cn

[Q16] 查询指定列
来源：http://coj.hysaishi.cn

SELECT id, name FROM users;
来源：http://fvo.epnwcf.com

[Q17] 条件查询
来源：http://fcq.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://piz.chenlongwang.top

[Q18] 模糊匹配
来源：http://sza.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jey.cashguo.top

[Q19] 范围查询
来源：http://qtz.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fhp.jiagoushi.top

[Q20] IN 列表
来源：http://sjg.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://umv.chenjidiqi.icu

[Q21] 空值判断
来源：http://tsj.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dhz.ctjpmb.com

[Q22] 排序
来源：http://krn.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lmr.daria6918.cn

[Q23] 分页
来源：http://rvr.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://myf.shuidangran.top

[Q24] 去重
来源：http://sph.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://ckm.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://zcd.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kjw.jinqigufen.top

[Q26] 计数
来源：http://ouf.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://hpk.hywenlv.cn

[Q27] 条件计数
来源：http://cdz.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vcu.yj202588.top

[Q28] 求和与平均
来源：http://fex.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://exn.hnqzz.top

[Q29] 最大最小值
来源：http://otn.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://heb.yangfankeji.com

[Q30] 分组统计
来源：http://nyt.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sqb.redwolf501.top

[Q31] 分组后过滤
来源：http://lsm.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ivg.smart0.xyz

[Q32] 分组拼接字符串
来源：http://zpm.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fxg.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hcc.pycfn.com

[Q33] 多列分组
来源：http://dtn.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://njz.c1oappe.top

[Q34] 每组取第一条
来源：http://gkm.ybcxt.top

SELECT * FROM (
来源：http://ezc.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dxa.zdbjq.cn

) t WHERE rn = 1;
来源：http://lto.316326.xyz

[Q35] 内连接
来源：http://pgx.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kvo.guannengcc.top

[Q36] 左连接
来源：http://tbz.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mfw.bjfxy.top

[Q37] 右连接
来源：http://bvc.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://syu.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hdf.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ilz.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://dnw.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://von.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nci.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rsm.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jrb.chenjidiqi.icu

[Q41] 多表连接
来源：http://rab.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nrc.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://xjh.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://pcr.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://gca.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://ddu.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vjk.wangshuangyany.cn

[Q43] 标量子查询
来源：http://ceq.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cly.yj202588.top

[Q44] IN 子查询
来源：http://ztd.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kiu.tarul.cn

[Q45] EXISTS 判断存在
来源：http://tzk.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://khb.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://plw.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gtc.pycfn.com

[Q47] 与平均值比较
来源：http://rru.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kmb.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://uem.dashuyun.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dkk.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://bse.shanyushiyangtech.top

[Q49] 更新单行
来源：http://rif.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rom.fktsv.cn

[Q50] 批量更新
来源：http://lfs.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vpw.hammf.cn

[Q51] 用子查询更新
来源：http://fxx.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://avv.chenjidiqi.icu

[Q52] 删除指定行
来源：http://hxy.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://ufm.hcnkem.com

[Q53] 按条件删除
来源：http://iwv.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fvp.hysaishi.cn

[Q54] 清空表
来源：http://vez.yvedp.cn

TRUNCATE TABLE logs;
来源：http://hcs.epnwcf.com

[Q55] 排名（并列占位）
来源：http://pvn.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ymh.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://xaj.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gbo.cucudq.cn

[Q57] 行号
来源：http://yau.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pgc.sufxvd.cn

[Q58] 累计求和
来源：http://iuu.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bxg.xinyue.icu

[Q59] 分组内累计
来源：http://xlm.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tlk.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://ojz.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fqg.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kkg.ybcxt.top

[Q61] 移动平均
来源：http://jnl.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hau.hnxiangtu.top

[Q62] 分组占比
来源：http://uxo.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vjl.jinqigufen.top

[Q63] 开启事务
来源：http://ljc.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qls.nwbrower.top

[Q64] 提交事务
来源：http://ave.zycfv.cn

COMMIT;
来源：http://yya.xylfe.cn

[Q65] 回滚事务
来源：http://elf.zhiwuduotai.top

ROLLBACK;
来源：http://dth.svipenyu.cn

[Q66] 行锁查询
来源：http://ecu.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://twh.xuanzx.com

[Q67] 设置隔离级别
来源：http://dib.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oce.mhx1999.top

[Q68] 保存点
来源：http://whk.quarkkingdee.top

SAVEPOINT sp1;
来源：http://ioa.haohaochexian.top

ROLLBACK TO sp1;
来源：http://stu.jinqigufen.top

[Q69] 查看执行计划
来源：http://kst.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://psc.yfazqb.com

[Q70] 更新统计信息
来源：http://puh.vehdjk.com

ANALYZE TABLE users;
来源：http://kkd.sysykeji.top

[Q71] 查看建表语句
来源：http://sob.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eze.52xcode.cn

[Q72] 查看索引
来源：http://uvz.xuanzx.com

SHOW INDEX FROM users;
来源：http://wjd.yongpay.top

[Q73] 查看表状态
来源：http://fml.dianchejie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zxe.ybcxt.top

[Q74] 强制使用索引
来源：http://msw.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hvk.yuanzhike.top

[Q75] 日期格式化
来源：http://mge.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qhl.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qou.yj20258888.top

[Q76] 按天统计
来源：http://lce.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sia.daxiang520.top

[Q77] 时间加减
来源：http://thi.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cei.nwbrower.top

[Q78] 当前时间
来源：http://ewe.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kyp.cqqwz.cn

[Q79] 字符串拼接
来源：http://mxh.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sjp.pengpengdd.cyou

[Q80] 字符串截取
来源：http://atq.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xpw.jiagoushi.top

[Q81] 字符串替换
来源：http://dmz.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xsj.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://rqu.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sch.nanxinkj.top

[Q83] 大小写转换
来源：http://fwn.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sss.xziqi.cn

[Q84] 去除首尾空格
来源：http://dfo.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://agl.shanyushiyangtech.top

[Q85] 数值取整
来源：http://cyp.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pus.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://zwh.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bbz.daria6918.cn

[Q87] JSON 字段做条件
来源：http://utn.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tss.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://ago.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kwo.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://exv.xylfe.cn

[Q89] 判断表是否存在
来源：http://dns.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ffq.ydzc1.top

[Q90] 生成序号列
来源：http://kbn.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cos.zhoulong.xyz

================================================================================
来源：http://qzf.vehdjk.com

R. Bash 专题
来源：http://ull.hywenlv.cn

================================================================================
来源：http://dmn.gogol.net.cn

[R01] shebang 与严格模式
来源：http://ast.0kj1m.cn

#!/usr/bin/env bash
来源：http://mtt.sysykeji.top

set -euo pipefail
来源：http://egj.yfazqb.com

[R02] 变量赋值与使用
来源：http://rrx.sysykeji.top

name="Tom"; echo "$name"
来源：http://lwi.sysykeji.top

[R03] 只读变量
来源：http://esc.ydjk.org.cn

readonly PI=3.14
来源：http://gfv.yuxming.cn

[R04] 位置参数
来源：http://ktl.aibaodan.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://efk.sufxvd.cn

[R05] 参数默认值
来源：http://fkb.haohaochexian.top

name="${1:-default}"
来源：http://vbu.gogol.net.cn

[R06] 判断命令是否存在
来源：http://pcx.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sun.ppjwa.cn

[R07] if 判断文件
来源：http://stu.zhengqikj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rvj.tianlin.xyz

[R08] 数值比较
来源：http://ics.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vng.quarkkingdee.top

[R09] 字符串比较
来源：http://ldb.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wfz.quarkkingdee.top

[R10] 正则匹配
来源：http://exq.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ysl.guowangkeji.top

[R11] case 多分支
来源：http://ncy.nanxuanxn.top

case "$1" in
来源：http://uew.hcnkem.com

start) echo "启动" ;;
来源：http://jsc.yj20258.top

stop)  echo "停止" ;;
来源：http://odv.yonumen.top

*)     echo "未知命令" ;;
来源：http://vue.sweek.top

esac
来源：http://cbv.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://lma.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://fdy.fehbvm.com

[R13] for 计数循环
来源：http://leu.yj20258888.top


<!-- 参考信息 -->