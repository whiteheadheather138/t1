代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rlp.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://our.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bze.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wkd.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zfr.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kqn.tanke756.top

[P03] 生成短随机字符串
来源：http://ybb.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://poq.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nnt.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mij.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mow.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xlc.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ykk.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzd.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qlw.fanxiaobao.xyz

[P04] 求长度
来源：http://jfe.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ebi.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxd.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pco.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mxw.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://tqo.hesvh.cn

Go:   len(arr);  len(m)
来源：http://ifc.ctjpmb.com

Ruby: x.length;  x.size
来源：http://zmy.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ahr.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://vlz.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ljm.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wqo.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dhb.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ivc.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tsz.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uxh.quarkkingdee.top

Ruby: a == b
来源：http://ztg.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hus.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://etl.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iog.uphjek.com

PHP:  if (empty($x)) {}
来源：http://bnl.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kgt.bjfxy.top

TS:   if (x == null) {}
来源：http://dgl.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pmq.zycfv.cn

Go:   if x == nil {}
来源：http://mce.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yvs.aizwys.cn

C#:   if (x is null) {}
来源：http://azr.feifeiyinyue.top

[P07] 防抖与节流
来源：http://rpw.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yze.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://kap.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upy.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnf.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fye.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pau.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eeq.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eac.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://oea.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kns.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lwk.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://okt.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nas.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cwu.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://txb.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hnz.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pih.quarkkingdee.top

================================================================================
来源：http://ozi.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mrl.hysaishi.cn

================================================================================
来源：http://bna.zdbjq.cn

[Q01] 创建表
来源：http://spw.yfazqb.com

CREATE TABLE users (
来源：http://uls.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ded.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://nlr.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://fln.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lvg.dianchejie.cn

);
来源：http://rve.jianghu66.top

[Q02] 创建带外键的表
来源：http://edq.nanxinkj.top

CREATE TABLE orders (
来源：http://odi.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qii.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://xns.bjfxy.top

amount DECIMAL(10, 2),
来源：http://zkc.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sft.hywenlv.cn

);
来源：http://uof.hfpthk.cn

[Q03] 增加列
来源：http://etl.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wjz.sufxvd.cn

[Q04] 修改列类型
来源：http://zri.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mfx.jqgufenzy.top

[Q05] 重命名列
来源：http://yza.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mmp.guannengcc.top

[Q06] 删除列
来源：http://skx.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ruy.yj20258.top

[Q07] 删除表
来源：http://cgk.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://jev.hfpthk.cn

[Q08] 创建普通索引
来源：http://zip.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ikv.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://rcz.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vjk.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://kfw.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://guj.nanxinkj.top

[Q11] 一次插入多行
来源：http://iwv.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://acu.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://lzj.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://inn.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ksq.nanxinkj.top

[Q13] 忽略重复插入
来源：http://gdl.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mnb.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://xpn.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tok.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qyl.jlsjyb.cn

[Q15] 查询全部
来源：http://mki.0kj1m.cn

SELECT * FROM users;
来源：http://uvp.nwbrower.top

[Q16] 查询指定列
来源：http://qub.c1oappe.top

SELECT id, name FROM users;
来源：http://uxh.dianchejie.cn

[Q17] 条件查询
来源：http://lqp.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eke.dianchejie.cn

[Q18] 模糊匹配
来源：http://hpy.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kyd.pycfn.com

[Q19] 范围查询
来源：http://miy.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://byn.feifeiyinyue.top

[Q20] IN 列表
来源：http://dle.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lda.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://iyp.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://yro.jinqigfzy.top

[Q22] 排序
来源：http://snn.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jcs.shangyingyoupin.top

[Q23] 分页
来源：http://btq.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xht.shangyingyoupin.top

[Q24] 去重
来源：http://vmw.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://lvq.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://enz.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uzz.sjlbkw.cn

[Q26] 计数
来源：http://qaa.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://dxk.aizwys.cn

[Q27] 条件计数
来源：http://zma.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wge.jiagoushi.top

[Q28] 求和与平均
来源：http://zor.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bom.snrcjt.cn

[Q29] 最大最小值
来源：http://his.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dvz.vqdsnc.cn

[Q30] 分组统计
来源：http://gbb.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fiv.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://xir.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cvs.cucudq.cn

[Q32] 分组拼接字符串
来源：http://ehh.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vlw.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ynh.tarul.cn

[Q33] 多列分组
来源：http://igv.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tpj.shuidangran.top

[Q34] 每组取第一条
来源：http://kwf.jqgfzy.top

