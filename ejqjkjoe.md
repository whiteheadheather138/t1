代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bbq.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lws.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kfp.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rwq.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vvm.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tct.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://mhx.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gbm.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vcq.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cvh.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrq.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qox.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zhz.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tpe.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fgv.zhengqikj.top

[P04] 求长度
来源：http://sqm.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nry.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmp.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iqg.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bye.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://iwv.shuidangran.top

Go:   len(arr);  len(m)
来源：http://foh.jqgfzy.top

Ruby: x.length;  x.size
来源：http://kvx.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mew.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://axs.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mpq.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wto.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pqb.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://axf.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zkm.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://ffp.ivvv.top

Ruby: a == b
来源：http://wfk.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ftz.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ndv.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://epf.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://xjw.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wxf.shuidangran.top

TS:   if (x == null) {}
来源：http://obm.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uwu.hywenlv.cn

Go:   if x == nil {}
来源：http://rsr.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yve.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://jhl.vehdjk.com

[P07] 防抖与节流
来源：http://zbm.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://brm.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://qcp.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxz.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ulo.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eum.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lne.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fxr.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ces.yfazqb.com

[P08] 处理浮点精度问题
来源：http://csq.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vfq.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nbb.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ssy.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pia.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://akq.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rqc.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fam.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jid.hfpthk.cn

================================================================================
来源：http://ohs.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zfi.ppjwa.cn

================================================================================
来源：http://pcz.zhixingplan.top

[Q01] 创建表
来源：http://xmd.xziqi.cn

CREATE TABLE users (
来源：http://amg.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xnb.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://fyn.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://xeq.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lnl.yonumen.top

);
来源：http://gag.meibo888.top

[Q02] 创建带外键的表
来源：http://hfv.birdmap.top

CREATE TABLE orders (
来源：http://aqw.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eew.hfpthk.cn

user_id INT NOT NULL,
来源：http://yhr.cucudq.cn

amount DECIMAL(10, 2),
来源：http://xgu.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tzd.sweek.top

);
来源：http://pym.hesvh.cn

[Q03] 增加列
来源：http://xev.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tpz.guannengcc.top

[Q04] 修改列类型
来源：http://ewx.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qdq.jinqigfzy.top

[Q05] 重命名列
来源：http://ebf.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kwn.xuetiantiany.cn

[Q06] 删除列
来源：http://xbh.jiagoushi.top

ALTER TABLE users DROP COLUMN age;
来源：http://awc.zdbjq.cn

[Q07] 删除表
来源：http://gzy.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://qgw.jyoumei.cn

[Q08] 创建普通索引
来源：http://mqu.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://nxb.cqqwz.cn

[Q09] 创建唯一索引
来源：http://udd.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fid.chenlongwang.top

[Q10] 插入单行
来源：http://yde.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zsm.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://cox.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blh.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://vag.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://osn.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xyt.aibaodan.cn

[Q13] 忽略重复插入
来源：http://qfz.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kwc.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://tqu.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gul.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jpw.vqdsnc.cn

[Q15] 查询全部
来源：http://yuq.yuanzhike.top

SELECT * FROM users;
来源：http://byu.bjfxy.top

[Q16] 查询指定列
来源：http://vum.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://gnh.316326.xyz

[Q17] 条件查询
来源：http://tbm.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yos.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://noa.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://psm.ehwqpu.com

[Q19] 范围查询
来源：http://efn.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sxb.hcnkem.com

[Q20] IN 列表
来源：http://qzq.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wqw.mhx1999.top

[Q21] 空值判断
来源：http://xqs.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nes.cqqwz.cn

[Q22] 排序
来源：http://msu.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qhn.chenlongwang.top

[Q23] 分页
来源：http://rwa.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qgr.haohaochexian.top

[Q24] 去重
来源：http://lrj.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://xds.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://oqd.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://apa.fengsongda.top

[Q26] 计数
来源：http://svj.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://rdy.fanxiaobao.xyz

[Q27] 条件计数
来源：http://eje.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kzk.chenjidiqi.icu

[Q28] 求和与平均
来源：http://bkb.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tln.yuanzhike.top

[Q29] 最大最小值
来源：http://qvv.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oll.ivvv.top

[Q30] 分组统计
来源：http://psg.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zhr.hnxiangtu.top

[Q31] 分组后过滤
来源：http://ejj.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qwk.cheryme.top

[Q32] 分组拼接字符串
来源：http://cng.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xug.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xxk.zhongyouzk.top

[Q33] 多列分组
来源：http://nci.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dxd.mhx1999.top

[Q34] 每组取第一条
来源：http://mgb.havefunace.top

SELECT * FROM (
来源：http://zxl.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wkx.jinqigfzy.top

) t WHERE rn = 1;
来源：http://elf.vehdjk.com

[Q35] 内连接
来源：http://zzd.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://evc.pengpengdd.cyou

[Q36] 左连接
来源：http://wlg.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cal.shzxlz.cn

[Q37] 右连接
来源：http://vls.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wfs.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://tib.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eat.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://mol.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://wpk.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bja.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://twe.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iib.yueranfly.top

[Q41] 多表连接
来源：http://cne.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pdw.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://emk.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://pfe.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://amv.hfpthk.cn

SELECT u.name, o.amount FROM users u
来源：http://ndu.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kvd.vqdsnc.cn

[Q43] 标量子查询
来源：http://jhy.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cvq.cqqwz.cn

[Q44] IN 子查询
来源：http://xoo.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://npl.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://sol.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpj.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://wmf.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dlt.bbcook.cn

