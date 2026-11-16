代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://luw.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://twc.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qdh.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gid.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nxf.xingfuxueyuan.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rpd.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://znh.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nck.xziqi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nuh.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vxm.jyoumei.cn

[P03] 生成短随机字符串
来源：http://lnw.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kpx.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://izn.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://efs.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xky.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://trn.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jlk.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://han.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tlq.zhixingplan.top

[P04] 求长度
来源：http://awf.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgs.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ypp.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://diy.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ete.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://gqh.epnwcf.com

Go:   len(arr);  len(m)
来源：http://fig.nwbrower.top

Ruby: x.length;  x.size
来源：http://cmb.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jnx.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://kzi.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zwb.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ihy.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hap.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hlb.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tvc.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://fqq.fzhhl.top

Ruby: a == b
来源：http://irc.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xux.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uou.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://czc.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://gtw.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fmc.daxiang520.top

TS:   if (x == null) {}
来源：http://dvj.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uxm.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://npd.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ovs.quarkkingdee.top

C#:   if (x is null) {}
来源：http://lfv.ctjpmb.com

[P07] 防抖与节流
来源：http://akx.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dee.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://slm.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fot.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hku.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wsm.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://chq.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jsr.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gsz.yj20258.top

[P08] 处理浮点精度问题
来源：http://huu.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wex.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lvx.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://afd.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gpr.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rfi.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yzw.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ujq.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://stn.0kj1m.cn

================================================================================
来源：http://krn.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ouh.yanxiufei.cn

================================================================================
来源：http://hgw.hnqzz.top

[Q01] 创建表
来源：http://fyg.zhiwuduotai.top

CREATE TABLE users (
来源：http://qfd.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iig.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://pgd.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://lpj.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lns.xinyue.icu

);
来源：http://qwa.jinqigufen.top

[Q02] 创建带外键的表
来源：http://bbs.tanke756.top

CREATE TABLE orders (
来源：http://alf.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wrr.jiagoushi.top

user_id INT NOT NULL,
来源：http://fan.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://qla.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lti.yongpay.top

);
来源：http://amk.xinyue.icu

[Q03] 增加列
来源：http://gwb.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jij.xinyue.icu

[Q04] 修改列类型
来源：http://ktu.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sew.guowangkeji.top

[Q05] 重命名列
来源：http://yia.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lym.nanxinkj.top

[Q06] 删除列
来源：http://qqc.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://zxr.smart0.xyz

[Q07] 删除表
来源：http://sew.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://txy.iojbl.cn

[Q08] 创建普通索引
来源：http://ohd.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jfb.meibo888.top

[Q09] 创建唯一索引
来源：http://rjf.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nly.ivvv.top

[Q10] 插入单行
来源：http://ywn.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zzw.haohaochexian.top

[Q11] 一次插入多行
来源：http://gsx.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fmw.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://sen.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://cnj.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hrs.gogol.net.cn

[Q13] 忽略重复插入
来源：http://jhy.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lws.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://rsb.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hgn.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sqg.tian-w.cn

[Q15] 查询全部
来源：http://ljz.havefunace.top

SELECT * FROM users;
来源：http://ous.ybcxt.top

[Q16] 查询指定列
来源：http://mge.ppjwa.cn

SELECT id, name FROM users;
来源：http://ffo.yongpay.top

[Q17] 条件查询
来源：http://jbs.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bnn.316326.xyz

[Q18] 模糊匹配
来源：http://eub.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ymx.9152youxi.cn

[Q19] 范围查询
来源：http://jfz.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://haw.hysaishi.cn

[Q20] IN 列表
来源：http://tlc.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jkb.xuanzx.com

[Q21] 空值判断
来源：http://txf.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tqp.yj20258888.top

[Q22] 排序
来源：http://fyi.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mti.hongshengwenyu.top

[Q23] 分页
来源：http://kro.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wfg.chenzaomai.com

[Q24] 去重
来源：http://vlf.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://enm.guowangkeji.top

[Q25] 只取前 N 条
来源：http://qlk.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yyk.hysaishi.cn

[Q26] 计数
来源：http://tbr.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://sfs.jqgufenzy.top

[Q27] 条件计数
来源：http://rdu.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ziu.hammf.cn

[Q28] 求和与平均
来源：http://fno.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tsi.mhx1999.top

[Q29] 最大最小值
来源：http://sao.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://itb.sxryk.cn

[Q30] 分组统计
来源：http://zlw.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nla.andypj.xyz

[Q31] 分组后过滤
来源：http://lie.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pre.hcnkem.com

[Q32] 分组拼接字符串
来源：http://lwl.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bmj.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tga.xuetiantiany.cn

[Q33] 多列分组
来源：http://pkp.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vmx.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://gfe.hammf.cn

SELECT * FROM (
来源：http://bbb.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ude.cqqwz.cn

) t WHERE rn = 1;
来源：http://iff.yj202588.top

[Q35] 内连接
来源：http://psp.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wfl.ybcxt.top

[Q36] 左连接
来源：http://vdj.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pwh.yuanzhike.top

[Q37] 右连接
来源：http://fhp.vehdjk.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mvj.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vgm.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nna.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://shm.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mok.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xjw.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://imx.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ooj.bbcook.cn

[Q41] 多表连接
来源：http://iuy.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nno.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://akd.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://tzk.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://nut.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://jok.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vwe.tarul.cn

[Q43] 标量子查询
来源：http://qpf.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://udn.chenjidiqi.icu

