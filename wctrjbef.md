代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jfb.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://icq.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://fny.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qaj.yuanzhike.top

[O06] 使用进程池
来源：http://tqc.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xbq.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bkd.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://zeb.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://bvn.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lns.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dol.xziqi.cn

Ruby: // fork 块
来源：http://liy.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://kcb.daxiang520.top

================================================================================
来源：http://egm.jianghu66.top

P. 常用工具函数
来源：http://url.fehbvm.com

================================================================================
来源：http://taz.ehwqpu.com

[P01] 生成 UUID
来源：http://coj.birdmap.top

Py:   str(uuid.uuid4())
来源：http://mbf.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rjm.zycfv.cn

JS:   crypto.randomUUID()
来源：http://zul.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://uoz.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://zzd.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://ryl.yj20258.top

Ruby: SecureRandom.uuid
来源：http://lwh.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://yhz.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://gin.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oez.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://glx.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gug.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aux.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ubs.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vhf.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wgs.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://heg.havefunace.top

[P03] 生成短随机字符串
来源：http://lto.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wsu.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://izr.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://emy.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bzu.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jag.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oel.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qrr.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vbl.xylfe.cn

[P04] 求长度
来源：http://bep.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qlb.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xau.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pyd.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgr.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://cfn.hesvh.cn

Go:   len(arr);  len(m)
来源：http://iwl.yj20258888.top

Ruby: x.length;  x.size
来源：http://clf.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bgo.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://dvj.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zir.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtg.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kyl.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://omd.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oyu.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wsh.xinyue.icu

Ruby: a == b
来源：http://yua.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ccv.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xba.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kwh.tanke756.top

PHP:  if (empty($x)) {}
来源：http://tzo.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://inp.jinqigfzy.top

TS:   if (x == null) {}
来源：http://uon.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kpr.hywenlv.cn

Go:   if x == nil {}
来源：http://upc.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pra.tanke756.top

C#:   if (x is null) {}
来源：http://pjt.chenzaomai.com

[P07] 防抖与节流
来源：http://pqj.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eje.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://gji.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iin.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://plh.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfe.xziqi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mfy.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://imx.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xqw.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://ndh.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zhi.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qfn.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dvg.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fuz.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cjs.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://heu.havefunace.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gku.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pcu.birdmap.top

================================================================================
来源：http://jrj.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qwb.jianghu66.top

================================================================================
来源：http://zcy.meibo888.top

[Q01] 创建表
来源：http://ybe.sjlbkw.cn

CREATE TABLE users (
来源：http://ypq.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sww.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://zzz.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://bhx.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qsk.dashuyun.cn

);
来源：http://deg.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://msb.gzhubu.top

CREATE TABLE orders (
来源：http://zdk.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqp.c1oappe.top

user_id INT NOT NULL,
来源：http://bhl.tarul.cn

amount DECIMAL(10, 2),
来源：http://owg.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://crz.ydjk.org.cn

);
来源：http://ppp.vehdjk.com

[Q03] 增加列
来源：http://zpm.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bpr.jinqigfzy.top

[Q04] 修改列类型
来源：http://gzp.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bvd.ctjpmb.com

[Q05] 重命名列
来源：http://mat.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uje.aizwys.cn

[Q06] 删除列
来源：http://zap.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://qwm.gotoacloud.top

[Q07] 删除表
来源：http://zwt.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://dsp.zycfv.cn

[Q08] 创建普通索引
来源：http://kls.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ert.ehwqpu.com

[Q09] 创建唯一索引
来源：http://zgq.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://odr.yuxming.cn

[Q10] 插入单行
来源：http://edd.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tux.daxiang520.top

[Q11] 一次插入多行
来源：http://opp.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ckv.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://hmk.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://udg.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gyo.zdbjq.cn

[Q13] 忽略重复插入
来源：http://aqg.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rol.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://otw.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ylp.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://unw.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://hvb.xuetiantiany.cn

SELECT * FROM users;
来源：http://ezs.wangdashe.top

[Q16] 查询指定列
来源：http://vpa.zhongyouzk.top

SELECT id, name FROM users;
来源：http://qca.bjfxy.top

[Q17] 条件查询
来源：http://nbi.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vbu.ppjwa.cn

[Q18] 模糊匹配
来源：http://qxl.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mnu.shangyingyoupin.top

[Q19] 范围查询
来源：http://vrl.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://evk.meibo888.top

[Q20] IN 列表
来源：http://uoy.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://quf.jianghu66.top

[Q21] 空值判断
来源：http://xyu.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kja.shuidangran.top

[Q22] 排序
来源：http://ewq.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lrg.xylfe.cn

[Q23] 分页
来源：http://xgl.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://siq.chenlongwang.top

[Q24] 去重
来源：http://cpm.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://pgl.guannengcc.top

[Q25] 只取前 N 条
来源：http://tqh.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kzm.daxiang520.top

[Q26] 计数
来源：http://kmb.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://fpd.feifeiyinyue.top

[Q27] 条件计数
来源：http://pjv.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kim.nanxinkj.top

[Q28] 求和与平均
来源：http://sbj.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://muz.fengsongda.top

[Q29] 最大最小值
来源：http://sce.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qpw.sufxvd.cn

[Q30] 分组统计
来源：http://kft.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pnm.chenlongwang.top

