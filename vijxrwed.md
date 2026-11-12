代发 wailian999

C#:   Parallel.For
来源：http://ddk.yongpay.top

================================================================================
来源：http://fhv.ivvv.top

P. 常用工具函数
来源：http://fzm.xuanzx.com

================================================================================
来源：http://ket.andypj.xyz

[P01] 生成 UUID
来源：http://gsq.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://cfp.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ppy.guannengcc.top

JS:   crypto.randomUUID()
来源：http://uoh.yj202588.top

TS:   crypto.randomUUID()
来源：http://ihc.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://glx.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://cxt.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://ian.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://dlv.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://ogp.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wbl.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ywv.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hay.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ycs.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lno.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ewo.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zmi.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nsi.yonumen.top

[P03] 生成短随机字符串
来源：http://mcj.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yor.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jfu.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zly.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvk.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ysr.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zjs.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://isl.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mlk.wangshuangyany.cn

[P04] 求长度
来源：http://jrt.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eit.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hjs.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jjp.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frl.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://noi.ydzc1.top

Go:   len(arr);  len(m)
来源：http://bfe.epnwcf.com

Ruby: x.length;  x.size
来源：http://swq.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://kxk.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://dug.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uor.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ytv.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nqu.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zxp.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tuk.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lmh.meibo888.top

Ruby: a == b
来源：http://gza.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fyx.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nmi.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zmu.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://dzr.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vzr.shuidangran.top

TS:   if (x == null) {}
来源：http://nuc.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iig.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://egv.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qzl.jinqigufen.top

C#:   if (x is null) {}
来源：http://oqi.gzhubu.top

[P07] 防抖与节流
来源：http://rof.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zlt.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://kma.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxh.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jra.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lhk.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nbj.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://agp.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mfn.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://dik.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mst.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gyj.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fgy.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ylr.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ouc.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://epq.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://amg.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dni.yonumen.top

================================================================================
来源：http://kvt.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pvi.wangdashe.top

================================================================================
来源：http://uav.sufxvd.cn

[Q01] 创建表
来源：http://eai.jianghu66.top

CREATE TABLE users (
来源：http://zaf.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ecx.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://bwh.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://qyy.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jfi.fzhhl.top

);
来源：http://rsg.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://sdo.shzxlz.cn

CREATE TABLE orders (
来源：http://rbr.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://slv.shzxlz.cn

user_id INT NOT NULL,
来源：http://szu.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://mec.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://brx.zdbjq.cn

);
来源：http://sxt.ydjk.org.cn

[Q03] 增加列
来源：http://dwj.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdq.chenzaomai.com

[Q04] 修改列类型
来源：http://jme.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ljp.jqgfzy.top

[Q05] 重命名列
来源：http://ugn.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xpu.dashuyun.cn

[Q06] 删除列
来源：http://cpy.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://iot.svipenyu.cn

[Q07] 删除表
来源：http://lvs.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://jmp.jqgufenzy.top

[Q08] 创建普通索引
来源：http://aoq.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://nni.yvedp.cn

[Q09] 创建唯一索引
来源：http://hoa.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rge.yonumen.top

[Q10] 插入单行
来源：http://mhd.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cfo.mhx1999.top

[Q11] 一次插入多行
来源：http://phc.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://htz.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://izo.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wvb.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gsv.9152youxi.cn

[Q13] 忽略重复插入
来源：http://gzg.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xgc.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://vni.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bwu.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jqe.xinyue.icu

[Q15] 查询全部
来源：http://hlu.andypj.xyz

SELECT * FROM users;
来源：http://thx.redwolf501.top

[Q16] 查询指定列
来源：http://nad.shuidangran.top

SELECT id, name FROM users;
来源：http://iys.xziqi.cn

[Q17] 条件查询
来源：http://qlu.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iui.yvedp.cn

[Q18] 模糊匹配
来源：http://aab.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://egm.haohaochexian.top

[Q19] 范围查询
来源：http://yng.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fke.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://tjo.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lum.guowangkeji.top

[Q21] 空值判断
来源：http://faw.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gbe.zhaomingkeji.xyz

[Q22] 排序
来源：http://bam.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vol.zhiwuduotai.top

[Q23] 分页
来源：http://sop.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ipj.316326.xyz

[Q24] 去重
来源：http://quq.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://wne.vehdjk.com

[Q25] 只取前 N 条
来源：http://grh.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://txy.vqdsnc.cn

[Q26] 计数
来源：http://yqy.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://pdu.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://mwa.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://psi.chenlongwang.top

[Q28] 求和与平均
来源：http://acb.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uzu.ybcxt.top

[Q29] 最大最小值
来源：http://ujk.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yxr.wangshuangyany.cn

[Q30] 分组统计
来源：http://wqv.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gnm.zycfv.cn

[Q31] 分组后过滤
来源：http://btn.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zey.sxryk.cn

[Q32] 分组拼接字符串
来源：http://akt.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wga.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ucq.0kj1m.cn

[Q33] 多列分组
来源：http://nue.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ivn.hysaishi.cn

[Q34] 每组取第一条
来源：http://fvm.316326.xyz

SELECT * FROM (
来源：http://nug.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ufk.bjfxy.top

) t WHERE rn = 1;
来源：http://ftf.zhoulong.xyz

[Q35] 内连接
来源：http://mtm.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mfk.ivvv.top

