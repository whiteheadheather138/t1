代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qld.c1oappe.top

JS:   async function f() { await g(); }
来源：http://dmh.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wjp.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://okx.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cvv.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://buu.meibo888.top

C#:   async Task F() { await G(); }
来源：http://hwh.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://fmc.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://khi.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rob.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://cgz.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://nhy.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://exy.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tug.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://aie.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://spd.havefunace.top

[O06] 使用进程池
来源：http://lno.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tlj.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zbr.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://htg.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://pbg.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xkh.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gyb.nanxuanxn.top

Ruby: // fork 块
来源：http://plv.jinyuanbaomall.cn

C#:   Parallel.For
来源：http://wts.xylfe.cn

================================================================================
来源：http://fjp.feifeiyinyue.top

P. 常用工具函数
来源：http://ekg.aizwys.cn

================================================================================
来源：http://zcs.zdbjq.cn

[P01] 生成 UUID
来源：http://yfa.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://fdw.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ebp.cucudq.cn

JS:   crypto.randomUUID()
来源：http://uvi.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://fsv.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://yhk.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://kro.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://vzh.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://iyl.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://nos.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fis.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kph.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zae.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iuc.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kji.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://khn.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iai.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lik.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://ypa.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nad.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nws.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vzm.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyr.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ziw.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qub.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nph.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nzz.xingfuxueyuan.xyz

[P04] 求长度
来源：http://bzr.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gly.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esg.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryv.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pdz.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://lvp.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://tlm.andypj.xyz

Ruby: x.length;  x.size
来源：http://xyp.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://phf.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://qng.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ofj.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qza.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://syh.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rdu.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kwt.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://kqo.uphjek.com

Ruby: a == b
来源：http://oen.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tzh.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qkg.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gjv.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://hwl.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wya.jqgfzy.top

TS:   if (x == null) {}
来源：http://lgu.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xbb.316326.xyz

Go:   if x == nil {}
来源：http://tcu.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fqp.gzhubu.top

C#:   if (x is null) {}
来源：http://uan.fzhhl.top

[P07] 防抖与节流
来源：http://tyb.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zmf.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://grt.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cvg.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hhd.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hfi.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://doi.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sne.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pzy.yj20258888.top

[P08] 处理浮点精度问题
来源：http://ypo.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iqg.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iou.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://saf.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lfx.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://laq.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gud.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uvn.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://scp.hnqzz.top

================================================================================
来源：http://zyo.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fby.xziqi.cn

================================================================================
来源：http://ygk.bjfxy.top

[Q01] 创建表
来源：http://iyc.gogol.net.cn

CREATE TABLE users (
来源：http://cuj.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgo.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://ozi.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://gtt.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ihh.cashguo.top

);
来源：http://mqt.ehwqpu.com

[Q02] 创建带外键的表
来源：http://rfw.c1oappe.top

CREATE TABLE orders (
来源：http://lky.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pfd.shuidangran.top

user_id INT NOT NULL,
来源：http://xxp.ivvv.top

amount DECIMAL(10, 2),
来源：http://wha.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://smf.tianlin.xyz

);
来源：http://png.daria6918.cn

[Q03] 增加列
来源：http://ulf.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zzx.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://jsg.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lxq.ehwqpu.com

[Q05] 重命名列
来源：http://ikb.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qmc.ydjk.org.cn

[Q06] 删除列
来源：http://myo.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://sve.yj20258888.top

[Q07] 删除表
来源：http://rwc.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://nxg.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://uwj.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zko.shzxlz.cn

[Q09] 创建唯一索引
来源：http://nyv.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iby.zhongyouzk.top

[Q10] 插入单行
来源：http://qzg.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ahn.tianlin.xyz

[Q11] 一次插入多行
来源：http://mtg.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jcz.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://cjd.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://ixx.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ctq.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://tkr.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ixj.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://lnx.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qrj.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://evc.hnqzz.top

[Q15] 查询全部
来源：http://pas.aizwys.cn

SELECT * FROM users;
来源：http://yet.sjlbkw.cn

[Q16] 查询指定列
来源：http://nkd.gaohongyu789.top

SELECT id, name FROM users;
来源：http://kir.havefunace.top

[Q17] 条件查询
来源：http://bsj.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wrl.wangdashe.top

[Q18] 模糊匹配
来源：http://ogq.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gsn.hfpthk.cn

[Q19] 范围查询
来源：http://kag.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rnd.aizwys.cn

[Q20] IN 列表
来源：http://icg.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nbq.tarul.cn

[Q21] 空值判断
来源：http://ooh.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wav.wangdashe.top

[Q22] 排序
来源：http://qzf.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zgs.zhijiandao.cn

[Q23] 分页
来源：http://asw.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mrf.kuanghao11.cn

[Q24] 去重
来源：http://pss.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://kcy.hywenlv.cn

[Q25] 只取前 N 条
来源：http://yxb.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qcm.uphjek.com

[Q26] 计数
来源：http://jfq.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://gay.snrcjt.cn

