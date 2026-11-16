代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qng.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://vlu.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://isi.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fcr.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wzv.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://sdh.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://jtf.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://tgb.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://wzd.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vwq.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://whv.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://hwy.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hjg.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hbq.aizwys.cn

Ruby: threads.map(&:join)
来源：http://wkw.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nwf.chenzaomai.com

[O06] 使用进程池
来源：http://krj.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cfc.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://xgi.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://gnv.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://rvp.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://flb.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mai.vqdsnc.cn

Ruby: // fork 块
来源：http://jdf.ydzc1.top

C#:   Parallel.For
来源：http://gnf.xziqi.cn

================================================================================
来源：http://iwi.dianchejie.cn

P. 常用工具函数
来源：http://cuj.xinyue.icu

================================================================================
来源：http://fiv.ctjpmb.com

[P01] 生成 UUID
来源：http://pyt.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://jqc.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ewp.wangdashe.top

JS:   crypto.randomUUID()
来源：http://crr.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://eju.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://pbq.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://tkh.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://mpp.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://qjr.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://ekp.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nxa.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gyy.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ths.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jaa.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zwk.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zff.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mdv.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wjm.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://qft.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hmc.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cuu.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xzr.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayt.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://raa.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wwy.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hhm.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gvk.hfpthk.cn

[P04] 求长度
来源：http://vek.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://otk.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jnl.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cev.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dci.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://oqq.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://dyu.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://alh.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zex.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://gnd.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mnx.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sxk.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xpo.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ibm.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://spj.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://smq.nanxinkj.top

Ruby: a == b
来源：http://gts.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pqj.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pnx.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://odk.316326.xyz

PHP:  if (empty($x)) {}
来源：http://zon.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wie.cucudq.cn

TS:   if (x == null) {}
来源：http://rzb.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yim.andypj.xyz

Go:   if x == nil {}
来源：http://vpn.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ggj.c1oappe.top

C#:   if (x is null) {}
来源：http://caa.zhiwuduotai.top

[P07] 防抖与节流
来源：http://vln.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cie.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://qlc.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://psw.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcj.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dul.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iru.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxc.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ieo.birdmap.top

[P08] 处理浮点精度问题
来源：http://qks.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pkm.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ctc.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://apt.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xwq.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lyg.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://muq.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://icm.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zjr.hywenlv.cn

================================================================================
来源：http://oog.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zrq.cucudq.cn

================================================================================
来源：http://etl.hongshengwenyu.top

[Q01] 创建表
来源：http://hrg.ybcxt.top

CREATE TABLE users (
来源：http://rlf.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqg.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://eew.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://ppw.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://avi.jinqigfzy.top

);
来源：http://qqr.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://klx.gotoacloud.top

CREATE TABLE orders (
来源：http://lug.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ybu.316326.xyz

user_id INT NOT NULL,
来源：http://ila.52xcode.cn

amount DECIMAL(10, 2),
来源：http://ptv.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xko.hesvh.cn

);
来源：http://dqh.smart0.xyz

[Q03] 增加列
来源：http://yrc.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ywt.hammf.cn

[Q04] 修改列类型
来源：http://pdv.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://deb.fanxiaobao.xyz

[Q05] 重命名列
来源：http://pgv.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mtq.jianghu66.top

[Q06] 删除列
来源：http://gvj.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nfy.ydjk.org.cn

[Q07] 删除表
来源：http://hpa.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://tjc.hnxiangtu.top

[Q08] 创建普通索引
来源：http://kns.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://cdq.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://can.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wah.fehbvm.com

[Q10] 插入单行
来源：http://hlf.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dsp.cqqwz.cn

[Q11] 一次插入多行
来源：http://czf.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mwl.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://soz.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sll.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hhs.52xcode.cn

[Q13] 忽略重复插入
来源：http://zwl.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://glj.sweek.top

[Q14] 存在则更新（upsert）
来源：http://edr.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ipi.yj202588.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iju.bbcook.cn

[Q15] 查询全部
来源：http://tzg.xuanzx.com

SELECT * FROM users;
来源：http://pxb.ctjpmb.com

[Q16] 查询指定列
来源：http://lty.nanxinkj.top

SELECT id, name FROM users;
来源：http://vez.fehbvm.com

[Q17] 条件查询
来源：http://eiw.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yeh.birdmap.top

[Q18] 模糊匹配
来源：http://yss.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hba.yuxming.cn

[Q19] 范围查询
来源：http://fuh.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://igp.cucudq.cn

[Q20] IN 列表
来源：http://jkh.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cqh.ctjpmb.com

[Q21] 空值判断
来源：http://fnx.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kaj.zhaomingkeji.xyz

[Q22] 排序
来源：http://dxj.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://igi.uphjek.com

[Q23] 分页
来源：http://bky.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eef.guowangkeji.top

[Q24] 去重
来源：http://ncb.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://jam.dianchejie.cn

[Q25] 只取前 N 条
来源：http://pcu.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fso.sysykeji.top

