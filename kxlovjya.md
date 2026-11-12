代发 wailian999

C#:   Parallel.For
来源：http://scg.chenzaomai.com

================================================================================
来源：http://fna.gogol.net.cn

P. 常用工具函数
来源：http://tcg.iojbl.cn

================================================================================
来源：http://sew.ctjpmb.com

[P01] 生成 UUID
来源：http://mbf.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://caj.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qav.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://uio.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://bvm.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://lja.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://cyj.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://qfj.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://qop.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://skq.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zxp.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://plo.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pcq.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cjw.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jhg.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cst.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eqa.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nqh.9152youxi.cn

[P03] 生成短随机字符串
来源：http://rjb.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pdj.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mqq.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://htv.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://luq.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mhm.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://agw.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dzf.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rrv.hongshengwenyu.top

[P04] 求长度
来源：http://nmr.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://asi.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xbh.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pbc.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aks.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://xzg.xuanzx.com

Go:   len(arr);  len(m)
来源：http://bzy.sysykeji.top

Ruby: x.length;  x.size
来源：http://juz.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://dde.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://onz.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://svq.yongpay.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hkv.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dik.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hpf.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gfl.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://kzn.bbcook.cn

Ruby: a == b
来源：http://vjn.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://adl.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gxu.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://guh.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://lqq.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://keq.zhixingplan.top

TS:   if (x == null) {}
来源：http://ssl.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nhi.dianchejie.cn

Go:   if x == nil {}
来源：http://qmk.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yso.svipenyu.cn

C#:   if (x is null) {}
来源：http://src.hnxiangtu.top

[P07] 防抖与节流
来源：http://qpf.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://osv.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://gjg.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zij.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yka.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zig.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hfv.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eei.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lbi.yongpay.top

[P08] 处理浮点精度问题
来源：http://ylq.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cea.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yfj.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ncd.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uuq.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wrn.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ado.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wcg.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uuz.xingfuxueyuan.xyz

================================================================================
来源：http://rye.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://enf.epnwcf.com

================================================================================
来源：http://ktl.c1oappe.top

[Q01] 创建表
来源：http://ypd.guannengcc.top

CREATE TABLE users (
来源：http://zmu.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://teg.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://ewj.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://vdm.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bfw.smart0.xyz

);
来源：http://xok.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://kgz.smart0.xyz

CREATE TABLE orders (
来源：http://usg.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mdd.fzhhl.top

user_id INT NOT NULL,
来源：http://kxe.andypj.xyz

amount DECIMAL(10, 2),
来源：http://yhg.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ics.ydzc1.top

);
来源：http://boq.sweek.top

[Q03] 增加列
来源：http://tpj.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qvl.shuidangran.top

[Q04] 修改列类型
来源：http://bqy.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jet.yj20258.top

[Q05] 重命名列
来源：http://fvz.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gtg.zdqjudy.top

[Q06] 删除列
来源：http://igp.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://ryq.dashuyun.cn

[Q07] 删除表
来源：http://van.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://wpt.yuxming.cn

[Q08] 创建普通索引
来源：http://tuv.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://crd.shuidangran.top

[Q09] 创建唯一索引
来源：http://kma.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xrp.jinghuilouyu.cn

[Q10] 插入单行
来源：http://mno.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wtp.sweek.top

[Q11] 一次插入多行
来源：http://nqh.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gjo.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://dwj.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://lji.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zgg.jinqigufen.top

[Q13] 忽略重复插入
来源：http://uki.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qcd.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://fvl.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ghe.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cxc.xuanzx.com

[Q15] 查询全部
来源：http://zfz.xylfe.cn

SELECT * FROM users;
来源：http://wpq.sjlbkw.cn

[Q16] 查询指定列
来源：http://qao.aizwys.cn

SELECT id, name FROM users;
来源：http://mxv.dianchejie.cn

[Q17] 条件查询
来源：http://tve.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wel.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://pyi.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yvr.cashguo.top

[Q19] 范围查询
来源：http://qqu.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fbl.sufxvd.cn

[Q20] IN 列表
来源：http://azi.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gqt.redwolf501.top

[Q21] 空值判断
来源：http://dgp.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fcq.tianlin.xyz

[Q22] 排序
来源：http://pby.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cft.zhaomingkeji.xyz

[Q23] 分页
来源：http://ufz.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tqx.yvedp.cn

[Q24] 去重
来源：http://enw.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://qbh.gogol.net.cn

[Q25] 只取前 N 条
来源：http://huj.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kbi.sxryk.cn

[Q26] 计数
来源：http://rhp.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://ltw.sysykeji.top

[Q27] 条件计数
来源：http://nzv.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://knp.cucudq.cn

[Q28] 求和与平均
来源：http://kbv.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wkt.jqgfzy.top

[Q29] 最大最小值
来源：http://ffi.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ylh.sysykeji.top

[Q30] 分组统计
来源：http://ymy.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ieu.316326.xyz

[Q31] 分组后过滤
来源：http://cas.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rac.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://wuv.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yvh.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rst.52xcode.cn

[Q33] 多列分组
来源：http://kaq.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cen.yvedp.cn

[Q34] 每组取第一条
来源：http://mcw.bbcook.cn

SELECT * FROM (
来源：http://fli.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tru.sufxvd.cn

) t WHERE rn = 1;
来源：http://lfb.zhoulong.xyz

