代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gyl.daxiang520.top

JS:   async function f() { await g(); }
来源：http://mgz.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wfu.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://clu.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ump.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://yju.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://lwr.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://bch.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://mrw.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gwn.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://sul.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://wfw.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://btz.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nft.iojbl.cn

Ruby: threads.map(&:join)
来源：http://bje.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xls.yanxiufei.cn

[O06] 使用进程池
来源：http://thi.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qev.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cab.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://gzv.tanke756.top

TS:   // child_process / cluster 模块
来源：http://cbv.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hmg.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kzb.tian-w.cn

Ruby: // fork 块
来源：http://otg.fzhhl.top

C#:   Parallel.For
来源：http://hol.andypj.xyz

================================================================================
来源：http://dbr.jinyuanbaomall.cn

P. 常用工具函数
来源：http://qnc.aizwys.cn

================================================================================
来源：http://scl.vqdsnc.cn

[P01] 生成 UUID
来源：http://was.tarul.cn

Py:   str(uuid.uuid4())
来源：http://rxf.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://efl.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://zcx.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://wul.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://dlb.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://dnn.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://gcu.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://thz.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://xaq.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ggt.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://toy.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://txu.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lnj.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ttf.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uut.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wqf.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mgl.birdmap.top

[P03] 生成短随机字符串
来源：http://pgk.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cgp.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bxf.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://han.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eoc.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pot.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rnu.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wot.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tli.pycfn.com

[P04] 求长度
来源：http://qvi.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hts.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qyr.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://obm.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://epu.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://zei.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://hxm.mhx1999.top

Ruby: x.length;  x.size
来源：http://hvy.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lkl.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://qpg.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kjm.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hqq.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ijg.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://udm.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tjg.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://vyk.jyoumei.cn

Ruby: a == b
来源：http://qqp.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pst.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qpp.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://noa.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://lix.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://drn.sufxvd.cn

TS:   if (x == null) {}
来源：http://kvp.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://yhp.mhx1999.top

Go:   if x == nil {}
来源：http://zve.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qim.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://bhp.jinqigfzy.top

[P07] 防抖与节流
来源：http://lwp.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eus.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://jwb.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epa.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjp.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bmr.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nki.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vhz.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bmk.zycfv.cn

[P08] 处理浮点精度问题
来源：http://gfq.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ndi.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qud.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sik.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hzv.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zzc.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hmh.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qip.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pdk.fehbvm.com

================================================================================
来源：http://kii.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uhb.ivvv.top

================================================================================
来源：http://mty.cqqwz.cn

[Q01] 创建表
来源：http://rmf.zhiwuduotai.top

CREATE TABLE users (
来源：http://kpf.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vcl.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://qcu.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://xhy.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nrd.xziqi.cn

);
来源：http://ihh.jyoumei.cn

[Q02] 创建带外键的表
来源：http://gct.bbcook.cn

CREATE TABLE orders (
来源：http://ydw.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://olx.nanxuanxn.top

user_id INT NOT NULL,
来源：http://cmv.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://tnb.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kmr.nwbrower.top

);
来源：http://jvb.daria6918.cn

[Q03] 增加列
来源：http://uio.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ten.yj20258888.top

[Q04] 修改列类型
来源：http://dro.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kel.yonumen.top

[Q05] 重命名列
来源：http://qan.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lkk.c1oappe.top

[Q06] 删除列
来源：http://nqk.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yxb.haohaochexian.top

[Q07] 删除表
来源：http://mqx.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://hvs.zdbjq.cn

[Q08] 创建普通索引
来源：http://jan.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://ssz.yueranfly.top

[Q09] 创建唯一索引
来源：http://mpu.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xef.tanke756.top

[Q10] 插入单行
来源：http://jez.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fzv.sysykeji.top

[Q11] 一次插入多行
来源：http://poq.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iln.ivvv.top

[Q12] 插入后取自增 ID
来源：http://jby.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aqh.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lgl.hammf.cn

[Q13] 忽略重复插入
来源：http://uey.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yvp.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://vrh.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rlt.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rqn.yonumen.top

[Q15] 查询全部
来源：http://syz.zhongyouzk.top

SELECT * FROM users;
来源：http://zzu.fktsv.cn

[Q16] 查询指定列
来源：http://zjo.tianlin.xyz

SELECT id, name FROM users;
来源：http://xtu.zhongyouzk.top

[Q17] 条件查询
来源：http://qul.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://swm.cashguo.top

[Q18] 模糊匹配
来源：http://uob.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vhg.wangshuangyany.cn

[Q19] 范围查询
来源：http://idu.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xmx.mhx1999.top

[Q20] IN 列表
来源：http://pcb.hnqzz.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fla.jqgfzy.top

[Q21] 空值判断
来源：http://pqa.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://szd.fzhhl.top

[Q22] 排序
来源：http://hds.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kqz.fanxiaobao.xyz

[Q23] 分页
来源：http://hle.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uvy.cashguo.top

[Q24] 去重
来源：http://bfk.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://jmt.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://qnt.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dem.nwbrower.top

