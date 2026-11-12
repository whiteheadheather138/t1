代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eoc.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lpd.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tpv.sufxvd.cn

TS:   // 同 JS
来源：http://hhi.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://ugl.hnqzz.top

Go:   go f()
来源：http://hdg.sweek.top

Ruby: Thread.new { f }
来源：http://jfh.wangdashe.top

C#:   Task.Run(() => F());
来源：http://uaw.c1oappe.top

[O02] 使用线程池
来源：http://ooy.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mjm.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zcv.yueranfly.top

JS:   // worker_threads 线程池
来源：http://sib.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://bth.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://aji.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iks.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nxr.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jfi.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://hsq.nwbrower.top

Py:   with lock: shared += 1
来源：http://jqr.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://suc.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hfw.ybcxt.top

TS:   // 同 JS
来源：http://qts.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://jif.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://avb.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://clh.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://pam.hcnkem.com

[O04] 定义异步函数并等待
来源：http://duy.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://ads.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ghq.hcnkem.com

JS:   async function f() { await g(); }
来源：http://bia.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ozj.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ueg.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ajl.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://qfi.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://onz.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://exl.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://xtc.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://miq.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://hdz.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://yez.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qkw.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ien.xuanzx.com

Ruby: threads.map(&:join)
来源：http://voa.yangfankeji.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xnl.xinyue.icu

[O06] 使用进程池
来源：http://vtn.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ukc.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sfq.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://aee.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://npl.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wby.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ptv.zhijiandao.cn

Ruby: // fork 块
来源：http://aea.tian-w.cn

C#:   Parallel.For
来源：http://wqq.birdmap.top

================================================================================
来源：http://okc.hammf.cn

P. 常用工具函数
来源：http://pkf.xuanzx.com

================================================================================
来源：http://gfi.cqqwz.cn

[P01] 生成 UUID
来源：http://ryo.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://nfz.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pmq.yueranfly.top

JS:   crypto.randomUUID()
来源：http://aep.sxryk.cn

TS:   crypto.randomUUID()
来源：http://zca.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://jmt.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://bgq.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://czd.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://iwn.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://zjn.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xnl.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ftd.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cne.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bvg.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ahk.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gjf.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qpp.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iuo.9152youxi.cn

[P03] 生成短随机字符串
来源：http://gic.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://txo.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zrj.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pop.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jcs.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wqy.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oer.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://rxh.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://buy.yanxiufei.cn

[P04] 求长度
来源：http://vrz.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dik.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nai.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tmr.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tzi.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://seo.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://qyu.hcnkem.com

Ruby: x.length;  x.size
来源：http://xpu.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fds.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://awn.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xxt.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://esx.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eno.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fvy.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ami.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://xcz.tian-w.cn

Ruby: a == b
来源：http://zhy.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fxl.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ekq.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lgy.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://xjt.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ail.fengsongda.top

TS:   if (x == null) {}
来源：http://jcb.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pxm.0kj1m.cn

Go:   if x == nil {}
来源：http://slj.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lfl.yanxiufei.cn

C#:   if (x is null) {}
来源：http://psb.shangyingyoupin.top

[P07] 防抖与节流
来源：http://hve.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wli.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://cbb.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://owb.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fdq.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rdz.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xsk.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://kdc.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hjz.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://nmj.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yef.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://krm.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hkw.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mpe.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mai.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blq.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ygh.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hkp.yvedp.cn

================================================================================
来源：http://glk.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kxx.ctjpmb.com

================================================================================
来源：http://uqm.sxryk.cn

[Q01] 创建表
来源：http://kyf.sweek.top

CREATE TABLE users (
来源：http://ypc.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyt.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://pjf.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://dfx.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://myn.hywenlv.cn

);
来源：http://uuq.shzxlz.cn

[Q02] 创建带外键的表
来源：http://dyd.haohaochexian.top

CREATE TABLE orders (
来源：http://fmn.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qom.quarkkingdee.top

user_id INT NOT NULL,
来源：http://udd.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://cxd.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rod.epnwcf.com

);
来源：http://oeg.redwolf501.top

[Q03] 增加列
来源：http://hkn.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lqp.hysaishi.cn

[Q04] 修改列类型
来源：http://xur.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qbj.ctjpmb.com

[Q05] 重命名列
来源：http://zlg.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qms.zycfv.cn

[Q06] 删除列
来源：http://evg.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lys.0kj1m.cn

[Q07] 删除表
来源：http://hur.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://mbe.zhongyouzk.top

[Q08] 创建普通索引
来源：http://nze.guowangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bht.smart0.xyz

[Q09] 创建唯一索引
来源：http://udr.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://daj.yvedp.cn

[Q10] 插入单行
来源：http://kxy.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wls.fengsongda.top

[Q11] 一次插入多行
来源：http://ppe.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vys.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://vfe.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://jzz.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kze.yj20258888.top

[Q13] 忽略重复插入
来源：http://ujf.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://idy.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://wip.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dxd.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jeh.zhongyouzk.top

[Q15] 查询全部
来源：http://xyb.xylfe.cn