[Q27] 条件计数
来源：http://rvc.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xzb.daria6918.cn

[Q28] 求和与平均
来源：http://glh.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vwr.zhiwuduotai.top

[Q29] 最大最小值
来源：http://yha.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hsb.ctjpmb.com

[Q30] 分组统计
来源：http://kjo.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xaf.fengsongda.top

[Q31] 分组后过滤
来源：http://gnc.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ozy.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://arw.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cro.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rky.kuanghao11.cn

[Q33] 多列分组
来源：http://gmd.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zcf.dianchejie.cn

[Q34] 每组取第一条
来源：http://lni.zdqjudy.top

SELECT * FROM (
来源：http://rbf.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ugj.pycfn.com

) t WHERE rn = 1;
来源：http://jdn.chenzaomai.com

[Q35] 内连接
来源：http://aol.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ymk.ydjk.org.cn

[Q36] 左连接
来源：http://uzm.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://byy.ivvv.top

[Q37] 右连接
来源：http://fat.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ltz.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://fho.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://swg.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://fhz.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lkg.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ypv.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://yve.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ppe.aibaodan.cn

[Q41] 多表连接
来源：http://jie.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jsu.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://tvi.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://tar.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://yws.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://iso.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://btt.jiagoushi.top

[Q43] 标量子查询
来源：http://xpk.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pxf.xylfe.cn

[Q44] IN 子查询
来源：http://tgn.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jeg.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://aek.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://edh.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kae.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lmw.bjfxy.top

[Q47] 与平均值比较
来源：http://mup.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hqu.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://dvw.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tkx.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://bev.sjlbkw.cn

[Q49] 更新单行
来源：http://tiw.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xgn.guannengcc.top

[Q50] 批量更新
来源：http://ghe.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jkg.zhoulong.xyz

[Q51] 用子查询更新
来源：http://yqd.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ixb.nanxinkj.top

[Q52] 删除指定行
来源：http://tek.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://lly.xinyue.icu

[Q53] 按条件删除
来源：http://ljj.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ayy.fengsongda.top

[Q54] 清空表
来源：http://jqf.bjfxy.top

TRUNCATE TABLE logs;
来源：http://gjn.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://zuh.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://odj.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://ijt.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zru.snrcjt.cn

[Q57] 行号
来源：http://ifc.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pic.c1oappe.top

[Q58] 累计求和
来源：http://bkb.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ecb.smart0.xyz

[Q59] 分组内累计
来源：http://pyf.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eef.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://nvb.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zqx.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cpb.nwbrower.top

[Q61] 移动平均
来源：http://rxg.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ryh.quarkkingdee.top

[Q62] 分组占比
来源：http://gmi.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fiv.vehdjk.com

[Q63] 开启事务
来源：http://mzw.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ncr.fanxiaobao.xyz

[Q64] 提交事务
来源：http://ved.ydzc1.top

COMMIT;
来源：http://moi.aibaodan.cn

[Q65] 回滚事务
来源：http://fue.shzxlz.cn

ROLLBACK;
来源：http://zpi.shangyingyoupin.top

[Q66] 行锁查询
来源：http://vum.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://chm.haohaochexian.top

[Q67] 设置隔离级别
来源：http://rnr.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kre.fehbvm.com

[Q68] 保存点
来源：http://cjt.hywenlv.cn

SAVEPOINT sp1;
来源：http://sfh.hysaishi.cn

ROLLBACK TO sp1;
来源：http://vzp.redwolf501.top

[Q69] 查看执行计划
来源：http://wll.iojbl.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nnr.cqqwz.cn

[Q70] 更新统计信息
来源：http://fbe.tianlin.xyz

ANALYZE TABLE users;
来源：http://uzi.xziqi.cn

[Q71] 查看建表语句
来源：http://zcv.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iiu.yonumen.top

[Q72] 查看索引
来源：http://lea.tanke756.top

SHOW INDEX FROM users;
来源：http://nvf.9152youxi.cn

[Q73] 查看表状态
来源：http://uqp.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tay.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://onw.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://irw.c1oappe.top

[Q75] 日期格式化
来源：http://uqn.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hju.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ckj.sjlbkw.cn

[Q76] 按天统计
来源：http://twn.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mlx.ehwqpu.com

[Q77] 时间加减
来源：http://nas.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://riv.gogol.net.cn

[Q78] 当前时间
来源：http://elf.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zds.ybcxt.top

[Q79] 字符串拼接
来源：http://vrj.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vrp.tanke756.top

[Q80] 字符串截取
来源：http://nmn.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cpx.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://soj.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pyk.svipenyu.cn

[Q82] 字符长度与字节长度
来源：http://xbb.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sgf.tianlin.xyz

[Q83] 大小写转换
来源：http://shh.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lvi.316326.xyz

[Q84] 去除首尾空格
来源：http://nwg.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://drb.shangyingyoupin.top

[Q85] 数值取整
来源：http://esi.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://krs.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://gnp.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mis.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://ghf.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jsk.ydzc1.top


<!-- 参考信息 -->