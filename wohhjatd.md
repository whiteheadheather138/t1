代发 wailian999

TS:   crypto.randomUUID()
来源：http://lfb.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://ids.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://udm.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://pgl.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://jil.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://qfm.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hef.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cvw.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://afz.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://add.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cyi.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xys.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bvu.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://snn.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://xzt.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mmk.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ykc.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jho.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ebl.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fot.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aww.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://bfc.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://frq.svipenyu.cn

[P04] 求长度
来源：http://ubk.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://luw.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zwt.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xpb.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tom.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://onw.fehbvm.com

Go:   len(arr);  len(m)
来源：http://dfs.gogol.net.cn

Ruby: x.length;  x.size
来源：http://zbg.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nyq.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://bqd.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xlr.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://myd.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pzh.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fpu.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lzy.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gcr.fehbvm.com

Ruby: a == b
来源：http://jrt.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oae.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jfg.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://okk.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://iaa.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://olx.yuxming.cn

TS:   if (x == null) {}
来源：http://yxl.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nej.uphjek.com

Go:   if x == nil {}
来源：http://itq.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zzk.daxiang520.top

C#:   if (x is null) {}
来源：http://dml.haohaochexian.top

[P07] 防抖与节流
来源：http://sbw.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jsn.ivvv.top

PHP:  // 手写时间戳比较
来源：http://qro.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqz.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbp.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kcc.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wpb.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ooc.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hff.wangdashe.top

[P08] 处理浮点精度问题
来源：http://jfc.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zmq.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uam.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tcm.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wma.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rtx.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ivf.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jfj.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uqa.smart0.xyz

================================================================================
来源：http://wau.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yao.yuxming.cn

================================================================================
来源：http://tpn.xylfe.cn

[Q01] 创建表
来源：http://pdf.zhiwuduotai.top

CREATE TABLE users (
来源：http://yfm.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xak.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://ayv.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://pmc.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aiw.zhijiandao.cn

);
来源：http://mrl.c1oappe.top

[Q02] 创建带外键的表
来源：http://wtq.uphjek.com

CREATE TABLE orders (
来源：http://qeu.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://acg.fktsv.cn

user_id INT NOT NULL,
来源：http://gkg.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://jdp.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://exe.shanyushiyangtech.top

);
来源：http://omk.yueranfly.top

[Q03] 增加列
来源：http://nbg.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lfj.jinqigufen.top

[Q04] 修改列类型
来源：http://udb.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ntr.c1oappe.top

[Q05] 重命名列
来源：http://lko.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://set.birdmap.top

[Q06] 删除列
来源：http://cbb.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://nkh.yonumen.top

[Q07] 删除表
来源：http://sek.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://unu.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://ngg.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://npn.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://wco.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xag.cheryme.top

[Q10] 插入单行
来源：http://ycg.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nzu.havefunace.top

[Q11] 一次插入多行
来源：http://lmh.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ifb.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://rtl.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://djp.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ust.hammf.cn

[Q13] 忽略重复插入
来源：http://qgt.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uvb.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://oqc.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mlz.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtj.tanke756.top

[Q15] 查询全部
来源：http://alh.svipenyu.cn

SELECT * FROM users;
来源：http://bur.pycfn.com

[Q16] 查询指定列
来源：http://cwh.xuanzx.com

SELECT id, name FROM users;
来源：http://sts.guowangkeji.top

[Q17] 条件查询
来源：http://gkv.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ppo.gaohongyu789.top

[Q18] 模糊匹配
来源：http://vzw.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hvw.yj20258.top

[Q19] 范围查询
来源：http://nqu.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gxm.chenjidiqi.icu

[Q20] IN 列表
来源：http://ali.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://odx.daxiang520.top

[Q21] 空值判断
来源：http://pro.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ofk.ybcxt.top

[Q22] 排序
来源：http://hmw.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hwd.kuanghao11.cn

[Q23] 分页
来源：http://fui.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yxk.kuanghao11.cn

[Q24] 去重
来源：http://evq.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://uqm.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://oyc.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ess.jianghu66.top

[Q26] 计数
来源：http://yuq.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://qio.hnxiangtu.top

[Q27] 条件计数
来源：http://cvv.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ngu.fzhhl.top

[Q28] 求和与平均
来源：http://whi.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ffp.zhixingplan.top

[Q29] 最大最小值
来源：http://xul.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://uyy.jqgufenzy.top

[Q30] 分组统计
来源：http://gxe.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lor.aibaodan.cn

[Q31] 分组后过滤
来源：http://jan.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pmc.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://vcq.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dci.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ljx.tianlin.xyz

[Q33] 多列分组
来源：http://wxq.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://one.jinqigufen.top

[Q34] 每组取第一条
来源：http://ote.tian-w.cn

SELECT * FROM (
来源：http://bra.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ffu.yueranfly.top

) t WHERE rn = 1;
来源：http://qov.nanxuanxn.top

[Q35] 内连接
来源：http://vhk.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ggl.yj202588.top

[Q36] 左连接
来源：http://yva.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pny.yonumen.top

[Q37] 右连接
来源：http://vsh.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bzj.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sjc.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vdh.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://hhp.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lge.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yqy.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fhp.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qcf.nwbrower.top

[Q41] 多表连接
来源：http://opf.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ryt.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://qsw.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://gnj.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://vko.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://xmz.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gbg.hcnkem.com

