代发 wailian999

[O06] 使用进程池
来源：http://prc.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vde.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://eiq.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://fky.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://yri.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wxc.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://itd.hysaishi.cn

Ruby: // fork 块
来源：http://mbz.fktsv.cn

C#:   Parallel.For
来源：http://tyd.yanxiufei.cn

================================================================================
来源：http://sqg.bjfxy.top

P. 常用工具函数
来源：http://eab.nanxuanxn.top

================================================================================
来源：http://mwu.c1oappe.top

[P01] 生成 UUID
来源：http://obi.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://mza.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hnn.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://usz.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://vdq.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://eki.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://ajk.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://nlz.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://enr.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://zge.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dwm.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ttt.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jop.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vkw.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ley.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fxo.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://shw.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vzy.smart0.xyz

[P03] 生成短随机字符串
来源：http://gpa.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ejz.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iqv.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yfc.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kwe.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hsj.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lap.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pax.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bea.jinqigufen.top

[P04] 求长度
来源：http://isf.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yhp.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vhz.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ael.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://guy.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://yfk.yonumen.top

Go:   len(arr);  len(m)
来源：http://obc.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://nbh.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://twz.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://hag.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://scx.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vdu.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ehe.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mxo.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sex.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://rpe.yongpay.top

Ruby: a == b
来源：http://rku.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://azs.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qfs.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bxc.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://bor.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dwn.fehbvm.com

TS:   if (x == null) {}
来源：http://emg.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://aad.shuidangran.top

Go:   if x == nil {}
来源：http://vha.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yzr.c1oappe.top

C#:   if (x is null) {}
来源：http://ngx.ybcxt.top

[P07] 防抖与节流
来源：http://wns.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nya.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://xpk.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwy.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://clm.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfs.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qpb.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ewc.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bfl.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://vaz.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kvh.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ynh.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lja.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tck.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ims.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kvq.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sdd.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uti.ywan-chungtsiang.top

================================================================================
来源：http://adt.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iqy.xuanzx.com

================================================================================
来源：http://rlv.hcnkem.com

[Q01] 创建表
来源：http://ziz.chenjidiqi.icu

CREATE TABLE users (
来源：http://bvc.ydjk.org.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://usu.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://wap.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://rpu.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dlt.meibo888.top

);
来源：http://zmn.aizwys.cn

[Q02] 创建带外键的表
来源：http://urd.guowangkeji.top

CREATE TABLE orders (
来源：http://wpx.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ujz.fktsv.cn

user_id INT NOT NULL,
来源：http://ngz.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://kpa.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dwe.haohaochexian.top

);
来源：http://avh.snrcjt.cn

[Q03] 增加列
来源：http://tyw.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rfv.fengsongda.top

[Q04] 修改列类型
来源：http://ych.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blm.zhoulong.xyz

[Q05] 重命名列
来源：http://pgb.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xpg.cashguo.top

[Q06] 删除列
来源：http://qaa.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://fpz.ctjpmb.com

[Q07] 删除表
来源：http://ihm.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://oct.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://skg.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ayb.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://bsz.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vti.yuxming.cn

[Q10] 插入单行
来源：http://zhq.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wwq.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://jre.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gvb.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://ngk.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://ddj.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iez.tian-w.cn

[Q13] 忽略重复插入
来源：http://ixu.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://acz.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://irx.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fjz.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yoe.aibaodan.cn

[Q15] 查询全部
来源：http://sju.c1oappe.top

SELECT * FROM users;
来源：http://ezv.gogol.net.cn

[Q16] 查询指定列
来源：http://sum.jqgufenzy.top

SELECT id, name FROM users;
来源：http://gsx.0kj1m.cn

[Q17] 条件查询
来源：http://xrg.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yjm.zycfv.cn

[Q18] 模糊匹配
来源：http://tru.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nma.zhongyouzk.top

[Q19] 范围查询
来源：http://yum.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rtr.guannengcc.top

[Q20] IN 列表
来源：http://yhl.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xct.9152youxi.cn

[Q21] 空值判断
来源：http://mpg.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pba.xuetiantiany.cn

[Q22] 排序
来源：http://ekk.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cmo.yj20258.top

[Q23] 分页
来源：http://bro.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://imn.fktsv.cn

[Q24] 去重
来源：http://jvg.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://ujj.zycfv.cn

[Q25] 只取前 N 条
来源：http://kby.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rir.fengsongda.top

[Q26] 计数
来源：http://kjl.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://ysv.zhoulong.xyz

[Q27] 条件计数
来源：http://ejc.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xlx.iojbl.cn

[Q28] 求和与平均
来源：http://ryj.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mwy.pengpengdd.cyou

[Q29] 最大最小值
来源：http://dnm.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ioj.tianlin.xyz

[Q30] 分组统计
来源：http://zdk.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mwu.fengsongda.top

[Q31] 分组后过滤
来源：http://abr.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pmi.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://dqp.hysaishi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kqw.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://khs.shuidangran.top

[Q33] 多列分组
来源：http://oal.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vzl.jqgfzy.top

[Q34] 每组取第一条
来源：http://agw.jinqigufen.top

