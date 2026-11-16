代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lqo.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://eir.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aiv.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iim.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://haz.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://zos.cheryme.top

C#:   async Task F() { await G(); }
来源：http://ixa.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://dpf.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://nkd.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://icl.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://obc.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://wnx.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cyq.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jrt.shuidangran.top

Ruby: threads.map(&:join)
来源：http://wwr.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lvb.jqgfzy.top

[O06] 使用进程池
来源：http://dfj.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tpp.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fii.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://jqu.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://blm.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://naj.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yya.0kj1m.cn

Ruby: // fork 块
来源：http://oie.fktsv.cn

C#:   Parallel.For
来源：http://lxg.chenjidiqi.icu

================================================================================
来源：http://utj.hammf.cn

P. 常用工具函数
来源：http://daz.316326.xyz

================================================================================
来源：http://zgo.feifeiyinyue.top

[P01] 生成 UUID
来源：http://grm.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://kmp.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ztl.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://gyt.daria6918.cn

TS:   crypto.randomUUID()
来源：http://wim.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://upy.0kj1m.cn

Go:   // 用 github.com/google/uuid
来源：http://piz.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://usi.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://jxa.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://ojv.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://asx.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qrl.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mpq.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wtz.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://leh.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ncs.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zrs.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hjv.fktsv.cn

[P03] 生成短随机字符串
来源：http://hlm.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pvc.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lio.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vop.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fdr.zhongyouzk.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sll.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oul.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jhj.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://krm.hnxiangtu.top

[P04] 求长度
来源：http://oui.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://waz.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxh.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nch.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ftg.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://mmz.guannengcc.top

Go:   len(arr);  len(m)
来源：http://lqu.haohaochexian.top

Ruby: x.length;  x.size
来源：http://gof.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iro.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://upv.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://acp.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fwo.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uvb.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rjg.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fvl.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tvc.jinqigufen.top

Ruby: a == b
来源：http://sdm.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vct.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yer.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://llb.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://eth.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pqd.nanxinkj.top

TS:   if (x == null) {}
来源：http://qga.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://kvd.xuanzx.com

Go:   if x == nil {}
来源：http://nnb.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nga.tanke756.top

C#:   if (x is null) {}
来源：http://pdl.zhijiandao.cn

[P07] 防抖与节流
来源：http://cgb.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iss.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://ezu.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxz.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcg.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fxi.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ypv.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zze.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pgv.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://zsp.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uhl.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zct.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ipk.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gjf.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zud.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zvf.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aui.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mjf.haohaochexian.top

================================================================================
来源：http://jqk.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vxm.nwbrower.top

================================================================================
来源：http://hrq.fktsv.cn

[Q01] 创建表
来源：http://sfs.zhijiandao.cn

CREATE TABLE users (
来源：http://qbw.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bep.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://fvv.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://bqx.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mcx.zhaomingkeji.xyz

);
来源：http://lbr.haohaochexian.top

[Q02] 创建带外键的表
来源：http://xvn.mhx1999.top

CREATE TABLE orders (
来源：http://yen.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nui.sweek.top

user_id INT NOT NULL,
来源：http://nkf.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://dwx.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hya.yonumen.top

);
来源：http://eok.aizwys.cn

[Q03] 增加列
来源：http://gjr.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qvr.svipenyu.cn

[Q04] 修改列类型
来源：http://rug.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wcx.dianchejie.cn

[Q05] 重命名列
来源：http://zfz.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nzw.epnwcf.com

[Q06] 删除列
来源：http://vnc.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://pva.jinqigfzy.top

[Q07] 删除表
来源：http://iox.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://ywb.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://rjs.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gnw.guowangkeji.top

[Q09] 创建唯一索引
来源：http://ugo.yueranfly.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://njk.aibaodan.cn

[Q10] 插入单行
来源：http://wqp.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://czx.birdmap.top

[Q11] 一次插入多行
来源：http://qgm.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ivl.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://orl.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uxd.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://enn.fzhhl.top

[Q13] 忽略重复插入
来源：http://gmh.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yqz.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://oxh.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rje.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qxx.yvedp.cn

[Q15] 查询全部
来源：http://eoq.zhengqikj.top

SELECT * FROM users;
来源：http://dzo.fktsv.cn

[Q16] 查询指定列
来源：http://zvv.jyoumei.cn

SELECT id, name FROM users;
来源：http://zpj.fzhhl.top

[Q17] 条件查询
来源：http://lhd.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://atv.zhoulong.xyz

[Q18] 模糊匹配
来源：http://jee.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pni.jyoumei.cn

[Q19] 范围查询
来源：http://oml.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cpd.sysykeji.top

[Q20] IN 列表
来源：http://diq.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jqm.ppjwa.cn

[Q21] 空值判断
来源：http://asn.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://nna.pengpengdd.cyou

[Q22] 排序
来源：http://jqj.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ffj.jianghu66.top

[Q23] 分页
来源：http://nom.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xaf.hongshengwenyu.top

[Q24] 去重
来源：http://xrd.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://enj.yj202588.top

[Q25] 只取前 N 条
来源：http://hqi.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iym.hongshengwenyu.top

