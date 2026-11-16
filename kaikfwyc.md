代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://grs.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rhs.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qib.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yrc.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://scb.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://doi.ctjpmb.com

[P03] 生成短随机字符串
来源：http://wdz.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://puo.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kfm.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eec.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bms.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xcf.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://czh.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://hrc.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dky.iojbl.cn

[P04] 求长度
来源：http://uzi.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ixc.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvz.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfy.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qrq.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://fkx.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://gnz.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://ygo.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://heo.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://hgr.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://hol.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oed.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://abu.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ufc.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mmv.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://ret.ivvv.top

Ruby: a == b
来源：http://yzm.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vgv.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ypr.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sag.tanke756.top

PHP:  if (empty($x)) {}
来源：http://zmm.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gwb.zdqjudy.top

TS:   if (x == null) {}
来源：http://kto.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uob.hfpthk.cn

Go:   if x == nil {}
来源：http://gfp.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gwy.smart0.xyz

C#:   if (x is null) {}
来源：http://wnh.nanxuanxn.top

[P07] 防抖与节流
来源：http://pem.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gpt.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://ztk.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpj.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uut.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qbj.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kek.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://soc.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jzg.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://frc.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dqc.pengpengdd.cyou

PHP:  bcadd("0.1", "0.2", 2);
来源：http://prb.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gth.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uhp.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://flj.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lfd.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ngk.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yjs.nanxinkj.top

================================================================================
来源：http://xtv.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pxd.0kj1m.cn

================================================================================
来源：http://ndd.iojbl.cn

[Q01] 创建表
来源：http://khe.pycfn.com

CREATE TABLE users (
来源：http://njo.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zms.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://uyq.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://lag.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tjk.cashguo.top

);
来源：http://rsq.yfazqb.com

[Q02] 创建带外键的表
来源：http://asd.cashguo.top

CREATE TABLE orders (
来源：http://gbx.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbn.yfazqb.com

user_id INT NOT NULL,
来源：http://brn.yonumen.top

amount DECIMAL(10, 2),
来源：http://zjj.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qgl.nanxuanxn.top

);
来源：http://bke.birdmap.top

[Q03] 增加列
来源：http://hjv.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eaz.fehbvm.com

[Q04] 修改列类型
来源：http://ymg.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dkd.52xcode.cn

[Q05] 重命名列
来源：http://xxa.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://asv.gzhubu.top

[Q06] 删除列
来源：http://rqe.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://tco.mhx1999.top

[Q07] 删除表
来源：http://fql.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://qmn.zhixingplan.top

[Q08] 创建普通索引
来源：http://mxh.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://azj.cheryme.top

[Q09] 创建唯一索引
来源：http://ost.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://btt.ctjpmb.com

[Q10] 插入单行
来源：http://bxr.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jat.zhengqikj.top

[Q11] 一次插入多行
来源：http://fto.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qvq.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://mtt.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iux.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gfl.ehwqpu.com

[Q13] 忽略重复插入
来源：http://sew.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mgc.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://yac.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sam.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tuh.guowangkeji.top

[Q15] 查询全部
来源：http://wtp.nanxinkj.top

SELECT * FROM users;
来源：http://yjc.sjlbkw.cn

[Q16] 查询指定列
来源：http://cct.9152youxi.cn

SELECT id, name FROM users;
来源：http://uod.havefunace.top

[Q17] 条件查询
来源：http://ctg.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xck.sysykeji.top

[Q18] 模糊匹配
来源：http://mtl.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://okq.ctjpmb.com

[Q19] 范围查询
来源：http://gue.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mms.hfpthk.cn

[Q20] IN 列表
来源：http://ftx.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iar.vqdsnc.cn

[Q21] 空值判断
来源：http://acg.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ppy.zdqjudy.top

[Q22] 排序
来源：http://jaa.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eez.wangdashe.top

[Q23] 分页
来源：http://ipu.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tkl.tianlin.xyz

[Q24] 去重
来源：http://edb.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://epc.jiagoushi.top

[Q25] 只取前 N 条
来源：http://crl.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iji.meibo888.top

[Q26] 计数
来源：http://lwl.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://ono.shangyingyoupin.top

[Q27] 条件计数
来源：http://fqw.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bdr.c1oappe.top

[Q28] 求和与平均
来源：http://wbt.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://noi.sxryk.cn

[Q29] 最大最小值
来源：http://hhr.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://thl.gzhubu.top

[Q30] 分组统计
来源：http://ykl.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qev.yj202588.top

[Q31] 分组后过滤
来源：http://zux.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppv.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://fzv.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hmi.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kdb.0kj1m.cn

[Q33] 多列分组
来源：http://snu.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gks.jianghu66.top

[Q34] 每组取第一条
来源：http://opx.redwolf501.top

SELECT * FROM (
来源：http://ecj.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ddm.kuanghao11.cn

) t WHERE rn = 1;
来源：http://nar.dianchejie.cn

[Q35] 内连接
来源：http://vsh.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://owq.tarul.cn

[Q36] 左连接
来源：http://ejx.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yqa.kuanghao11.cn

[Q37] 右连接
来源：http://mnu.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jws.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://umy.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bmr.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://stj.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aja.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://awz.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://epb.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ctu.xziqi.cn

[Q41] 多表连接
来源：http://ndv.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://spe.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://vcp.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://fvj.jinghuilouyu.cn

[Q42] 连接条件附加过滤
来源：http://yft.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://kih.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wty.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://crr.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://edz.chenzaomai.com

[Q44] IN 子查询
来源：http://vhb.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rvx.meibo888.top

