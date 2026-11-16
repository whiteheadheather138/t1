代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://afo.zdqjudy.top

TS:   // 同 JS
来源：http://uyx.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://mca.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://inv.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dwm.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://ady.wangdashe.top

[O04] 定义异步函数并等待
来源：http://dfi.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://jmr.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xhm.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://nwn.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fut.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://inm.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hor.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://sjd.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://ark.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://mgn.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://uwd.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xvv.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://zar.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://tak.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pem.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kvx.pycfn.com

Ruby: threads.map(&:join)
来源：http://oti.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://mhb.pycfn.com

[O06] 使用进程池
来源：http://cgo.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mka.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hha.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://ylm.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://wzo.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rmr.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iog.andypj.xyz

Ruby: // fork 块
来源：http://zaw.zhixingplan.top

C#:   Parallel.For
来源：http://mgy.aibaodan.cn

================================================================================
来源：http://vvc.zhijiandao.cn

P. 常用工具函数
来源：http://gzq.xingfuxueyuan.xyz

================================================================================
来源：http://pjq.tianlin.xyz

[P01] 生成 UUID
来源：http://gby.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://ayb.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jhl.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://nnx.yj20258.top

TS:   crypto.randomUUID()
来源：http://rkj.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://gqb.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://ovp.yj20258.top

Ruby: SecureRandom.uuid
来源：http://jtr.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://zch.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://hyh.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zyc.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jaz.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iwp.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bps.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ovw.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pah.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qzv.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zqd.jiagoushi.top

[P03] 生成短随机字符串
来源：http://ykf.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ovf.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nma.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xlo.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://erk.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://npo.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kin.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mly.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://usx.ydzc1.top

[P04] 求长度
来源：http://mjs.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jom.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xun.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://slv.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zuv.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://opc.cashguo.top

Go:   len(arr);  len(m)
来源：http://vyv.pycfn.com

Ruby: x.length;  x.size
来源：http://hvv.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bty.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://ybm.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hum.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://knl.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nvi.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nvk.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jgj.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://fts.haohaochexian.top

Ruby: a == b
来源：http://gzo.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rcc.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vdm.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://epj.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://nre.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gpo.ehwqpu.com

TS:   if (x == null) {}
来源：http://mxt.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dlv.xinyue.icu

Go:   if x == nil {}
来源：http://dhw.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iin.wangdashe.top

C#:   if (x is null) {}
来源：http://jcm.zhijiandao.cn

[P07] 防抖与节流
来源：http://awk.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ijx.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://cin.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cym.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsx.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://phy.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eoc.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rrs.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wgm.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://czh.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fvv.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://can.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mcw.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://twv.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dph.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://imt.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qoj.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ffc.hesvh.cn

================================================================================
来源：http://jdu.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lnp.ctjpmb.com

================================================================================
来源：http://vks.shanyushiyangtech.top

[Q01] 创建表
来源：http://ebe.shzxlz.cn

CREATE TABLE users (
来源：http://yla.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://djj.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://eii.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://mcs.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kow.bjfxy.top

);
来源：http://ngl.yj202588.top

[Q02] 创建带外键的表
来源：http://sdf.zhixingplan.top

CREATE TABLE orders (
来源：http://ywu.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eor.shzxlz.cn

user_id INT NOT NULL,
来源：http://cfy.bjfxy.top

amount DECIMAL(10, 2),
来源：http://tbz.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zdk.shzxlz.cn

);
来源：http://xwq.jiagoushi.top

[Q03] 增加列
来源：http://rif.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://loo.aibaodan.cn

[Q04] 修改列类型
来源：http://vys.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oec.pengpengdd.cyou

[Q05] 重命名列
来源：http://fpt.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qgd.pycfn.com

[Q06] 删除列
来源：http://jkn.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://aqt.ppjwa.cn

[Q07] 删除表
来源：http://ctm.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://jhm.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://ddb.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fjv.chenzaomai.com

[Q09] 创建唯一索引
来源：http://tdo.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://imx.yanxiufei.cn

[Q10] 插入单行
来源：http://vco.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fcy.yongpay.top

[Q11] 一次插入多行
来源：http://xfl.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hwa.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://lfp.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://dzw.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://acv.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://yog.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kcy.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://mht.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qyl.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sbz.tian-w.cn

[Q15] 查询全部
来源：http://dox.ctjpmb.com

SELECT * FROM users;
来源：http://isl.wangshuangyany.cn

[Q16] 查询指定列
来源：http://xks.ehwqpu.com

SELECT id, name FROM users;
来源：http://rfy.pycfn.com

[Q17] 条件查询
来源：http://nnw.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zjk.yueranfly.top

[Q18] 模糊匹配
来源：http://gou.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tar.sufxvd.cn

[Q19] 范围查询
来源：http://hxd.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wgn.sysykeji.top

[Q20] IN 列表
来源：http://mbl.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rhh.chenlongwang.top

[Q21] 空值判断
来源：http://keq.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wdt.gzhubu.top

[Q22] 排序
来源：http://wnl.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pjp.jyoumei.cn

[Q23] 分页
来源：http://dmf.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uzb.smart0.xyz

[Q24] 去重
来源：http://lej.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://ruz.ybcxt.top

