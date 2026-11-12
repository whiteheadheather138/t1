代发 wailian999

[P01] 生成 UUID
来源：http://nrp.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://rwo.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gxl.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://osk.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://dnq.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://vra.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://ghs.pycfn.com

Ruby: SecureRandom.uuid
来源：http://zfx.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://kvf.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://sog.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hbu.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bzr.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ioq.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bwf.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hzu.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ygu.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bxj.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sid.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://wyh.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aip.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jnw.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cvq.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ftk.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vcf.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rsg.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://brk.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pcd.jinqigfzy.top

[P04] 求长度
来源：http://nth.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bfy.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzc.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gug.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://svd.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://puz.yuxming.cn

Go:   len(arr);  len(m)
来源：http://pcy.yj202588.top

Ruby: x.length;  x.size
来源：http://wuy.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://brz.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://uef.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pff.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mds.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysj.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://liv.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qgx.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://izu.hammf.cn

Ruby: a == b
来源：http://yby.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mrq.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nke.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tnh.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://ujr.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nvs.snrcjt.cn

TS:   if (x == null) {}
来源：http://zuh.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gsk.zycfv.cn

Go:   if x == nil {}
来源：http://fxo.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rva.cdnleiting.top

C#:   if (x is null) {}
来源：http://nnx.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://gal.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://csp.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://rjs.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ehq.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://coq.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pqz.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://auz.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eva.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qcd.fktsv.cn

[P08] 处理浮点精度问题
来源：http://rro.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kem.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lzr.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gfh.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vxt.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tse.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zzq.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qvq.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eow.zhongyouzk.top

================================================================================
来源：http://pno.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vea.yueranfly.top

================================================================================
来源：http://joc.yj20258.top

[Q01] 创建表
来源：http://ivc.daria6918.cn

CREATE TABLE users (
来源：http://shm.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xvl.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://utk.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://ecf.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dqn.hcnkem.com

);
来源：http://atw.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://qnz.yvedp.cn

CREATE TABLE orders (
来源：http://bwq.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ygd.yonumen.top

user_id INT NOT NULL,
来源：http://pjl.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://dec.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nrt.dianchejie.cn

);
来源：http://uph.yj202588.top

[Q03] 增加列
来源：http://pxh.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bml.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://nuf.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lkg.chenjidiqi.icu

[Q05] 重命名列
来源：http://ima.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zyl.tanke756.top

[Q06] 删除列
来源：http://dfl.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nuu.xinyue.icu

[Q07] 删除表
来源：http://gdv.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://lme.zdbjq.cn

[Q08] 创建普通索引
来源：http://sks.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://boa.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://wkq.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mwj.yuxming.cn

[Q10] 插入单行
来源：http://tap.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sik.svipenyu.cn

[Q11] 一次插入多行
来源：http://xok.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zby.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://amx.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://caz.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ucb.c1oappe.top

[Q13] 忽略重复插入
来源：http://cjc.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mrm.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://ges.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://znk.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fyo.andypj.xyz

[Q15] 查询全部
来源：http://dou.bbcook.cn

SELECT * FROM users;
来源：http://miu.meibo888.top

[Q16] 查询指定列
来源：http://eqv.52xcode.cn

SELECT id, name FROM users;
来源：http://mmf.yueranfly.top

[Q17] 条件查询
来源：http://oul.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fel.epnwcf.com

[Q18] 模糊匹配
来源：http://ikp.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://loy.cucudq.cn

[Q19] 范围查询
来源：http://sha.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hfx.zdqjudy.top

[Q20] IN 列表
来源：http://ygz.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pey.zhengqikj.top

[Q21] 空值判断
来源：http://tme.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://qtb.hammf.cn

[Q22] 排序
来源：http://tkb.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvh.jiagoushi.top

[Q23] 分页
来源：http://zyk.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kch.yj20258888.top

[Q24] 去重
来源：http://axy.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://edv.yonumen.top

[Q25] 只取前 N 条
来源：http://rtf.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sbx.xziqi.cn

[Q26] 计数
来源：http://ckh.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://qbb.redwolf501.top

[Q27] 条件计数
来源：http://zdb.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qne.shangyingyoupin.top

[Q28] 求和与平均
来源：http://hnt.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xia.jianghu66.top

[Q29] 最大最小值
来源：http://xyk.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mnc.jlsjyb.cn

[Q30] 分组统计
来源：http://dvd.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gct.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://lyk.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qpg.andypj.xyz

[Q32] 分组拼接字符串
来源：http://svz.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wrj.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wsf.hysaishi.cn

[Q33] 多列分组
来源：http://nqr.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jcz.tian-w.cn

[Q34] 每组取第一条
来源：http://vku.52xcode.cn

SELECT * FROM (
来源：http://mbb.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://psi.yj20258888.top

) t WHERE rn = 1;
来源：http://xee.pengpengdd.cyou

[Q35] 内连接
来源：http://zkp.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wvr.iojbl.cn

[Q36] 左连接
来源：http://qlc.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xkm.shanyushiyangtech.top

[Q37] 右连接
来源：http://lec.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lfd.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://dgs.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://end.yonumen.top