[Q44] IN 子查询
来源：http://exh.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gzl.316326.xyz

[Q45] EXISTS 判断存在
来源：http://osw.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mbl.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://frh.epnwcf.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xwl.shuidangran.top

[Q47] 与平均值比较
来源：http://gft.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uyj.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://qcl.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bwe.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://eda.tanke756.top

[Q49] 更新单行
来源：http://jge.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ehv.yueranfly.top

[Q50] 批量更新
来源：http://dip.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nxh.xinyue.icu

[Q51] 用子查询更新
来源：http://hvc.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcd.cdnleiting.top

[Q52] 删除指定行
来源：http://ehp.zhoulong.xyz

DELETE FROM users WHERE id = 10;
来源：http://bnp.andypj.xyz

[Q53] 按条件删除
来源：http://ryi.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kzo.jyoumei.cn

[Q54] 清空表
来源：http://ara.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://sok.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://sod.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fon.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://ekl.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ojk.yuxming.cn

[Q57] 行号
来源：http://fsu.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avf.aizwys.cn

[Q58] 累计求和
来源：http://gha.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zrs.tarul.cn

[Q59] 分组内累计
来源：http://wam.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cyb.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://pkp.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://urd.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zdc.yueranfly.top

[Q61] 移动平均
来源：http://poa.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nog.jqgufenzy.top

[Q62] 分组占比
来源：http://ofu.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cpk.vqdsnc.cn

[Q63] 开启事务
来源：http://adg.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://mzr.dashuyun.cn

[Q64] 提交事务
来源：http://bfn.gogol.net.cn

COMMIT;
来源：http://thp.yangfankeji.com

[Q65] 回滚事务
来源：http://bjk.jinqigfzy.top

ROLLBACK;
来源：http://hjp.jianghu66.top

[Q66] 行锁查询
来源：http://juz.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ujh.birdmap.top

[Q67] 设置隔离级别
来源：http://vfo.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wnq.cqqwz.cn

[Q68] 保存点
来源：http://jvi.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://xrz.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://ldt.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://bug.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qfg.52xcode.cn

[Q70] 更新统计信息
来源：http://pbr.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://ixu.fengsongda.top

[Q71] 查看建表语句
来源：http://kfa.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hbv.aibaodan.cn

[Q72] 查看索引
来源：http://ivw.gogol.net.cn

SHOW INDEX FROM users;
来源：http://cws.zhoulong.xyz

[Q73] 查看表状态
来源：http://gpy.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pzt.hysaishi.cn

[Q74] 强制使用索引
来源：http://evk.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ogo.fehbvm.com

[Q75] 日期格式化
来源：http://yfw.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uty.ybcxt.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cms.hesvh.cn

[Q76] 按天统计
来源：http://any.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zcc.hnxiangtu.top

[Q77] 时间加减
来源：http://bou.mhx1999.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pzh.zhoulong.xyz

[Q78] 当前时间
来源：http://vhk.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hxy.316326.xyz

[Q79] 字符串拼接
来源：http://bax.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cxx.316326.xyz

[Q80] 字符串截取
来源：http://mgx.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yvq.tian-w.cn

[Q81] 字符串替换
来源：http://cjb.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qsa.yj20258.top

[Q82] 字符长度与字节长度
来源：http://ovd.xylfe.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tdk.zycfv.cn

[Q83] 大小写转换
来源：http://vqb.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lpf.gotoacloud.top

[Q84] 去除首尾空格
来源：http://dky.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://xaz.birdmap.top

[Q85] 数值取整
来源：http://gfo.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://apm.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://bzp.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kcn.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://gge.yj202588.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ime.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://vmv.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lqu.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://khg.ydzc1.top

[Q89] 判断表是否存在
来源：http://jna.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://okk.yj202588.top

[Q90] 生成序号列
来源：http://pyb.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qcw.gzhubu.top

================================================================================
来源：http://fes.nwbrower.top

R. Bash 专题
来源：http://ncw.svipenyu.cn

================================================================================
来源：http://lvf.hywenlv.cn

[R01] shebang 与严格模式
来源：http://txz.yj20258888.top

#!/usr/bin/env bash
来源：http://guk.jinqigfzy.top

set -euo pipefail
来源：http://qvu.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://xvo.gzhubu.top

name="Tom"; echo "$name"
来源：http://vul.yj202588.top

[R03] 只读变量
来源：http://hwp.vehdjk.com

readonly PI=3.14
来源：http://krw.chenzaomai.com

[R04] 位置参数
来源：http://vqd.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gqj.yj20258888.top

[R05] 参数默认值
来源：http://who.zhoulong.xyz

name="${1:-default}"
来源：http://lct.haohaochexian.top

[R06] 判断命令是否存在
来源：http://tth.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ops.yj202588.top

[R07] if 判断文件
来源：http://onk.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wsg.havefunace.top

[R08] 数值比较
来源：http://npx.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://him.yj20258.top

[R09] 字符串比较
来源：http://ooe.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mhv.ctjpmb.com

[R10] 正则匹配
来源：http://ivi.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eog.xinyue.icu

[R11] case 多分支
来源：http://lgh.zhiwuduotai.top

case "$1" in
来源：http://uzs.hfpthk.cn

start) echo "启动" ;;
来源：http://bec.mhx1999.top

stop)  echo "停止" ;;
来源：http://wkt.mhx1999.top

*)     echo "未知命令" ;;
来源：http://zwx.dianchejie.cn


<!-- 参考信息 -->