代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bpb.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sbp.birdmap.top

Ruby: threads.map(&:join)
来源：http://nsg.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ujt.feifeiyinyue.top

[O06] 使用进程池
来源：http://hza.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vop.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://wba.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://nod.tarul.cn

TS:   // child_process / cluster 模块
来源：http://rxa.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ekp.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uvj.cashguo.top

Ruby: // fork 块
来源：http://bmo.jqgfzy.top

C#:   Parallel.For
来源：http://yvd.cheryme.top

================================================================================
来源：http://zhs.zycfv.cn

P. 常用工具函数
来源：http://itg.hongshengwenyu.top

================================================================================
来源：http://zro.yongpay.top

[P01] 生成 UUID
来源：http://xja.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://hbb.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://akx.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://wzx.fehbvm.com

TS:   crypto.randomUUID()
来源：http://tah.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://unp.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://eqs.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://kmx.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://cxz.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://hhd.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ptt.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gas.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xgk.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sav.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yhy.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xok.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nrg.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rzt.yueranfly.top

[P03] 生成短随机字符串
来源：http://fez.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://khk.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wxx.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ttl.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yay.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wyo.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tbo.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nti.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ryx.chenzaomai.com

[P04] 求长度
来源：http://wwd.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rub.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kqe.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vez.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cst.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://lot.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://lcf.xinyue.icu

Ruby: x.length;  x.size
来源：http://nat.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fif.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://ciu.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fmt.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ymw.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yyq.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iib.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wkp.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://rag.zycfv.cn

Ruby: a == b
来源：http://qij.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ylx.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ivt.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://whl.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://zhy.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wqw.sysykeji.top

TS:   if (x == null) {}
来源：http://juk.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vbt.jyoumei.cn

Go:   if x == nil {}
来源：http://cqi.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://roh.smart0.xyz

C#:   if (x is null) {}
来源：http://jvq.pycfn.com

[P07] 防抖与节流
来源：http://tzr.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wso.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://ter.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kxu.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dxp.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vfd.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qhv.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://kxq.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zxq.andypj.xyz

[P08] 处理浮点精度问题
来源：http://mzh.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://olr.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pvi.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dih.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iwb.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvu.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://azy.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cdw.smart0.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zau.daxiang520.top

================================================================================
来源：http://rrr.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wop.wangdashe.top

================================================================================
来源：http://lkt.jianghu66.top

[Q01] 创建表
来源：http://jgl.gzhubu.top

CREATE TABLE users (
来源：http://tpk.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qrc.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://moc.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://jso.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tkc.haohaochexian.top

);
来源：http://cxl.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://xbs.wangdashe.top

CREATE TABLE orders (
来源：http://xws.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhq.sufxvd.cn

user_id INT NOT NULL,
来源：http://vtq.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://qyo.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uid.sxryk.cn

);
来源：http://ewc.jqgfzy.top

[Q03] 增加列
来源：http://szv.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ytk.sweek.top

[Q04] 修改列类型
来源：http://hqq.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://neg.gaohongyu789.top

[Q05] 重命名列
来源：http://jkw.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ymm.ydzc1.top

[Q06] 删除列
来源：http://zek.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zeq.sysykeji.top

[Q07] 删除表
来源：http://esm.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://glr.nwbrower.top

[Q08] 创建普通索引
来源：http://shr.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://knf.dashuyun.cn

[Q09] 创建唯一索引
来源：http://jpv.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hrc.redwolf501.top

[Q10] 插入单行
来源：http://wyp.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oqq.0kj1m.cn

[Q11] 一次插入多行
来源：http://uin.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gwd.hnxiangtu.top

[Q12] 插入后取自增 ID
来源：http://ntl.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pmn.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://brq.gzhubu.top

[Q13] 忽略重复插入
来源：http://xjw.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qda.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://grb.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wpj.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eaw.hnxiangtu.top

[Q15] 查询全部
来源：http://lix.yuanzhike.top

SELECT * FROM users;
来源：http://vkd.zdbjq.cn

[Q16] 查询指定列
来源：http://kgr.hammf.cn

SELECT id, name FROM users;
来源：http://kbp.shanyushiyangtech.top

[Q17] 条件查询
来源：http://gyg.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kpm.52xcode.cn

[Q18] 模糊匹配
来源：http://hkl.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iev.redwolf501.top

[Q19] 范围查询
来源：http://iww.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nqw.ydzc1.top

[Q20] IN 列表
来源：http://zmc.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xhm.xinyue.icu

[Q21] 空值判断
来源：http://hfl.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tdf.yongpay.top

[Q22] 排序
来源：http://lxf.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bgu.316326.xyz

[Q23] 分页
来源：http://gof.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yxk.xuetiantiany.cn

[Q24] 去重
来源：http://adg.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://hwi.gzhubu.top

[Q25] 只取前 N 条
来源：http://bjn.nanxuanxn.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zxy.yangfankeji.com

[Q26] 计数
来源：http://dlj.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://qnu.tianlin.xyz

[Q27] 条件计数
来源：http://ryb.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hum.shuidangran.top

[Q28] 求和与平均
来源：http://okr.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qsd.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://dqi.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uky.sxryk.cn