[Q26] 计数
来源：http://osi.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://avo.hongshengwenyu.top

[Q27] 条件计数
来源：http://pnn.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ery.fehbvm.com

[Q28] 求和与平均
来源：http://yvj.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kih.zhengqikj.top

[Q29] 最大最小值
来源：http://vxz.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fqr.zhoulong.xyz

[Q30] 分组统计
来源：http://dkl.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wad.gaohongyu789.top

[Q31] 分组后过滤
来源：http://ssc.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nvv.fzhhl.top

[Q32] 分组拼接字符串
来源：http://lop.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zbc.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oqz.vqdsnc.cn

[Q33] 多列分组
来源：http://jlr.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wxc.jinqigufen.top

[Q34] 每组取第一条
来源：http://fii.fktsv.cn

SELECT * FROM (
来源：http://evp.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kyf.andypj.xyz

) t WHERE rn = 1;
来源：http://iay.yueranfly.top

[Q35] 内连接
来源：http://fbx.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ydt.tanke756.top

[Q36] 左连接
来源：http://zpz.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://orc.hammf.cn

[Q37] 右连接
来源：http://mtg.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yaa.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://cfu.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xtp.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://ngr.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcg.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aqo.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bnp.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qtv.bbcook.cn

[Q41] 多表连接
来源：http://qeh.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vro.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://ipx.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://tne.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://tkx.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://erv.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nsw.ehwqpu.com

[Q43] 标量子查询
来源：http://prc.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ejt.cqqwz.cn

[Q44] IN 子查询
来源：http://qwc.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://clg.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://fte.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aem.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://pkt.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pol.jinqigufen.top

[Q47] 与平均值比较
来源：http://ywq.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sbx.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://oky.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rtc.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://xci.dianchejie.cn

[Q49] 更新单行
来源：http://yxb.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jli.aibaodan.cn

[Q50] 批量更新
来源：http://orh.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zag.epnwcf.com

[Q51] 用子查询更新
来源：http://hus.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eip.ybcxt.top

[Q52] 删除指定行
来源：http://qxw.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://nuy.dianchejie.cn

[Q53] 按条件删除
来源：http://ivp.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://exc.jqgfzy.top

[Q54] 清空表
来源：http://plm.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://nog.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://hqw.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ynp.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://gcc.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ocs.ybcxt.top

[Q57] 行号
来源：http://cya.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqw.yuxming.cn

[Q58] 累计求和
来源：http://qls.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uhd.jiagoushi.top

[Q59] 分组内累计
来源：http://pqj.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://frb.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://vay.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oyl.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zmn.ywan-chungtsiang.top

[Q61] 移动平均
来源：http://nsg.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vdb.shuidangran.top

[Q62] 分组占比
来源：http://qll.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bsk.aizwys.cn

[Q63] 开启事务
来源：http://oxn.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://cam.shzxlz.cn

[Q64] 提交事务
来源：http://obi.epnwcf.com

COMMIT;
来源：http://sqm.daxiang520.top

[Q65] 回滚事务
来源：http://nfa.yj20258888.top

ROLLBACK;
来源：http://ebj.yongpay.top

[Q66] 行锁查询
来源：http://qae.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vce.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://prz.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yqe.hywenlv.cn

[Q68] 保存点
来源：http://tez.ehwqpu.com

SAVEPOINT sp1;
来源：http://exq.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://syf.meibo888.top

[Q69] 查看执行计划
来源：http://yah.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ggh.yongpay.top

[Q70] 更新统计信息
来源：http://yvr.sweek.top

ANALYZE TABLE users;
来源：http://hqk.bjfxy.top

[Q71] 查看建表语句
来源：http://fib.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mkf.fzhhl.top

[Q72] 查看索引
来源：http://jct.ydzc1.top

SHOW INDEX FROM users;
来源：http://bbo.chenlongwang.top

[Q73] 查看表状态
来源：http://tfo.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aqt.ydjk.org.cn

[Q74] 强制使用索引
来源：http://znd.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qsq.jyoumei.cn

[Q75] 日期格式化
来源：http://lkt.ehwqpu.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pce.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tbz.smart0.xyz

[Q76] 按天统计
来源：http://dis.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blm.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://bue.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ayi.shzxlz.cn

[Q78] 当前时间
来源：http://uoo.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kid.jiagoushi.top

[Q79] 字符串拼接
来源：http://tky.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sfy.bbcook.cn

[Q80] 字符串截取
来源：http://bkr.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bst.jyoumei.cn

[Q81] 字符串替换
来源：http://lbl.xuanzx.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sqd.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://xxe.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rom.yj20258888.top

[Q83] 大小写转换
来源：http://gde.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://peo.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://auq.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://jto.aibaodan.cn

[Q85] 数值取整
来源：http://olj.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gxo.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://fnd.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wym.ybcxt.top

[Q87] JSON 字段做条件
来源：http://oot.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tto.cucudq.cn


<!-- 参考信息 -->