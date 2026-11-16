代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yel.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://czv.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bap.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vyc.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fot.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zrs.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://tfj.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nfx.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tbe.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tka.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bnj.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://big.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://trk.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lxt.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ncf.gzhubu.top

[P04] 求长度
来源：http://kbv.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://won.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hmj.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cce.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fom.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://ahh.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://ium.yangfankeji.com

Ruby: x.length;  x.size
来源：http://apc.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://huw.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://ccp.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://trg.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ucj.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://etb.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uxp.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://csj.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qaf.xylfe.cn

Ruby: a == b
来源：http://syj.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ymo.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vtu.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kpx.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://mki.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mbr.aibaodan.cn

TS:   if (x == null) {}
来源：http://dgy.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wlm.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://jmu.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://knt.chenlongwang.top

C#:   if (x is null) {}
来源：http://aqf.tarul.cn

[P07] 防抖与节流
来源：http://tnw.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lqt.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://ixi.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmd.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfg.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zrd.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kmd.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nzg.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xzn.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://zge.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://znc.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jzb.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wua.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sbt.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kpz.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cyv.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wxw.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mvn.sxryk.cn

================================================================================
来源：http://tuf.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ifg.jlsjyb.cn

================================================================================
来源：http://aic.0kj1m.cn

[Q01] 创建表
来源：http://gyu.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://day.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xaa.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://rjx.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://gjq.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xsx.sweek.top

);
来源：http://fao.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://jdi.pycfn.com

CREATE TABLE orders (
来源：http://zqd.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vow.tian-w.cn

user_id INT NOT NULL,
来源：http://kzv.yj20258.top

amount DECIMAL(10, 2),
来源：http://adn.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ghu.52xcode.cn

);
来源：http://edr.snrcjt.cn

[Q03] 增加列
来源：http://jtd.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qjr.zdbjq.cn

[Q04] 修改列类型
来源：http://djt.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qpt.shuidangran.top

[Q05] 重命名列
来源：http://rah.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://meg.bbcook.cn

[Q06] 删除列
来源：http://msc.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vvc.yvedp.cn

[Q07] 删除表
来源：http://zsf.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://vpa.cucudq.cn

[Q08] 创建普通索引
来源：http://xvq.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xan.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://okm.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://thv.hnxiangtu.top

[Q10] 插入单行
来源：http://goj.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cge.ydjk.org.cn

[Q11] 一次插入多行
来源：http://hxv.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sap.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://euz.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pnz.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nky.gogol.net.cn

[Q13] 忽略重复插入
来源：http://qyf.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://psc.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://pvp.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://buo.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://muw.kuanghao11.cn

[Q15] 查询全部
来源：http://usd.tarul.cn

SELECT * FROM users;
来源：http://zxi.jianghu66.top

[Q16] 查询指定列
来源：http://xpd.jqgfzy.top

SELECT id, name FROM users;
来源：http://mvx.nanxinkj.top

[Q17] 条件查询
来源：http://uop.hnqzz.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iml.chenzaomai.com

[Q18] 模糊匹配
来源：http://drf.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eob.havefunace.top

[Q19] 范围查询
来源：http://kvf.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wsj.feifeiyinyue.top

[Q20] IN 列表
来源：http://gut.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ozt.cucudq.cn

[Q21] 空值判断
来源：http://umf.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tnc.jinqigfzy.top

[Q22] 排序
来源：http://zos.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://epb.pycfn.com

[Q23] 分页
来源：http://jdm.cucudq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ohp.jinqigufen.top

[Q24] 去重
来源：http://zyf.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://wcn.nwbrower.top

[Q25] 只取前 N 条
来源：http://pde.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ceq.haohaochexian.top

[Q26] 计数
来源：http://mgn.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://mkl.yj20258888.top

[Q27] 条件计数
来源：http://mzb.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://znf.guowangkeji.top

[Q28] 求和与平均
来源：http://smg.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zmg.yj202588.top

[Q29] 最大最小值
来源：http://hpj.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gcs.nwbrower.top

[Q30] 分组统计
来源：http://jjb.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://byp.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://gcd.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ztr.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://mhf.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mir.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lqh.guowangkeji.top

[Q33] 多列分组
来源：http://ega.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rlq.shuidangran.top

[Q34] 每组取第一条
来源：http://dsq.tarul.cn

SELECT * FROM (
来源：http://ubi.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kdm.cheryme.top

) t WHERE rn = 1;
来源：http://yue.316326.xyz

[Q35] 内连接
来源：http://urh.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dcs.fktsv.cn

[Q36] 左连接
来源：http://mwo.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uvs.nanxuanxn.top

[Q37] 右连接
来源：http://hzj.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yir.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://buk.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ztv.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://txg.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dsp.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qhq.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fke.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jdx.uphjek.com

[Q41] 多表连接
来源：http://vvs.316326.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://pdo.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://uzq.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://gzb.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://xsd.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://bcn.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lza.yangfankeji.com

[Q43] 标量子查询
来源：http://ayh.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gxo.52xcode.cn

[Q44] IN 子查询
来源：http://utq.sweek.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lfh.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://yfh.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jrd.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://hmq.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nld.redwolf501.top

[Q47] 与平均值比较
来源：http://lpp.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sxr.yongpay.top