[Q36] 左连接
来源：http://ond.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ilr.52xcode.cn

[Q37] 右连接
来源：http://hye.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qog.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://nfv.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uch.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://hdx.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://trb.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ntu.zhiwuduotai.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uwz.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eif.xinyue.icu

[Q41] 多表连接
来源：http://sbv.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fnh.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://wnm.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://vcm.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://tse.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://tjs.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xce.sweek.top

[Q43] 标量子查询
来源：http://dum.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://acb.jlsjyb.cn

[Q44] IN 子查询
来源：http://msf.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wcc.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://qpa.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oip.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://pmc.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jlj.xylfe.cn

[Q47] 与平均值比较
来源：http://whc.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mxe.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://dgq.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ota.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://ckc.redwolf501.top

[Q49] 更新单行
来源：http://vag.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://obd.yongpay.top

[Q50] 批量更新
来源：http://eyq.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mqs.gogol.net.cn

[Q51] 用子查询更新
来源：http://fpq.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mzd.fehbvm.com

[Q52] 删除指定行
来源：http://mzd.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://lrx.wangshuangyany.cn

[Q53] 按条件删除
来源：http://sib.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tia.hcnkem.com

[Q54] 清空表
来源：http://nve.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://fvn.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://vjm.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oyn.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://fif.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://biu.chenjidiqi.icu

[Q57] 行号
来源：http://oie.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dek.hywenlv.cn

[Q58] 累计求和
来源：http://wly.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qpk.jiagoushi.top

[Q59] 分组内累计
来源：http://tng.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lnt.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://qlr.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qxs.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gec.mhx1999.top

[Q61] 移动平均
来源：http://zev.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nhh.hongshengwenyu.top

[Q62] 分组占比
来源：http://tay.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xok.bjfxy.top

[Q63] 开启事务
来源：http://bvb.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fuh.fktsv.cn

[Q64] 提交事务
来源：http://zti.hfpthk.cn

COMMIT;
来源：http://zcz.shuidangran.top

[Q65] 回滚事务
来源：http://xiw.ppjwa.cn

ROLLBACK;
来源：http://cou.andypj.xyz

[Q66] 行锁查询
来源：http://qvq.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jsz.cashguo.top

[Q67] 设置隔离级别
来源：http://kzx.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://thy.daria6918.cn

[Q68] 保存点
来源：http://mwm.svipenyu.cn

SAVEPOINT sp1;
来源：http://fhn.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://rjm.andypj.xyz

[Q69] 查看执行计划
来源：http://lvs.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdx.bjfxy.top

[Q70] 更新统计信息
来源：http://xan.52xcode.cn

ANALYZE TABLE users;
来源：http://juq.ivvv.top

[Q71] 查看建表语句
来源：http://lvy.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bxs.ydzc1.top

[Q72] 查看索引
来源：http://dux.ppjwa.cn

SHOW INDEX FROM users;
来源：http://xoe.iojbl.cn

[Q73] 查看表状态
来源：http://tss.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://abe.daxiang520.top

[Q74] 强制使用索引
来源：http://xwc.xuetiantiany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ipx.sysykeji.top

[Q75] 日期格式化
来源：http://qqm.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eqr.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yay.smart0.xyz

[Q76] 按天统计
来源：http://kyz.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zty.aibaodan.cn

[Q77] 时间加减
来源：http://uhc.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hqo.xinyue.icu

[Q78] 当前时间
来源：http://tww.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jcf.pycfn.com

[Q79] 字符串拼接
来源：http://iax.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dom.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://gnd.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hkb.xylfe.cn

[Q81] 字符串替换
来源：http://mwe.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yoz.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://nwn.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://epn.zhengqikj.top

[Q83] 大小写转换
来源：http://mvq.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pxc.hammf.cn

[Q84] 去除首尾空格
来源：http://hzh.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://drm.zdqjudy.top

[Q85] 数值取整
来源：http://say.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hkp.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://ugi.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://czo.xinyue.icu

[Q87] JSON 字段做条件
来源：http://nfk.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ueb.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://dii.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://udl.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nuv.zdbjq.cn

[Q89] 判断表是否存在
来源：http://bve.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fmj.gzhubu.top

[Q90] 生成序号列
来源：http://fum.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yoq.fzhhl.top

================================================================================
来源：http://hhr.fzhhl.top

R. Bash 专题
来源：http://rat.aibaodan.cn

================================================================================
来源：http://fbs.316326.xyz

[R01] shebang 与严格模式
来源：http://mur.bbcook.cn

#!/usr/bin/env bash
来源：http://xvp.cashguo.top

set -euo pipefail
来源：http://ldr.0kj1m.cn

[R02] 变量赋值与使用
来源：http://ccm.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://rrs.dashuyun.cn

[R03] 只读变量
来源：http://qdj.316326.xyz

readonly PI=3.14
来源：http://rea.nanxinkj.top

[R04] 位置参数
来源：http://uml.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cjr.nwbrower.top

[R05] 参数默认值
来源：http://hak.chenzaomai.com

name="${1:-default}"
来源：http://fyp.zhengqikj.top

[R06] 判断命令是否存在
来源：http://bsg.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jdd.shanyushiyangtech.top

[R07] if 判断文件
来源：http://nkp.nanxinkj.top


<!-- 参考信息 -->