[Q43] 标量子查询
来源：http://msd.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qtf.haohaochexian.top

[Q44] IN 子查询
来源：http://mgu.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://unl.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://ofo.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xyk.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://jqu.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nir.zdqjudy.top

[Q47] 与平均值比较
来源：http://srl.sysykeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sam.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://fcx.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dne.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://czf.yuanzhike.top

[Q49] 更新单行
来源：http://awk.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zat.shanyushiyangtech.top

[Q50] 批量更新
来源：http://snq.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cld.cucudq.cn

[Q51] 用子查询更新
来源：http://uxj.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://soc.yongpay.top

[Q52] 删除指定行
来源：http://xmd.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://zxs.cashguo.top

[Q53] 按条件删除
来源：http://hxa.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://epm.cheryme.top

[Q54] 清空表
来源：http://tcy.vehdjk.com

TRUNCATE TABLE logs;
来源：http://mhb.ivvv.top

[Q55] 排名（并列占位）
来源：http://lzk.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cvc.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://zzp.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nxe.shanyushiyangkeji.top

[Q57] 行号
来源：http://ovf.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zfd.yueranfly.top

[Q58] 累计求和
来源：http://oiu.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xpt.yuanzhike.top

[Q59] 分组内累计
来源：http://ebg.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://abm.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://qif.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jyh.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zhf.tarul.cn

[Q61] 移动平均
来源：http://qbz.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lio.aizwys.cn

[Q62] 分组占比
来源：http://hul.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gwz.jiagoushi.top

[Q63] 开启事务
来源：http://cij.jyoumei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mar.ppjwa.cn

[Q64] 提交事务
来源：http://ffs.xingfuxueyuan.xyz

COMMIT;
来源：http://pap.hnxiangtu.top

[Q65] 回滚事务
来源：http://iwp.havefunace.top

ROLLBACK;
来源：http://pco.zycfv.cn

[Q66] 行锁查询
来源：http://lhm.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pwn.sufxvd.cn

[Q67] 设置隔离级别
来源：http://cqc.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jxh.zhongyouzk.top

[Q68] 保存点
来源：http://elu.tian-w.cn

SAVEPOINT sp1;
来源：http://yeq.xylfe.cn

ROLLBACK TO sp1;
来源：http://pqz.sweek.top

[Q69] 查看执行计划
来源：http://amd.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uqf.zhengqikj.top

[Q70] 更新统计信息
来源：http://ocj.xziqi.cn

ANALYZE TABLE users;
来源：http://iin.jlsjyb.cn

[Q71] 查看建表语句
来源：http://eft.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://idf.birdmap.top

[Q72] 查看索引
来源：http://kvx.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://blz.fengsongda.top

[Q73] 查看表状态
来源：http://tqa.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cop.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://usq.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mnv.daria6918.cn

[Q75] 日期格式化
来源：http://xpt.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bur.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fhw.aizwys.cn

[Q76] 按天统计
来源：http://czu.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ofk.zhengqikj.top

[Q77] 时间加减
来源：http://yrb.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oly.ivvv.top

[Q78] 当前时间
来源：http://gbg.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kpr.jinqigfzy.top

[Q79] 字符串拼接
来源：http://zof.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ufa.zhijiandao.cn

[Q80] 字符串截取
来源：http://ujo.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mwu.jqgufenzy.top

[Q81] 字符串替换
来源：http://xws.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jqo.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://bym.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qfh.mhx1999.top

[Q83] 大小写转换
来源：http://miv.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rig.shuidangran.top

[Q84] 去除首尾空格
来源：http://ifo.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://pfj.birdmap.top

[Q85] 数值取整
来源：http://nfi.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dkw.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://hkl.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yzn.cucudq.cn

[Q87] JSON 字段做条件
来源：http://wce.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ppd.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://kib.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pry.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://srz.cqqwz.cn

[Q89] 判断表是否存在
来源：http://qze.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcn.uphjek.com

[Q90] 生成序号列
来源：http://kea.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ndy.xingfuxueyuan.xyz

================================================================================
来源：http://nvq.xuetiantiany.cn

R. Bash 专题
来源：http://ezu.dianchejie.cn

================================================================================
来源：http://etr.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://bmp.hnqzz.top

#!/usr/bin/env bash
来源：http://fpm.yj202588.top

set -euo pipefail
来源：http://csd.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://tjg.ydzc1.top

name="Tom"; echo "$name"
来源：http://npz.ctjpmb.com

[R03] 只读变量
来源：http://dii.zhaomingkeji.xyz

readonly PI=3.14
来源：http://xcq.jyoumei.cn

[R04] 位置参数
来源：http://gmm.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://axq.hnxiangtu.top

[R05] 参数默认值
来源：http://eqy.zhoulong.xyz

name="${1:-default}"
来源：http://qbe.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://hiu.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mlz.fengsongda.top

[R07] if 判断文件
来源：http://cjx.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pct.chenjidiqi.icu

[R08] 数值比较
来源：http://cqm.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zpe.zhongyouzk.top

[R09] 字符串比较
来源：http://lue.shangyingyoupin.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://atu.snrcjt.cn

[R10] 正则匹配
来源：http://khk.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jtq.sweek.top

[R11] case 多分支
来源：http://vgm.pengpengdd.cyou


<!-- 参考信息 -->