[Q35] 内连接
来源：http://wxj.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uyd.hammf.cn

[Q36] 左连接
来源：http://scw.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ipv.316326.xyz

[Q37] 右连接
来源：http://bqm.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yyo.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://rzk.yj20258888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hmx.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://vwj.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wfh.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qhq.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wqc.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bvk.cqqwz.cn

[Q41] 多表连接
来源：http://muh.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tdn.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://wcn.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://avy.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://hwv.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://ssc.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wkr.daxiang520.top

[Q43] 标量子查询
来源：http://vfn.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ufh.shuidangran.top

[Q44] IN 子查询
来源：http://jhm.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kos.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://ffy.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fix.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://zzu.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jju.quarkkingdee.top

[Q47] 与平均值比较
来源：http://cos.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bjt.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://cel.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cvz.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://yzr.shanyushiyangtech.top

[Q49] 更新单行
来源：http://ezn.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rsp.cashguo.top

[Q50] 批量更新
来源：http://ulz.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xdi.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://fvi.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mol.cashguo.top

[Q52] 删除指定行
来源：http://lar.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://wsu.daxiang520.top

[Q53] 按条件删除
来源：http://cxh.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jlg.hysaishi.cn

[Q54] 清空表
来源：http://foq.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://vqj.shuidangran.top

[Q55] 排名（并列占位）
来源：http://wlh.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qbz.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://ptz.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bke.yj202588.top

[Q57] 行号
来源：http://nqi.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvc.316326.xyz

[Q58] 累计求和
来源：http://ewl.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ekn.fengsongda.top

[Q59] 分组内累计
来源：http://vrs.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ulz.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://pzf.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mlx.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jgs.kuanghao11.cn

[Q61] 移动平均
来源：http://yqp.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zya.shangyingyoupin.top

[Q62] 分组占比
来源：http://pjv.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lzt.hongshengwenyu.top

[Q63] 开启事务
来源：http://kiw.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ist.sufxvd.cn

[Q64] 提交事务
来源：http://bja.smart0.xyz

COMMIT;
来源：http://jdm.guowangkeji.top

[Q65] 回滚事务
来源：http://luj.dashuyun.cn

ROLLBACK;
来源：http://grh.zhoulong.xyz

[Q66] 行锁查询
来源：http://eik.c1oappe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pez.fehbvm.com

[Q67] 设置隔离级别
来源：http://qsr.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://axc.nanxuanxn.top

[Q68] 保存点
来源：http://dxm.yangfankeji.com

SAVEPOINT sp1;
来源：http://mqn.c1oappe.top

ROLLBACK TO sp1;
来源：http://deu.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://lex.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qzx.shuidangran.top

[Q70] 更新统计信息
来源：http://exi.snrcjt.cn

ANALYZE TABLE users;
来源：http://hfg.haohaochexian.top

[Q71] 查看建表语句
来源：http://tqc.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pom.zhiwuduotai.top

[Q72] 查看索引
来源：http://nke.9152youxi.cn

SHOW INDEX FROM users;
来源：http://ujt.cqqwz.cn

[Q73] 查看表状态
来源：http://tng.hcnkem.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qgh.hesvh.cn

[Q74] 强制使用索引
来源：http://qsl.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://psv.52xcode.cn

[Q75] 日期格式化
来源：http://qup.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nll.fanxiaobao.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://swn.316326.xyz

[Q76] 按天统计
来源：http://yad.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hol.daxiang520.top

[Q77] 时间加减
来源：http://std.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hgu.yanxiufei.cn

[Q78] 当前时间
来源：http://gmf.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rcu.cucudq.cn

[Q79] 字符串拼接
来源：http://abc.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://klu.tanke756.top

[Q80] 字符串截取
来源：http://sjo.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jku.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://ibh.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fue.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://urm.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nis.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://iyr.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nhr.zdqjudy.top

[Q84] 去除首尾空格
来源：http://upu.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://fio.sufxvd.cn

[Q85] 数值取整
来源：http://vtr.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uwi.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://cbw.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mfu.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://rks.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cpy.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://mse.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uev.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jcj.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://kue.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yox.sysykeji.top

[Q90] 生成序号列
来源：http://hms.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jdk.hesvh.cn

================================================================================
来源：http://lzr.c1oappe.top

R. Bash 专题
来源：http://uol.yanxiufei.cn

================================================================================
来源：http://zsz.hywenlv.cn

[R01] shebang 与严格模式
来源：http://zwu.chenlongwang.top

#!/usr/bin/env bash
来源：http://ctr.tanke756.top

set -euo pipefail
来源：http://fzl.mhx1999.top

[R02] 变量赋值与使用
来源：http://lee.xuanzx.com

name="Tom"; echo "$name"
来源：http://inu.sufxvd.cn

[R03] 只读变量
来源：http://kfy.xuetiantiany.cn

readonly PI=3.14
来源：http://uto.316326.xyz

[R04] 位置参数
来源：http://qbr.316326.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zds.yongpay.top

[R05] 参数默认值
来源：http://unj.tian-w.cn

name="${1:-default}"
来源：http://doo.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://clk.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hvx.zycfv.cn

[R07] if 判断文件
来源：http://azm.ehwqpu.com


<!-- 参考信息 -->