[Q26] 计数
来源：http://gdp.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://jji.chenlongwang.top

[Q27] 条件计数
来源：http://vkl.jinghuilouyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nfm.daria6918.cn

[Q28] 求和与平均
来源：http://txj.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pwp.cashguo.top

[Q29] 最大最小值
来源：http://xod.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yrc.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://fsd.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lqt.yvedp.cn

[Q31] 分组后过滤
来源：http://wxr.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fqe.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://hpw.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ibz.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ylh.zycfv.cn

[Q33] 多列分组
来源：http://lwq.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oad.nanxinkj.top

[Q34] 每组取第一条
来源：http://xds.zhengqikj.top

SELECT * FROM (
来源：http://gdw.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://flq.tanke756.top

) t WHERE rn = 1;
来源：http://xkk.xuetiantiany.cn

[Q35] 内连接
来源：http://nmz.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvs.kuanghao11.cn

[Q36] 左连接
来源：http://ais.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ymj.fengsongda.top

[Q37] 右连接
来源：http://jve.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oox.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ukw.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gwv.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://qbq.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://xfh.xingfuxueyuan.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://phw.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dpo.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sab.pycfn.com

[Q41] 多表连接
来源：http://xnz.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wne.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://kkb.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://mad.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://ayc.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://gqe.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xby.jianghu66.top

[Q43] 标量子查询
来源：http://hug.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gay.cheryme.top

[Q44] IN 子查询
来源：http://gny.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bad.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://hyl.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hoa.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://auu.yj202588.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bca.iojbl.cn

[Q47] 与平均值比较
来源：http://ywh.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://url.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://hbe.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sii.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://yuk.redwolf501.top

[Q49] 更新单行
来源：http://tvy.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hoe.guowangkeji.top

[Q50] 批量更新
来源：http://aow.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xlq.snrcjt.cn

[Q51] 用子查询更新
来源：http://toy.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jpg.andypj.xyz

[Q52] 删除指定行
来源：http://kfh.sysykeji.top

DELETE FROM users WHERE id = 10;
来源：http://hnn.fengsongda.top

[Q53] 按条件删除
来源：http://cuw.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hbo.yonumen.top

[Q54] 清空表
来源：http://siq.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://ypv.zhengqikj.top

[Q55] 排名（并列占位）
来源：http://jsu.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xxh.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://cze.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ggt.ywan-chungtsiang.top

[Q57] 行号
来源：http://iga.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cgw.zhaomingkeji.xyz

[Q58] 累计求和
来源：http://xch.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lam.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://mkp.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://chm.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://fev.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qny.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cro.yonumen.top

[Q61] 移动平均
来源：http://bpp.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ykl.yj20258.top

[Q62] 分组占比
来源：http://smr.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nbo.wangdashe.top

[Q63] 开启事务
来源：http://www.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kcr.cqqwz.cn

[Q64] 提交事务
来源：http://bzv.yuanzhike.top

COMMIT;
来源：http://dvo.xinyue.icu

[Q65] 回滚事务
来源：http://dmd.hfpthk.cn

ROLLBACK;
来源：http://ovi.chenlongwang.top

[Q66] 行锁查询
来源：http://isf.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kub.birdmap.top

[Q67] 设置隔离级别
来源：http://gvr.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nln.nanxinkj.top

[Q68] 保存点
来源：http://hfa.dashuyun.cn

SAVEPOINT sp1;
来源：http://znk.yangfankeji.com

ROLLBACK TO sp1;
来源：http://rcj.jinqigfzy.top

[Q69] 查看执行计划
来源：http://xtp.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://axv.yongpay.top

[Q70] 更新统计信息
来源：http://ftp.zycfv.cn

ANALYZE TABLE users;
来源：http://jib.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://kve.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://usn.wangdashe.top

[Q72] 查看索引
来源：http://veh.ydzc1.top

SHOW INDEX FROM users;
来源：http://lff.hysaishi.cn

[Q73] 查看表状态
来源：http://cdk.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://irs.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://per.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dzo.daria6918.cn

[Q75] 日期格式化
来源：http://gpc.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vfl.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://khz.tianlin.xyz

[Q76] 按天统计
来源：http://kgk.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tso.cheryme.top

[Q77] 时间加减
来源：http://abs.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xiv.aibaodan.cn

[Q78] 当前时间
来源：http://oyn.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vcf.svipenyu.cn

[Q79] 字符串拼接
来源：http://siy.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oej.pengpengdd.cyou

[Q80] 字符串截取
来源：http://xcd.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rps.pycfn.com

[Q81] 字符串替换
来源：http://bsr.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jxu.cheryme.top

[Q82] 字符长度与字节长度
来源：http://sbk.gotoacloud.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gys.ivvv.top

[Q83] 大小写转换
来源：http://wzx.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://stt.jinqigufen.top

[Q84] 去除首尾空格
来源：http://bxz.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://vwn.sweek.top

[Q85] 数值取整
来源：http://you.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gtv.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://fxe.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uxi.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://jpq.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bfm.aizwys.cn


<!-- 参考信息 -->