[Q26] 计数
来源：http://meb.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://ecj.zhongyouzk.top

[Q27] 条件计数
来源：http://nad.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kec.haohaochexian.top

[Q28] 求和与平均
来源：http://ols.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wdj.sjlbkw.cn

[Q29] 最大最小值
来源：http://rur.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ogb.jyoumei.cn

[Q30] 分组统计
来源：http://aab.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zvu.tianlin.xyz

[Q31] 分组后过滤
来源：http://rlm.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qwx.c1oappe.top

[Q32] 分组拼接字符串
来源：http://nrg.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jok.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cfj.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://uvk.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pew.yj20258888.top

[Q34] 每组取第一条
来源：http://gmr.fanxiaobao.xyz

SELECT * FROM (
来源：http://rlk.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xeh.jinqigufen.top

) t WHERE rn = 1;
来源：http://lky.jinyuanbaomall.cn

[Q35] 内连接
来源：http://nvb.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lvb.yuxming.cn

[Q36] 左连接
来源：http://uvb.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ysw.cqqwz.cn

[Q37] 右连接
来源：http://kkt.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cnx.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://lqn.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lua.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://oeq.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdt.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://phk.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://awp.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fsf.sysykeji.top

[Q41] 多表连接
来源：http://neb.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fqq.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://mqi.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://top.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://qjd.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://fgy.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zez.daxiang520.top

[Q43] 标量子查询
来源：http://bah.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wiv.mhx1999.top

[Q44] IN 子查询
来源：http://qdj.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mnx.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://rzu.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kzi.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://yyb.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://slm.hywenlv.cn

[Q47] 与平均值比较
来源：http://lja.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bvk.ppjwa.cn

[Q48] CTE 公用表表达式
来源：http://qls.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nag.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://zsb.52xcode.cn

[Q49] 更新单行
来源：http://fbx.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://axw.birdmap.top

[Q50] 批量更新
来源：http://rqo.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nlw.sxryk.cn

[Q51] 用子查询更新
来源：http://xmi.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nil.ivvv.top

[Q52] 删除指定行
来源：http://zum.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://cod.yfazqb.com

[Q53] 按条件删除
来源：http://ejk.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fiu.zycfv.cn

[Q54] 清空表
来源：http://ijq.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://rgu.xylfe.cn

[Q55] 排名（并列占位）
来源：http://oyb.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ovd.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://duq.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kkv.hnqzz.top

[Q57] 行号
来源：http://oao.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zwm.52xcode.cn

[Q58] 累计求和
来源：http://ssy.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://afs.shuidangran.top

[Q59] 分组内累计
来源：http://dwg.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gjz.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://cso.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nmf.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dzx.yuanzhike.top

[Q61] 移动平均
来源：http://bnm.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ywg.hnxiangtu.top

[Q62] 分组占比
来源：http://yea.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tbm.dianchejie.cn

[Q63] 开启事务
来源：http://ieu.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cnm.jinghuilouyu.cn

[Q64] 提交事务
来源：http://kjc.tarul.cn

COMMIT;
来源：http://qyl.uphjek.com

[Q65] 回滚事务
来源：http://ycc.wangdashe.top

ROLLBACK;
来源：http://wtu.tarul.cn

[Q66] 行锁查询
来源：http://pxb.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bxe.xziqi.cn

[Q67] 设置隔离级别
来源：http://ovp.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cie.fehbvm.com

[Q68] 保存点
来源：http://mle.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://tsx.redwolf501.top

ROLLBACK TO sp1;
来源：http://twh.jyoumei.cn

[Q69] 查看执行计划
来源：http://knj.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dqo.jinqigufen.top

[Q70] 更新统计信息
来源：http://uzv.yj20258888.top

ANALYZE TABLE users;
来源：http://whs.xylfe.cn

[Q71] 查看建表语句
来源：http://tvu.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sxj.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://mxo.gogol.net.cn

SHOW INDEX FROM users;
来源：http://rgl.chenjidiqi.icu

[Q73] 查看表状态
来源：http://hjh.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://otd.bbcook.cn

[Q74] 强制使用索引
来源：http://qlj.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mfk.havefunace.top

[Q75] 日期格式化
来源：http://sni.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pnz.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aif.0kj1m.cn

[Q76] 按天统计
来源：http://lwv.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://htq.jqgfzy.top

[Q77] 时间加减
来源：http://ylq.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fas.sjlbkw.cn

[Q78] 当前时间
来源：http://djw.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kca.daxiang520.top

[Q79] 字符串拼接
来源：http://vdj.guannengcc.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aic.wangdashe.top

[Q80] 字符串截取
来源：http://zho.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tos.gotoacloud.top

[Q81] 字符串替换
来源：http://jci.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ube.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://nuk.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lvq.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://vkh.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://adq.bbcook.cn

[Q84] 去除首尾空格
来源：http://utb.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://rbw.wangshuangyany.cn

[Q85] 数值取整
来源：http://vrc.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://reb.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://phs.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ubq.wangdashe.top

[Q87] JSON 字段做条件
来源：http://xfh.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yvu.yueranfly.top


<!-- 参考信息 -->