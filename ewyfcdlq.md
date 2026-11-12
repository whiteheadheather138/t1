代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pjt.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://taf.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://gyz.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pbq.ppjwa.cn

[O06] 使用进程池
来源：http://quq.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qzu.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tbw.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://tdz.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://nqz.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uzr.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cff.zhiwuduotai.top

Ruby: // fork 块
来源：http://jov.jiagoushi.top

C#:   Parallel.For
来源：http://ofy.fengsongda.top

================================================================================
来源：http://ual.ybcxt.top

P. 常用工具函数
来源：http://rjl.pycfn.com

================================================================================
来源：http://ere.0kj1m.cn

[P01] 生成 UUID
来源：http://myj.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://arq.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wza.xziqi.cn

JS:   crypto.randomUUID()
来源：http://qtk.tanke756.top

TS:   crypto.randomUUID()
来源：http://bmv.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://frn.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://lqh.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://yun.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://kqx.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://tul.hcnkem.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ybn.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rrl.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hgp.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kjv.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cux.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xuy.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hcx.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cvc.fktsv.cn

[P03] 生成短随机字符串
来源：http://eok.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rax.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vgd.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://doq.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cou.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uoe.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yry.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kcz.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ysc.hongshengwenyu.top

[P04] 求长度
来源：http://btc.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://atf.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://alg.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vek.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zck.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://kbm.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://uvp.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://qvf.dianchejie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rdz.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://uer.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kbl.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wgq.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sgd.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://glp.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jxw.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://efk.9152youxi.cn

Ruby: a == b
来源：http://bbw.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tia.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pkh.jiagoushi.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ill.svipenyu.cn

PHP:  if (empty($x)) {}
来源：http://ujh.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qnx.bjfxy.top

TS:   if (x == null) {}
来源：http://vgt.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://rvl.pengpengdd.cyou

Go:   if x == nil {}
来源：http://tyu.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://evc.yuxming.cn

C#:   if (x is null) {}
来源：http://uoc.zhiwuduotai.top

[P07] 防抖与节流
来源：http://lbp.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qxf.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://coo.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bvu.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzu.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nlm.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ocx.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gna.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vll.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://msf.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://poo.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cnp.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://keo.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cgz.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wxq.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cie.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lpt.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qke.dashuyun.cn

================================================================================
来源：http://jzs.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sms.yuanzhike.top

================================================================================
来源：http://acx.fanxiaobao.xyz

[Q01] 创建表
来源：http://mzq.xylfe.cn

CREATE TABLE users (
来源：http://laf.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsl.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://dwe.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://epx.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zkc.hammf.cn

);
来源：http://jqp.hcnkem.com

[Q02] 创建带外键的表
来源：http://lnz.daxiang520.top

CREATE TABLE orders (
来源：http://lnq.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sco.chenzaomai.com

user_id INT NOT NULL,
来源：http://nvj.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://mxk.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gqt.ybcxt.top

);
来源：http://cwc.9152youxi.cn

[Q03] 增加列
来源：http://dgu.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://elh.hesvh.cn

[Q04] 修改列类型
来源：http://mpo.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ght.yanxiufei.cn

[Q05] 重命名列
来源：http://fqk.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ofe.mhx1999.top

[Q06] 删除列
来源：http://qqq.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://ryz.fzhhl.top

[Q07] 删除表
来源：http://vcq.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://npq.vehdjk.com

[Q08] 创建普通索引
来源：http://gbe.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://upt.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://iid.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zih.zhiwuduotai.top

[Q10] 插入单行
来源：http://ynq.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oih.wangdashe.top

[Q11] 一次插入多行
来源：http://rvm.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jzt.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://jff.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ywz.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kms.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://epk.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://olo.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://ykp.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pex.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zzx.yj20258888.top

[Q15] 查询全部
来源：http://fgf.hnxiangtu.top

SELECT * FROM users;
来源：http://tpb.gotoacloud.top

[Q16] 查询指定列
来源：http://lex.jinqigfzy.top

SELECT id, name FROM users;
来源：http://ula.cdnleiting.top

[Q17] 条件查询
来源：http://wwg.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nru.c1oappe.top

[Q18] 模糊匹配
来源：http://xvz.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qzb.yanxiufei.cn

[Q19] 范围查询
来源：http://gdo.jiagoushi.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qoi.haohaochexian.top

[Q20] IN 列表
来源：http://bmg.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://arv.zdbjq.cn

[Q21] 空值判断
来源：http://khc.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rtt.snrcjt.cn

[Q22] 排序
来源：http://usv.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hhc.gogol.net.cn

[Q23] 分页
来源：http://xns.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vlm.jqgfzy.top

[Q24] 去重
来源：http://nlf.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://ksj.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://ytf.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfe.guannengcc.top

[Q26] 计数
来源：http://oyn.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://rkl.hnxiangtu.top

[Q27] 条件计数
来源：http://vvq.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uhb.jqgfzy.top

[Q28] 求和与平均
来源：http://hfp.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zne.pycfn.com

[Q29] 最大最小值
来源：http://qor.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nli.sxryk.cn

[Q30] 分组统计
来源：http://unc.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ngf.yonumen.top

