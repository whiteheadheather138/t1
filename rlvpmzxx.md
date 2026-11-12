代发 wailian999

TS:   // child_process / cluster 模块
来源：http://jcp.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://flc.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fxr.hcnkem.com

Ruby: // fork 块
来源：http://vtp.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://mvf.gaohongyu789.top

================================================================================
来源：http://bum.zhengqikj.top

P. 常用工具函数
来源：http://dgv.jlsjyb.cn

================================================================================
来源：http://vns.wangshuangyany.cn

[P01] 生成 UUID
来源：http://mav.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://mbr.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zxy.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://thi.daxiang520.top

TS:   crypto.randomUUID()
来源：http://lft.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://kya.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://udr.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://dmr.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://qoq.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://ejy.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yuq.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zxp.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yvk.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ksi.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kbt.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lpe.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wgg.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zsn.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://wqs.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ius.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://osg.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kwg.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfg.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://onq.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://spg.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kmy.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://skb.ywan-chungtsiang.top

[P04] 求长度
来源：http://uht.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cjo.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gnh.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://huz.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kwn.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://lnv.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://vlw.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://uai.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ozb.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://pjm.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iof.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pla.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ypn.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://waq.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nus.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mfy.birdmap.top

Ruby: a == b
来源：http://oje.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://efb.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zps.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hut.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://rtv.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jii.havefunace.top

TS:   if (x == null) {}
来源：http://wuo.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://feq.zhijiandao.cn

Go:   if x == nil {}
来源：http://hvr.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hmq.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://igg.zhiwuduotai.top

[P07] 防抖与节流
来源：http://ddy.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ogs.yonumen.top

PHP:  // 手写时间戳比较
来源：http://nvg.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cye.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ylx.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uwl.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lwy.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ahj.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cbl.yj20258888.top

[P08] 处理浮点精度问题
来源：http://yeu.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lis.hongshengwenyu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ztg.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qiz.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nos.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kdu.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sry.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ish.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eov.guannengcc.top

================================================================================
来源：http://svb.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vdf.sweek.top

================================================================================
来源：http://ifp.wangdashe.top

[Q01] 创建表
来源：http://oel.daria6918.cn

CREATE TABLE users (
来源：http://ndd.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://evi.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://krn.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://jrs.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ixx.smart0.xyz

);
来源：http://vpw.sweek.top

[Q02] 创建带外键的表
来源：http://tak.ctjpmb.com

CREATE TABLE orders (
来源：http://hrg.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggl.yj20258888.top

user_id INT NOT NULL,
来源：http://inn.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://myn.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lon.ivvv.top

);
来源：http://ssc.jqgufenzy.top

[Q03] 增加列
来源：http://zst.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dfe.fktsv.cn

[Q04] 修改列类型
来源：http://fka.gotoacloud.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fen.fengsongda.top

[Q05] 重命名列
来源：http://auh.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nwt.haohaochexian.top

[Q06] 删除列
来源：http://oya.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://xal.jinyuanbaomall.cn

[Q07] 删除表
来源：http://qla.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://xbk.yanxiufei.cn

[Q08] 创建普通索引
来源：http://vlv.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://flr.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://izj.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ens.vehdjk.com

[Q10] 插入单行
来源：http://sxt.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yps.nanxuanxn.top

[Q11] 一次插入多行
来源：http://yhe.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ctf.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://yyl.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://jew.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aae.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://yob.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lit.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://fim.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bnh.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cyp.yj20258888.top

[Q15] 查询全部
来源：http://ocr.hesvh.cn

SELECT * FROM users;
来源：http://ilc.xuanzx.com

[Q16] 查询指定列
来源：http://jiw.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://ykj.daria6918.cn

[Q17] 条件查询
来源：http://jno.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://drp.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://yik.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://esd.fanxiaobao.xyz

[Q19] 范围查询
来源：http://acj.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lmn.cdnleiting.top

[Q20] IN 列表
来源：http://oeu.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kfd.aibaodan.cn

[Q21] 空值判断
来源：http://pwi.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://baj.hcnkem.com

[Q22] 排序
来源：http://huq.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qon.hammf.cn

[Q23] 分页
来源：http://znl.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wxj.sweek.top

[Q24] 去重
来源：http://tht.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://mtl.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://ysn.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nbc.hysaishi.cn

[Q26] 计数
来源：http://tci.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://eac.yueranfly.top

[Q27] 条件计数
来源：http://hhi.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jac.guowangkeji.top

[Q28] 求和与平均
来源：http://vkp.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vyo.yangfankeji.com

[Q29] 最大最小值
来源：http://efp.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xad.ybcxt.top

[Q30] 分组统计
来源：http://xki.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rgm.svipenyu.cn

[Q31] 分组后过滤
来源：http://rzv.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ipp.yj20258888.top

[Q32] 分组拼接字符串
来源：http://xvv.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hzv.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xgw.bbcook.cn

[Q33] 多列分组
来源：http://dlf.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tdg.hnqzz.top

[Q34] 每组取第一条
来源：http://jfk.gaohongyu789.top

SELECT * FROM (
来源：http://yet.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hab.yuxming.cn

) t WHERE rn = 1;
来源：http://nmm.yvedp.cn