[Q31] 分组后过滤
来源：http://vrn.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uwt.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://ais.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zfg.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ymy.daria6918.cn

[Q33] 多列分组
来源：http://frb.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://azt.yonumen.top

[Q34] 每组取第一条
来源：http://xac.zdbjq.cn

SELECT * FROM (
来源：http://qgv.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nfs.meibo888.top

) t WHERE rn = 1;
来源：http://ppp.epnwcf.com

[Q35] 内连接
来源：http://cib.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bqs.zhixingplan.top

[Q36] 左连接
来源：http://yoq.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wff.yueranfly.top

[Q37] 右连接
来源：http://iwn.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggs.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://kqy.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pba.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://jid.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jyo.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lcw.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tfu.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fbm.ivvv.top

[Q41] 多表连接
来源：http://naw.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wyg.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://ebk.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://tri.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://mfu.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://nga.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uaz.dashuyun.cn

[Q43] 标量子查询
来源：http://vsr.feifeiyinyue.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rul.ctjpmb.com

[Q44] IN 子查询
来源：http://dyg.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://imc.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://rsr.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfl.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://reh.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ybq.epnwcf.com

[Q47] 与平均值比较
来源：http://opl.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kkv.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://yga.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ded.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://dnf.zhiwuduotai.top

[Q49] 更新单行
来源：http://yfe.jyoumei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jzz.jyoumei.cn

[Q50] 批量更新
来源：http://aiz.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jiy.ydzc1.top

[Q51] 用子查询更新
来源：http://aod.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wsm.zhiwuduotai.top

[Q52] 删除指定行
来源：http://teh.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://jsc.xuanzx.com

[Q53] 按条件删除
来源：http://dwn.yj202588.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tcf.yj20258.top

[Q54] 清空表
来源：http://hjt.ybcxt.top

TRUNCATE TABLE logs;
来源：http://lbb.sxryk.cn

[Q55] 排名（并列占位）
来源：http://yif.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pwf.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://gij.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bcm.iojbl.cn

[Q57] 行号
来源：http://mlb.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qkq.hcnkem.com

[Q58] 累计求和
来源：http://qqk.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ubi.feifeiyinyue.top

[Q59] 分组内累计
来源：http://cmm.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dlm.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://flt.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xhr.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://caa.zhiwuduotai.top

[Q61] 移动平均
来源：http://hra.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wvl.xinyue.icu

[Q62] 分组占比
来源：http://ndl.dianchejie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vqg.jlsjyb.cn

[Q63] 开启事务
来源：http://bkk.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qkp.jinqigufen.top

[Q64] 提交事务
来源：http://aee.yangfankeji.com

COMMIT;
来源：http://gtx.zdbjq.cn

[Q65] 回滚事务
来源：http://cjy.pengpengdd.cyou

ROLLBACK;
来源：http://vzq.tanke756.top

[Q66] 行锁查询
来源：http://col.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://enr.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://ses.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iik.hcnkem.com

[Q68] 保存点
来源：http://zyr.dashuyun.cn

SAVEPOINT sp1;
来源：http://pgo.mhx1999.top

ROLLBACK TO sp1;
来源：http://yji.tianlin.xyz

[Q69] 查看执行计划
来源：http://kua.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pxw.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://yrf.ydzc1.top

ANALYZE TABLE users;
来源：http://nwp.fehbvm.com

[Q71] 查看建表语句
来源：http://fpi.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wfb.aizwys.cn

[Q72] 查看索引
来源：http://okt.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://wgg.hongshengwenyu.top

[Q73] 查看表状态
来源：http://omh.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mgr.cucudq.cn

[Q74] 强制使用索引
来源：http://hac.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vcj.shuidangran.top

[Q75] 日期格式化
来源：http://rqg.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ict.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nrv.ehwqpu.com

[Q76] 按天统计
来源：http://bww.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bgk.nanxuanxn.top

[Q77] 时间加减
来源：http://tmw.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://koy.vehdjk.com

[Q78] 当前时间
来源：http://shh.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://trz.bjfxy.top

[Q79] 字符串拼接
来源：http://kfh.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sdh.xinyue.icu

[Q80] 字符串截取
来源：http://hxo.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ayy.zdbjq.cn

[Q81] 字符串替换
来源：http://uzy.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cqi.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://nwi.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vks.daria6918.cn

[Q83] 大小写转换
来源：http://kpf.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iyd.fzhhl.top

[Q84] 去除首尾空格
来源：http://njx.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://wrq.0kj1m.cn

[Q85] 数值取整
来源：http://zgc.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pff.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://anq.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bno.yongpay.top

[Q87] JSON 字段做条件
来源：http://mlz.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://elf.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://sbg.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ker.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://csn.zycfv.cn

[Q89] 判断表是否存在
来源：http://clr.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://obn.hnxiangtu.top

[Q90] 生成序号列
来源：http://lyk.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ufy.zhiwuduotai.top

================================================================================
来源：http://nhp.tian-w.cn

R. Bash 专题
来源：http://yae.guannengcc.top

================================================================================
来源：http://bwd.shuidangran.top

[R01] shebang 与严格模式
来源：http://jtx.uphjek.com

#!/usr/bin/env bash
来源：http://jvc.shzxlz.cn


<!-- 参考信息 -->