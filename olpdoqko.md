代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://wan.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://odm.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jmw.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hxo.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rji.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lhe.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vtt.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xav.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hpi.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yhf.yj20258888.top

[P03] 生成短随机字符串
来源：http://myg.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cwj.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rsf.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khw.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mcy.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lzy.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gsy.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aaa.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://isx.yfazqb.com

[P04] 求长度
来源：http://njo.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lvi.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ybf.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zea.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tjm.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://dxl.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://yvy.bjfxy.top

Ruby: x.length;  x.size
来源：http://mvm.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://unm.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://wwj.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sfi.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://htv.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://haa.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oqx.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://agj.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://iyi.52xcode.cn

Ruby: a == b
来源：http://avx.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iqn.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vzm.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qhw.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://fbl.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nde.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://mnc.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iiv.birdmap.top

Go:   if x == nil {}
来源：http://lrk.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kra.cucudq.cn

C#:   if (x is null) {}
来源：http://gyi.ydjk.org.cn

[P07] 防抖与节流
来源：http://nrq.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bhn.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://dnu.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywj.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swx.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ldg.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ggi.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://cbf.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gle.pycfn.com

[P08] 处理浮点精度问题
来源：http://qaa.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vph.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://njr.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vvs.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xiu.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kil.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kst.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mgi.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bls.chenlongwang.top

================================================================================
来源：http://gxb.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://udg.sjlbkw.cn

================================================================================
来源：http://rwv.yanxiufei.cn

[Q01] 创建表
来源：http://ash.hesvh.cn

CREATE TABLE users (
来源：http://uky.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ilw.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://jra.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://xze.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zdn.aibaodan.cn

);
来源：http://fby.mhx1999.top

[Q02] 创建带外键的表
来源：http://lbz.havefunace.top

CREATE TABLE orders (
来源：http://cwr.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpf.mhx1999.top

user_id INT NOT NULL,
来源：http://vwu.cheryme.top

amount DECIMAL(10, 2),
来源：http://ore.tian-w.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://toz.ydjk.org.cn

);
来源：http://rwo.aibaodan.cn

[Q03] 增加列
来源：http://tzr.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lhv.guowangkeji.top

[Q04] 修改列类型
来源：http://jys.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kll.hywenlv.cn

[Q05] 重命名列
来源：http://lhw.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://psm.shzxlz.cn

[Q06] 删除列
来源：http://idc.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://cor.zhixingplan.top

[Q07] 删除表
来源：http://dft.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://kak.cqqwz.cn

[Q08] 创建普通索引
来源：http://xal.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xdq.9152youxi.cn

[Q09] 创建唯一索引
来源：http://tkp.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dyz.fengsongda.top

[Q10] 插入单行
来源：http://uxk.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://csj.zhijiandao.cn

[Q11] 一次插入多行
来源：http://waj.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://alt.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://mzx.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eab.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mon.cheryme.top

[Q13] 忽略重复插入
来源：http://cfe.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lpp.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://vyo.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nyd.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://viv.dashuyun.cn

[Q15] 查询全部
来源：http://cpk.aizwys.cn

SELECT * FROM users;
来源：http://tfq.tianlin.xyz

[Q16] 查询指定列
来源：http://ceu.hcnkem.com

SELECT id, name FROM users;
来源：http://cxt.zhoulong.xyz

[Q17] 条件查询
来源：http://kps.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://drn.jinqigfzy.top

[Q18] 模糊匹配
来源：http://eyr.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gtx.yonumen.top

[Q19] 范围查询
来源：http://cql.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qez.bbcook.cn

[Q20] IN 列表
来源：http://foe.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vfg.zhijiandao.cn

[Q21] 空值判断
来源：http://dij.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://kqq.fanxiaobao.xyz

[Q22] 排序
来源：http://rdt.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://una.tian-w.cn

[Q23] 分页
来源：http://bjz.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://opc.meibo888.top

[Q24] 去重
来源：http://rzp.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://gwi.nanxinkj.top

[Q25] 只取前 N 条
来源：http://zpz.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jku.xuetiantiany.cn

[Q26] 计数
来源：http://esy.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://bzf.quarkkingdee.top

[Q27] 条件计数
来源：http://wdv.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zuw.yangfankeji.com

[Q28] 求和与平均
来源：http://url.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zfk.xziqi.cn

[Q29] 最大最小值
来源：http://acr.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://tio.ppjwa.cn

[Q30] 分组统计
来源：http://zyp.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ino.vqdsnc.cn

[Q31] 分组后过滤
来源：http://ihc.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eoa.jianghu66.top

[Q32] 分组拼接字符串
来源：http://yzx.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mme.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qsz.xziqi.cn

[Q33] 多列分组
来源：http://eey.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yil.yuanzhike.top

[Q34] 每组取第一条
来源：http://jom.hnxiangtu.top

SELECT * FROM (
来源：http://lho.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vhq.xylfe.cn

) t WHERE rn = 1;
来源：http://oro.vqdsnc.cn

[Q35] 内连接
来源：http://pxm.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ulc.aibaodan.cn

[Q36] 左连接
来源：http://qqa.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hdc.nanxuanxn.top

[Q37] 右连接
来源：http://yhb.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mza.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://wgi.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uzh.uphjek.com

[Q39] 自连接（查上下级）
来源：http://hhe.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://plf.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cby.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://wlw.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dhz.yueranfly.top

