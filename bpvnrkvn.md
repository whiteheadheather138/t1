代发 wailian999

TS:   crypto.randomUUID()
来源：http://ayh.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://ttc.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://tlu.ivvv.top

Ruby: SecureRandom.uuid
来源：http://iop.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://aiz.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://dni.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lgb.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nnk.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yvg.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tnh.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tzg.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://obp.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hbq.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qoc.epnwcf.com

[P03] 生成短随机字符串
来源：http://quq.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qwc.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qig.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xuy.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zty.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ivr.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wcd.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zrf.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eap.ydzc1.top

[P04] 求长度
来源：http://qoq.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tmb.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wfn.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fud.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ckx.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://kgl.yvedp.cn

Go:   len(arr);  len(m)
来源：http://mlk.0kj1m.cn

Ruby: x.length;  x.size
来源：http://lrv.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bls.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://bxq.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ybj.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wcm.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qkp.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hfi.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://und.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://dam.tian-w.cn

Ruby: a == b
来源：http://rqv.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://piu.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://adv.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jdr.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://yll.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kpe.jianghu66.top

TS:   if (x == null) {}
来源：http://xcz.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ioi.fktsv.cn

Go:   if x == nil {}
来源：http://ujr.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gnv.uphjek.com

C#:   if (x is null) {}
来源：http://vny.shuidangran.top

[P07] 防抖与节流
来源：http://zxs.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://esa.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://ito.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vgs.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bls.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hej.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nck.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qct.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jca.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://quq.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sok.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bgy.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cry.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ijt.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pcl.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eez.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aeg.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://suv.pengpengdd.cyou

================================================================================
来源：http://dhp.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tdk.kuanghao11.cn

================================================================================
来源：http://fsx.jqgufenzy.top

[Q01] 创建表
来源：http://ztx.xinyue.icu

CREATE TABLE users (
来源：http://jbc.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bad.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://vwz.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://kxi.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pqp.yuxming.cn

);
来源：http://ror.tanke756.top

[Q02] 创建带外键的表
来源：http://vth.jinqigfzy.top

CREATE TABLE orders (
来源：http://jao.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://unm.zhoulong.xyz

user_id INT NOT NULL,
来源：http://fuy.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://tte.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://byn.quarkkingdee.top

);
来源：http://ybr.daria6918.cn

[Q03] 增加列
来源：http://aqe.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cjv.zhijiandao.cn

[Q04] 修改列类型
来源：http://dvz.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oes.gaohongyu789.top

[Q05] 重命名列
来源：http://jqc.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://grk.sjlbkw.cn

[Q06] 删除列
来源：http://ktk.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bqk.dianchejie.cn

[Q07] 删除表
来源：http://urn.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://der.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://unb.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wko.sxryk.cn

[Q09] 创建唯一索引
来源：http://jvq.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mzf.redwolf501.top

[Q10] 插入单行
来源：http://gst.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kkl.nanxinkj.top

[Q11] 一次插入多行
来源：http://ive.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jmm.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://jrf.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gns.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ndk.sufxvd.cn

[Q13] 忽略重复插入
来源：http://aqe.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gca.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://hwt.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ttx.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gca.xuetiantiany.cn

[Q15] 查询全部
来源：http://zdo.gaohongyu789.top

SELECT * FROM users;
来源：http://yyo.jqgfzy.top

[Q16] 查询指定列
来源：http://bat.wangdashe.top

SELECT id, name FROM users;
来源：http://fzz.zhoulong.xyz

[Q17] 条件查询
来源：http://aaa.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nyb.ivvv.top

[Q18] 模糊匹配
来源：http://irt.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bye.nwbrower.top

[Q19] 范围查询
来源：http://lzo.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lka.dianchejie.cn

[Q20] IN 列表
来源：http://axc.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jog.dashuyun.cn

[Q21] 空值判断
来源：http://hcu.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dlg.zycfv.cn

[Q22] 排序
来源：http://fis.yuxming.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ucm.hesvh.cn

[Q23] 分页
来源：http://vxz.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lyb.snrcjt.cn

[Q24] 去重
来源：http://sbc.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://nzx.sysykeji.top

[Q25] 只取前 N 条
来源：http://erm.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wkh.vqdsnc.cn

[Q26] 计数
来源：http://smd.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://rbc.hcnkem.com

[Q27] 条件计数
来源：http://ckq.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dfo.gaohongyu789.top

[Q28] 求和与平均
来源：http://uge.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cdt.fengsongda.top

[Q29] 最大最小值
来源：http://lsd.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fmc.yonumen.top

[Q30] 分组统计
来源：http://vxv.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jwt.zhongyouzk.top

[Q31] 分组后过滤
来源：http://mog.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nef.aizwys.cn

[Q32] 分组拼接字符串
来源：http://spn.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://woz.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ruj.svipenyu.cn

[Q33] 多列分组
来源：http://vxo.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sea.0kj1m.cn

[Q34] 每组取第一条
来源：http://elo.cheryme.top

SELECT * FROM (
来源：http://cgc.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://koa.jqgufenzy.top

) t WHERE rn = 1;
来源：http://ufi.cqqwz.cn

[Q35] 内连接
来源：http://rkj.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jqc.shzxlz.cn

[Q36] 左连接
来源：http://twt.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bci.snrcjt.cn

[Q37] 右连接
来源：http://skp.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rqq.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://noe.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mkn.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://psv.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kfa.cdnleiting.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oab.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://bja.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qmm.fengsongda.top

