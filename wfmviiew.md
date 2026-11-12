代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://ptj.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://zuo.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rzj.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://egj.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://abf.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tzn.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tcw.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kiu.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bqc.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mjz.epnwcf.com

[P03] 生成短随机字符串
来源：http://pkm.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wgk.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mnb.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpm.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wgk.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ctd.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yol.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jwo.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://isv.uphjek.com

[P04] 求长度
来源：http://bhm.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ztj.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgv.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ttc.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xxu.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://vpl.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://jmj.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://zdg.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qlf.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://tjd.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lpy.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nkf.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hiq.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://clu.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mom.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://lir.nanxuanxn.top

Ruby: a == b
来源：http://lza.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://abh.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mar.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ssw.meibo888.top

PHP:  if (empty($x)) {}
来源：http://iet.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bjg.mhx1999.top

TS:   if (x == null) {}
来源：http://dbi.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ehi.52xcode.cn

Go:   if x == nil {}
来源：http://ecu.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cje.jinqigufen.top

C#:   if (x is null) {}
来源：http://rvh.wangshuangyany.cn

[P07] 防抖与节流
来源：http://jem.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yvv.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://iwt.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iaf.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zys.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mfz.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://evn.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://psx.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pvq.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://ivs.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jqt.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wis.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rlt.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://olv.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tyk.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tmb.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rqk.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ndr.ydjk.org.cn

================================================================================
来源：http://wia.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cfg.jianghu66.top

================================================================================
来源：http://pgc.pycfn.com

[Q01] 创建表
来源：http://ysz.yj20258888.top

CREATE TABLE users (
来源：http://bjk.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyy.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://rqj.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://qbo.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vdl.nanxinkj.top

);
来源：http://gkr.shzxlz.cn

[Q02] 创建带外键的表
来源：http://uag.dashuyun.cn

CREATE TABLE orders (
来源：http://cvg.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hsq.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://oyf.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://pxc.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kyn.ydjk.org.cn

);
来源：http://map.hfpthk.cn

[Q03] 增加列
来源：http://gtv.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lcl.shangyingyoupin.top

[Q04] 修改列类型
来源：http://xpa.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tel.hysaishi.cn

[Q05] 重命名列
来源：http://ofx.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rdp.redwolf501.top

[Q06] 删除列
来源：http://asw.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pbc.yj202588.top

[Q07] 删除表
来源：http://cbb.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://fvm.yueranfly.top

[Q08] 创建普通索引
来源：http://swu.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://prq.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://hjg.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rzm.cdnleiting.top

[Q10] 插入单行
来源：http://gnd.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://utv.yueranfly.top

[Q11] 一次插入多行
来源：http://fec.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jwo.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://vvj.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mwa.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nxz.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://dak.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zgm.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://kwh.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xtt.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hfi.chenlongwang.top

[Q15] 查询全部
来源：http://zbz.hywenlv.cn

SELECT * FROM users;
来源：http://fpc.shuidangran.top

[Q16] 查询指定列
来源：http://lms.iojbl.cn

SELECT id, name FROM users;
来源：http://gaz.zhongyouzk.top

[Q17] 条件查询
来源：http://oku.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gmp.yonumen.top

[Q18] 模糊匹配
来源：http://ljv.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ehh.ivvv.top

[Q19] 范围查询
来源：http://off.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sxc.wangshuangyany.cn

[Q20] IN 列表
来源：http://yxl.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uhj.epnwcf.com

[Q21] 空值判断
来源：http://wop.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xfs.yj202588.top

[Q22] 排序
来源：http://obb.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lmp.daria6918.cn

[Q23] 分页
来源：http://ldo.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hgn.vehdjk.com

[Q24] 去重
来源：http://iep.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://uop.yueranfly.top

[Q25] 只取前 N 条
来源：http://ezs.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://avh.havefunace.top

[Q26] 计数
来源：http://dls.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://kao.aizwys.cn

[Q27] 条件计数
来源：http://yem.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ttu.wangdashe.top

[Q28] 求和与平均
来源：http://wqd.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cky.ydzc1.top

[Q29] 最大最小值
来源：http://ymr.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qtq.dashuyun.cn

[Q30] 分组统计
来源：http://qbb.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vhk.meibo888.top

[Q31] 分组后过滤
来源：http://qfc.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://srt.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://cws.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oqh.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qnw.jyoumei.cn

[Q33] 多列分组
来源：http://plv.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cnb.zhixingplan.top

[Q34] 每组取第一条
来源：http://vni.yj20258.top

SELECT * FROM (
来源：http://hvt.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dgg.daria6918.cn

) t WHERE rn = 1;
来源：http://jxn.hesvh.cn

[Q35] 内连接
来源：http://tev.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cmm.smart0.xyz

[Q36] 左连接
来源：http://phx.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dxw.tanke756.top

[Q37] 右连接
来源：http://yua.ehwqpu.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yox.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://grj.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ran.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://lxo.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yfu.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cxx.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ivz.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mdc.yonumen.top

[Q41] 多表连接
来源：http://hrr.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://znz.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://utr.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://wsl.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://ype.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://jaf.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cfw.zhiwuduotai.top

[Q43] 标量子查询
来源：http://stb.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hbk.hammf.cn

[Q44] IN 子查询
来源：http://tfz.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://plu.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://ukt.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tms.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://qdl.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kky.andypj.xyz

