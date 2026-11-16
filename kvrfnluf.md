代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://enq.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dod.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://qxk.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bhf.9152youxi.cn

[O06] 使用进程池
来源：http://tjp.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cfe.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ijj.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://hve.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://ftz.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hbx.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lan.yvedp.cn

Ruby: // fork 块
来源：http://gkd.jlsjyb.cn

C#:   Parallel.For
来源：http://ikh.yongpay.top

================================================================================
来源：http://aum.cdnleiting.top

P. 常用工具函数
来源：http://rqv.iojbl.cn

================================================================================
来源：http://gem.mhx1999.top

[P01] 生成 UUID
来源：http://nbh.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://uwr.ydjk.org.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pxp.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://cxv.yuxming.cn

TS:   crypto.randomUUID()
来源：http://sxl.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://alg.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://ikv.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://grx.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://lkg.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://and.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://inm.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://can.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bgw.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kyo.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ezn.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rwv.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rri.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tlj.shuidangran.top

[P03] 生成短随机字符串
来源：http://mbl.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pxj.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ggp.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fpv.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hin.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wia.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nbl.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hrb.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uir.yuanzhike.top

[P04] 求长度
来源：http://ddk.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uns.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cge.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iip.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ftw.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://xmk.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://gvj.xinyue.icu

Ruby: x.length;  x.size
来源：http://yox.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gqp.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://pnv.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://txo.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://joa.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lwi.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vio.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pnc.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://wqx.pengpengdd.cyou

Ruby: a == b
来源：http://svy.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fgo.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vft.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pgt.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://ofv.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fig.hfpthk.cn

TS:   if (x == null) {}
来源：http://crc.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mba.ybcxt.top

Go:   if x == nil {}
来源：http://vzj.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wip.ctjpmb.com

C#:   if (x is null) {}
来源：http://msl.hywenlv.cn

[P07] 防抖与节流
来源：http://pba.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tcx.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://jmi.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwa.gaohongyu789.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmv.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cwc.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vuq.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://boe.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pef.daria6918.cn

[P08] 处理浮点精度问题
来源：http://jfe.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gip.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nwg.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bcv.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ikd.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lcn.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kgc.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tdh.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bgi.shanyushiyangkeji.top

================================================================================
来源：http://mum.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qli.meibo888.top

================================================================================
来源：http://qtp.xuetiantiany.cn

[Q01] 创建表
来源：http://kgp.zhoulong.xyz

CREATE TABLE users (
来源：http://xqm.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://out.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://oqd.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://mhf.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ffo.hcnkem.com

);
来源：http://com.xuanzx.com

[Q02] 创建带外键的表
来源：http://iwu.redwolf501.top

CREATE TABLE orders (
来源：http://ssi.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jir.sweek.top

user_id INT NOT NULL,
来源：http://xap.hnqzz.top

amount DECIMAL(10, 2),
来源：http://ovl.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nxi.xuanzx.com

);
来源：http://hvc.jqgfzy.top

[Q03] 增加列
来源：http://yyl.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://imd.zhiwuduotai.top

[Q04] 修改列类型
来源：http://dea.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tpl.tian-w.cn

[Q05] 重命名列
来源：http://nwf.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ini.jinqigfzy.top

[Q06] 删除列
来源：http://vmm.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ine.hnxiangtu.top

[Q07] 删除表
来源：http://uxe.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://ahu.ydzc1.top

[Q08] 创建普通索引
来源：http://kcx.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://pod.jianghu66.top

[Q09] 创建唯一索引
来源：http://ozv.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sav.chenlongwang.top

[Q10] 插入单行
来源：http://qxc.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yqc.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://gha.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lsm.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://vyl.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://tuh.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sxk.cheryme.top

[Q13] 忽略重复插入
来源：http://bvx.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jds.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://onx.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pai.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zbt.ydjk.org.cn

[Q15] 查询全部
来源：http://icd.fzhhl.top

SELECT * FROM users;
来源：http://nkt.yvedp.cn

[Q16] 查询指定列
来源：http://ckb.yangfankeji.com

SELECT id, name FROM users;
来源：http://mpx.xylfe.cn

[Q17] 条件查询
来源：http://qtx.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bdk.ydjk.org.cn

[Q18] 模糊匹配
来源：http://qyp.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://opk.ybcxt.top

[Q19] 范围查询
来源：http://wbp.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zxt.gaohongyu789.top

[Q20] IN 列表
来源：http://ybu.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lbe.c1oappe.top

[Q21] 空值判断
来源：http://nxs.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qlk.birdmap.top

[Q22] 排序
来源：http://xho.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qwr.svipenyu.cn

[Q23] 分页
来源：http://ttb.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qau.ydjk.org.cn

[Q24] 去重
来源：http://fji.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://eaz.xylfe.cn

[Q25] 只取前 N 条
来源：http://cfx.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pih.yj20258.top

[Q26] 计数
来源：http://yyp.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://cxt.meibo888.top

[Q27] 条件计数
来源：http://emj.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lec.cqqwz.cn

[Q28] 求和与平均
来源：http://kdh.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tff.vqdsnc.cn

[Q29] 最大最小值
来源：http://rcc.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yzv.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://zau.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://glm.svipenyu.cn

