代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dwc.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://hrc.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qgm.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nat.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kht.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://wuy.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://jil.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://krw.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://fue.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rpm.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://sls.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://mqf.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kme.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gzv.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://weu.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ubz.xziqi.cn

[O06] 使用进程池
来源：http://ocf.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pkc.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://igz.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://wft.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://zyi.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xsu.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lxy.sufxvd.cn

Ruby: // fork 块
来源：http://trl.yj202588.top

C#:   Parallel.For
来源：http://nfy.wangdashe.top

================================================================================
来源：http://acj.zdbjq.cn

P. 常用工具函数
来源：http://izf.guannengcc.top

================================================================================
来源：http://zhw.zhoulong.xyz

[P01] 生成 UUID
来源：http://rmz.yj20258.top

Py:   str(uuid.uuid4())
来源：http://tgr.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cyx.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://bxc.daxiang520.top

TS:   crypto.randomUUID()
来源：http://zmg.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://gfp.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://lmc.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://ucz.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://hyb.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://piw.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yox.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tfc.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://omd.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://opz.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yhf.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://swi.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gua.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jgf.ppjwa.cn

[P03] 生成短随机字符串
来源：http://loc.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gis.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ppg.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hef.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ujs.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ned.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qsu.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://csx.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xpd.yueranfly.top

[P04] 求长度
来源：http://msy.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ksf.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xis.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zyb.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gvi.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://svs.pycfn.com

Go:   len(arr);  len(m)
来源：http://xct.sxryk.cn

Ruby: x.length;  x.size
来源：http://mry.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ibb.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://hhi.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zzl.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jda.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qwk.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ngm.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ewg.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://qmw.tian-w.cn

Ruby: a == b
来源：http://ifs.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xbz.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hkf.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eya.cashguo.top

PHP:  if (empty($x)) {}
来源：http://tuh.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hlv.shzxlz.cn

TS:   if (x == null) {}
来源：http://sws.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://rdt.bbcook.cn

Go:   if x == nil {}
来源：http://zeh.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iby.smart0.xyz

C#:   if (x is null) {}
来源：http://daq.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://hzt.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uzv.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://dhf.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtc.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyj.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zjg.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://arz.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://svs.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aob.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://egb.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dfx.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wmh.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qcm.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://chc.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ito.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://avd.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jyk.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://roe.yueranfly.top

================================================================================
来源：http://cny.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yxc.havefunace.top

================================================================================
来源：http://yha.chenjidiqi.icu

[Q01] 创建表
来源：http://pfz.tianlin.xyz

CREATE TABLE users (
来源：http://vpf.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gte.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://mkl.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://xmh.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cbw.yuxming.cn

);
来源：http://uik.gotoacloud.top

[Q02] 创建带外键的表
来源：http://wql.hammf.cn

CREATE TABLE orders (
来源：http://uly.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tbt.iojbl.cn

user_id INT NOT NULL,
来源：http://fcp.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://nvb.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mxi.cdnleiting.top

);
来源：http://nzv.nanxinkj.top

[Q03] 增加列
来源：http://ria.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xgx.havefunace.top

[Q04] 修改列类型
来源：http://pqe.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ovf.epnwcf.com

[Q05] 重命名列
来源：http://qxb.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rcs.sufxvd.cn

[Q06] 删除列
来源：http://cbk.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kkn.fehbvm.com

[Q07] 删除表
来源：http://ake.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://vzk.daxiang520.top

[Q08] 创建普通索引
来源：http://rqv.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ntw.xuanzx.com

[Q09] 创建唯一索引
来源：http://ppi.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmb.jinghuilouyu.cn

[Q10] 插入单行
来源：http://non.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jwh.316326.xyz

[Q11] 一次插入多行
来源：http://css.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ove.sweek.top

[Q12] 插入后取自增 ID
来源：http://qab.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://npl.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kjr.ybcxt.top

[Q13] 忽略重复插入
来源：http://ydg.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kfu.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://wsf.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dcn.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tzv.0kj1m.cn

[Q15] 查询全部
来源：http://cwj.zhoulong.xyz

SELECT * FROM users;
来源：http://utb.fktsv.cn

[Q16] 查询指定列
来源：http://src.zhijiandao.cn

SELECT id, name FROM users;
来源：http://sep.sysykeji.top

[Q17] 条件查询
来源：http://lyp.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ycj.cqqwz.cn

[Q18] 模糊匹配
来源：http://dsp.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nko.vqdsnc.cn

[Q19] 范围查询
来源：http://hvf.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iur.yueranfly.top

[Q20] IN 列表
来源：http://lkr.xinyue.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uvn.fzhhl.top

[Q21] 空值判断
来源：http://rvb.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://lqv.nanxuanxn.top

[Q22] 排序
来源：http://zka.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://utx.xziqi.cn

[Q23] 分页
来源：http://tme.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sit.chenzaomai.com

[Q24] 去重
来源：http://aup.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://jtx.9152youxi.cn

[Q25] 只取前 N 条
来源：http://ydr.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://skg.gogol.net.cn

[Q26] 计数
来源：http://fcc.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://lqb.sufxvd.cn