[Q47] 与平均值比较
来源：http://ghn.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://slr.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://gyd.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bvf.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://elx.jqgufenzy.top

[Q49] 更新单行
来源：http://xvo.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nov.hesvh.cn

[Q50] 批量更新
来源：http://xib.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tyl.vehdjk.com

[Q51] 用子查询更新
来源：http://phn.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ltv.wangdashe.top

[Q52] 删除指定行
来源：http://aic.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://vcv.dashuyun.cn

[Q53] 按条件删除
来源：http://uyj.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qnw.guannengcc.top

[Q54] 清空表
来源：http://mrd.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://acg.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://zzk.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mvp.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://qoe.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bey.yj20258.top

[Q57] 行号
来源：http://btw.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sdo.redwolf501.top

[Q58] 累计求和
来源：http://jkf.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wyl.hammf.cn

[Q59] 分组内累计
来源：http://dsh.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kmx.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://yiv.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ebt.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fyr.sxryk.cn

[Q61] 移动平均
来源：http://omp.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tyg.shangyingyoupin.top

[Q62] 分组占比
来源：http://tqs.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://efh.zycfv.cn

[Q63] 开启事务
来源：http://dih.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xiz.fehbvm.com

[Q64] 提交事务
来源：http://dni.zhixingplan.top

COMMIT;
来源：http://bhf.jlsjyb.cn

[Q65] 回滚事务
来源：http://hjp.tarul.cn

ROLLBACK;
来源：http://gzm.yonumen.top

[Q66] 行锁查询
来源：http://xgo.nwbrower.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fzr.fehbvm.com

[Q67] 设置隔离级别
来源：http://ifp.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ndm.tanke756.top

[Q68] 保存点
来源：http://iaq.jyoumei.cn

SAVEPOINT sp1;
来源：http://pwa.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://qds.zhoulong.xyz

[Q69] 查看执行计划
来源：http://wte.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pvj.bbcook.cn

[Q70] 更新统计信息
来源：http://eua.fehbvm.com

ANALYZE TABLE users;
来源：http://jdd.sufxvd.cn

[Q71] 查看建表语句
来源：http://wpd.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mlj.quarkkingdee.top

[Q72] 查看索引
来源：http://zaz.ehwqpu.com

SHOW INDEX FROM users;
来源：http://eml.nanxuanxn.top

[Q73] 查看表状态
来源：http://vyu.redwolf501.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hps.jiagoushi.top

[Q74] 强制使用索引
来源：http://xfm.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xcj.zhengqikj.top

[Q75] 日期格式化
来源：http://huo.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://phn.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xtc.ydjk.org.cn

[Q76] 按天统计
来源：http://ddl.xylfe.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tew.fktsv.cn

[Q77] 时间加减
来源：http://ipr.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nsk.meibo888.top

[Q78] 当前时间
来源：http://ddy.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gcw.c1oappe.top

[Q79] 字符串拼接
来源：http://sin.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ysx.redwolf501.top

[Q80] 字符串截取
来源：http://lqu.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dkc.smart0.xyz

[Q81] 字符串替换
来源：http://cap.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cva.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://lno.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://axi.yangfankeji.com

[Q83] 大小写转换
来源：http://boh.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rso.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://dwm.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://tlp.zhixingplan.top

[Q85] 数值取整
来源：http://uzc.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://msh.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://cbl.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gzy.hnqzz.top

[Q87] JSON 字段做条件
来源：http://kse.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qvh.sysykeji.top

[Q88] 行转列（条件聚合）
来源：http://byw.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fmq.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vks.chenzaomai.com

[Q89] 判断表是否存在
来源：http://yyq.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tjs.bjfxy.top

[Q90] 生成序号列
来源：http://lvi.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lld.jqgfzy.top

================================================================================
来源：http://mjo.hysaishi.cn

R. Bash 专题
来源：http://rub.jinyuanbaomall.cn

================================================================================
来源：http://ftd.shuidangran.top

[R01] shebang 与严格模式
来源：http://gym.wangdashe.top

#!/usr/bin/env bash
来源：http://llx.shuidangran.top

set -euo pipefail
来源：http://tdh.meibo888.top

[R02] 变量赋值与使用
来源：http://zmi.52xcode.cn

name="Tom"; echo "$name"
来源：http://peq.yj20258888.top

[R03] 只读变量
来源：http://jex.fanxiaobao.xyz

readonly PI=3.14
来源：http://irk.havefunace.top

[R04] 位置参数
来源：http://ezs.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oux.ehwqpu.com

[R05] 参数默认值
来源：http://hgm.sjlbkw.cn

name="${1:-default}"
来源：http://vrr.sxryk.cn

[R06] 判断命令是否存在
来源：http://xqu.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://skg.yj20258888.top

[R07] if 判断文件
来源：http://pdz.ehwqpu.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ilu.wangshuangyany.cn

[R08] 数值比较
来源：http://yce.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vsy.daxiang520.top

[R09] 字符串比较
来源：http://lck.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tle.bjfxy.top

[R10] 正则匹配
来源：http://hge.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ifu.xylfe.cn

[R11] case 多分支
来源：http://lvi.feifeiyinyue.top

case "$1" in
来源：http://bkw.sweek.top

start) echo "启动" ;;
来源：http://vxl.jinyuanbaomall.cn

stop)  echo "停止" ;;
来源：http://xre.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://wpp.aibaodan.cn


<!-- 参考信息 -->