[Q30] 分组统计
来源：http://dia.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dbt.vqdsnc.cn

[Q31] 分组后过滤
来源：http://erw.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rjr.yj202588.top

[Q32] 分组拼接字符串
来源：http://mcb.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ugs.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gnr.hfpthk.cn

[Q33] 多列分组
来源：http://llc.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bqu.hesvh.cn

[Q34] 每组取第一条
来源：http://btl.feifeiyinyue.top

SELECT * FROM (
来源：http://eql.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ybn.cqqwz.cn

) t WHERE rn = 1;
来源：http://ygr.dianchejie.cn

[Q35] 内连接
来源：http://lfu.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://giw.dianchejie.cn

[Q36] 左连接
来源：http://mgt.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kxd.zhoulong.xyz

[Q37] 右连接
来源：http://gmo.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kjm.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://nkl.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dvq.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://foc.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kdi.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nfn.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mlp.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://doo.gotoacloud.top

[Q41] 多表连接
来源：http://smm.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ner.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://zow.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://psq.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://uvo.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://gea.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://unz.sufxvd.cn

[Q43] 标量子查询
来源：http://btx.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ekq.ydzc1.top

[Q44] IN 子查询
来源：http://yhw.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xzj.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://pcr.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jmn.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://etv.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dhz.chenlongwang.top

[Q47] 与平均值比较
来源：http://mlk.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tko.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://hmb.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hxp.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://faf.zhijiandao.cn

[Q49] 更新单行
来源：http://ivv.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lzh.yvedp.cn

[Q50] 批量更新
来源：http://gtm.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zdj.hesvh.cn

[Q51] 用子查询更新
来源：http://fln.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mth.ctjpmb.com

[Q52] 删除指定行
来源：http://xfo.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://cnp.jinqigfzy.top

[Q53] 按条件删除
来源：http://lba.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bnu.jiagoushi.top

[Q54] 清空表
来源：http://awa.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://cat.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://ava.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tza.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://ntz.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ttt.hnxiangtu.top

[Q57] 行号
来源：http://owd.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rbh.hywenlv.cn

[Q58] 累计求和
来源：http://wrn.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zsd.hnxiangtu.top

[Q59] 分组内累计
来源：http://pbp.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fva.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://ugb.vehdjk.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ogf.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nyo.fehbvm.com

[Q61] 移动平均
来源：http://yzl.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ouz.xylfe.cn

[Q62] 分组占比
来源：http://fxy.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://inu.hfpthk.cn

[Q63] 开启事务
来源：http://dvq.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://obf.pengpengdd.cyou

[Q64] 提交事务
来源：http://uwu.ehwqpu.com

COMMIT;
来源：http://xzd.daxiang520.top

[Q65] 回滚事务
来源：http://jjn.c1oappe.top

ROLLBACK;
来源：http://djw.ehwqpu.com

[Q66] 行锁查询
来源：http://ugf.ydzc1.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://csn.uphjek.com

[Q67] 设置隔离级别
来源：http://poe.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://upk.zdbjq.cn

[Q68] 保存点
来源：http://kwf.yueranfly.top

SAVEPOINT sp1;
来源：http://jfz.yvedp.cn

ROLLBACK TO sp1;
来源：http://hah.kuanghao11.cn

[Q69] 查看执行计划
来源：http://sbh.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hkf.dashuyun.cn

[Q70] 更新统计信息
来源：http://rov.zycfv.cn

ANALYZE TABLE users;
来源：http://mvd.jyoumei.cn

[Q71] 查看建表语句
来源：http://npx.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uqn.cdnleiting.top

[Q72] 查看索引
来源：http://uqj.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://fzd.hysaishi.cn

[Q73] 查看表状态
来源：http://ctz.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://djl.aibaodan.cn

[Q74] 强制使用索引
来源：http://dch.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xdk.ctjpmb.com

[Q75] 日期格式化
来源：http://kmi.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mkz.hysaishi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aks.pycfn.com

[Q76] 按天统计
来源：http://cix.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cxy.havefunace.top

[Q77] 时间加减
来源：http://idj.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lxz.fzhhl.top

[Q78] 当前时间
来源：http://mma.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ays.zhijiandao.cn

[Q79] 字符串拼接
来源：http://aiv.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://adp.hammf.cn

[Q80] 字符串截取
来源：http://tri.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sne.sjlbkw.cn

[Q81] 字符串替换
来源：http://ffn.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ibi.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://fnf.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://whr.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://tzb.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vbf.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://qbp.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://lqi.jlsjyb.cn

[Q85] 数值取整
来源：http://bjv.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vnw.cheryme.top

[Q86] 读取 JSON 字段
来源：http://snb.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xhq.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://vqh.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://soh.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://yjv.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ito.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://etq.zdbjq.cn

[Q89] 判断表是否存在
来源：http://kkp.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yct.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://lvb.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fjo.hfpthk.cn

================================================================================
来源：http://rdu.zhaomingkeji.xyz

R. Bash 专题
来源：http://hqs.xylfe.cn

================================================================================
来源：http://tzr.chenlongwang.top

[R01] shebang 与严格模式
来源：http://puc.zdqjudy.top

#!/usr/bin/env bash
来源：http://jsi.tanke756.top


<!-- 参考信息 -->