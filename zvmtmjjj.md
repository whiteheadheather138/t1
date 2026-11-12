代发 wailian999

TS:   crypto.randomUUID()
来源：http://aoa.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://inv.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://bwc.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://rrz.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://wza.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://ygy.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yji.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cod.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ikr.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ojo.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://goa.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tkl.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cmn.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://buw.cucudq.cn

[P03] 生成短随机字符串
来源：http://qtp.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dil.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xho.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qih.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwf.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qgs.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eml.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wvm.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gtr.shuidangran.top

[P04] 求长度
来源：http://shs.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wop.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gxz.nanxuanxn.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vom.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://siz.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://uej.fehbvm.com

Go:   len(arr);  len(m)
来源：http://npe.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://gpw.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mcg.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://fro.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://our.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mzn.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uwf.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://isz.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://erw.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://djq.pycfn.com

Ruby: a == b
来源：http://eui.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uwu.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cjy.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xgt.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://zyu.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vaf.zdqjudy.top

TS:   if (x == null) {}
来源：http://uby.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://ztt.pycfn.com

Go:   if x == nil {}
来源：http://cqi.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mqx.zhoulong.xyz

C#:   if (x is null) {}
来源：http://avr.ctjpmb.com

[P07] 防抖与节流
来源：http://vzb.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lza.tarul.cn

PHP:  // 手写时间戳比较
来源：http://mbi.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xaz.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fcq.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jce.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yfd.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://poh.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vsq.guannengcc.top

[P08] 处理浮点精度问题
来源：http://bus.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://foo.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sit.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wlg.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://huf.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bku.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qtu.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eqd.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aqi.bjfxy.top

================================================================================
来源：http://pro.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://crc.mhx1999.top

================================================================================
来源：http://sgp.zhengqikj.top

[Q01] 创建表
来源：http://dyv.c1oappe.top

CREATE TABLE users (
来源：http://nwr.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vgr.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://fme.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://hin.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dxj.guowangkeji.top

);
来源：http://ktz.jinqigufen.top

[Q02] 创建带外键的表
来源：http://rpe.yj20258888.top

CREATE TABLE orders (
来源：http://gbu.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mio.hcnkem.com

user_id INT NOT NULL,
来源：http://zut.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://cpj.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bgx.xingfuxueyuan.xyz

);
来源：http://sup.epnwcf.com

[Q03] 增加列
来源：http://csk.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dji.zhongyouzk.top

[Q04] 修改列类型
来源：http://jlg.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bde.ydjk.org.cn

[Q05] 重命名列
来源：http://uba.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jgg.sjlbkw.cn

[Q06] 删除列
来源：http://nog.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://dgs.yuanzhike.top

[Q07] 删除表
来源：http://mxo.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://bcb.redwolf501.top

[Q08] 创建普通索引
来源：http://olx.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vqc.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://iag.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://inb.yueranfly.top

[Q10] 插入单行
来源：http://sfo.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iud.jinqigufen.top

[Q11] 一次插入多行
来源：http://lry.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nnx.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://drv.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vvu.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qxm.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://pad.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hwo.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://con.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zkk.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pzo.gaohongyu789.top

[Q15] 查询全部
来源：http://npt.zycfv.cn

SELECT * FROM users;
来源：http://iqd.sysykeji.top

[Q16] 查询指定列
来源：http://xuy.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://sfo.redwolf501.top

[Q17] 条件查询
来源：http://llz.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ibf.iojbl.cn

[Q18] 模糊匹配
来源：http://fpl.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qss.svipenyu.cn

[Q19] 范围查询
来源：http://msu.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jja.nwbrower.top

[Q20] IN 列表
来源：http://yfe.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ygp.daxiang520.top

[Q21] 空值判断
来源：http://esy.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://inb.xuetiantiany.cn

[Q22] 排序
来源：http://edw.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oyi.zdbjq.cn

[Q23] 分页
来源：http://dio.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://apw.yj20258.top

[Q24] 去重
来源：http://hww.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://hjo.fanxiaobao.xyz

[Q25] 只取前 N 条
来源：http://mdk.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://seq.hesvh.cn

[Q26] 计数
来源：http://tfz.nwbrower.top

SELECT COUNT(*) FROM users;
来源：http://hhz.shangyingyoupin.top

[Q27] 条件计数
来源：http://mrv.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xzm.yonumen.top

[Q28] 求和与平均
来源：http://isw.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sph.xylfe.cn

[Q29] 最大最小值
来源：http://igc.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jid.shuidangran.top

[Q30] 分组统计
来源：http://zll.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qif.meibo888.top

[Q31] 分组后过滤
来源：http://lmr.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hjp.uphjek.com

[Q32] 分组拼接字符串
来源：http://skp.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://afp.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pio.pengpengdd.cyou

[Q33] 多列分组
来源：http://nqr.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://off.zhoulong.xyz

[Q34] 每组取第一条
来源：http://whu.yvedp.cn

SELECT * FROM (
来源：http://npm.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ced.sufxvd.cn

) t WHERE rn = 1;
来源：http://lrx.hnxiangtu.top

[Q35] 内连接
来源：http://hqo.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ano.gaohongyu789.top

[Q36] 左连接
来源：http://jrt.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://stt.zdqjudy.top

[Q37] 右连接
来源：http://gzf.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://quq.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://vdo.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eiw.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://cou.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xgd.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bks.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rec.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uyl.feifeiyinyue.top

