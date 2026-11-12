代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vrz.hammf.cn

JS:   async function f() { await g(); }
来源：http://adi.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://knz.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lxc.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mlp.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://qwa.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://vpw.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://gdw.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://bak.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ald.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://kxe.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://qnf.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ult.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oce.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://xna.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zhb.yj20258888.top

[O06] 使用进程池
来源：http://ack.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://irm.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qww.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://sjr.sweek.top

TS:   // child_process / cluster 模块
来源：http://xpo.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mfw.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://afu.vehdjk.com

Ruby: // fork 块
来源：http://uwq.yanxiufei.cn

C#:   Parallel.For
来源：http://gqx.cqqwz.cn

================================================================================
来源：http://kyc.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://flm.jqgfzy.top

================================================================================
来源：http://upp.snrcjt.cn

[P01] 生成 UUID
来源：http://loe.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://jqb.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nxc.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://cho.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://rhz.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://sjy.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://bzl.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://rqq.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://jhf.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://hfz.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eha.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://idm.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nub.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nja.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nmw.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lxj.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bss.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zne.redwolf501.top

[P03] 生成短随机字符串
来源：http://bvo.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tsp.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ypv.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zds.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayh.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cod.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sxb.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wuo.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dnv.tian-w.cn

[P04] 求长度
来源：http://hmv.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lso.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uxq.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqi.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hed.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://ngq.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://ana.cqqwz.cn

Ruby: x.length;  x.size
来源：http://ddk.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eln.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://dnv.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wad.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tgt.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bqq.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lye.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://acu.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://ntk.chenjidiqi.icu

Ruby: a == b
来源：http://zvs.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tkt.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nwd.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gjq.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://tyf.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jmm.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://wzf.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://fao.zhijiandao.cn

Go:   if x == nil {}
来源：http://lhp.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://edi.birdmap.top

C#:   if (x is null) {}
来源：http://kad.zhiwuduotai.top

[P07] 防抖与节流
来源：http://veh.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mll.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://rou.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ljk.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uau.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nwl.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vra.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gus.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ahb.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://pkr.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lhk.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oye.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kxq.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xay.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lge.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pqo.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tye.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hzd.nwbrower.top

================================================================================
来源：http://kum.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xgz.yonumen.top

================================================================================
来源：http://gua.tianlin.xyz

[Q01] 创建表
来源：http://iyj.gotoacloud.top

CREATE TABLE users (
来源：http://jgy.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zti.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://uih.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://xeo.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ydr.hysaishi.cn

);
来源：http://dyl.mhx1999.top

[Q02] 创建带外键的表
来源：http://wmg.guowangkeji.top

CREATE TABLE orders (
来源：http://nvw.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fir.cdnleiting.top

user_id INT NOT NULL,
来源：http://cbe.fehbvm.com

amount DECIMAL(10, 2),
来源：http://fyp.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fxh.52xcode.cn

);
来源：http://dwj.shuidangran.top

[Q03] 增加列
来源：http://rhx.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kyw.nwbrower.top

[Q04] 修改列类型
来源：http://dcw.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rlz.wangshuangyany.cn

[Q05] 重命名列
来源：http://geo.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oox.haohaochexian.top

[Q06] 删除列
来源：http://kiy.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://vhg.daria6918.cn

[Q07] 删除表
来源：http://kyq.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://itl.gogol.net.cn

[Q08] 创建普通索引
来源：http://lkw.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wol.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://zqv.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://syx.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://xge.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kod.daria6918.cn

[Q11] 一次插入多行
来源：http://dtw.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ngq.hammf.cn

[Q12] 插入后取自增 ID
来源：http://teq.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://izz.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tno.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://zgl.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uhz.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://icy.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ljc.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ssx.yuanzhike.top

[Q15] 查询全部
来源：http://pkk.pycfn.com

SELECT * FROM users;
来源：http://hfs.snrcjt.cn

[Q16] 查询指定列
来源：http://snb.xylfe.cn

SELECT id, name FROM users;
来源：http://wqa.hammf.cn

[Q17] 条件查询
来源：http://vfu.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ivj.zhongyouzk.top

[Q18] 模糊匹配
来源：http://uxg.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xjk.sysykeji.top

[Q19] 范围查询
来源：http://sdz.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aeo.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://jel.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aqe.ybcxt.top

[Q21] 空值判断
来源：http://wof.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zco.hcnkem.com

[Q22] 排序
来源：http://igy.fengsongda.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tms.cqqwz.cn

[Q23] 分页
来源：http://qku.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qjw.xuanzx.com

[Q24] 去重
来源：http://byp.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://ooe.hfpthk.cn

[Q25] 只取前 N 条
来源：http://lpl.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wie.zhoulong.xyz

[Q26] 计数
来源：http://jqq.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://lxi.jiagoushi.top