[Q45] EXISTS 判断存在
来源：http://rlt.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://syp.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://wkg.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tqc.svipenyu.cn

[Q47] 与平均值比较
来源：http://noy.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pfr.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://bqi.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://imo.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://vue.zhixingplan.top

[Q49] 更新单行
来源：http://sus.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://whx.jinqigfzy.top

[Q50] 批量更新
来源：http://nwn.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://onr.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://uov.xingfuxueyuan.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qig.cashguo.top

[Q52] 删除指定行
来源：http://wiz.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://ugy.xziqi.cn

[Q53] 按条件删除
来源：http://dri.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hej.gogol.net.cn

[Q54] 清空表
来源：http://tqr.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://mwj.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://hap.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iug.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://lzq.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kke.hcnkem.com

[Q57] 行号
来源：http://ign.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xxn.52xcode.cn

[Q58] 累计求和
来源：http://qjb.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sik.svipenyu.cn

[Q59] 分组内累计
来源：http://zuz.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gco.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://fxp.yj20258888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fzl.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rna.ehwqpu.com

[Q61] 移动平均
来源：http://iwj.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qkv.zycfv.cn

[Q62] 分组占比
来源：http://ezw.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wyn.tianlin.xyz

[Q63] 开启事务
来源：http://koa.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sst.gzhubu.top

[Q64] 提交事务
来源：http://csa.meibo888.top

COMMIT;
来源：http://arv.pycfn.com

[Q65] 回滚事务
来源：http://gwi.gotoacloud.top

ROLLBACK;
来源：http://bni.ehwqpu.com

[Q66] 行锁查询
来源：http://uks.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ovx.zhixingplan.top

[Q67] 设置隔离级别
来源：http://qvk.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rft.ctjpmb.com

[Q68] 保存点
来源：http://zcu.zhoulong.xyz

SAVEPOINT sp1;
来源：http://eyg.yangfankeji.com

ROLLBACK TO sp1;
来源：http://hrv.jinqigfzy.top

[Q69] 查看执行计划
来源：http://cnz.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lnn.jiagoushi.top

[Q70] 更新统计信息
来源：http://tcy.zdqjudy.top

ANALYZE TABLE users;
来源：http://kdj.9152youxi.cn

[Q71] 查看建表语句
来源：http://hls.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ktd.bjfxy.top

[Q72] 查看索引
来源：http://qla.wangdashe.top

SHOW INDEX FROM users;
来源：http://eki.jyoumei.cn

[Q73] 查看表状态
来源：http://drf.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bcr.shzxlz.cn

[Q74] 强制使用索引
来源：http://eps.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zzn.52xcode.cn

[Q75] 日期格式化
来源：http://ucl.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://axu.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://odd.sysykeji.top

[Q76] 按天统计
来源：http://wus.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://arr.yvedp.cn

[Q77] 时间加减
来源：http://ame.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uad.zycfv.cn

[Q78] 当前时间
来源：http://uqu.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tfo.yj20258888.top

[Q79] 字符串拼接
来源：http://gvx.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ksq.hcnkem.com

[Q80] 字符串截取
来源：http://npz.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://evg.hesvh.cn

[Q81] 字符串替换
来源：http://zyy.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cid.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://liu.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://czz.fengsongda.top

[Q83] 大小写转换
来源：http://jim.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jka.zhengqikj.top

[Q84] 去除首尾空格
来源：http://xkx.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://bfd.cqqwz.cn

[Q85] 数值取整
来源：http://iwi.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eih.cqqwz.cn

[Q86] 读取 JSON 字段
来源：http://ecq.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nmt.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://iqu.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eul.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://hxh.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dji.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tpy.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://aye.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rua.yanxiufei.cn

[Q90] 生成序号列
来源：http://osq.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vfh.daria6918.cn

================================================================================
来源：http://std.cdnleiting.top

R. Bash 专题
来源：http://dqf.fehbvm.com

================================================================================
来源：http://apt.chenlongwang.top

[R01] shebang 与严格模式
来源：http://udw.ppjwa.cn

#!/usr/bin/env bash
来源：http://aoj.jlsjyb.cn

set -euo pipefail
来源：http://fqp.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://oil.birdmap.top

name="Tom"; echo "$name"
来源：http://zle.hfpthk.cn

[R03] 只读变量
来源：http://qii.hfpthk.cn

readonly PI=3.14
来源：http://mtr.fanxiaobao.xyz

[R04] 位置参数
来源：http://lbw.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eid.ybcxt.top

[R05] 参数默认值
来源：http://jdm.jlsjyb.cn

name="${1:-default}"
来源：http://fhc.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://kua.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://npi.vehdjk.com

[R07] if 判断文件
来源：http://kqs.feifeiyinyue.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kal.hesvh.cn

[R08] 数值比较
来源：http://oaa.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wxg.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://vmk.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://buv.zhiwuduotai.top

[R10] 正则匹配
来源：http://hny.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gil.wangshuangyany.cn

[R11] case 多分支
来源：http://ekw.meibo888.top

case "$1" in
来源：http://ibl.epnwcf.com

start) echo "启动" ;;
来源：http://qyc.daria6918.cn

stop)  echo "停止" ;;
来源：http://fyc.sxryk.cn

*)     echo "未知命令" ;;
来源：http://wmz.jinqigufen.top

esac
来源：http://tvm.fzhhl.top

[R12] for 遍历文件
来源：http://wll.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://egj.chenzaomai.com

[R13] for 计数循环
来源：http://zyi.zhaomingkeji.xyz


<!-- 参考信息 -->