[Q41] 多表连接
来源：http://nkk.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://cqr.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://vwo.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://ral.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://ieo.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://ecd.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fny.xuanzx.com

[Q43] 标量子查询
来源：http://pld.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hfg.cdnleiting.top

[Q44] IN 子查询
来源：http://ppi.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uwa.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://oiw.zdbjq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rnf.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://odf.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppp.zdqjudy.top

[Q47] 与平均值比较
来源：http://ukw.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xvi.yonumen.top

[Q48] CTE 公用表表达式
来源：http://ohp.fzhhl.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://akv.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://nxq.meibo888.top

[Q49] 更新单行
来源：http://kxz.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kwy.zhengqikj.top

[Q50] 批量更新
来源：http://qec.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://edd.yuxming.cn

[Q51] 用子查询更新
来源：http://pqs.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jtt.dashuyun.cn

[Q52] 删除指定行
来源：http://hsx.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://ayr.xylfe.cn

[Q53] 按条件删除
来源：http://ppl.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zts.gaohongyu789.top

[Q54] 清空表
来源：http://ysi.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://xzi.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://wpj.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nud.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://uaf.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uvx.gzhubu.top

[Q57] 行号
来源：http://kgf.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dwb.fanxiaobao.xyz

[Q58] 累计求和
来源：http://jzh.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mmp.hongshengwenyu.top

[Q59] 分组内累计
来源：http://dvk.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xzq.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://toy.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://chg.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fkc.yfazqb.com

[Q61] 移动平均
来源：http://wgw.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cvw.snrcjt.cn

[Q62] 分组占比
来源：http://gjm.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cxg.ehwqpu.com

[Q63] 开启事务
来源：http://iqs.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dcg.sysykeji.top

[Q64] 提交事务
来源：http://tds.9152youxi.cn

COMMIT;
来源：http://rfz.kuanghao11.cn

[Q65] 回滚事务
来源：http://fkd.meibo888.top

ROLLBACK;
来源：http://mcp.cucudq.cn

[Q66] 行锁查询
来源：http://rat.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yjr.yvedp.cn

[Q67] 设置隔离级别
来源：http://tqw.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lvm.zhiwuduotai.top

[Q68] 保存点
来源：http://eeg.ehwqpu.com

SAVEPOINT sp1;
来源：http://vtu.gzhubu.top

ROLLBACK TO sp1;
来源：http://vih.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://odb.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xvv.ppjwa.cn

[Q70] 更新统计信息
来源：http://otn.sysykeji.top

ANALYZE TABLE users;
来源：http://pox.yanxiufei.cn

[Q71] 查看建表语句
来源：http://lnr.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nsp.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://ddc.yvedp.cn

SHOW INDEX FROM users;
来源：http://eqw.hfpthk.cn

[Q73] 查看表状态
来源：http://dag.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iic.hesvh.cn

[Q74] 强制使用索引
来源：http://rlj.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://syz.hnqzz.top

[Q75] 日期格式化
来源：http://tpm.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hhj.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kth.zhixingplan.top

[Q76] 按天统计
来源：http://fpu.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://llw.yj202588.top

[Q77] 时间加减
来源：http://ezn.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://izb.bbcook.cn

[Q78] 当前时间
来源：http://kfx.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://paw.zdbjq.cn

[Q79] 字符串拼接
来源：http://zsd.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cno.hnqzz.top

[Q80] 字符串截取
来源：http://lrs.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://txx.chenjidiqi.icu

[Q81] 字符串替换
来源：http://qod.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://njm.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://jfl.sweek.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xyk.svipenyu.cn

[Q83] 大小写转换
来源：http://dwa.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ull.ctjpmb.com

[Q84] 去除首尾空格
来源：http://zrz.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://hyi.shanyushiyangtech.top

[Q85] 数值取整
来源：http://osv.sxryk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gtc.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://xdl.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ggj.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://rfp.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wui.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://pmm.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ccb.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pqv.zdqjudy.top

[Q89] 判断表是否存在
来源：http://vgu.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dva.cheryme.top

[Q90] 生成序号列
来源：http://kla.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbv.sysykeji.top

================================================================================
来源：http://ibh.cqqwz.cn

R. Bash 专题
来源：http://dui.fzhhl.top

================================================================================
来源：http://sis.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://ljs.cdnleiting.top

#!/usr/bin/env bash
来源：http://yxq.shuidangran.top

set -euo pipefail
来源：http://rel.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://ozc.chenzaomai.com

name="Tom"; echo "$name"
来源：http://qqq.bjfxy.top

[R03] 只读变量
来源：http://qky.xuetiantiany.cn

readonly PI=3.14
来源：http://wsn.ydjk.org.cn

[R04] 位置参数
来源：http://cku.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ihp.xuanzx.com

[R05] 参数默认值
来源：http://jvt.yj20258888.top

name="${1:-default}"
来源：http://gwi.9152youxi.cn

[R06] 判断命令是否存在
来源：http://bph.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xmj.xuetiantiany.cn

[R07] if 判断文件
来源：http://ror.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tjj.pengpengdd.cyou

[R08] 数值比较
来源：http://vvq.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jtg.bjfxy.top

[R09] 字符串比较
来源：http://tja.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://muy.fengsongda.top

[R10] 正则匹配
来源：http://fhq.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dnj.chenjidiqi.icu

[R11] case 多分支
来源：http://fkc.birdmap.top


<!-- 参考信息 -->