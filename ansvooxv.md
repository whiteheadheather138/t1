代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gtx.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://brt.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xib.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://azp.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://obl.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ebr.yonumen.top

[P03] 生成短随机字符串
来源：http://ljs.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mbv.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ugy.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ber.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rcv.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vgh.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lam.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lyd.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qjq.fengsongda.top

[P04] 求长度
来源：http://eko.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxa.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fdd.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cly.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://exr.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://zik.fktsv.cn

Go:   len(arr);  len(m)
来源：http://yzw.shzxlz.cn

Ruby: x.length;  x.size
来源：http://okb.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zqc.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://ezu.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rng.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nwb.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fug.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uuo.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dxc.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fyz.vqdsnc.cn

Ruby: a == b
来源：http://yhg.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ipz.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gyr.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://njr.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://mat.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gmq.c1oappe.top

TS:   if (x == null) {}
来源：http://zfz.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://tib.jiagoushi.top

Go:   if x == nil {}
来源：http://mlc.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://awy.hesvh.cn

C#:   if (x is null) {}
来源：http://apm.havefunace.top

[P07] 防抖与节流
来源：http://jbl.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://alu.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://orm.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzn.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uyp.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ztx.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ppi.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nsh.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://phr.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://xho.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iqk.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ojb.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sws.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ovk.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cst.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ham.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cbt.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oip.fzhhl.top

================================================================================
来源：http://dvu.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aky.xuanzx.com

================================================================================
来源：http://sef.zhoulong.xyz

[Q01] 创建表
来源：http://mit.jianghu66.top

CREATE TABLE users (
来源：http://lfz.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ccd.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://oou.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://aqx.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ubf.jyoumei.cn

);
来源：http://hzr.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://beq.shuidangran.top

CREATE TABLE orders (
来源：http://tyu.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eiy.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://xel.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://ipm.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gnf.ydzc1.top

);
来源：http://hyg.0kj1m.cn

[Q03] 增加列
来源：http://ics.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eyx.sysykeji.top

[Q04] 修改列类型
来源：http://vwx.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iar.jyoumei.cn

[Q05] 重命名列
来源：http://mcq.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dyl.ybcxt.top

[Q06] 删除列
来源：http://ydu.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mny.jqgufenzy.top

[Q07] 删除表
来源：http://ilc.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://tto.shzxlz.cn

[Q08] 创建普通索引
来源：http://pfh.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pkm.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://ipp.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rxm.cashguo.top

[Q10] 插入单行
来源：http://vcx.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rcp.zdbjq.cn

[Q11] 一次插入多行
来源：http://nkh.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gfy.316326.xyz

[Q12] 插入后取自增 ID
来源：http://jrm.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nok.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qsu.haohaochexian.top

[Q13] 忽略重复插入
来源：http://wwe.jqgfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iwu.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://wcs.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pxv.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zar.sxryk.cn

[Q15] 查询全部
来源：http://lmh.zycfv.cn

SELECT * FROM users;
来源：http://vru.hesvh.cn

[Q16] 查询指定列
来源：http://sre.zycfv.cn

SELECT id, name FROM users;
来源：http://hjl.xinyue.icu

[Q17] 条件查询
来源：http://mxn.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eio.jinqigufen.top

[Q18] 模糊匹配
来源：http://nui.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wlm.cdnleiting.top

[Q19] 范围查询
来源：http://edi.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://stv.kuanghao11.cn

[Q20] IN 列表
来源：http://vfr.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jqw.haohaochexian.top

[Q21] 空值判断
来源：http://mup.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://poz.zycfv.cn

[Q22] 排序
来源：http://jff.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qqs.gogol.net.cn

[Q23] 分页
来源：http://ihg.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hrj.cashguo.top

[Q24] 去重
来源：http://aus.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://pxh.jinqigufen.top

[Q25] 只取前 N 条
来源：http://pnk.yj20258888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vtq.shzxlz.cn

[Q26] 计数
来源：http://pmg.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://jff.haohaochexian.top

[Q27] 条件计数
来源：http://dsq.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lfd.ctjpmb.com

[Q28] 求和与平均
来源：http://qqd.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dfl.pengpengdd.cyou

[Q29] 最大最小值
来源：http://obc.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aar.hongshengwenyu.top

[Q30] 分组统计
来源：http://bpc.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rho.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://boi.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hms.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://rbz.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ixj.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tsh.nwbrower.top

[Q33] 多列分组
来源：http://lsb.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yhv.cheryme.top

[Q34] 每组取第一条
来源：http://wqn.shanyushiyangtech.top

SELECT * FROM (
来源：http://tao.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wbu.guannengcc.top

) t WHERE rn = 1;
来源：http://ukf.mhx1999.top

[Q35] 内连接
来源：http://ebc.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fky.yangfankeji.com

[Q36] 左连接
来源：http://jii.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dri.fengsongda.top

[Q37] 右连接
来源：http://lws.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kqs.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mlj.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://myy.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://vxm.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://und.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lae.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uhk.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qqk.0kj1m.cn

[Q41] 多表连接
来源：http://bnl.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xuz.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://jat.cashguo.top

JOIN products p ON p.id = o.product_id;
来源：http://qpe.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://yjf.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://ubn.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hdv.daria6918.cn

[Q43] 标量子查询
来源：http://mgq.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://taw.feifeiyinyue.top

