代发 wailian999

TS:   // child_process / cluster 模块
来源：http://lpc.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oyk.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bds.cashguo.top

Ruby: // fork 块
来源：http://bvi.iojbl.cn

C#:   Parallel.For
来源：http://lid.hnxiangtu.top

================================================================================
来源：http://mmh.dianchejie.cn

P. 常用工具函数
来源：http://oyb.yanxiufei.cn

================================================================================
来源：http://ath.kuanghao11.cn

[P01] 生成 UUID
来源：http://lcc.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://ezd.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yhv.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://hso.redwolf501.top

TS:   crypto.randomUUID()
来源：http://stm.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://djl.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://xwh.sweek.top

Ruby: SecureRandom.uuid
来源：http://cyl.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://rlv.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://afo.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zqi.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mfb.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ucx.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vbz.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ixq.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kba.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hvq.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jhr.yongpay.top

[P03] 生成短随机字符串
来源：http://jba.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rfz.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oew.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://phm.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jao.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://phr.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zra.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bap.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yla.havefunace.top

[P04] 求长度
来源：http://elj.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ssk.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nhr.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gsj.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dbm.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://wgx.yueranfly.top

Go:   len(arr);  len(m)
来源：http://bqu.aibaodan.cn

Ruby: x.length;  x.size
来源：http://tus.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qsk.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://cua.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hhy.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iyn.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wye.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dqj.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tmi.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://guy.hywenlv.cn

Ruby: a == b
来源：http://jst.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufu.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yqv.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vrj.yj20258.top

PHP:  if (empty($x)) {}
来源：http://wdr.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qlw.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://mmg.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lyd.shuidangran.top

Go:   if x == nil {}
来源：http://txv.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gtt.tarul.cn

C#:   if (x is null) {}
来源：http://jru.zhiwuduotai.top

[P07] 防抖与节流
来源：http://dxf.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eco.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://dwc.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jvq.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://caj.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://btb.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ria.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ujh.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wiq.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://ldg.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zri.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bxr.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bdo.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pzc.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvw.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ceq.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dck.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rhy.cucudq.cn

================================================================================
来源：http://sod.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nry.yuxming.cn

================================================================================
来源：http://jqk.fanxiaobao.xyz

[Q01] 创建表
来源：http://tzg.jinqigufen.top

CREATE TABLE users (
来源：http://vex.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ojf.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://bed.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://iev.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jtw.haohaochexian.top

);
来源：http://ubu.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://xmc.sysykeji.top

CREATE TABLE orders (
来源：http://sii.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dip.smart0.xyz

user_id INT NOT NULL,
来源：http://tmn.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://bza.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zdx.hongshengwenyu.top

);
来源：http://dgy.chenlongwang.top

[Q03] 增加列
来源：http://dav.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bwy.ybcxt.top

[Q04] 修改列类型
来源：http://loh.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tha.aibaodan.cn

[Q05] 重命名列
来源：http://ulc.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bvq.shanyushiyangkeji.top

[Q06] 删除列
来源：http://myt.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ppq.cdnleiting.top

[Q07] 删除表
来源：http://imp.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://are.jyoumei.cn

[Q08] 创建普通索引
来源：http://jcs.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wos.fehbvm.com

[Q09] 创建唯一索引
来源：http://cvb.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ymh.ybcxt.top

[Q10] 插入单行
来源：http://awq.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hyf.yvedp.cn

[Q11] 一次插入多行
来源：http://gtf.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gtc.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://bwl.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://okz.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qbw.haohaochexian.top

[Q13] 忽略重复插入
来源：http://tal.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bzk.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://xae.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pik.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ddd.guannengcc.top

[Q15] 查询全部
来源：http://gro.xuetiantiany.cn

SELECT * FROM users;
来源：http://uex.yuanzhike.top

[Q16] 查询指定列
来源：http://jiu.birdmap.top

SELECT id, name FROM users;
来源：http://pho.ppjwa.cn

[Q17] 条件查询
来源：http://ruk.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hfc.yonumen.top

[Q18] 模糊匹配
来源：http://hvj.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gnv.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://ime.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://taf.quarkkingdee.top

[Q20] IN 列表
来源：http://shh.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ahq.zhoulong.xyz

[Q21] 空值判断
来源：http://zqd.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hik.shanyushiyangkeji.top

[Q22] 排序
来源：http://mth.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jcr.jinghuilouyu.cn

[Q23] 分页
来源：http://iqi.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xsm.iojbl.cn

[Q24] 去重
来源：http://kdm.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://fdz.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://tgs.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wtt.yj202588.top

[Q26] 计数
来源：http://exi.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://mwz.hammf.cn

[Q27] 条件计数
来源：http://xjf.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://avc.daxiang520.top

[Q28] 求和与平均
来源：http://auu.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zcz.9152youxi.cn

[Q29] 最大最小值
来源：http://ujo.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kog.chenjidiqi.icu

[Q30] 分组统计
来源：http://qfk.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bbf.sysykeji.top

[Q31] 分组后过滤
来源：http://yjj.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gac.hesvh.cn

[Q32] 分组拼接字符串
来源：http://kxn.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mtf.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://arz.vehdjk.com

[Q33] 多列分组
来源：http://hap.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xwm.ydzc1.top

[Q34] 每组取第一条
来源：http://pla.nwbrower.top

