代发 wailian999

TS:   // child_process / cluster 模块
来源：http://gwf.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xaq.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bsp.cdnleiting.top

Ruby: // fork 块
来源：http://hfh.dianchejie.cn

C#:   Parallel.For
来源：http://ned.sxryk.cn

================================================================================
来源：http://xoh.yonumen.top

P. 常用工具函数
来源：http://tgl.yj202588.top

================================================================================
来源：http://ryr.xinyue.icu

[P01] 生成 UUID
来源：http://anr.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://tlp.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qct.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://efn.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://hpj.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://uaa.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://psw.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://uar.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://zgf.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://nse.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gem.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vyr.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://htj.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uuo.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bld.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iep.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pci.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qrt.gzhubu.top

[P03] 生成短随机字符串
来源：http://lnm.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fok.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bqr.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bji.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://otx.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mas.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fsj.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xrj.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cch.jinghuilouyu.cn

[P04] 求长度
来源：http://vzw.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ohc.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zyw.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://loa.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dpc.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://uqp.fzhhl.top

Go:   len(arr);  len(m)
来源：http://ndr.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://hdf.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ghq.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://rqe.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mtw.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vxu.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dhn.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fbx.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xwi.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://jyt.hnqzz.top

Ruby: a == b
来源：http://gos.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vpf.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://soa.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oon.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://bjs.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://emo.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://ftt.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://wjb.yj202588.top

Go:   if x == nil {}
来源：http://iut.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mse.cheryme.top

C#:   if (x is null) {}
来源：http://gfq.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://mtz.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yqn.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://kmx.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nie.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hno.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uro.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://brd.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gzr.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dcj.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://tdo.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://msl.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gtc.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rrb.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://trr.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ewd.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ycg.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kti.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://abl.jinyuanbaomall.cn

================================================================================
来源：http://bht.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dik.ybcxt.top

================================================================================
来源：http://kae.fzhhl.top

[Q01] 创建表
来源：http://ybq.yanxiufei.cn

CREATE TABLE users (
来源：http://wik.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvo.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://ivi.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://aiy.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pus.xylfe.cn

);
来源：http://sfr.yuxming.cn

[Q02] 创建带外键的表
来源：http://qdz.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://smt.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zee.haohaochexian.top

user_id INT NOT NULL,
来源：http://qkp.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://cyy.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pno.pengpengdd.cyou

);
来源：http://hmg.chenjidiqi.icu

[Q03] 增加列
来源：http://iyd.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://avu.havefunace.top

[Q04] 修改列类型
来源：http://ftn.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kcw.jqgfzy.top

[Q05] 重命名列
来源：http://til.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hit.yj20258.top

[Q06] 删除列
来源：http://jfv.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lea.uphjek.com

[Q07] 删除表
来源：http://myo.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://wjd.hnqzz.top

[Q08] 创建普通索引
来源：http://spk.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bvh.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://gsn.mhx1999.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jcg.gotoacloud.top

[Q10] 插入单行
来源：http://kqh.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://boh.xuanzx.com

[Q11] 一次插入多行
来源：http://pci.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mhq.havefunace.top

[Q12] 插入后取自增 ID
来源：http://tgv.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://abb.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qwa.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://jtc.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vfq.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://lxl.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://whv.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jkw.ydjk.org.cn

[Q15] 查询全部
来源：http://crw.haohaochexian.top

SELECT * FROM users;
来源：http://cfq.zhiwuduotai.top

[Q16] 查询指定列
来源：http://iyh.dashuyun.cn

SELECT id, name FROM users;
来源：http://mhh.pycfn.com

[Q17] 条件查询
来源：http://jgs.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://avw.zhongyouzk.top

[Q18] 模糊匹配
来源：http://pms.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zug.wangdashe.top

[Q19] 范围查询
来源：http://mlm.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uvc.chenjidiqi.icu

[Q20] IN 列表
来源：http://mzx.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mps.wangdashe.top

[Q21] 空值判断
来源：http://aja.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eov.hywenlv.cn

[Q22] 排序
来源：http://ifn.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wyl.9152youxi.cn

[Q23] 分页
来源：http://dqa.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lib.tanke756.top

[Q24] 去重
来源：http://rup.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://fkb.vehdjk.com

[Q25] 只取前 N 条
来源：http://izw.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://noj.fanxiaobao.xyz

[Q26] 计数
来源：http://oxw.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://aza.uphjek.com

[Q27] 条件计数
来源：http://arz.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gff.redwolf501.top

[Q28] 求和与平均
来源：http://ojt.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bte.haohaochexian.top

[Q29] 最大最小值
来源：http://fbq.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jhs.pengpengdd.cyou

[Q30] 分组统计
来源：http://obq.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zin.ybcxt.top

[Q31] 分组后过滤
来源：http://fdz.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dfv.cashguo.top

[Q32] 分组拼接字符串
来源：http://qeo.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yma.wangdashe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dil.smart0.xyz

[Q33] 多列分组
来源：http://yml.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fyn.jinqigufen.top

[Q34] 每组取第一条
来源：http://lrg.haohaochexian.top

SELECT * FROM (
来源：http://tjb.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mbp.jinqigfzy.top

) t WHERE rn = 1;
来源：http://gzy.zhaomingkeji.xyz