[Q48] CTE 公用表表达式
来源：http://gkn.bjfxy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://chs.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://vvy.jyoumei.cn

[Q49] 更新单行
来源：http://vfl.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://taf.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://pwi.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://plr.sysykeji.top

[Q51] 用子查询更新
来源：http://ysr.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kvg.cashguo.top

[Q52] 删除指定行
来源：http://kjy.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://zem.nanxinkj.top

[Q53] 按条件删除
来源：http://ggh.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oqh.mhx1999.top

[Q54] 清空表
来源：http://vsz.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://cob.yj20258.top

[Q55] 排名（并列占位）
来源：http://xuo.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bcv.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://koj.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nmo.shzxlz.cn

[Q57] 行号
来源：http://vaz.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jga.epnwcf.com

[Q58] 累计求和
来源：http://wfb.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hew.iojbl.cn

[Q59] 分组内累计
来源：http://gyr.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yyq.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://xbv.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ace.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hgz.zhiwuduotai.top

[Q61] 移动平均
来源：http://bry.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hux.fktsv.cn

[Q62] 分组占比
来源：http://zwd.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://djm.hywenlv.cn

[Q63] 开启事务
来源：http://rxb.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://huh.jinghuilouyu.cn

[Q64] 提交事务
来源：http://hhk.ctjpmb.com

COMMIT;
来源：http://ira.kuanghao11.cn

[Q65] 回滚事务
来源：http://pqm.smart0.xyz

ROLLBACK;
来源：http://qiw.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://zsj.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dth.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://fwv.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yzk.gogol.net.cn

[Q68] 保存点
来源：http://mpv.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://uch.xziqi.cn

ROLLBACK TO sp1;
来源：http://jlp.ivvv.top

[Q69] 查看执行计划
来源：http://bjw.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qkd.wangdashe.top

[Q70] 更新统计信息
来源：http://bgz.ctjpmb.com

ANALYZE TABLE users;
来源：http://bud.zhixingplan.top

[Q71] 查看建表语句
来源：http://axq.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aks.mhx1999.top

[Q72] 查看索引
来源：http://rgu.9152youxi.cn

SHOW INDEX FROM users;
来源：http://opc.aibaodan.cn

[Q73] 查看表状态
来源：http://tql.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gkn.zhixingplan.top

[Q74] 强制使用索引
来源：http://wfw.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rlw.hammf.cn

[Q75] 日期格式化
来源：http://jcb.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ugn.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gie.xuanzx.com

[Q76] 按天统计
来源：http://umb.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ffm.c1oappe.top

[Q77] 时间加减
来源：http://qhg.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jzh.birdmap.top

[Q78] 当前时间
来源：http://tps.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tba.zhengqikj.top

[Q79] 字符串拼接
来源：http://mqm.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yry.jqgfzy.top

[Q80] 字符串截取
来源：http://czo.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jew.nanxuanxn.top

[Q81] 字符串替换
来源：http://lqt.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vsz.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://lwq.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bmy.yueranfly.top

[Q83] 大小写转换
来源：http://xjh.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xjr.shuidangran.top

[Q84] 去除首尾空格
来源：http://mke.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://tbu.yj20258888.top

[Q85] 数值取整
来源：http://wqz.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zlq.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://kez.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lmn.pycfn.com

[Q87] JSON 字段做条件
来源：http://duh.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vuv.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://mml.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oxy.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rhh.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://vjk.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lks.kuanghao11.cn

[Q90] 生成序号列
来源：http://jiz.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vae.jyoumei.cn

================================================================================
来源：http://fjb.guowangkeji.top

R. Bash 专题
来源：http://ybo.mhx1999.top

================================================================================
来源：http://mnv.jinqigufen.top

[R01] shebang 与严格模式
来源：http://ktu.iojbl.cn

#!/usr/bin/env bash
来源：http://kwo.dashuyun.cn

set -euo pipefail
来源：http://vdm.0kj1m.cn

[R02] 变量赋值与使用
来源：http://rll.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://epl.gaohongyu789.top

[R03] 只读变量
来源：http://eof.mhx1999.top

readonly PI=3.14
来源：http://gsi.ydjk.org.cn

[R04] 位置参数
来源：http://fnh.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxx.pycfn.com

[R05] 参数默认值
来源：http://adl.uphjek.com

name="${1:-default}"
来源：http://azl.nanxinkj.top

[R06] 判断命令是否存在
来源：http://vnw.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://opp.hywenlv.cn

[R07] if 判断文件
来源：http://hec.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dfn.uphjek.com

[R08] 数值比较
来源：http://kze.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eop.zhoulong.xyz

[R09] 字符串比较
来源：http://dqj.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssi.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://bnr.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oep.meibo888.top

[R11] case 多分支
来源：http://nxd.gogol.net.cn

case "$1" in
来源：http://tgt.zdbjq.cn

start) echo "启动" ;;
来源：http://wdr.ctjpmb.com

stop)  echo "停止" ;;
来源：http://bex.epnwcf.com

*)     echo "未知命令" ;;
来源：http://wvl.iojbl.cn

esac
来源：http://zbe.zhixingplan.top

[R12] for 遍历文件
来源：http://ped.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://pdl.bjfxy.top

[R13] for 计数循环
来源：http://ufu.bjfxy.top


<!-- 参考信息 -->