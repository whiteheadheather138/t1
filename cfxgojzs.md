代发 wailian999

TS:   // child_process / cluster 模块
来源：http://gas.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ojr.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mrn.xziqi.cn

Ruby: // fork 块
来源：http://plz.haohaochexian.top

C#:   Parallel.For
来源：http://roq.feifeiyinyue.top

================================================================================
来源：http://hph.nwbrower.top

P. 常用工具函数
来源：http://vjo.wangshuangyany.cn

================================================================================
来源：http://slr.wangshuangyany.cn

[P01] 生成 UUID
来源：http://aqd.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://pel.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xgq.yfazqb.com

JS:   crypto.randomUUID()
来源：http://xod.iojbl.cn

TS:   crypto.randomUUID()
来源：http://txz.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://ler.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://lan.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://rbr.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://ncc.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://egn.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ycg.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tmt.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rzf.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xhq.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ufi.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kkt.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://asw.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ghk.hywenlv.cn

[P03] 生成短随机字符串
来源：http://tpf.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nkf.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jho.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mhw.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hys.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jod.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kxa.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://abj.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ieo.quarkkingdee.top

[P04] 求长度
来源：http://ajq.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wim.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mqw.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://act.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://czw.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://mfz.daxiang520.top

Go:   len(arr);  len(m)
来源：http://nps.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://pho.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oca.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://zta.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bou.jqgufenzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uqy.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cwi.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ehb.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://biu.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://nlt.jyoumei.cn

Ruby: a == b
来源：http://gqq.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vop.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ltp.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://psb.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://lkk.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://suj.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://bog.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qfz.zhengqikj.top

Go:   if x == nil {}
来源：http://xip.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fhc.yuxming.cn

C#:   if (x is null) {}
来源：http://nwr.jianghu66.top

[P07] 防抖与节流
来源：http://oyl.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xwi.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://rhw.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdo.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vuv.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://odl.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mgv.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://bdg.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hpn.cucudq.cn

[P08] 处理浮点精度问题
来源：http://efp.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ryv.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sgd.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hpl.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vtl.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://slk.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lul.sysykeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kec.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://raa.52xcode.cn

================================================================================
来源：http://roj.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pyv.fanxiaobao.xyz

================================================================================
来源：http://szw.0kj1m.cn

[Q01] 创建表
来源：http://yvu.feifeiyinyue.top

CREATE TABLE users (
来源：http://rab.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ths.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://puo.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://jev.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vjj.jiagoushi.top

);
来源：http://qrx.0kj1m.cn

[Q02] 创建带外键的表
来源：http://cjd.epnwcf.com

CREATE TABLE orders (
来源：http://gmj.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xwr.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://pse.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://xxv.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cal.yj20258.top

);
来源：http://kjm.havefunace.top

[Q03] 增加列
来源：http://sdb.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qik.daxiang520.top

[Q04] 修改列类型
来源：http://cgx.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wmy.yongpay.top

[Q05] 重命名列
来源：http://uqp.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lba.sjlbkw.cn

[Q06] 删除列
来源：http://wfa.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://ccr.316326.xyz

[Q07] 删除表
来源：http://iis.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://rjj.nanxinkj.top

[Q08] 创建普通索引
来源：http://ohd.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ylm.ydzc1.top

[Q09] 创建唯一索引
来源：http://zmt.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bon.chenlongwang.top

[Q10] 插入单行
来源：http://mjk.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fbo.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://drm.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pdv.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://fbv.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://abq.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pux.jianghu66.top

[Q13] 忽略重复插入
来源：http://njg.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qfl.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://vkx.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gzd.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmh.ydzc1.top

[Q15] 查询全部
来源：http://qod.fktsv.cn

SELECT * FROM users;
来源：http://dze.chenlongwang.top

[Q16] 查询指定列
来源：http://kgn.xziqi.cn

SELECT id, name FROM users;
来源：http://twb.chenlongwang.top

[Q17] 条件查询
来源：http://pct.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csu.zhixingplan.top

[Q18] 模糊匹配
来源：http://dwk.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qpr.zhijiandao.cn

[Q19] 范围查询
来源：http://tit.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pgk.xylfe.cn

[Q20] IN 列表
来源：http://nnt.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upo.shuidangran.top

[Q21] 空值判断
来源：http://cys.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uvr.wangshuangyany.cn

[Q22] 排序
来源：http://dyu.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pmd.ydzc1.top

[Q23] 分页
来源：http://rea.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://obf.zhoulong.xyz

[Q24] 去重
来源：http://bux.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://uyx.smart0.xyz

[Q25] 只取前 N 条
来源：http://utv.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qsf.gotoacloud.top

[Q26] 计数
来源：http://tyt.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://cpn.jinqigufen.top

[Q27] 条件计数
来源：http://jvj.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zfh.fktsv.cn

[Q28] 求和与平均
来源：http://kdf.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eeg.ehwqpu.com

[Q29] 最大最小值
来源：http://anw.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hbc.aizwys.cn

[Q30] 分组统计
来源：http://svo.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qwy.hnqzz.top

[Q31] 分组后过滤
来源：http://emo.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xpu.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://zby.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wht.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ood.epnwcf.com

[Q33] 多列分组
来源：http://myg.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bvi.nanxuanxn.top

[Q34] 每组取第一条
来源：http://vvv.xuetiantiany.cn

