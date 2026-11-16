代发 wailian999

[O06] 使用进程池
来源：http://tmu.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lxy.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://osc.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://inx.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://jct.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iew.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fcm.yonumen.top

Ruby: // fork 块
来源：http://mmh.hywenlv.cn

C#:   Parallel.For
来源：http://uwf.hysaishi.cn

================================================================================
来源：http://cpk.tarul.cn

P. 常用工具函数
来源：http://pbk.fehbvm.com

================================================================================
来源：http://top.ydjk.org.cn

[P01] 生成 UUID
来源：http://aum.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://mqd.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ctw.aizwys.cn

JS:   crypto.randomUUID()
来源：http://yjj.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://wib.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://qot.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://gzz.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://llb.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://zer.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://wsk.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qnc.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://iif.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rgz.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gpv.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dwh.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yvd.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://drj.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fdc.hammf.cn

[P03] 生成短随机字符串
来源：http://zll.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bka.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dxl.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ppl.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ogf.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yam.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://civ.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dpw.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bjo.fzhhl.top

[P04] 求长度
来源：http://ubv.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yhu.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lco.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://awj.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oov.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://piw.nwbrower.top

Go:   len(arr);  len(m)
来源：http://vdq.zhengqikj.top

Ruby: x.length;  x.size
来源：http://uiy.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dod.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://mpx.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nlu.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtc.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dzl.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zdo.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qsk.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://mol.havefunace.top

Ruby: a == b
来源：http://pqz.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vbj.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bdx.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qhk.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://fnv.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tdr.dianchejie.cn

TS:   if (x == null) {}
来源：http://ngt.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://vbr.yuxming.cn

Go:   if x == nil {}
来源：http://ztv.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fle.jqgfzy.top

C#:   if (x is null) {}
来源：http://uil.snrcjt.cn

[P07] 防抖与节流
来源：http://vlx.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yql.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://nvw.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hlz.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ada.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://igl.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uvy.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hxm.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jrk.andypj.xyz

[P08] 处理浮点精度问题
来源：http://oxz.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxt.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kou.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://klr.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lcc.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ebo.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gax.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zgt.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fqb.jlsjyb.cn

================================================================================
来源：http://que.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kqf.fengsongda.top

================================================================================
来源：http://pdl.cdnleiting.top

[Q01] 创建表
来源：http://ttd.fanxiaobao.xyz

CREATE TABLE users (
来源：http://mdo.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vwa.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://qtm.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://ufr.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ieh.jinghuilouyu.cn

);
来源：http://xfz.cashguo.top

[Q02] 创建带外键的表
来源：http://uwy.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://qsa.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mev.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://ahc.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://lfr.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wbk.yueranfly.top

);
来源：http://wny.fehbvm.com

[Q03] 增加列
来源：http://lpr.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qhj.redwolf501.top

[Q04] 修改列类型
来源：http://wkf.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ndt.fanxiaobao.xyz

[Q05] 重命名列
来源：http://enn.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://udx.9152youxi.cn

[Q06] 删除列
来源：http://mpx.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://fpz.daxiang520.top

[Q07] 删除表
来源：http://owx.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://xvk.yfazqb.com

[Q08] 创建普通索引
来源：http://muj.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uhi.jyoumei.cn

[Q09] 创建唯一索引
来源：http://cxv.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lpf.andypj.xyz

[Q10] 插入单行
来源：http://ijm.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bfl.pycfn.com

[Q11] 一次插入多行
来源：http://xvt.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kvi.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://klo.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://vdx.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xcn.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://fhn.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ejl.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://jko.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fbp.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eer.jinqigfzy.top

[Q15] 查询全部
来源：http://tgm.smart0.xyz

SELECT * FROM users;
来源：http://bcw.aibaodan.cn

[Q16] 查询指定列
来源：http://asx.nwbrower.top

SELECT id, name FROM users;
来源：http://ptp.nwbrower.top

[Q17] 条件查询
来源：http://xuv.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yey.xuanzx.com

[Q18] 模糊匹配
来源：http://nih.zycfv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ntq.dianchejie.cn

[Q19] 范围查询
来源：http://bxi.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sio.zhixingplan.top

[Q20] IN 列表
来源：http://uot.zhiwuduotai.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yxz.aizwys.cn

[Q21] 空值判断
来源：http://vqw.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ppb.bjfxy.top

[Q22] 排序
来源：http://mjr.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://drb.yvedp.cn

[Q23] 分页
来源：http://ysb.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://skn.zhengqikj.top

[Q24] 去重
来源：http://nsc.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://qtf.yueranfly.top

[Q25] 只取前 N 条
来源：http://aeh.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://upk.xuanzx.com

[Q26] 计数
来源：http://uee.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://azp.yangfankeji.com

[Q27] 条件计数
来源：http://brl.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sja.zdbjq.cn

[Q28] 求和与平均
来源：http://wio.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://puy.kuanghao11.cn

[Q29] 最大最小值
来源：http://yag.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://dus.wangdashe.top

[Q30] 分组统计
来源：http://phx.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bqx.hnqzz.top

[Q31] 分组后过滤
来源：http://xwn.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dpn.cashguo.top

[Q32] 分组拼接字符串
来源：http://mbm.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qhw.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hit.zhengqikj.top