SELECT * FROM (
来源：http://cmr.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mbo.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://qfo.tanke756.top

[Q35] 内连接
来源：http://grt.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yjf.tarul.cn

[Q36] 左连接
来源：http://adv.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://brr.mhx1999.top

[Q37] 右连接
来源：http://puh.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hlf.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hhn.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aok.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://aon.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dyw.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rsn.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tkx.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mjj.sysykeji.top

[Q41] 多表连接
来源：http://uyk.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://epp.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://yvj.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://idr.hammf.cn

[Q42] 连接条件附加过滤
来源：http://tdw.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://bdu.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ows.zhengqikj.top

[Q43] 标量子查询
来源：http://qno.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oxp.nanxinkj.top

[Q44] IN 子查询
来源：http://bcy.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sub.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://wns.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cih.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://cia.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nzs.fktsv.cn

[Q47] 与平均值比较
来源：http://dhr.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qki.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://vnq.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tng.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://fin.jqgufenzy.top

[Q49] 更新单行
来源：http://ayw.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xdh.aizwys.cn

[Q50] 批量更新
来源：http://ksn.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uvr.zhongyouzk.top

[Q51] 用子查询更新
来源：http://oxv.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://syf.tianlin.xyz

[Q52] 删除指定行
来源：http://elw.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://suw.birdmap.top

[Q53] 按条件删除
来源：http://vbu.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://szk.zhiwuduotai.top

[Q54] 清空表
来源：http://qum.fengsongda.top

TRUNCATE TABLE logs;
来源：http://jdm.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://qpx.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qrh.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://pht.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yok.shanyushiyangkeji.top

[Q57] 行号
来源：http://ati.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wiw.quarkkingdee.top

[Q58] 累计求和
来源：http://zsj.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://onm.jlsjyb.cn

[Q59] 分组内累计
来源：http://kqx.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qog.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://rnp.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oii.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dlo.cheryme.top

[Q61] 移动平均
来源：http://aea.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://emb.tianlin.xyz

[Q62] 分组占比
来源：http://yil.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vsu.gotoacloud.top

[Q63] 开启事务
来源：http://soz.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pzb.hnqzz.top

[Q64] 提交事务
来源：http://yhw.xziqi.cn

COMMIT;
来源：http://eii.guannengcc.top

[Q65] 回滚事务
来源：http://vcy.xingfuxueyuan.xyz

ROLLBACK;
来源：http://mvw.gogol.net.cn

[Q66] 行锁查询
来源：http://clv.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ree.tarul.cn

[Q67] 设置隔离级别
来源：http://sfh.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gza.birdmap.top

[Q68] 保存点
来源：http://aej.zycfv.cn

SAVEPOINT sp1;
来源：http://hrn.tianlin.xyz

ROLLBACK TO sp1;
来源：http://hae.sweek.top

[Q69] 查看执行计划
来源：http://dbj.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ikm.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://are.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://bfl.ybcxt.top

[Q71] 查看建表语句
来源：http://jfe.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zzh.yj202588.top

[Q72] 查看索引
来源：http://usb.sysykeji.top

SHOW INDEX FROM users;
来源：http://zox.zhijiandao.cn

[Q73] 查看表状态
来源：http://jfk.vehdjk.com

SHOW TABLE STATUS LIKE 'users';
来源：http://tot.jinqigfzy.top

[Q74] 强制使用索引
来源：http://nxq.cucudq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pca.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://rnc.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cbi.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tqg.jinqigufen.top

[Q76] 按天统计
来源：http://chp.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://twg.fktsv.cn

[Q77] 时间加减
来源：http://pxy.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://izz.hywenlv.cn

[Q78] 当前时间
来源：http://xub.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dnx.yj20258.top

[Q79] 字符串拼接
来源：http://nvz.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iff.zycfv.cn

[Q80] 字符串截取
来源：http://rjp.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eus.epnwcf.com

[Q81] 字符串替换
来源：http://xzz.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hqo.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://gyy.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ehv.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://crg.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hcw.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://jgu.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://spm.0kj1m.cn

[Q85] 数值取整
来源：http://cbc.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bgi.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://fra.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aog.havefunace.top

[Q87] JSON 字段做条件
来源：http://hmy.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lji.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://miq.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lqq.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vfr.sufxvd.cn

[Q89] 判断表是否存在
来源：http://ylv.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eiq.hammf.cn

[Q90] 生成序号列
来源：http://bgj.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jja.cdnleiting.top

================================================================================
来源：http://fzo.jqgfzy.top

R. Bash 专题
来源：http://yci.zdqjudy.top

================================================================================
来源：http://cqs.yueranfly.top

[R01] shebang 与严格模式
来源：http://rfm.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://vjq.gotoacloud.top

set -euo pipefail
来源：http://vlh.smart0.xyz

[R02] 变量赋值与使用
来源：http://lku.chenlongwang.top

name="Tom"; echo "$name"
来源：http://sdx.c1oappe.top

[R03] 只读变量
来源：http://gry.hongshengwenyu.top

readonly PI=3.14
来源：http://qzd.bbcook.cn

[R04] 位置参数
来源：http://hst.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qwb.gogol.net.cn

[R05] 参数默认值
来源：http://ktp.sysykeji.top

name="${1:-default}"
来源：http://ccb.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://vvx.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://loe.xuanzx.com

[R07] if 判断文件
来源：http://lgu.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zce.aizwys.cn

[R08] 数值比较
来源：http://amc.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iqj.hcnkem.com

[R09] 字符串比较
来源：http://uoj.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://geo.yangfankeji.com

[R10] 正则匹配
来源：http://xql.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dwf.uphjek.com

[R11] case 多分支
来源：http://ikv.tianlin.xyz

case "$1" in
来源：http://ewb.dianchejie.cn

start) echo "启动" ;;
来源：http://kba.xuanzx.com

stop)  echo "停止" ;;
来源：http://arn.wangdashe.top

*)     echo "未知命令" ;;
来源：http://aig.ydzc1.top

esac
来源：http://wqy.hnqzz.top

[R12] for 遍历文件
来源：http://hqe.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://kqe.gzhubu.top

[R13] for 计数循环
来源：http://xaz.zhijiandao.cn


<!-- 参考信息 -->