[Q41] 多表连接
来源：http://pao.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsh.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://ryx.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://jfn.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://hub.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://iis.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yne.hcnkem.com

[Q43] 标量子查询
来源：http://nlv.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lkw.ydzc1.top

[Q44] IN 子查询
来源：http://mqc.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hhy.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://yjw.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jvf.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://ptv.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ntr.quarkkingdee.top

[Q47] 与平均值比较
来源：http://jla.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jvb.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://tcs.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ykk.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://rfc.wangshuangyany.cn

[Q49] 更新单行
来源：http://nhl.quarkkingdee.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vxj.fengsongda.top

[Q50] 批量更新
来源：http://syb.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wiv.svipenyu.cn

[Q51] 用子查询更新
来源：http://eez.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mdv.cdnleiting.top

[Q52] 删除指定行
来源：http://ysy.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://ktf.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://jdj.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uft.aizwys.cn

[Q54] 清空表
来源：http://ajm.guannengcc.top

TRUNCATE TABLE logs;
来源：http://wxd.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://rrv.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dxm.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://het.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ksu.zhixingplan.top

[Q57] 行号
来源：http://juu.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wsb.hfpthk.cn

[Q58] 累计求和
来源：http://nba.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://axq.tanke756.top

[Q59] 分组内累计
来源：http://kpy.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nfa.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://srr.xuetiantiany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwq.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://htz.xuetiantiany.cn

[Q61] 移动平均
来源：http://jbh.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xaq.chenlongwang.top

[Q62] 分组占比
来源：http://yjg.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nne.dianchejie.cn

[Q63] 开启事务
来源：http://zjj.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bqg.snrcjt.cn

[Q64] 提交事务
来源：http://uyv.ywan-chungtsiang.top

COMMIT;
来源：http://wsh.jyoumei.cn

[Q65] 回滚事务
来源：http://nxa.feifeiyinyue.top

ROLLBACK;
来源：http://wct.fengsongda.top

[Q66] 行锁查询
来源：http://ztj.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://caj.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://ifq.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lxf.ivvv.top

[Q68] 保存点
来源：http://avn.quarkkingdee.top

SAVEPOINT sp1;
来源：http://ckg.jinqigufen.top

ROLLBACK TO sp1;
来源：http://avm.chenlongwang.top

[Q69] 查看执行计划
来源：http://qxu.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://far.pycfn.com

[Q70] 更新统计信息
来源：http://qvx.jyoumei.cn

ANALYZE TABLE users;
来源：http://zgv.nanxuanxn.top

[Q71] 查看建表语句
来源：http://ebe.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://awz.sxryk.cn

[Q72] 查看索引
来源：http://inq.hcnkem.com

SHOW INDEX FROM users;
来源：http://otf.fehbvm.com

[Q73] 查看表状态
来源：http://oew.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zdc.daxiang520.top

[Q74] 强制使用索引
来源：http://qvn.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wjb.gaohongyu789.top

[Q75] 日期格式化
来源：http://vfm.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vxd.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ljm.zdqjudy.top

[Q76] 按天统计
来源：http://fto.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://npw.jiagoushi.top

[Q77] 时间加减
来源：http://zmf.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kfw.tian-w.cn

[Q78] 当前时间
来源：http://kka.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hul.cheryme.top

[Q79] 字符串拼接
来源：http://yyb.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hjr.jinqigufen.top

[Q80] 字符串截取
来源：http://qpr.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hqa.cucudq.cn

[Q81] 字符串替换
来源：http://qxt.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://irx.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://mbg.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://imu.yangfankeji.com

[Q83] 大小写转换
来源：http://sgk.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bij.gotoacloud.top

[Q84] 去除首尾空格
来源：http://mvh.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://lvx.dashuyun.cn

[Q85] 数值取整
来源：http://oik.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lek.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://qwz.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ytb.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://bjn.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cev.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://ldz.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gnx.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tzs.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://kuz.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oru.tanke756.top

[Q90] 生成序号列
来源：http://zze.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://axe.jinqigufen.top

================================================================================
来源：http://xgt.jiagoushi.top

R. Bash 专题
来源：http://yku.shzxlz.cn

================================================================================
来源：http://wry.9152youxi.cn

[R01] shebang 与严格模式
来源：http://vfd.c1oappe.top

#!/usr/bin/env bash
来源：http://miv.9152youxi.cn

set -euo pipefail
来源：http://ckw.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://ctc.hysaishi.cn

name="Tom"; echo "$name"
来源：http://kyq.xuetiantiany.cn

[R03] 只读变量
来源：http://szt.cucudq.cn

readonly PI=3.14
来源：http://cqi.quarkkingdee.top

[R04] 位置参数
来源：http://bzy.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ylz.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://pkk.zdbjq.cn

name="${1:-default}"
来源：http://ixq.dianchejie.cn

[R06] 判断命令是否存在
来源：http://jof.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vwy.tarul.cn

[R07] if 判断文件
来源：http://glc.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://url.birdmap.top

[R08] 数值比较
来源：http://pkv.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vqd.xylfe.cn

[R09] 字符串比较
来源：http://lcu.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rvs.yj202588.top

[R10] 正则匹配
来源：http://vqx.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hlm.jinqigufen.top

[R11] case 多分支
来源：http://mlg.hywenlv.cn

case "$1" in
来源：http://ibi.sysykeji.top

start) echo "启动" ;;
来源：http://flw.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://gzz.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://wgq.dianchejie.cn


<!-- 参考信息 -->