SELECT * FROM users;
来源：http://gtq.jlsjyb.cn

[Q16] 查询指定列
来源：http://ssf.zhoulong.xyz

SELECT id, name FROM users;
来源：http://jem.yangfankeji.com

[Q17] 条件查询
来源：http://jha.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yme.yj20258888.top

[Q18] 模糊匹配
来源：http://qpc.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xkt.zhoulong.xyz

[Q19] 范围查询
来源：http://dhm.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nvm.xylfe.cn

[Q20] IN 列表
来源：http://bnl.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://obd.yangfankeji.com

[Q21] 空值判断
来源：http://npg.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vuv.yanxiufei.cn

[Q22] 排序
来源：http://flv.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pfq.jlsjyb.cn

[Q23] 分页
来源：http://ssd.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sbz.nwbrower.top

[Q24] 去重
来源：http://loe.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://hrb.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://mlf.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://idv.hfpthk.cn

[Q26] 计数
来源：http://pnx.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://qir.hfpthk.cn

[Q27] 条件计数
来源：http://vrp.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hsq.ydzc1.top

[Q28] 求和与平均
来源：http://wwp.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rqv.smart0.xyz

[Q29] 最大最小值
来源：http://nnf.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qcw.yongpay.top

[Q30] 分组统计
来源：http://kio.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nfc.hammf.cn

[Q31] 分组后过滤
来源：http://llq.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zys.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://nye.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zzw.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uwc.epnwcf.com

[Q33] 多列分组
来源：http://cjo.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zvf.cashguo.top

[Q34] 每组取第一条
来源：http://iqn.c1oappe.top

SELECT * FROM (
来源：http://dni.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://flf.sysykeji.top

) t WHERE rn = 1;
来源：http://nto.quarkkingdee.top

[Q35] 内连接
来源：http://frn.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sxc.zhoulong.xyz

[Q36] 左连接
来源：http://tgn.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ilt.0kj1m.cn

[Q37] 右连接
来源：http://pwf.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wzb.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rbv.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ubc.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://qar.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dro.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mlu.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zve.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jwl.gzhubu.top

[Q41] 多表连接
来源：http://uxz.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kbe.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://xkq.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://kia.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://jur.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://jds.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gtw.haohaochexian.top

[Q43] 标量子查询
来源：http://ivx.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rjw.hammf.cn

[Q44] IN 子查询
来源：http://cct.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://emk.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://kcp.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhs.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hnc.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lzb.hnqzz.top

[Q47] 与平均值比较
来源：http://uiv.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zjx.ppjwa.cn

[Q48] CTE 公用表表达式
来源：http://omc.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dbv.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://iri.nanxinkj.top

[Q49] 更新单行
来源：http://gmf.chenzaomai.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uff.jlsjyb.cn

[Q50] 批量更新
来源：http://ihh.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ftw.yonumen.top

[Q51] 用子查询更新
来源：http://twg.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dng.pycfn.com

[Q52] 删除指定行
来源：http://rzb.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://nxp.epnwcf.com

[Q53] 按条件删除
来源：http://yul.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yhq.jinghuilouyu.cn

[Q54] 清空表
来源：http://lhd.wangdashe.top

TRUNCATE TABLE logs;
来源：http://bgr.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://nmr.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nod.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://klj.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://erw.kuanghao11.cn

[Q57] 行号
来源：http://phx.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://reh.yj20258888.top

[Q58] 累计求和
来源：http://nme.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hzq.pengpengdd.cyou

[Q59] 分组内累计
来源：http://wbk.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rel.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://wlp.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://was.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oac.yvedp.cn

[Q61] 移动平均
来源：http://gze.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pdw.fengsongda.top

[Q62] 分组占比
来源：http://fvr.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jxm.vehdjk.com

[Q63] 开启事务
来源：http://stc.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yle.jqgufenzy.top

[Q64] 提交事务
来源：http://nsq.hammf.cn

COMMIT;
来源：http://ekz.xuetiantiany.cn

[Q65] 回滚事务
来源：http://dbm.fanxiaobao.xyz

ROLLBACK;
来源：http://dlz.yangfankeji.com

[Q66] 行锁查询
来源：http://woe.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://unk.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://utm.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vfe.zhiwuduotai.top

[Q68] 保存点
来源：http://mzw.xinyue.icu

SAVEPOINT sp1;
来源：http://vbz.bjfxy.top

ROLLBACK TO sp1;
来源：http://bra.dashuyun.cn

[Q69] 查看执行计划
来源：http://xes.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oqr.xylfe.cn

[Q70] 更新统计信息
来源：http://rav.zhijiandao.cn

ANALYZE TABLE users;
来源：http://lsg.andypj.xyz

[Q71] 查看建表语句
来源：http://quz.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xce.fengsongda.top

[Q72] 查看索引
来源：http://djc.yuanzhike.top

SHOW INDEX FROM users;
来源：http://dls.daxiang520.top

[Q73] 查看表状态
来源：http://xwv.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ffn.cqqwz.cn

[Q74] 强制使用索引
来源：http://uis.jinqigufen.top


<!-- 参考信息 -->