[Q47] 与平均值比较
来源：http://bdu.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ody.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://evt.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zjq.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://ozv.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://doo.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wug.zhengqikj.top

[Q50] 批量更新
来源：http://leu.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uco.yvedp.cn

[Q51] 用子查询更新
来源：http://igf.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ngz.jlsjyb.cn

[Q52] 删除指定行
来源：http://bcx.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://tkj.pycfn.com

[Q53] 按条件删除
来源：http://fyc.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qtu.tian-w.cn

[Q54] 清空表
来源：http://mjv.yj20258888.top

TRUNCATE TABLE logs;
来源：http://bxo.epnwcf.com

[Q55] 排名（并列占位）
来源：http://czx.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://psb.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://bbx.yueranfly.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kct.hfpthk.cn

[Q57] 行号
来源：http://lap.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uxn.shzxlz.cn

[Q58] 累计求和
来源：http://nrn.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jef.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://uzo.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gnp.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://djm.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mmk.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hra.nanxinkj.top

[Q61] 移动平均
来源：http://ufs.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://khi.hfpthk.cn

[Q62] 分组占比
来源：http://tjs.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vkp.mhx1999.top

[Q63] 开启事务
来源：http://zry.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://njz.svipenyu.cn

[Q64] 提交事务
来源：http://djr.hysaishi.cn

COMMIT;
来源：http://ten.jyoumei.cn

[Q65] 回滚事务
来源：http://heo.cucudq.cn

ROLLBACK;
来源：http://fik.fehbvm.com

[Q66] 行锁查询
来源：http://xvb.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pqa.zhixingplan.top

[Q67] 设置隔离级别
来源：http://uvu.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://onl.cqqwz.cn

[Q68] 保存点
来源：http://pxc.yanxiufei.cn

SAVEPOINT sp1;
来源：http://snm.hesvh.cn

ROLLBACK TO sp1;
来源：http://tmr.hysaishi.cn

[Q69] 查看执行计划
来源：http://jgr.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://drm.yuxming.cn

[Q70] 更新统计信息
来源：http://emt.ppjwa.cn

ANALYZE TABLE users;
来源：http://txu.daria6918.cn

[Q71] 查看建表语句
来源：http://tix.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ytm.havefunace.top

[Q72] 查看索引
来源：http://yfz.havefunace.top

SHOW INDEX FROM users;
来源：http://dyz.316326.xyz

[Q73] 查看表状态
来源：http://gwp.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ayt.ydjk.org.cn

[Q74] 强制使用索引
来源：http://mat.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tjd.nanxuanxn.top

[Q75] 日期格式化
来源：http://sjf.xziqi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dnm.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kup.yvedp.cn

[Q76] 按天统计
来源：http://vfx.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://maf.chenjidiqi.icu

[Q77] 时间加减
来源：http://mtx.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pks.sysykeji.top

[Q78] 当前时间
来源：http://ksn.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ldo.ctjpmb.com

[Q79] 字符串拼接
来源：http://aip.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gid.redwolf501.top

[Q80] 字符串截取
来源：http://aap.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ywr.chenjidiqi.icu

[Q81] 字符串替换
来源：http://stb.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pqz.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://qmq.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://thm.bjfxy.top

[Q83] 大小写转换
来源：http://pem.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vfi.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://yiq.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://txo.yonumen.top

[Q85] 数值取整
来源：http://uhz.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mcu.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://cjb.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ngo.tian-w.cn

[Q87] JSON 字段做条件
来源：http://uik.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://chh.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://kph.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gup.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ayv.ivvv.top

[Q89] 判断表是否存在
来源：http://xhw.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wbq.yonumen.top

[Q90] 生成序号列
来源：http://uqz.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mio.yuanzhike.top

================================================================================
来源：http://tva.yvedp.cn

R. Bash 专题
来源：http://ycx.jiagoushi.top

================================================================================
来源：http://uxm.cashguo.top

[R01] shebang 与严格模式
来源：http://uci.zycfv.cn

#!/usr/bin/env bash
来源：http://xmh.feifeiyinyue.top

set -euo pipefail
来源：http://wef.hammf.cn

[R02] 变量赋值与使用
来源：http://due.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://dun.gzhubu.top

[R03] 只读变量
来源：http://prd.feifeiyinyue.top

readonly PI=3.14
来源：http://bvr.hongshengwenyu.top

[R04] 位置参数
来源：http://wbt.xuetiantiany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kfz.tanke756.top

[R05] 参数默认值
来源：http://qet.xinyue.icu

name="${1:-default}"
来源：http://hjp.zdbjq.cn

[R06] 判断命令是否存在
来源：http://wzb.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nea.yonumen.top

[R07] if 判断文件
来源：http://zew.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qmr.hfpthk.cn

[R08] 数值比较
来源：http://eyw.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xjk.yanxiufei.cn

[R09] 字符串比较
来源：http://kfz.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gla.yanxiufei.cn

[R10] 正则匹配
来源：http://dzl.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cel.jinqigufen.top

[R11] case 多分支
来源：http://sdi.guannengcc.top

case "$1" in
来源：http://qmu.zycfv.cn

start) echo "启动" ;;
来源：http://hmt.jyoumei.cn

stop)  echo "停止" ;;
来源：http://mcp.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://iuh.sufxvd.cn

esac
来源：http://gor.redwolf501.top

[R12] for 遍历文件
来源：http://bmq.tianlin.xyz

for f in *.txt; do echo "$f"; done
来源：http://des.sysykeji.top

[R13] for 计数循环
来源：http://qmj.jlsjyb.cn


<!-- 参考信息 -->