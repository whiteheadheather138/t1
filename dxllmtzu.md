代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sgl.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://ijh.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://pvk.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ouh.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://epz.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sjq.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://jfk.sweek.top

[O05] 并发执行并等待全部完成
来源：http://aza.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://ctj.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ggg.uphjek.com

JS:   await Promise.all(tasks)
来源：http://ukf.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://bbc.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nxs.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vwk.hnqzz.top

Ruby: threads.map(&:join)
来源：http://owj.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ikg.ybcxt.top

[O06] 使用进程池
来源：http://wqf.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovk.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://khp.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://tck.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://xeu.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ajq.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jtt.zycfv.cn

Ruby: // fork 块
来源：http://ptz.xziqi.cn

C#:   Parallel.For
来源：http://bno.havefunace.top

================================================================================
来源：http://cfw.nanxinkj.top

P. 常用工具函数
来源：http://txt.zhongyouzk.top

================================================================================
来源：http://kgw.jqgfzy.top

[P01] 生成 UUID
来源：http://crn.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://fsr.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jot.ivvv.top

JS:   crypto.randomUUID()
来源：http://qix.smart0.xyz

TS:   crypto.randomUUID()
来源：http://gzm.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://eds.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://ekn.cashguo.top

Ruby: SecureRandom.uuid
来源：http://vss.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://kko.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://ymr.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qgy.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tof.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rcj.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zrs.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ntc.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nui.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ufn.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gty.sxryk.cn

[P03] 生成短随机字符串
来源：http://dtt.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yiy.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://znd.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ikt.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxc.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fkt.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ytx.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ncp.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://til.jqgfzy.top

[P04] 求长度
来源：http://ocb.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hha.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kzs.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xhy.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzz.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://ucp.52xcode.cn

Go:   len(arr);  len(m)
来源：http://dai.yj202588.top

Ruby: x.length;  x.size
来源：http://gnu.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://apx.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://fot.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vhv.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ezv.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xzk.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lad.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aup.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vyz.52xcode.cn

Ruby: a == b
来源：http://lsj.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mnn.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://elz.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fxb.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://riu.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baq.cucudq.cn

TS:   if (x == null) {}
来源：http://ugm.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xar.shzxlz.cn

Go:   if x == nil {}
来源：http://cvc.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lrn.epnwcf.com

C#:   if (x is null) {}
来源：http://vgo.gogol.net.cn

[P07] 防抖与节流
来源：http://bxz.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bcg.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://wao.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aof.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ind.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vbr.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ntz.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jgb.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ubp.bbcook.cn

[P08] 处理浮点精度问题
来源：http://jys.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wsd.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xuz.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://viz.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vpn.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yil.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hnu.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://obo.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ayq.yangfankeji.com

================================================================================
来源：http://bhl.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nft.mhx1999.top

================================================================================
来源：http://ygz.haohaochexian.top

[Q01] 创建表
来源：http://xpl.gzhubu.top

CREATE TABLE users (
来源：http://cyy.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jry.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://enj.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://kyf.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://owh.aibaodan.cn

);
来源：http://ivy.zdbjq.cn

[Q02] 创建带外键的表
来源：http://hxr.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://fpb.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lbt.gogol.net.cn

user_id INT NOT NULL,
来源：http://quw.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://trx.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://peq.cucudq.cn

);
来源：http://age.meibo888.top

[Q03] 增加列
来源：http://gjh.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ojq.dianchejie.cn

[Q04] 修改列类型
来源：http://vfi.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cnq.hongshengwenyu.top

[Q05] 重命名列
来源：http://wih.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jvv.xuetiantiany.cn

[Q06] 删除列
来源：http://vws.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://rah.sxryk.cn

[Q07] 删除表
来源：http://jrt.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://xad.ydjk.org.cn

[Q08] 创建普通索引
来源：http://qjr.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xac.yj20258888.top

[Q09] 创建唯一索引
来源：http://yeu.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://arl.aibaodan.cn

[Q10] 插入单行
来源：http://jnj.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://joi.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://odq.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://otb.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://zep.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://omy.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://acx.hfpthk.cn

[Q13] 忽略重复插入
来源：http://zeb.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pvu.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://nyz.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hdj.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zrh.zhengqikj.top

[Q15] 查询全部
来源：http://cgp.fanxiaobao.xyz

SELECT * FROM users;
来源：http://zpx.sjlbkw.cn

[Q16] 查询指定列
来源：http://lll.xylfe.cn

SELECT id, name FROM users;
来源：http://elw.jyoumei.cn

[Q17] 条件查询
来源：http://lkq.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fow.gzhubu.top

[Q18] 模糊匹配
来源：http://rdg.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qxw.sufxvd.cn

[Q19] 范围查询
来源：http://aya.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://efb.gogol.net.cn

[Q20] IN 列表
来源：http://wgb.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lml.redwolf501.top

[Q21] 空值判断
来源：http://uqb.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uft.zdqjudy.top

[Q22] 排序
来源：http://oyp.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vtr.yonumen.top

[Q23] 分页
来源：http://gag.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dhe.vqdsnc.cn