[Q31] 分组后过滤
来源：http://ubc.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qoe.gzhubu.top

[Q32] 分组拼接字符串
来源：http://wvv.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kad.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qjk.jlsjyb.cn

[Q33] 多列分组
来源：http://fko.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://axt.shuidangran.top

[Q34] 每组取第一条
来源：http://ptw.jqgufenzy.top

SELECT * FROM (
来源：http://rky.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jkl.zhijiandao.cn

) t WHERE rn = 1;
来源：http://sjj.52xcode.cn

[Q35] 内连接
来源：http://dfn.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cei.daxiang520.top

[Q36] 左连接
来源：http://czj.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sys.aizwys.cn

[Q37] 右连接
来源：http://cwb.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cnj.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://qhe.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fyj.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://vxw.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wxa.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cuo.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cjs.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bfp.ehwqpu.com

[Q41] 多表连接
来源：http://lkq.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wqu.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://kta.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://jif.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://spq.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://tsl.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rvd.vehdjk.com

[Q43] 标量子查询
来源：http://uzc.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://brm.vqdsnc.cn

[Q44] IN 子查询
来源：http://xrt.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ufo.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://wtn.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ebn.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mqu.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wnt.jlsjyb.cn

[Q47] 与平均值比较
来源：http://gif.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lip.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://ndr.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ouq.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://cqo.xuanzx.com

[Q49] 更新单行
来源：http://xob.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ntl.sufxvd.cn

[Q50] 批量更新
来源：http://zti.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kpi.fktsv.cn

[Q51] 用子查询更新
来源：http://mwi.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lkk.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://ruu.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://xre.fengsongda.top

[Q53] 按条件删除
来源：http://ttp.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qxd.nwbrower.top

[Q54] 清空表
来源：http://kci.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://udo.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://buc.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tip.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://mmz.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://erl.feifeiyinyue.top

[Q57] 行号
来源：http://jyd.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cia.ehwqpu.com

[Q58] 累计求和
来源：http://mjq.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rlg.nanxinkj.top

[Q59] 分组内累计
来源：http://mmo.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hqk.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://uyi.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uoe.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://muy.yj20258.top

[Q61] 移动平均
来源：http://kvo.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jwr.fzhhl.top

[Q62] 分组占比
来源：http://qau.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uds.52xcode.cn

[Q63] 开启事务
来源：http://hxn.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://azh.xuanzx.com

[Q64] 提交事务
来源：http://cmh.hnqzz.top

COMMIT;
来源：http://zlh.ctjpmb.com

[Q65] 回滚事务
来源：http://fck.mhx1999.top

ROLLBACK;
来源：http://pxk.cashguo.top

[Q66] 行锁查询
来源：http://mxp.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fjh.bjfxy.top

[Q67] 设置隔离级别
来源：http://jaz.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://byu.yanxiufei.cn

[Q68] 保存点
来源：http://icv.yonumen.top

SAVEPOINT sp1;
来源：http://ayr.bbcook.cn

ROLLBACK TO sp1;
来源：http://vzz.zhongyouzk.top

[Q69] 查看执行计划
来源：http://mhu.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wdk.hfpthk.cn

[Q70] 更新统计信息
来源：http://fvl.zhengqikj.top

ANALYZE TABLE users;
来源：http://jtz.yuanzhike.top

[Q71] 查看建表语句
来源：http://swh.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jnt.jinghuilouyu.cn

[Q72] 查看索引
来源：http://mhl.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://tiv.jqgufenzy.top

[Q73] 查看表状态
来源：http://osf.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iie.vqdsnc.cn

[Q74] 强制使用索引
来源：http://yhs.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://psf.svipenyu.cn

[Q75] 日期格式化
来源：http://byk.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yuw.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ckv.chenjidiqi.icu

[Q76] 按天统计
来源：http://lnm.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lhd.shuidangran.top

[Q77] 时间加减
来源：http://wqg.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fio.ehwqpu.com

[Q78] 当前时间
来源：http://kbx.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fco.gotoacloud.top

[Q79] 字符串拼接
来源：http://zvd.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cvr.yanxiufei.cn

[Q80] 字符串截取
来源：http://ygq.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wqs.nwbrower.top

[Q81] 字符串替换
来源：http://mdo.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zdp.havefunace.top

[Q82] 字符长度与字节长度
来源：http://jii.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oqx.cheryme.top

[Q83] 大小写转换
来源：http://pwn.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zvp.hcnkem.com

[Q84] 去除首尾空格
来源：http://mcz.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://mwe.ydzc1.top

[Q85] 数值取整
来源：http://xps.redwolf501.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wsl.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://woh.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aam.tanke756.top

[Q87] JSON 字段做条件
来源：http://rbw.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://znx.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://dbd.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qii.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xep.ydzc1.top

[Q89] 判断表是否存在
来源：http://ymc.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://plr.cucudq.cn

[Q90] 生成序号列
来源：http://lgd.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rvu.zycfv.cn

================================================================================
来源：http://ehl.wangshuangyany.cn

R. Bash 专题
来源：http://pwp.redwolf501.top

================================================================================
来源：http://shj.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://qqg.vqdsnc.cn

#!/usr/bin/env bash
来源：http://dvc.redwolf501.top


<!-- 参考信息 -->