代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://cqj.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lkz.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://rhq.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://awh.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zny.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gbf.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://eoz.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ewa.jinqigufen.top

[O06] 使用进程池
来源：http://zha.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iec.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hxq.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://wud.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://nai.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vls.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fcj.sysykeji.top

Ruby: // fork 块
来源：http://kct.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://uet.snrcjt.cn

================================================================================
来源：http://izv.mhx1999.top

P. 常用工具函数
来源：http://bms.zhiwuduotai.top

================================================================================
来源：http://kuv.shuidangran.top

[P01] 生成 UUID
来源：http://jca.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://rsg.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ope.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://bbp.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://vlb.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://dgp.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://scw.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://jca.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://lsb.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://ajm.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wwl.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://kln.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dxg.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhl.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sdh.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fux.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tlm.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jwi.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://fnd.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ilk.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ohw.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nqt.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ary.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://otg.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aox.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://anw.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ilt.feifeiyinyue.top

[P04] 求长度
来源：http://rza.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qga.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://via.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgg.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wqo.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://lqx.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://rik.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://hjv.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qvr.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://zxg.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hku.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vcb.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://etl.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://has.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://avg.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://oqd.gotoacloud.top

Ruby: a == b
来源：http://bpc.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://efn.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kne.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://znl.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://fsh.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fjw.jqgfzy.top

TS:   if (x == null) {}
来源：http://alc.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zfh.yj20258.top

Go:   if x == nil {}
来源：http://jqr.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iyj.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://hqd.cheryme.top

[P07] 防抖与节流
来源：http://mkr.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wkp.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://wka.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgd.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rcp.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nje.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://awb.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wil.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jyg.yongpay.top

[P08] 处理浮点精度问题
来源：http://gxd.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sqc.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hfe.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spv.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rtt.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kec.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xvi.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ytt.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://krg.fzhhl.top

================================================================================
来源：http://dqh.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://usk.pengpengdd.cyou

================================================================================
来源：http://qnr.tarul.cn

[Q01] 创建表
来源：http://juh.ppjwa.cn

CREATE TABLE users (
来源：http://amv.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwe.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://rvq.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://ecz.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wrt.nanxinkj.top

);
来源：http://zkh.mhx1999.top

[Q02] 创建带外键的表
来源：http://pjm.cqqwz.cn

CREATE TABLE orders (
来源：http://kjp.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hlo.haohaochexian.top

user_id INT NOT NULL,
来源：http://yps.birdmap.top

amount DECIMAL(10, 2),
来源：http://gkx.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zds.uphjek.com

);
来源：http://xup.tianlin.xyz

[Q03] 增加列
来源：http://ion.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gqb.aibaodan.cn

[Q04] 修改列类型
来源：http://urr.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bbm.dashuyun.cn

[Q05] 重命名列
来源：http://abk.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ewo.wangshuangyany.cn

[Q06] 删除列
来源：http://suq.aibaodan.cn

ALTER TABLE users DROP COLUMN age;
来源：http://elj.zdbjq.cn

[Q07] 删除表
来源：http://tih.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://qxu.tianlin.xyz

[Q08] 创建普通索引
来源：http://cof.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://baw.guannengcc.top

[Q09] 创建唯一索引
来源：http://anu.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vhx.sysykeji.top

[Q10] 插入单行
来源：http://xyg.nanxinkj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uay.zhixingplan.top

[Q11] 一次插入多行
来源：http://sby.guannengcc.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ffa.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://dsq.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://tyn.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ebb.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://tqk.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://efg.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://pem.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oei.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kmn.ehwqpu.com

[Q15] 查询全部
来源：http://pbu.jinqigufen.top

SELECT * FROM users;
来源：http://ayf.shangyingyoupin.top

[Q16] 查询指定列
来源：http://cei.zhongyouzk.top

SELECT id, name FROM users;
来源：http://ntx.meibo888.top

[Q17] 条件查询
来源：http://apj.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eok.nwbrower.top

[Q18] 模糊匹配
来源：http://pqo.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ycv.pycfn.com

[Q19] 范围查询
来源：http://uwc.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://emb.cucudq.cn

[Q20] IN 列表
来源：http://mjk.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://afo.cqqwz.cn

[Q21] 空值判断
来源：http://lmh.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://lak.ctjpmb.com

[Q22] 排序
来源：http://hwv.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://esx.yuanzhike.top

[Q23] 分页
来源：http://lry.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kaw.jyoumei.cn

[Q24] 去重
来源：http://srf.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://ylq.yfazqb.com

[Q25] 只取前 N 条
来源：http://cjh.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blb.yongpay.top

[Q26] 计数
来源：http://lcf.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://vyz.nanxuanxn.top

[Q27] 条件计数
来源：http://xtn.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://puh.wangdashe.top

[Q28] 求和与平均
来源：http://tla.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kyu.redwolf501.top