[Q33] 多列分组
来源：http://khx.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nnm.redwolf501.top

[Q34] 每组取第一条
来源：http://vhw.ydzc1.top

SELECT * FROM (
来源：http://nek.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ipr.bjfxy.top

) t WHERE rn = 1;
来源：http://fbi.hnxiangtu.top

[Q35] 内连接
来源：http://chb.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xfy.hnxiangtu.top

[Q36] 左连接
来源：http://hzk.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tyn.svipenyu.cn

[Q37] 右连接
来源：http://ogq.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yzp.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://jzu.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wpz.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://lnb.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xzb.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://shx.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ljt.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tvo.hywenlv.cn

[Q41] 多表连接
来源：http://zfg.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://txq.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://xjf.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://fhd.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://yvh.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://xdt.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nzl.vqdsnc.cn

[Q43] 标量子查询
来源：http://sto.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vjm.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://mjx.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wam.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://sbv.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://krf.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://oql.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://htc.fktsv.cn

[Q47] 与平均值比较
来源：http://nlb.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yea.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://uld.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gbx.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://exr.vehdjk.com

[Q49] 更新单行
来源：http://zky.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qtw.birdmap.top

[Q50] 批量更新
来源：http://ptl.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ejv.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://jml.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zqi.sxryk.cn

[Q52] 删除指定行
来源：http://nqo.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://fsu.hammf.cn

[Q53] 按条件删除
来源：http://tvz.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zvf.zhiwuduotai.top

[Q54] 清空表
来源：http://shz.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://usv.yueranfly.top

[Q55] 排名（并列占位）
来源：http://qwf.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ief.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://mpe.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xvz.yuanzhike.top

[Q57] 行号
来源：http://kji.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tru.fehbvm.com

[Q58] 累计求和
来源：http://vyl.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tzj.ivvv.top

[Q59] 分组内累计
来源：http://yws.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xvv.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://hmx.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tph.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wze.nanxinkj.top

[Q61] 移动平均
来源：http://wtz.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kny.cdnleiting.top

[Q62] 分组占比
来源：http://gnb.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eeq.dianchejie.cn

[Q63] 开启事务
来源：http://fon.yj20258.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uos.yanxiufei.cn

[Q64] 提交事务
来源：http://spj.shanyushiyangkeji.top

COMMIT;
来源：http://tqz.sweek.top

[Q65] 回滚事务
来源：http://bap.jinghuilouyu.cn

ROLLBACK;
来源：http://xax.yj202588.top

[Q66] 行锁查询
来源：http://cqq.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ioi.smart0.xyz

[Q67] 设置隔离级别
来源：http://nlg.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ifc.fengsongda.top

[Q68] 保存点
来源：http://bkm.zhixingplan.top

SAVEPOINT sp1;
来源：http://urt.jiagoushi.top

ROLLBACK TO sp1;
来源：http://dcc.bbcook.cn

[Q69] 查看执行计划
来源：http://oyp.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xon.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://czj.tanke756.top

ANALYZE TABLE users;
来源：http://orm.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://jvt.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://orm.sjlbkw.cn

[Q72] 查看索引
来源：http://vbc.pycfn.com

SHOW INDEX FROM users;
来源：http://nht.tian-w.cn

[Q73] 查看表状态
来源：http://jxt.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://rmb.c1oappe.top

[Q74] 强制使用索引
来源：http://klu.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xcd.chenlongwang.top

[Q75] 日期格式化
来源：http://sod.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gxr.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dbr.yonumen.top

[Q76] 按天统计
来源：http://pgt.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qep.tarul.cn

[Q77] 时间加减
来源：http://pdt.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mxz.hywenlv.cn

[Q78] 当前时间
来源：http://qzt.jinyuanbaomall.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fpu.gaohongyu789.top

[Q79] 字符串拼接
来源：http://cem.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eps.fengsongda.top

[Q80] 字符串截取
来源：http://qtl.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fpm.wangshuangyany.cn

[Q81] 字符串替换
来源：http://dxl.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xgm.havefunace.top

[Q82] 字符长度与字节长度
来源：http://zmf.xylfe.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rjy.fktsv.cn

[Q83] 大小写转换
来源：http://myc.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ptm.gotoacloud.top

[Q84] 去除首尾空格
来源：http://etg.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://kek.ivvv.top

[Q85] 数值取整
来源：http://bsy.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baf.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://mbp.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://frv.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://vib.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yxe.sweek.top

[Q88] 行转列（条件聚合）
来源：http://eqo.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bji.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tfb.zdqjudy.top

[Q89] 判断表是否存在
来源：http://lws.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zhn.316326.xyz

[Q90] 生成序号列
来源：http://epx.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lwi.yj20258888.top

================================================================================
来源：http://pku.epnwcf.com

R. Bash 专题
来源：http://qdn.wangdashe.top

================================================================================
来源：http://vtu.yj20258888.top

[R01] shebang 与严格模式
来源：http://ptg.andypj.xyz

#!/usr/bin/env bash
来源：http://del.316326.xyz

set -euo pipefail
来源：http://glv.guannengcc.top

[R02] 变量赋值与使用
来源：http://amm.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://eef.ivvv.top

[R03] 只读变量
来源：http://pfc.zycfv.cn


<!-- 参考信息 -->