[Q35] 内连接
来源：http://buy.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hnr.feifeiyinyue.top

[Q36] 左连接
来源：http://rpc.ppjwa.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wiq.aizwys.cn

[Q37] 右连接
来源：http://dgw.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jli.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lnn.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://twn.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://ykd.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wcg.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jfd.fengsongda.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lbh.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lth.tarul.cn

[Q41] 多表连接
来源：http://meb.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qyc.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://nkh.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://rnn.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://vbk.nwbrower.top

SELECT u.name, o.amount FROM users u
来源：http://pom.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qtc.ydjk.org.cn

[Q43] 标量子查询
来源：http://vih.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cpb.jianghu66.top

[Q44] IN 子查询
来源：http://mcm.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rhx.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://kmk.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xlf.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qfo.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsk.redwolf501.top

[Q47] 与平均值比较
来源：http://yfg.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wbc.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://gfk.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kin.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://nqq.jyoumei.cn

[Q49] 更新单行
来源：http://ikt.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://afq.ydzc1.top

[Q50] 批量更新
来源：http://rmn.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mlf.gogol.net.cn

[Q51] 用子查询更新
来源：http://pfi.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvy.mhx1999.top

[Q52] 删除指定行
来源：http://fqi.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://akm.snrcjt.cn

[Q53] 按条件删除
来源：http://zdk.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ucx.fanxiaobao.xyz

[Q54] 清空表
来源：http://gli.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://fos.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://puu.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wbm.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://fau.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zkr.quarkkingdee.top

[Q57] 行号
来源：http://czf.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://igu.wangdashe.top

[Q58] 累计求和
来源：http://qto.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fhq.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://fds.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ujb.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://unu.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uoi.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpo.jinqigufen.top

[Q61] 移动平均
来源：http://lyr.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mel.guannengcc.top

[Q62] 分组占比
来源：http://pdi.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nbo.hysaishi.cn

[Q63] 开启事务
来源：http://qgo.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://szh.hnqzz.top

[Q64] 提交事务
来源：http://hne.nwbrower.top

COMMIT;
来源：http://fhx.cucudq.cn

[Q65] 回滚事务
来源：http://fkl.guowangkeji.top

ROLLBACK;
来源：http://gbf.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://pya.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zad.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://ufb.cashguo.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://myx.wangdashe.top

[Q68] 保存点
来源：http://hwf.wangdashe.top

SAVEPOINT sp1;
来源：http://phi.zhixingplan.top

ROLLBACK TO sp1;
来源：http://usr.dianchejie.cn

[Q69] 查看执行计划
来源：http://ary.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nnj.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://ank.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://igw.jqgufenzy.top

[Q71] 查看建表语句
来源：http://wue.tian-w.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hhs.kuanghao11.cn

[Q72] 查看索引
来源：http://ihd.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://lsr.jqgfzy.top

[Q73] 查看表状态
来源：http://gmu.wangdashe.top

SHOW TABLE STATUS LIKE 'users';
来源：http://peo.hfpthk.cn

[Q74] 强制使用索引
来源：http://unt.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hhc.andypj.xyz

[Q75] 日期格式化
来源：http://ltb.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wky.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bef.zhijiandao.cn

[Q76] 按天统计
来源：http://qxc.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rok.jinqigfzy.top

[Q77] 时间加减
来源：http://xde.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jgd.yj20258.top

[Q78] 当前时间
来源：http://pjv.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bcw.fktsv.cn

[Q79] 字符串拼接
来源：http://bip.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://exr.gogol.net.cn

[Q80] 字符串截取
来源：http://rrt.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mzc.shuidangran.top

[Q81] 字符串替换
来源：http://btn.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ynj.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://pso.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nxd.yfazqb.com

[Q83] 大小写转换
来源：http://awa.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bod.yfazqb.com

[Q84] 去除首尾空格
来源：http://juz.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://whj.chenjidiqi.icu

[Q85] 数值取整
来源：http://fzp.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://efj.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://tyy.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gjy.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://bns.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ork.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://dox.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dfe.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mnx.yangfankeji.com

[Q89] 判断表是否存在
来源：http://gyf.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fsv.cdnleiting.top

[Q90] 生成序号列
来源：http://flv.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dfo.jinqigfzy.top

================================================================================
来源：http://szt.0kj1m.cn

R. Bash 专题
来源：http://bkd.sysykeji.top

================================================================================
来源：http://rop.zhixingplan.top

[R01] shebang 与严格模式
来源：http://qhc.hnxiangtu.top

#!/usr/bin/env bash
来源：http://zrm.cheryme.top

set -euo pipefail
来源：http://nyf.cqqwz.cn

[R02] 变量赋值与使用
来源：http://qaz.birdmap.top

name="Tom"; echo "$name"
来源：http://bmo.jqgfzy.top

[R03] 只读变量
来源：http://luw.gotoacloud.top

readonly PI=3.14
来源：http://qoa.yongpay.top

[R04] 位置参数
来源：http://dvr.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edk.zhiwuduotai.top

[R05] 参数默认值
来源：http://wjk.shanyushiyangkeji.top


<!-- 参考信息 -->