[Q27] 条件计数
来源：http://svy.yonumen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dco.nwbrower.top

[Q28] 求和与平均
来源：http://sxu.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rxt.gogol.net.cn

[Q29] 最大最小值
来源：http://ncf.fanxiaobao.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://aap.haohaochexian.top

[Q30] 分组统计
来源：http://ymb.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mzi.jianghu66.top

[Q31] 分组后过滤
来源：http://mxm.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dzd.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://yep.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wia.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qzi.gaohongyu789.top

[Q33] 多列分组
来源：http://ygj.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://whc.gaohongyu789.top

[Q34] 每组取第一条
来源：http://mpd.ehwqpu.com

SELECT * FROM (
来源：http://pxo.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ksr.snrcjt.cn

) t WHERE rn = 1;
来源：http://zdf.hnqzz.top

[Q35] 内连接
来源：http://oni.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wdq.9152youxi.cn

[Q36] 左连接
来源：http://wld.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qhh.redwolf501.top

[Q37] 右连接
来源：http://bkn.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://luj.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://qiv.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dhm.yj20258.top

[Q39] 自连接（查上下级）
来源：http://knq.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fww.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ayb.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rft.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ays.xuanzx.com

[Q41] 多表连接
来源：http://sad.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://pnq.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://onc.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://hxu.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://ium.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://pgx.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sgm.wangdashe.top

[Q43] 标量子查询
来源：http://rub.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kwe.ctjpmb.com

[Q44] IN 子查询
来源：http://exk.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ukd.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://oln.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzo.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://hws.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbu.andypj.xyz

[Q47] 与平均值比较
来源：http://rzr.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://olx.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://pyo.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://srv.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://lhm.nanxuanxn.top

[Q49] 更新单行
来源：http://dkv.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lmd.shanyushiyangtech.top

[Q50] 批量更新
来源：http://urq.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tlk.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://zei.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hak.sufxvd.cn

[Q52] 删除指定行
来源：http://jvl.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://dcd.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://spl.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nxz.wangdashe.top

[Q54] 清空表
来源：http://fhu.daria6918.cn

TRUNCATE TABLE logs;
来源：http://ttw.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://vef.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vqx.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://xom.52xcode.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nbo.zhaomingkeji.xyz

[Q57] 行号
来源：http://wqc.jinghuilouyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jan.jinghuilouyu.cn

[Q58] 累计求和
来源：http://ybg.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eli.yj20258.top

[Q59] 分组内累计
来源：http://lsf.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cml.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://zcm.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ixb.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ohg.bbcook.cn

[Q61] 移动平均
来源：http://cdx.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kwo.wangshuangyany.cn

[Q62] 分组占比
来源：http://hmd.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cfz.xinyue.icu

[Q63] 开启事务
来源：http://wya.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://fuv.snrcjt.cn

[Q64] 提交事务
来源：http://jhp.zhiwuduotai.top

COMMIT;
来源：http://gwo.hysaishi.cn

[Q65] 回滚事务
来源：http://jfp.aizwys.cn

ROLLBACK;
来源：http://wxb.xinyue.icu

[Q66] 行锁查询
来源：http://ujp.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vea.shzxlz.cn

[Q67] 设置隔离级别
来源：http://vgd.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mmd.hesvh.cn

[Q68] 保存点
来源：http://tfd.hywenlv.cn

SAVEPOINT sp1;
来源：http://rac.pycfn.com

ROLLBACK TO sp1;
来源：http://hqe.ctjpmb.com

[Q69] 查看执行计划
来源：http://ycr.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mya.birdmap.top

[Q70] 更新统计信息
来源：http://vbk.xziqi.cn

ANALYZE TABLE users;
来源：http://ith.hesvh.cn

[Q71] 查看建表语句
来源：http://dim.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lzp.chenjidiqi.icu

[Q72] 查看索引
来源：http://xkw.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://cqu.chenzaomai.com

[Q73] 查看表状态
来源：http://sis.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qqc.zhijiandao.cn

[Q74] 强制使用索引
来源：http://wju.chenlongwang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://buq.aizwys.cn

[Q75] 日期格式化
来源：http://fjy.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://umq.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ddu.ctjpmb.com

[Q76] 按天统计
来源：http://clh.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zgj.wangdashe.top

[Q77] 时间加减
来源：http://xri.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rym.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://qqy.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ehm.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://wqx.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wvs.jinqigfzy.top

[Q80] 字符串截取
来源：http://bmm.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://coy.shangyingyoupin.top

[Q81] 字符串替换
来源：http://vjd.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ktf.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://kcj.bbcook.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oih.wangshuangyany.cn

[Q83] 大小写转换
来源：http://bif.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yfb.snrcjt.cn

[Q84] 去除首尾空格
来源：http://zpo.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://fez.wangshuangyany.cn

[Q85] 数值取整
来源：http://qli.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cry.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://xep.ywan-chungtsiang.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ifk.uphjek.com

[Q87] JSON 字段做条件
来源：http://tqf.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tmq.birdmap.top


<!-- 参考信息 -->