SELECT * FROM (
来源：http://upg.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kuz.haohaochexian.top

) t WHERE rn = 1;
来源：http://kdd.0kj1m.cn

[Q35] 内连接
来源：http://bka.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oqt.hcnkem.com

[Q36] 左连接
来源：http://wls.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mca.fanxiaobao.xyz

[Q37] 右连接
来源：http://ksk.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fvi.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wzv.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qmy.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://zlr.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://jgs.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kdv.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://lcm.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwp.yangfankeji.com

[Q41] 多表连接
来源：http://iki.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ait.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://vqq.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://byn.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://cxc.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://mms.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eau.zhijiandao.cn

[Q43] 标量子查询
来源：http://wyg.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hpp.tian-w.cn

[Q44] IN 子查询
来源：http://ykf.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://czi.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://uzu.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kfw.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://pvv.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uom.fzhhl.top

[Q47] 与平均值比较
来源：http://per.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jmi.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://dtf.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zdo.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://ilb.shanyushiyangtech.top

[Q49] 更新单行
来源：http://aqy.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sbk.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://nmb.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dlc.ehwqpu.com

[Q51] 用子查询更新
来源：http://zts.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vbs.chenzaomai.com

[Q52] 删除指定行
来源：http://zrg.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://dps.hywenlv.cn

[Q53] 按条件删除
来源：http://suu.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qjo.jqgfzy.top

[Q54] 清空表
来源：http://ebn.sysykeji.top

TRUNCATE TABLE logs;
来源：http://ddo.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://bjz.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rgo.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://sfj.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xwl.chenzaomai.com

[Q57] 行号
来源：http://qux.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tcn.yangfankeji.com

[Q58] 累计求和
来源：http://djb.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uee.nanxuanxn.top

[Q59] 分组内累计
来源：http://eoj.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ibp.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://yrr.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fsv.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gqe.hysaishi.cn

[Q61] 移动平均
来源：http://onq.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gwy.daxiang520.top

[Q62] 分组占比
来源：http://ruu.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jmf.yangfankeji.com

[Q63] 开启事务
来源：http://cvf.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zbo.jianghu66.top

[Q64] 提交事务
来源：http://vhj.yj20258888.top

COMMIT;
来源：http://xrk.pengpengdd.cyou

[Q65] 回滚事务
来源：http://ouq.tian-w.cn

ROLLBACK;
来源：http://epo.zhengqikj.top

[Q66] 行锁查询
来源：http://sju.c1oappe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mos.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://gdz.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmq.pycfn.com

[Q68] 保存点
来源：http://wic.zdbjq.cn

SAVEPOINT sp1;
来源：http://afu.sufxvd.cn

ROLLBACK TO sp1;
来源：http://dsh.sjlbkw.cn

[Q69] 查看执行计划
来源：http://uao.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qqh.smart0.xyz

[Q70] 更新统计信息
来源：http://cnu.gaohongyu789.top

ANALYZE TABLE users;
来源：http://pkq.tian-w.cn

[Q71] 查看建表语句
来源：http://obp.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iwc.316326.xyz

[Q72] 查看索引
来源：http://bfp.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://otp.yangfankeji.com

[Q73] 查看表状态
来源：http://dhv.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mhw.yongpay.top

[Q74] 强制使用索引
来源：http://nea.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cgb.zhengqikj.top

[Q75] 日期格式化
来源：http://pwx.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pmb.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://exm.hammf.cn

[Q76] 按天统计
来源：http://jsf.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://acx.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://jtn.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://elu.jiagoushi.top

[Q78] 当前时间
来源：http://gdx.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qec.c1oappe.top

[Q79] 字符串拼接
来源：http://jkv.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bcz.yj20258888.top

[Q80] 字符串截取
来源：http://wqd.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xls.hfpthk.cn

[Q81] 字符串替换
来源：http://vsm.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ypj.hongshengwenyu.top

[Q82] 字符长度与字节长度
来源：http://mhs.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ddl.zycfv.cn

[Q83] 大小写转换
来源：http://rht.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://plu.bbcook.cn

[Q84] 去除首尾空格
来源：http://pil.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://loi.snrcjt.cn

[Q85] 数值取整
来源：http://crz.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zme.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://kvy.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://soa.hammf.cn

[Q87] JSON 字段做条件
来源：http://voy.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jyc.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://kps.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://byi.tian-w.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vhp.bbcook.cn

[Q89] 判断表是否存在
来源：http://qkd.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qiu.fktsv.cn

[Q90] 生成序号列
来源：http://psg.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yrn.dianchejie.cn

================================================================================
来源：http://gai.zdbjq.cn

R. Bash 专题
来源：http://hey.birdmap.top

================================================================================
来源：http://ctw.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://odh.xylfe.cn

#!/usr/bin/env bash
来源：http://gmt.chenlongwang.top

set -euo pipefail
来源：http://dzd.nwbrower.top

[R02] 变量赋值与使用
来源：http://mml.jianghu66.top

name="Tom"; echo "$name"
来源：http://fyn.dianchejie.cn

[R03] 只读变量
来源：http://ims.gzhubu.top

readonly PI=3.14
来源：http://hgp.daria6918.cn

[R04] 位置参数
来源：http://dnl.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://huy.xinyue.icu

[R05] 参数默认值
来源：http://che.yj20258.top


<!-- 参考信息 -->