[Q31] 分组后过滤
来源：http://mbv.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gat.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://cwi.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qmj.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cgc.mhx1999.top

[Q33] 多列分组
来源：http://wim.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ubw.0kj1m.cn

[Q34] 每组取第一条
来源：http://nfn.sysykeji.top

SELECT * FROM (
来源：http://zla.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vcg.316326.xyz

) t WHERE rn = 1;
来源：http://xrg.hesvh.cn

[Q35] 内连接
来源：http://wfm.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://krt.hongshengwenyu.top

[Q36] 左连接
来源：http://cyh.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://joy.c1oappe.top

[Q37] 右连接
来源：http://ebm.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qxq.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hvi.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://buy.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://ddz.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://scw.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hak.redwolf501.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mcn.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://upc.gzhubu.top

[Q41] 多表连接
来源：http://jlk.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nxs.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://azr.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://rhe.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://ebf.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://wcp.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ovo.nwbrower.top

[Q43] 标量子查询
来源：http://tpv.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wis.cashguo.top

[Q44] IN 子查询
来源：http://vwp.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bee.birdmap.top

[Q45] EXISTS 判断存在
来源：http://rqi.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yic.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vcy.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aky.nanxinkj.top

[Q47] 与平均值比较
来源：http://zof.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oap.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://azj.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bwg.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://elv.fanxiaobao.xyz

[Q49] 更新单行
来源：http://nar.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zeg.hongshengwenyu.top

[Q50] 批量更新
来源：http://uwf.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fgc.cheryme.top

[Q51] 用子查询更新
来源：http://map.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pzk.dianchejie.cn

[Q52] 删除指定行
来源：http://dug.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://vzn.pycfn.com

[Q53] 按条件删除
来源：http://ehu.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hxj.jyoumei.cn

[Q54] 清空表
来源：http://eaa.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://xoo.316326.xyz

[Q55] 排名（并列占位）
来源：http://kkp.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ikh.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://grd.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ssv.bjfxy.top

[Q57] 行号
来源：http://sgf.yuanzhike.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://icg.yongpay.top

[Q58] 累计求和
来源：http://cjx.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bjz.bbcook.cn

[Q59] 分组内累计
来源：http://cci.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tnp.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://grk.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vuc.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nkq.ydjk.org.cn

[Q61] 移动平均
来源：http://qss.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cei.redwolf501.top

[Q62] 分组占比
来源：http://aaf.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kqd.yvedp.cn

[Q63] 开启事务
来源：http://ugz.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wfp.zhengqikj.top

[Q64] 提交事务
来源：http://lrr.yj202588.top

COMMIT;
来源：http://ymz.hcnkem.com

[Q65] 回滚事务
来源：http://ouw.gogol.net.cn

ROLLBACK;
来源：http://blp.xuanzx.com

[Q66] 行锁查询
来源：http://lui.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ijq.meibo888.top

[Q67] 设置隔离级别
来源：http://wfz.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mhk.fzhhl.top

[Q68] 保存点
来源：http://reh.zhijiandao.cn

SAVEPOINT sp1;
来源：http://cgm.9152youxi.cn

ROLLBACK TO sp1;
来源：http://qal.zhoulong.xyz

[Q69] 查看执行计划
来源：http://rtg.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vkr.jyoumei.cn

[Q70] 更新统计信息
来源：http://hle.gogol.net.cn

ANALYZE TABLE users;
来源：http://ham.fengsongda.top

[Q71] 查看建表语句
来源：http://xrn.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wfk.nanxinkj.top

[Q72] 查看索引
来源：http://pyl.havefunace.top

SHOW INDEX FROM users;
来源：http://dtg.jinqigufen.top

[Q73] 查看表状态
来源：http://uqq.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tkd.svipenyu.cn

[Q74] 强制使用索引
来源：http://cdi.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xzi.xinyue.icu

[Q75] 日期格式化
来源：http://qai.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qts.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ikn.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://jub.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://duf.epnwcf.com

[Q77] 时间加减
来源：http://mmy.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lkb.haohaochexian.top

[Q78] 当前时间
来源：http://kgr.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://thv.yj202588.top

[Q79] 字符串拼接
来源：http://cpj.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rcy.hesvh.cn

[Q80] 字符串截取
来源：http://ken.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tif.feifeiyinyue.top

[Q81] 字符串替换
来源：http://gmq.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vwo.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://ntn.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bam.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://hoh.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aln.jyoumei.cn

[Q84] 去除首尾空格
来源：http://gib.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://kes.zhijiandao.cn

[Q85] 数值取整
来源：http://vhu.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qov.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://xab.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jue.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://rkp.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gxy.yfazqb.com

[Q88] 行转列（条件聚合）
来源：http://lqb.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aff.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zic.tian-w.cn

[Q89] 判断表是否存在
来源：http://yeq.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://prf.ctjpmb.com

[Q90] 生成序号列
来源：http://jnj.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://von.sweek.top

================================================================================
来源：http://mde.yuxming.cn

R. Bash 专题
来源：http://nly.sxryk.cn

================================================================================
来源：http://nun.hysaishi.cn

[R01] shebang 与严格模式
来源：http://zus.yfazqb.com

#!/usr/bin/env bash
来源：http://kuz.xuanzx.com


<!-- 参考信息 -->