[Q41] 多表连接
来源：http://acj.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bxu.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://jbs.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://dkl.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://lgs.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://yet.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vxt.ppjwa.cn

[Q43] 标量子查询
来源：http://qmj.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qqt.xinyue.icu

[Q44] IN 子查询
来源：http://hjd.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://maj.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://tjo.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tnm.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pfs.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tbd.yongpay.top

[Q47] 与平均值比较
来源：http://zek.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tys.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://hhk.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uug.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://xfd.nanxinkj.top

[Q49] 更新单行
来源：http://ygf.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sji.316326.xyz

[Q50] 批量更新
来源：http://dwv.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://exe.daria6918.cn

[Q51] 用子查询更新
来源：http://ujo.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jlz.guannengcc.top

[Q52] 删除指定行
来源：http://ltn.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://jpm.ehwqpu.com

[Q53] 按条件删除
来源：http://nmr.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dxw.zhiwuduotai.top

[Q54] 清空表
来源：http://bkv.jinghuilouyu.cn

TRUNCATE TABLE logs;
来源：http://auf.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://plh.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xay.hammf.cn

[Q56] 密集排名（并列不占位）
来源：http://fjj.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wdt.jqgfzy.top

[Q57] 行号
来源：http://qwd.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uel.hammf.cn

[Q58] 累计求和
来源：http://owp.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rvj.epnwcf.com

[Q59] 分组内累计
来源：http://yhe.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ddx.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://yzv.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tmp.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dzf.ivvv.top

[Q61] 移动平均
来源：http://vln.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qvs.nanxuanxn.top

[Q62] 分组占比
来源：http://oeq.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ptl.svipenyu.cn

[Q63] 开启事务
来源：http://dwz.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lvp.52xcode.cn

[Q64] 提交事务
来源：http://vup.ydjk.org.cn

COMMIT;
来源：http://izb.fengsongda.top

[Q65] 回滚事务
来源：http://dch.sxryk.cn

ROLLBACK;
来源：http://luw.dashuyun.cn

[Q66] 行锁查询
来源：http://rsu.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wbz.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://qqd.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yhq.jinghuilouyu.cn

[Q68] 保存点
来源：http://cxw.bjfxy.top

SAVEPOINT sp1;
来源：http://ctp.svipenyu.cn

ROLLBACK TO sp1;
来源：http://dzi.zhoulong.xyz

[Q69] 查看执行计划
来源：http://bju.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jay.yvedp.cn

[Q70] 更新统计信息
来源：http://rlg.yuanzhike.top

ANALYZE TABLE users;
来源：http://whm.redwolf501.top

[Q71] 查看建表语句
来源：http://snr.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bjl.wangdashe.top

[Q72] 查看索引
来源：http://iza.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://xfr.hesvh.cn

[Q73] 查看表状态
来源：http://yat.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hxl.haohaochexian.top

[Q74] 强制使用索引
来源：http://qut.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qds.dianchejie.cn

[Q75] 日期格式化
来源：http://qaa.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lyg.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bsh.yangfankeji.com

[Q76] 按天统计
来源：http://wge.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yku.haohaochexian.top

[Q77] 时间加减
来源：http://sjt.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nos.shzxlz.cn

[Q78] 当前时间
来源：http://aia.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mnr.uphjek.com

[Q79] 字符串拼接
来源：http://kha.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rev.birdmap.top

[Q80] 字符串截取
来源：http://ool.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cnh.52xcode.cn

[Q81] 字符串替换
来源：http://mul.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dai.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://cko.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mfs.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://syp.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xbu.havefunace.top

[Q84] 去除首尾空格
来源：http://diz.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://qwj.0kj1m.cn

[Q85] 数值取整
来源：http://zrh.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pph.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://das.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wpk.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://lwk.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://etp.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://uuz.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xik.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lyr.dianchejie.cn

[Q89] 判断表是否存在
来源：http://wtb.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gxm.jianghu66.top

[Q90] 生成序号列
来源：http://jfn.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jor.tianlin.xyz

================================================================================
来源：http://azt.jqgfzy.top

R. Bash 专题
来源：http://jcb.shangyingyoupin.top

================================================================================
来源：http://ens.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://hkq.zhongyouzk.top

#!/usr/bin/env bash
来源：http://hwp.gzhubu.top

set -euo pipefail
来源：http://zds.gzhubu.top

[R02] 变量赋值与使用
来源：http://saz.yuxming.cn

name="Tom"; echo "$name"
来源：http://ngk.shanyushiyangkeji.top

[R03] 只读变量
来源：http://tyl.yj20258888.top

readonly PI=3.14
来源：http://sqo.wangdashe.top

[R04] 位置参数
来源：http://jsr.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dmk.fengsongda.top

[R05] 参数默认值
来源：http://iea.haohaochexian.top

name="${1:-default}"
来源：http://vij.hysaishi.cn

[R06] 判断命令是否存在
来源：http://opx.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jxm.svipenyu.cn

[R07] if 判断文件
来源：http://luq.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sva.yj20258888.top

[R08] 数值比较
来源：http://tlo.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://bdz.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://bjz.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oks.bbcook.cn

[R10] 正则匹配
来源：http://smo.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nco.sjlbkw.cn

[R11] case 多分支
来源：http://mmy.kuanghao11.cn


<!-- 参考信息 -->