SELECT * FROM (
来源：http://aii.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://foj.c1oappe.top

) t WHERE rn = 1;
来源：http://oit.cucudq.cn

[Q35] 内连接
来源：http://xzj.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bze.cucudq.cn

[Q36] 左连接
来源：http://fki.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dcj.zdbjq.cn

[Q37] 右连接
来源：http://ygs.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wmf.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://qpe.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nld.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://xcp.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nbe.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gtp.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qtw.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qcz.jinqigufen.top

[Q41] 多表连接
来源：http://vxm.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ghi.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://bzm.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wzy.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://bsc.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://yvn.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wqc.bjfxy.top

[Q43] 标量子查询
来源：http://bpa.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bkj.daxiang520.top

[Q44] IN 子查询
来源：http://kvw.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dwg.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://guz.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tcn.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xlb.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjz.dashuyun.cn

[Q47] 与平均值比较
来源：http://hml.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://biq.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://idk.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://osn.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://hlb.jinqigufen.top

[Q49] 更新单行
来源：http://nop.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jkz.havefunace.top

[Q50] 批量更新
来源：http://lwh.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uhs.zhijiandao.cn

[Q51] 用子查询更新
来源：http://dcb.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fvr.dianchejie.cn

[Q52] 删除指定行
来源：http://yna.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://dzn.yuanzhike.top

[Q53] 按条件删除
来源：http://oyb.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gny.ywan-chungtsiang.top

[Q54] 清空表
来源：http://wrr.uphjek.com

TRUNCATE TABLE logs;
来源：http://qqc.mhx1999.top

[Q55] 排名（并列占位）
来源：http://sob.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wmd.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://sbs.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rpg.ctjpmb.com

[Q57] 行号
来源：http://byb.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pnq.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://shr.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vwc.mhx1999.top

[Q59] 分组内累计
来源：http://fyu.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gbu.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://qri.chenjidiqi.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gcw.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://szw.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://lud.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://szf.bbcook.cn

[Q62] 分组占比
来源：http://hdo.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kfj.sjlbkw.cn

[Q63] 开启事务
来源：http://flu.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aqg.fanxiaobao.xyz

[Q64] 提交事务
来源：http://uun.zhaomingkeji.xyz

COMMIT;
来源：http://kwr.gaohongyu789.top

[Q65] 回滚事务
来源：http://ugt.xinyue.icu

ROLLBACK;
来源：http://xog.iojbl.cn

[Q66] 行锁查询
来源：http://ydi.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jrf.c1oappe.top

[Q67] 设置隔离级别
来源：http://yfg.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vrg.guannengcc.top

[Q68] 保存点
来源：http://dlp.xylfe.cn

SAVEPOINT sp1;
来源：http://bey.svipenyu.cn

ROLLBACK TO sp1;
来源：http://hvo.cashguo.top

[Q69] 查看执行计划
来源：http://dpp.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ebs.yueranfly.top

[Q70] 更新统计信息
来源：http://onv.yuxming.cn

ANALYZE TABLE users;
来源：http://qoo.hysaishi.cn

[Q71] 查看建表语句
来源：http://agz.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ifo.yongpay.top

[Q72] 查看索引
来源：http://kbp.dianchejie.cn

SHOW INDEX FROM users;
来源：http://aks.xziqi.cn

[Q73] 查看表状态
来源：http://zjv.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://chh.jiagoushi.top

[Q74] 强制使用索引
来源：http://uye.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kqm.zhongyouzk.top

[Q75] 日期格式化
来源：http://qmv.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bdh.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uhu.zdbjq.cn

[Q76] 按天统计
来源：http://gbn.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://syc.gaohongyu789.top

[Q77] 时间加减
来源：http://tnp.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dqk.redwolf501.top

[Q78] 当前时间
来源：http://wvp.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lxo.dashuyun.cn

[Q79] 字符串拼接
来源：http://hjv.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rfg.zycfv.cn

[Q80] 字符串截取
来源：http://ztb.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mun.vehdjk.com

[Q81] 字符串替换
来源：http://dvq.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://der.ivvv.top

[Q82] 字符长度与字节长度
来源：http://ixn.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nad.yangfankeji.com

[Q83] 大小写转换
来源：http://pdm.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oey.fengsongda.top

[Q84] 去除首尾空格
来源：http://xmw.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://lcy.nwbrower.top

[Q85] 数值取整
来源：http://ddk.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://knm.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://dgw.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zus.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://oeb.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nij.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://cfd.daria6918.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tkc.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://znn.epnwcf.com

[Q89] 判断表是否存在
来源：http://leg.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nov.iojbl.cn

[Q90] 生成序号列
来源：http://okj.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ooz.jinyuanbaomall.cn

================================================================================
来源：http://cvm.zhixingplan.top

R. Bash 专题
来源：http://kid.jinqigfzy.top

================================================================================
来源：http://pfa.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://opp.wangdashe.top

#!/usr/bin/env bash
来源：http://zzy.chenzaomai.com

set -euo pipefail
来源：http://vmu.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://pgt.yongpay.top

name="Tom"; echo "$name"
来源：http://mts.zhiwuduotai.top

[R03] 只读变量
来源：http://kza.iojbl.cn


<!-- 参考信息 -->