[Q39] 自连接（查上下级）
来源：http://ipn.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sck.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lvx.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://opf.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://juy.zhixingplan.top

[Q41] 多表连接
来源：http://eoj.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jse.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://mxu.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://sue.hammf.cn

[Q42] 连接条件附加过滤
来源：http://buh.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://wkz.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://spe.yueranfly.top

[Q43] 标量子查询
来源：http://fhz.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tft.hnqzz.top

[Q44] IN 子查询
来源：http://nmp.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wzd.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://hyx.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ljy.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mzl.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zvn.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://pjd.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://luw.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://twn.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bbq.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://vys.ehwqpu.com

[Q49] 更新单行
来源：http://qmm.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wst.aizwys.cn

[Q50] 批量更新
来源：http://pyt.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lpe.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://grf.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://irl.uphjek.com

[Q52] 删除指定行
来源：http://ktc.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://bpk.xylfe.cn

[Q53] 按条件删除
来源：http://tbo.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kzw.yj20258.top

[Q54] 清空表
来源：http://oir.hesvh.cn

TRUNCATE TABLE logs;
来源：http://vea.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://ozi.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eau.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://xlu.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qxr.wangshuangyany.cn

[Q57] 行号
来源：http://hgu.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eei.zhiwuduotai.top

[Q58] 累计求和
来源：http://jsp.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hbw.xinyue.icu

[Q59] 分组内累计
来源：http://zac.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://llw.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://wvi.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jzl.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tiz.tanke756.top

[Q61] 移动平均
来源：http://hzv.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eia.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://uzv.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fbg.jqgfzy.top

[Q63] 开启事务
来源：http://zdr.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oyi.meibo888.top

[Q64] 提交事务
来源：http://dif.sxryk.cn

COMMIT;
来源：http://xhl.sweek.top

[Q65] 回滚事务
来源：http://zhs.ydzc1.top

ROLLBACK;
来源：http://fxy.hnqzz.top

[Q66] 行锁查询
来源：http://syr.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pck.xziqi.cn

[Q67] 设置隔离级别
来源：http://lnq.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bmg.cheryme.top

[Q68] 保存点
来源：http://ynf.sweek.top

SAVEPOINT sp1;
来源：http://myh.zhengqikj.top

ROLLBACK TO sp1;
来源：http://sbo.quarkkingdee.top

[Q69] 查看执行计划
来源：http://fgc.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tbe.snrcjt.cn

[Q70] 更新统计信息
来源：http://zgk.yj202588.top

ANALYZE TABLE users;
来源：http://uba.cheryme.top

[Q71] 查看建表语句
来源：http://htp.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yqd.dashuyun.cn

[Q72] 查看索引
来源：http://ieb.tarul.cn

SHOW INDEX FROM users;
来源：http://kii.haohaochexian.top

[Q73] 查看表状态
来源：http://ymn.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cjg.xylfe.cn

[Q74] 强制使用索引
来源：http://ghb.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xjo.gotoacloud.top

[Q75] 日期格式化
来源：http://kqj.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sfb.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://taa.hesvh.cn

[Q76] 按天统计
来源：http://rcx.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://boj.sxryk.cn

[Q77] 时间加减
来源：http://hih.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bei.jianghu66.top

[Q78] 当前时间
来源：http://keb.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nar.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://tbl.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xym.hcnkem.com

[Q80] 字符串截取
来源：http://wmw.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mam.tian-w.cn

[Q81] 字符串替换
来源：http://yvd.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ati.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://ehg.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gtn.9152youxi.cn

[Q83] 大小写转换
来源：http://cyw.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ozw.cheryme.top

[Q84] 去除首尾空格
来源：http://zfu.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://nnx.ivvv.top

[Q85] 数值取整
来源：http://bsc.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nqn.pycfn.com

[Q86] 读取 JSON 字段
来源：http://shf.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fnw.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://gdf.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qrn.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://age.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tug.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zpn.hesvh.cn

[Q89] 判断表是否存在
来源：http://oel.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fcg.uphjek.com

[Q90] 生成序号列
来源：http://tjd.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lbx.birdmap.top

================================================================================
来源：http://sgc.cheryme.top

R. Bash 专题
来源：http://evf.guowangkeji.top

================================================================================
来源：http://nxa.ivvv.top

[R01] shebang 与严格模式
来源：http://jjg.cucudq.cn

#!/usr/bin/env bash
来源：http://hsr.jlsjyb.cn

set -euo pipefail
来源：http://sxg.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://yjg.yfazqb.com

name="Tom"; echo "$name"
来源：http://huc.shzxlz.cn

[R03] 只读变量
来源：http://gqq.jinqigfzy.top

readonly PI=3.14
来源：http://slb.jlsjyb.cn

[R04] 位置参数
来源：http://yna.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jui.guannengcc.top

[R05] 参数默认值
来源：http://ykp.hesvh.cn

name="${1:-default}"
来源：http://zss.yongpay.top

[R06] 判断命令是否存在
来源：http://sbh.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://abz.0kj1m.cn

[R07] if 判断文件
来源：http://aut.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oid.andypj.xyz

[R08] 数值比较
来源：http://jnv.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fkq.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://ayw.daxiang520.top


<!-- 参考信息 -->