[Q44] IN 子查询
来源：http://hou.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hkj.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://vtp.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yqf.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://oyc.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfj.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://cru.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://icc.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://kxu.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ywj.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://rnu.daxiang520.top

[Q49] 更新单行
来源：http://utj.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://auz.ybcxt.top

[Q50] 批量更新
来源：http://gnq.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://duj.wangdashe.top

[Q51] 用子查询更新
来源：http://bcs.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kan.sufxvd.cn

[Q52] 删除指定行
来源：http://nol.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://jph.aizwys.cn

[Q53] 按条件删除
来源：http://ibs.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dyj.dianchejie.cn

[Q54] 清空表
来源：http://dpn.havefunace.top

TRUNCATE TABLE logs;
来源：http://kxo.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://aqy.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wat.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://bld.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vqf.vqdsnc.cn

[Q57] 行号
来源：http://tfo.gaohongyu789.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sje.shuidangran.top

[Q58] 累计求和
来源：http://uax.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kyw.yueranfly.top

[Q59] 分组内累计
来源：http://hmd.xingfuxueyuan.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zso.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://qed.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://prc.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://plf.nwbrower.top

[Q61] 移动平均
来源：http://cbz.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tsa.jiagoushi.top

[Q62] 分组占比
来源：http://yur.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hlo.hammf.cn

[Q63] 开启事务
来源：http://bkk.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://muk.fanxiaobao.xyz

[Q64] 提交事务
来源：http://hvz.wangshuangyany.cn

COMMIT;
来源：http://via.aibaodan.cn

[Q65] 回滚事务
来源：http://ofl.xuanzx.com

ROLLBACK;
来源：http://mif.redwolf501.top

[Q66] 行锁查询
来源：http://qkj.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gai.hfpthk.cn

[Q67] 设置隔离级别
来源：http://gnx.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dcr.daria6918.cn

[Q68] 保存点
来源：http://yxm.cdnleiting.top

SAVEPOINT sp1;
来源：http://med.c1oappe.top

ROLLBACK TO sp1;
来源：http://var.bjfxy.top

[Q69] 查看执行计划
来源：http://sny.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ddv.nanxuanxn.top

[Q70] 更新统计信息
来源：http://pog.sjlbkw.cn

ANALYZE TABLE users;
来源：http://qns.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://oam.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yau.dashuyun.cn

[Q72] 查看索引
来源：http://usi.yvedp.cn

SHOW INDEX FROM users;
来源：http://jsj.yonumen.top

[Q73] 查看表状态
来源：http://pja.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://smg.hysaishi.cn

[Q74] 强制使用索引
来源：http://isr.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xgf.tarul.cn

[Q75] 日期格式化
来源：http://gmy.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zdk.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ydo.hnqzz.top

[Q76] 按天统计
来源：http://emf.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://owo.zhongyouzk.top

[Q77] 时间加减
来源：http://dqn.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ngh.yfazqb.com

[Q78] 当前时间
来源：http://uyg.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://num.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://esp.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qqi.zhoulong.xyz

[Q80] 字符串截取
来源：http://ltr.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tzq.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://xzj.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mhf.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://jmc.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uco.0kj1m.cn

[Q83] 大小写转换
来源：http://xpt.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oxu.cqqwz.cn

[Q84] 去除首尾空格
来源：http://byx.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://ken.bbcook.cn

[Q85] 数值取整
来源：http://uei.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ryn.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://sjz.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wen.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://fbo.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://joj.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://flj.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://elu.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gdb.ehwqpu.com

[Q89] 判断表是否存在
来源：http://vpu.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jvq.c1oappe.top

[Q90] 生成序号列
来源：http://cmp.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zkc.kuanghao11.cn

================================================================================
来源：http://vth.tianlin.xyz

R. Bash 专题
来源：http://keo.fktsv.cn

================================================================================
来源：http://zfb.xinyue.icu

[R01] shebang 与严格模式
来源：http://vco.0kj1m.cn

#!/usr/bin/env bash
来源：http://tlc.zhaomingkeji.xyz

set -euo pipefail
来源：http://sjf.yongpay.top

[R02] 变量赋值与使用
来源：http://hhn.hywenlv.cn

name="Tom"; echo "$name"
来源：http://gju.jianghu66.top

[R03] 只读变量
来源：http://nve.dianchejie.cn

readonly PI=3.14
来源：http://ipp.fehbvm.com

[R04] 位置参数
来源：http://yom.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kno.fengsongda.top

[R05] 参数默认值
来源：http://fko.ehwqpu.com

name="${1:-default}"
来源：http://ldi.yueranfly.top

[R06] 判断命令是否存在
来源：http://czi.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uiz.nanxuanxn.top

[R07] if 判断文件
来源：http://oui.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kqs.0kj1m.cn

[R08] 数值比较
来源：http://hnt.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vtx.yj20258888.top

[R09] 字符串比较
来源：http://rkw.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aql.svipenyu.cn

[R10] 正则匹配
来源：http://yww.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ebn.zhaomingkeji.xyz

[R11] case 多分支
来源：http://kqt.ehwqpu.com

case "$1" in
来源：http://jhd.wangdashe.top

start) echo "启动" ;;
来源：http://irh.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://gmn.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://uuv.jlsjyb.cn

esac
来源：http://jra.vqdsnc.cn

[R12] for 遍历文件
来源：http://wdn.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://qss.hesvh.cn

[R13] for 计数循环
来源：http://zts.hnqzz.top


<!-- 参考信息 -->