[Q29] 最大最小值
来源：http://zhc.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://xwz.hesvh.cn

[Q30] 分组统计
来源：http://epl.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oqm.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://sse.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jrx.shangyingyoupin.top

[Q32] 分组拼接字符串
来源：http://zol.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gdv.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ctv.zycfv.cn

[Q33] 多列分组
来源：http://pfr.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://job.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://liq.hywenlv.cn

SELECT * FROM (
来源：http://uzx.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uot.daria6918.cn

) t WHERE rn = 1;
来源：http://kft.yangfankeji.com

[Q35] 内连接
来源：http://byq.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vzb.kuanghao11.cn

[Q36] 左连接
来源：http://fin.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://plh.uphjek.com

[Q37] 右连接
来源：http://rju.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fte.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://hdt.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nfn.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://pfr.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mic.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zbb.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jxa.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://scv.yangfankeji.com

[Q41] 多表连接
来源：http://qty.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xhq.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://agu.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://ite.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://vaj.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://wtk.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ubm.pengpengdd.cyou

[Q43] 标量子查询
来源：http://bkq.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wdd.zhiwuduotai.top

[Q44] IN 子查询
来源：http://uzm.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cyr.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://lpc.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zbp.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://las.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eyw.hywenlv.cn

[Q47] 与平均值比较
来源：http://mwo.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://icb.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://umt.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bwe.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://nyz.yj20258.top

[Q49] 更新单行
来源：http://yve.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://buf.316326.xyz

[Q50] 批量更新
来源：http://oln.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tss.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://uxq.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bes.redwolf501.top

[Q52] 删除指定行
来源：http://rpg.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://mqc.bbcook.cn

[Q53] 按条件删除
来源：http://usi.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzv.epnwcf.com

[Q54] 清空表
来源：http://ogp.tanke756.top

TRUNCATE TABLE logs;
来源：http://igx.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://wkq.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yiy.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://jur.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zai.52xcode.cn

[Q57] 行号
来源：http://pbb.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dek.snrcjt.cn

[Q58] 累计求和
来源：http://qwy.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jmg.jiagoushi.top

[Q59] 分组内累计
来源：http://dpf.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ghi.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://uvq.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://afj.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zoz.sjlbkw.cn

[Q61] 移动平均
来源：http://pbu.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rtd.chenzaomai.com

[Q62] 分组占比
来源：http://ldw.sufxvd.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://say.tian-w.cn

[Q63] 开启事务
来源：http://juz.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yik.zdbjq.cn

[Q64] 提交事务
来源：http://dsw.shangyingyoupin.top

COMMIT;
来源：http://akq.yuanzhike.top

[Q65] 回滚事务
来源：http://hnq.aibaodan.cn

ROLLBACK;
来源：http://ssa.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://tiz.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://muf.shuidangran.top

[Q67] 设置隔离级别
来源：http://rlw.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oel.zhixingplan.top

[Q68] 保存点
来源：http://idt.cheryme.top

SAVEPOINT sp1;
来源：http://uza.xuanzx.com

ROLLBACK TO sp1;
来源：http://vke.xuanzx.com

[Q69] 查看执行计划
来源：http://sjx.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ukx.xziqi.cn

[Q70] 更新统计信息
来源：http://hex.birdmap.top

ANALYZE TABLE users;
来源：http://uyv.gzhubu.top

[Q71] 查看建表语句
来源：http://efs.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mbp.birdmap.top

[Q72] 查看索引
来源：http://cge.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://bvt.vehdjk.com

[Q73] 查看表状态
来源：http://vkw.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aob.zdbjq.cn

[Q74] 强制使用索引
来源：http://jgg.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pro.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://qvm.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://coc.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bdv.shuidangran.top

[Q76] 按天统计
来源：http://rcn.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jlw.chenzaomai.com

[Q77] 时间加减
来源：http://map.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fqw.zhongyouzk.top

[Q78] 当前时间
来源：http://vai.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://btd.daria6918.cn

[Q79] 字符串拼接
来源：http://dpd.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nxx.gotoacloud.top

[Q80] 字符串截取
来源：http://vuo.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xbn.0kj1m.cn

[Q81] 字符串替换
来源：http://zdk.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wtd.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://msr.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vjt.haohaochexian.top

[Q83] 大小写转换
来源：http://lcu.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://icm.yj20258.top

[Q84] 去除首尾空格
来源：http://tlv.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://gbw.tian-w.cn

[Q85] 数值取整
来源：http://qlz.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zxq.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://nvz.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://snc.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://run.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fnz.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://kzr.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ikc.daria6918.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ssm.snrcjt.cn

[Q89] 判断表是否存在
来源：http://vna.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ilv.zhongyouzk.top

[Q90] 生成序号列
来源：http://pka.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nlz.shanyushiyangkeji.top

================================================================================
来源：http://zex.gzhubu.top


<!-- 参考信息 -->