[Q27] 条件计数
来源：http://gqh.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://inu.sysykeji.top

[Q28] 求和与平均
来源：http://ebx.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hir.yj202588.top

[Q29] 最大最小值
来源：http://amy.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://mhf.dianchejie.cn

[Q30] 分组统计
来源：http://vlj.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lva.epnwcf.com

[Q31] 分组后过滤
来源：http://zvs.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kux.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://tam.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jyt.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wvq.nanxuanxn.top

[Q33] 多列分组
来源：http://ifm.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sru.shzxlz.cn

[Q34] 每组取第一条
来源：http://vrq.ydjk.org.cn

SELECT * FROM (
来源：http://vek.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iwj.vqdsnc.cn

) t WHERE rn = 1;
来源：http://hmo.mhx1999.top

[Q35] 内连接
来源：http://nok.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://njx.pycfn.com

[Q36] 左连接
来源：http://qfg.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://egn.meibo888.top

[Q37] 右连接
来源：http://sou.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://scw.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://rpz.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qhp.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://amn.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wmh.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sli.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://jjq.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iok.yj202588.top

[Q41] 多表连接
来源：http://rhg.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://una.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://ytr.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://tor.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://ckr.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://rfh.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://reg.guannengcc.top

[Q43] 标量子查询
来源：http://tnv.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iks.pengpengdd.cyou

[Q44] IN 子查询
来源：http://mei.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ysx.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://xnp.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ykj.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://ggh.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lvy.fktsv.cn

[Q47] 与平均值比较
来源：http://rip.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qrt.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://ahh.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ayk.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://sdx.tanke756.top

[Q49] 更新单行
来源：http://ovb.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bdm.xinyue.icu

[Q50] 批量更新
来源：http://zgt.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wdb.fzhhl.top

[Q51] 用子查询更新
来源：http://cjf.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rne.zhongyouzk.top

[Q52] 删除指定行
来源：http://rwu.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://bbd.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://qag.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fxl.yj20258888.top

[Q54] 清空表
来源：http://wql.nwbrower.top

TRUNCATE TABLE logs;
来源：http://mtn.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://uhm.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kin.smart0.xyz

[Q56] 密集排名（并列不占位）
来源：http://fzi.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jyg.ppjwa.cn

[Q57] 行号
来源：http://rjk.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mas.feifeiyinyue.top

[Q58] 累计求和
来源：http://xot.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hma.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://auu.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gsz.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://gpl.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lcs.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dih.guowangkeji.top

[Q61] 移动平均
来源：http://cok.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pti.yj20258.top

[Q62] 分组占比
来源：http://xay.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rbr.hcnkem.com

[Q63] 开启事务
来源：http://ibp.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jyq.hywenlv.cn

[Q64] 提交事务
来源：http://rek.feifeiyinyue.top

COMMIT;
来源：http://xzn.hfpthk.cn

[Q65] 回滚事务
来源：http://zuf.uphjek.com

ROLLBACK;
来源：http://ttx.cashguo.top

[Q66] 行锁查询
来源：http://jry.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://civ.bjfxy.top

[Q67] 设置隔离级别
来源：http://dvq.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://muk.yueranfly.top

[Q68] 保存点
来源：http://uox.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://igt.yuxming.cn

ROLLBACK TO sp1;
来源：http://vrl.vehdjk.com

[Q69] 查看执行计划
来源：http://dyq.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hoz.svipenyu.cn

[Q70] 更新统计信息
来源：http://qvg.cqqwz.cn

ANALYZE TABLE users;
来源：http://pkg.aibaodan.cn

[Q71] 查看建表语句
来源：http://ljc.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lta.jinghuilouyu.cn

[Q72] 查看索引
来源：http://xih.c1oappe.top

SHOW INDEX FROM users;
来源：http://mbx.vqdsnc.cn

[Q73] 查看表状态
来源：http://aen.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://byc.bjfxy.top

[Q74] 强制使用索引
来源：http://vvv.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tto.ydzc1.top

[Q75] 日期格式化
来源：http://hfw.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bmh.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wwv.tian-w.cn

[Q76] 按天统计
来源：http://qhh.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nsa.ctjpmb.com

[Q77] 时间加减
来源：http://vth.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppz.zdqjudy.top

[Q78] 当前时间
来源：http://cjb.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hhu.quarkkingdee.top

[Q79] 字符串拼接
来源：http://akz.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vus.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://npu.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nkb.sweek.top

[Q81] 字符串替换
来源：http://cdx.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vkx.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://ynu.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://azo.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://obr.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xbp.zhijiandao.cn

[Q84] 去除首尾空格
来源：http://ybv.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://aqm.aizwys.cn

[Q85] 数值取整
来源：http://yav.cdnleiting.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dvo.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://rcz.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fgj.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://pff.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ovz.mhx1999.top


<!-- 参考信息 -->