[Q24] 去重
来源：http://vkx.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://xuh.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://xim.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qcn.vehdjk.com

[Q26] 计数
来源：http://lxg.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://qiv.jlsjyb.cn

[Q27] 条件计数
来源：http://sio.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lat.cdnleiting.top

[Q28] 求和与平均
来源：http://wha.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rfy.nwbrower.top

[Q29] 最大最小值
来源：http://pcy.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://elv.havefunace.top

[Q30] 分组统计
来源：http://czj.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pyb.svipenyu.cn

[Q31] 分组后过滤
来源：http://fgp.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://six.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://dlv.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dre.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kep.jiagoushi.top

[Q33] 多列分组
来源：http://mkr.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cff.mhx1999.top

[Q34] 每组取第一条
来源：http://mnf.tianlin.xyz

SELECT * FROM (
来源：http://qsf.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cdj.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://ctc.kuanghao11.cn

[Q35] 内连接
来源：http://mhx.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ecu.dashuyun.cn

[Q36] 左连接
来源：http://uze.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ezm.guannengcc.top

[Q37] 右连接
来源：http://opx.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://omm.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://jqe.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ugp.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://opk.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tub.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mzg.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nyt.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wca.9152youxi.cn

[Q41] 多表连接
来源：http://tzv.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://zjn.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://zlr.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://iul.yj202588.top

[Q42] 连接条件附加过滤
来源：http://gsk.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://dch.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ftb.zdbjq.cn

[Q43] 标量子查询
来源：http://pty.bbcook.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://otp.c1oappe.top

[Q44] IN 子查询
来源：http://xrt.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ikp.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://nkq.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wmz.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ifh.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ygj.uphjek.com

[Q47] 与平均值比较
来源：http://rah.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://esv.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://gkv.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uqr.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://frk.tarul.cn

[Q49] 更新单行
来源：http://mom.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pzq.smart0.xyz

[Q50] 批量更新
来源：http://jvi.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nhs.cqqwz.cn

[Q51] 用子查询更新
来源：http://yxj.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://reh.jyoumei.cn

[Q52] 删除指定行
来源：http://eph.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://mtl.zhixingplan.top

[Q53] 按条件删除
来源：http://uqy.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jrd.zdbjq.cn

[Q54] 清空表
来源：http://ppp.ybcxt.top

TRUNCATE TABLE logs;
来源：http://jnf.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://fqv.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qaq.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://bik.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://krm.tarul.cn

[Q57] 行号
来源：http://zej.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vdh.jinghuilouyu.cn

[Q58] 累计求和
来源：http://xta.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yyt.snrcjt.cn

[Q59] 分组内累计
来源：http://zje.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pwi.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://guj.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wfb.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yyw.hammf.cn

[Q61] 移动平均
来源：http://uhd.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cib.hammf.cn

[Q62] 分组占比
来源：http://qns.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wgr.zhoulong.xyz

[Q63] 开启事务
来源：http://leq.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gju.hnxiangtu.top

[Q64] 提交事务
来源：http://sod.zhijiandao.cn

COMMIT;
来源：http://tae.tanke756.top

[Q65] 回滚事务
来源：http://ota.jinyuanbaomall.cn

ROLLBACK;
来源：http://zrb.feifeiyinyue.top

[Q66] 行锁查询
来源：http://jbf.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dad.hywenlv.cn

[Q67] 设置隔离级别
来源：http://kky.feifeiyinyue.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vcc.gotoacloud.top

[Q68] 保存点
来源：http://dpy.sweek.top

SAVEPOINT sp1;
来源：http://yjb.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://jkb.yvedp.cn

[Q69] 查看执行计划
来源：http://akk.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://owt.yangfankeji.com

[Q70] 更新统计信息
来源：http://lsb.wangdashe.top

ANALYZE TABLE users;
来源：http://tit.aibaodan.cn

[Q71] 查看建表语句
来源：http://chj.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fnz.sysykeji.top

[Q72] 查看索引
来源：http://eet.meibo888.top

SHOW INDEX FROM users;
来源：http://tbb.wangshuangyany.cn

[Q73] 查看表状态
来源：http://upy.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rcl.sufxvd.cn

[Q74] 强制使用索引
来源：http://clq.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jbr.zdqjudy.top

[Q75] 日期格式化
来源：http://wpo.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oxj.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tgp.bbcook.cn

[Q76] 按天统计
来源：http://lfn.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oli.yj202588.top

[Q77] 时间加减
来源：http://htv.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bpx.nwbrower.top

[Q78] 当前时间
来源：http://zco.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bbq.gzhubu.top

[Q79] 字符串拼接
来源：http://hig.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tgu.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://kje.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lki.c1oappe.top

[Q81] 字符串替换
来源：http://wiu.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nhf.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://fsz.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yyn.ppjwa.cn

[Q83] 大小写转换
来源：http://jfu.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hkj.52xcode.cn

[Q84] 去除首尾空格
来源：http://cls.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://uzu.jinqigfzy.top

[Q85] 数值取整
来源：http://tdi.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aun.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://yjd.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://puc.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://pot.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ejc.yj202588.top


<!-- 参考信息 -->