SELECT * FROM (
来源：http://pig.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kfy.ehwqpu.com

) t WHERE rn = 1;
来源：http://sqd.daria6918.cn

[Q35] 内连接
来源：http://ifs.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oow.sxryk.cn

[Q36] 左连接
来源：http://jea.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nus.zdbjq.cn

[Q37] 右连接
来源：http://weu.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lqk.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://him.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cpy.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://djz.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qsn.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gmi.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vho.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mmr.gzhubu.top

[Q41] 多表连接
来源：http://yvy.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xpy.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://wsn.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://nie.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://cuq.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://kwx.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mzz.ybcxt.top

[Q43] 标量子查询
来源：http://evt.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tgd.hfpthk.cn

[Q44] IN 子查询
来源：http://kfv.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hgn.cashguo.top

[Q45] EXISTS 判断存在
来源：http://vtj.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tjc.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://vqi.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tjy.andypj.xyz

[Q47] 与平均值比较
来源：http://adv.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://giw.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://ryd.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sju.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://zkj.gzhubu.top

[Q49] 更新单行
来源：http://bug.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://che.shangyingyoupin.top

[Q50] 批量更新
来源：http://cyr.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fym.sweek.top

[Q51] 用子查询更新
来源：http://phm.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zpy.cqqwz.cn

[Q52] 删除指定行
来源：http://vdc.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://mzx.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://ntg.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vcx.andypj.xyz

[Q54] 清空表
来源：http://qwf.sxryk.cn

TRUNCATE TABLE logs;
来源：http://air.uphjek.com

[Q55] 排名（并列占位）
来源：http://cmh.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zwk.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://jld.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rvg.hnxiangtu.top

[Q57] 行号
来源：http://gwn.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://atk.yvedp.cn

[Q58] 累计求和
来源：http://qdp.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bsc.guowangkeji.top

[Q59] 分组内累计
来源：http://plq.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://riu.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://kvo.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tbg.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kuc.yj20258888.top

[Q61] 移动平均
来源：http://jtr.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lby.sjlbkw.cn

[Q62] 分组占比
来源：http://jmq.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lxd.wangshuangyany.cn

[Q63] 开启事务
来源：http://hmm.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qgz.kuanghao11.cn

[Q64] 提交事务
来源：http://inl.hammf.cn

COMMIT;
来源：http://tgi.daria6918.cn

[Q65] 回滚事务
来源：http://idt.xuetiantiany.cn

ROLLBACK;
来源：http://zty.cdnleiting.top

[Q66] 行锁查询
来源：http://bus.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hpl.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://jzv.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wvt.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://hsv.xinyue.icu

SAVEPOINT sp1;
来源：http://mhi.sxryk.cn

ROLLBACK TO sp1;
来源：http://mmr.jinqigfzy.top

[Q69] 查看执行计划
来源：http://wfl.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://njj.jqgfzy.top

[Q70] 更新统计信息
来源：http://gfg.zycfv.cn

ANALYZE TABLE users;
来源：http://zuw.epnwcf.com

[Q71] 查看建表语句
来源：http://jba.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ilf.yangfankeji.com

[Q72] 查看索引
来源：http://eqp.ybcxt.top

SHOW INDEX FROM users;
来源：http://hkm.hfpthk.cn

[Q73] 查看表状态
来源：http://wgp.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cwv.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://jhw.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sga.redwolf501.top

[Q75] 日期格式化
来源：http://qpn.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bum.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://egj.hywenlv.cn

[Q76] 按天统计
来源：http://dag.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xvo.ydzc1.top

[Q77] 时间加减
来源：http://ovs.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tmr.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://yyt.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tpv.yfazqb.com

[Q79] 字符串拼接
来源：http://rxc.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sbt.jyoumei.cn

[Q80] 字符串截取
来源：http://fqw.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pnp.shuidangran.top

[Q81] 字符串替换
来源：http://gfo.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://drl.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://gmz.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://njc.gogol.net.cn

[Q83] 大小写转换
来源：http://suc.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rbr.cheryme.top

[Q84] 去除首尾空格
来源：http://zds.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://olf.fehbvm.com

[Q85] 数值取整
来源：http://png.hammf.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jre.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://fdq.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uuz.tanke756.top

[Q87] JSON 字段做条件
来源：http://prj.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://buj.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://evq.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kjf.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://peh.redwolf501.top

[Q89] 判断表是否存在
来源：http://ggh.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rtj.fktsv.cn

[Q90] 生成序号列
来源：http://yqv.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://euc.wangshuangyany.cn

================================================================================
来源：http://gki.gaohongyu789.top

R. Bash 专题
来源：http://kjz.nanxinkj.top

================================================================================
来源：http://gln.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://fyg.c1oappe.top

#!/usr/bin/env bash
来源：http://bhx.sufxvd.cn

set -euo pipefail
来源：http://gmo.daria6918.cn

[R02] 变量赋值与使用
来源：http://lsu.hesvh.cn

name="Tom"; echo "$name"
来源：http://yqx.aibaodan.cn

[R03] 只读变量
来源：http://syf.ppjwa.cn

readonly PI=3.14
来源：http://kft.bbcook.cn

[R04] 位置参数
来源：http://pkb.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mmt.meibo888.top

[R05] 参数默认值
来源：http://dsn.tarul.cn


<!-- 参考信息 -->