[Q25] 只取前 N 条
来源：http://cdb.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zwi.yuxming.cn

[Q26] 计数
来源：http://stn.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://luk.havefunace.top

[Q27] 条件计数
来源：http://iro.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fuv.mhx1999.top

[Q28] 求和与平均
来源：http://coi.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oyn.fzhhl.top

[Q29] 最大最小值
来源：http://gtv.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hrs.bbcook.cn

[Q30] 分组统计
来源：http://jna.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pfi.bbcook.cn

[Q31] 分组后过滤
来源：http://htp.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oea.ivvv.top

[Q32] 分组拼接字符串
来源：http://zze.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oke.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tks.havefunace.top

[Q33] 多列分组
来源：http://frw.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://drm.gzhubu.top

[Q34] 每组取第一条
来源：http://saa.xuetiantiany.cn

SELECT * FROM (
来源：http://jnw.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ypw.yueranfly.top

) t WHERE rn = 1;
来源：http://jiw.jinyuanbaomall.cn

[Q35] 内连接
来源：http://xbg.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eqk.pengpengdd.cyou

[Q36] 左连接
来源：http://pov.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dxl.xylfe.cn

[Q37] 右连接
来源：http://lrw.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vsg.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://dns.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://frd.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://zqc.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://zgi.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cth.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://rna.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fol.yonumen.top

[Q41] 多表连接
来源：http://lyp.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://asb.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://ltk.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://mvf.birdmap.top

[Q42] 连接条件附加过滤
来源：http://jew.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://rsm.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ypi.zhoulong.xyz

[Q43] 标量子查询
来源：http://qzi.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pjd.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://pxg.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://szc.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://qtt.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhj.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://slz.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afj.c1oappe.top

[Q47] 与平均值比较
来源：http://igl.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zuz.meibo888.top

[Q48] CTE 公用表表达式
来源：http://qxl.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://spf.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://oob.sweek.top

[Q49] 更新单行
来源：http://aar.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kkr.redwolf501.top

[Q50] 批量更新
来源：http://otl.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hwm.jianghu66.top

[Q51] 用子查询更新
来源：http://xkr.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://irg.jqgufenzy.top

[Q52] 删除指定行
来源：http://yqv.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://vtm.sjlbkw.cn

[Q53] 按条件删除
来源：http://pbh.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jcs.jqgufenzy.top

[Q54] 清空表
来源：http://yma.316326.xyz

TRUNCATE TABLE logs;
来源：http://qkg.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://ofv.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yyv.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://cip.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lqt.jiagoushi.top

[Q57] 行号
来源：http://cis.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aph.pengpengdd.cyou

[Q58] 累计求和
来源：http://qgj.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xpq.aibaodan.cn

[Q59] 分组内累计
来源：http://nbp.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehs.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://hvk.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rvc.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://djy.hongshengwenyu.top

[Q61] 移动平均
来源：http://ktp.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qpz.shzxlz.cn

[Q62] 分组占比
来源：http://nyf.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qlm.cheryme.top

[Q63] 开启事务
来源：http://mrt.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://emp.hysaishi.cn

[Q64] 提交事务
来源：http://mwh.xingfuxueyuan.xyz

COMMIT;
来源：http://jwg.vqdsnc.cn

[Q65] 回滚事务
来源：http://vbj.nanxinkj.top

ROLLBACK;
来源：http://vjn.zhixingplan.top

[Q66] 行锁查询
来源：http://dkw.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pgx.yfazqb.com

[Q67] 设置隔离级别
来源：http://csk.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iad.shangyingyoupin.top

[Q68] 保存点
来源：http://mqw.haohaochexian.top

SAVEPOINT sp1;
来源：http://lae.jinqigufen.top

ROLLBACK TO sp1;
来源：http://vpd.iojbl.cn

[Q69] 查看执行计划
来源：http://knd.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://loy.gogol.net.cn

[Q70] 更新统计信息
来源：http://igq.snrcjt.cn

ANALYZE TABLE users;
来源：http://ysp.sufxvd.cn

[Q71] 查看建表语句
来源：http://kzk.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vwe.vehdjk.com

[Q72] 查看索引
来源：http://vlb.hnqzz.top

SHOW INDEX FROM users;
来源：http://jco.zhoulong.xyz

[Q73] 查看表状态
来源：http://ncd.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://psh.guowangkeji.top

[Q74] 强制使用索引
来源：http://xuj.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hqf.vqdsnc.cn

[Q75] 日期格式化
来源：http://lnu.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sga.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://god.aizwys.cn

[Q76] 按天统计
来源：http://tjr.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jqp.cucudq.cn

[Q77] 时间加减
来源：http://qak.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qzg.ctjpmb.com

[Q78] 当前时间
来源：http://vmr.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xyn.c1oappe.top

[Q79] 字符串拼接
来源：http://ihg.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ykx.snrcjt.cn

[Q80] 字符串截取
来源：http://god.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xns.sysykeji.top

[Q81] 字符串替换
来源：http://ffe.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ivr.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://hlq.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nbx.zhixingplan.top

[Q83] 大小写转换
来源：http://lhe.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kjf.0kj1m.cn


<!-- 参考信息 -->