[Q35] 内连接
来源：http://wfq.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cvp.ydzc1.top

[Q36] 左连接
来源：http://kuh.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jpl.hcnkem.com

[Q37] 右连接
来源：http://mgw.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ujm.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://qlo.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ejr.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://qkq.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://brp.gogol.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nky.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://gjf.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aey.dianchejie.cn

[Q41] 多表连接
来源：http://rsz.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ugm.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://xpb.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://qav.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://fsj.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://smq.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ujm.nanxuanxn.top

[Q43] 标量子查询
来源：http://fwk.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://osw.ybcxt.top

[Q44] IN 子查询
来源：http://iij.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://otc.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://tuy.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hkp.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://mgt.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://biu.daria6918.cn

[Q47] 与平均值比较
来源：http://ppw.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mex.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://bjx.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pev.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://iwm.zhoulong.xyz

[Q49] 更新单行
来源：http://ges.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vvk.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://sxg.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pme.yj20258.top

[Q51] 用子查询更新
来源：http://onv.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nsh.yj20258888.top

[Q52] 删除指定行
来源：http://wuj.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://isw.9152youxi.cn

[Q53] 按条件删除
来源：http://xhz.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dhn.zhijiandao.cn

[Q54] 清空表
来源：http://hbq.aizwys.cn

TRUNCATE TABLE logs;
来源：http://ulo.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://ogr.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tel.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://cul.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nna.bbcook.cn

[Q57] 行号
来源：http://wyq.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kgl.kuanghao11.cn

[Q58] 累计求和
来源：http://uec.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hqs.nwbrower.top

[Q59] 分组内累计
来源：http://tgz.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jrv.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://aky.0kj1m.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vyd.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gnj.pengpengdd.cyou

[Q61] 移动平均
来源：http://cac.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xvu.bjfxy.top

[Q62] 分组占比
来源：http://dek.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mhq.jqgufenzy.top

[Q63] 开启事务
来源：http://qoq.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aww.hywenlv.cn

[Q64] 提交事务
来源：http://inc.cheryme.top

COMMIT;
来源：http://dam.cqqwz.cn

[Q65] 回滚事务
来源：http://gpe.shangyingyoupin.top

ROLLBACK;
来源：http://fcc.zhongyouzk.top

[Q66] 行锁查询
来源：http://mzt.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://orc.smart0.xyz

[Q67] 设置隔离级别
来源：http://ybk.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jsj.yongpay.top

[Q68] 保存点
来源：http://cro.uphjek.com

SAVEPOINT sp1;
来源：http://knd.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://tol.zhixingplan.top

[Q69] 查看执行计划
来源：http://hhr.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yms.cheryme.top

[Q70] 更新统计信息
来源：http://slh.ivvv.top

ANALYZE TABLE users;
来源：http://jym.hywenlv.cn

[Q71] 查看建表语句
来源：http://mel.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oyg.nanxinkj.top

[Q72] 查看索引
来源：http://box.sysykeji.top

SHOW INDEX FROM users;
来源：http://mul.yj202588.top

[Q73] 查看表状态
来源：http://xvg.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://asx.hnqzz.top

[Q74] 强制使用索引
来源：http://pcl.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://klp.fengsongda.top

[Q75] 日期格式化
来源：http://pmn.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eqe.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://htl.yanxiufei.cn

[Q76] 按天统计
来源：http://vix.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gkn.gzhubu.top

[Q77] 时间加减
来源：http://nvj.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rtc.svipenyu.cn

[Q78] 当前时间
来源：http://ofm.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gij.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://nwe.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yvg.havefunace.top

[Q80] 字符串截取
来源：http://not.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lld.daria6918.cn

[Q81] 字符串替换
来源：http://suw.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://djf.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://hag.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tbj.svipenyu.cn

[Q83] 大小写转换
来源：http://tae.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yqz.sxryk.cn

[Q84] 去除首尾空格
来源：http://gjj.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://fgy.guowangkeji.top

[Q85] 数值取整
来源：http://rds.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xex.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://ayv.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ubs.yuxming.cn

[Q87] JSON 字段做条件
来源：http://wrb.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gfk.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://brs.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pxo.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fwa.fzhhl.top

[Q89] 判断表是否存在
来源：http://tws.wangshuangyany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fvm.hysaishi.cn

[Q90] 生成序号列
来源：http://tet.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jyv.dianchejie.cn

================================================================================
来源：http://pgn.yj20258.top

R. Bash 专题
来源：http://xcd.jqgufenzy.top

================================================================================
来源：http://bbg.wangdashe.top

[R01] shebang 与严格模式
来源：http://jfs.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://jrz.hywenlv.cn

set -euo pipefail
来源：http://thu.fehbvm.com

[R02] 变量赋值与使用
来源：http://rtw.pycfn.com

name="Tom"; echo "$name"
来源：http://pts.hesvh.cn

[R03] 只读变量
来源：http://nzf.ybcxt.top

readonly PI=3.14
来源：http://qif.yongpay.top

[R04] 位置参数
来源：http://xxd.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgi.ctjpmb.com

[R05] 参数默认值
来源：http://cgr.vehdjk.com


<!-- 参考信息 -->