代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fyn.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ubo.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vlk.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dem.wangdashe.top

================================================================================
来源：http://vzy.jiagoushi.top

O. 并发与异步
来源：http://wgt.9152youxi.cn

================================================================================
来源：http://xae.nanxinkj.top

[O01] 启动一个线程
来源：http://yoq.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fbp.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qof.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cia.jqgufenzy.top

TS:   // 同 JS
来源：http://uzo.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://myd.iojbl.cn

Go:   go f()
来源：http://wxz.hysaishi.cn

Ruby: Thread.new { f }
来源：http://iav.shuidangran.top

C#:   Task.Run(() => F());
来源：http://dqs.zhoulong.xyz

[O02] 使用线程池
来源：http://wxc.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xou.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jnn.tarul.cn

JS:   // worker_threads 线程池
来源：http://gip.52xcode.cn

TS:   // worker_threads 线程池
来源：http://vxb.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://qhp.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vcp.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://olp.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jbe.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://hmh.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://zyo.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://afr.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zwl.jinqigfzy.top

TS:   // 同 JS
来源：http://hpj.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://zax.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xwd.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xqf.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://sqm.tian-w.cn

[O04] 定义异步函数并等待
来源：http://vpx.meibo888.top

Py:   async def f():⏎    await g()
来源：http://voz.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ogi.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://raz.gaohongyu789.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wut.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://taw.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzd.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://set.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://swh.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://hvs.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://tsq.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://poi.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://pdf.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://lye.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dlg.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dba.epnwcf.com

Ruby: threads.map(&:join)
来源：http://whj.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tlh.bbcook.cn

[O06] 使用进程池
来源：http://pxg.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vhx.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://knk.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://nud.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://dzr.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ocg.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nho.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://vjq.yanxiufei.cn

C#:   Parallel.For
来源：http://lzf.nanxuanxn.top

================================================================================
来源：http://myu.shuidangran.top

P. 常用工具函数
来源：http://fhl.hnxiangtu.top

================================================================================
来源：http://rvp.zhijiandao.cn

[P01] 生成 UUID
来源：http://qsv.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://sjh.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fco.mhx1999.top

JS:   crypto.randomUUID()
来源：http://bjo.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://fll.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://uxm.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://zci.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://wyv.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://meu.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://brc.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://reb.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uto.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qfd.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jwt.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zhc.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mrx.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://epu.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://opd.zycfv.cn

[P03] 生成短随机字符串
来源：http://zfd.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yqb.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cii.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://civ.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jmq.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lzs.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nni.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://roo.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ojt.iojbl.cn

[P04] 求长度
来源：http://zxn.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qhz.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwd.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahy.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hwj.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://qnm.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://gws.xziqi.cn

Ruby: x.length;  x.size
来源：http://lnv.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gaz.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://yuf.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fwh.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uvc.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://urb.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rmm.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jui.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kzw.jinqigufen.top

Ruby: a == b
来源：http://iyn.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://knk.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vvd.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nvx.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://ryz.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hvh.hcnkem.com

TS:   if (x == null) {}
来源：http://fcy.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://evf.smart0.xyz

Go:   if x == nil {}
来源：http://wkd.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yoo.birdmap.top

C#:   if (x is null) {}
来源：http://fdg.cheryme.top

[P07] 防抖与节流
来源：http://ebv.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yws.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://veh.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxo.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezz.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ukb.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ixi.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ivq.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nmr.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://qlq.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tvj.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fma.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qyj.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wfo.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ksk.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ycr.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cyv.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tfn.wangshuangyany.cn

================================================================================
来源：http://dqn.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cup.pycfn.com

================================================================================
来源：http://qxr.ppjwa.cn

[Q01] 创建表
来源：http://qca.cheryme.top

CREATE TABLE users (
来源：http://rux.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aaw.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://zct.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://jsb.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vfz.yvedp.cn

);
来源：http://esk.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://owl.xuanzx.com

CREATE TABLE orders (
来源：http://bco.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sop.meibo888.top

user_id INT NOT NULL,
来源：http://rcb.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://mly.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gjz.tarul.cn

);
来源：http://wfu.fzhhl.top

[Q03] 增加列
来源：http://glx.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rdo.jianghu66.top

[Q04] 修改列类型
来源：http://kjb.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cvl.andypj.xyz

[Q05] 重命名列
来源：http://nkk.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yhn.zhoulong.xyz

[Q06] 删除列
来源：http://vlk.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://inz.tianlin.xyz

[Q07] 删除表
来源：http://yno.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://hxy.cdnleiting.top

[Q08] 创建普通索引
来源：http://scu.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mqp.jyoumei.cn

[Q09] 创建唯一索引
来源：http://pgz.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://agd.yj202588.top

[Q10] 插入单行
来源：http://kra.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zpq.kuanghao11.cn

[Q11] 一次插入多行
来源：http://kwx.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eoz.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://sfj.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://byi.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ukl.ctjpmb.com

[Q13] 忽略重复插入
来源：http://oql.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wep.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://ths.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ngy.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmt.chenlongwang.top

[Q15] 查询全部
来源：http://okh.fehbvm.com

SELECT * FROM users;
来源：http://wyf.sufxvd.cn

[Q16] 查询指定列
来源：http://vwl.sweek.top

SELECT id, name FROM users;
来源：http://xgu.shzxlz.cn

[Q17] 条件查询
来源：http://oks.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://osy.birdmap.top

[Q18] 模糊匹配
来源：http://yxz.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kbs.shangyingyoupin.top

[Q19] 范围查询
来源：http://yup.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hgp.gzhubu.top

[Q20] IN 列表
来源：http://uoe.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uti.c1oappe.top

[Q21] 空值判断
来源：http://tyr.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://evq.jinqigfzy.top

[Q22] 排序
来源：http://lzt.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fsm.hfpthk.cn

[Q23] 分页
来源：http://igw.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://phr.nwbrower.top

[Q24] 去重
来源：http://obh.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://kpk.fzhhl.top

[Q25] 只取前 N 条
来源：http://nbn.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dcv.redwolf501.top

[Q26] 计数
来源：http://xfp.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://dsd.zhengqikj.top

[Q27] 条件计数
来源：http://tgc.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vor.vqdsnc.cn

[Q28] 求和与平均
来源：http://mgo.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mjl.yuanzhike.top

[Q29] 最大最小值
来源：http://ice.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aqu.havefunace.top

[Q30] 分组统计
来源：http://jcf.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vhv.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://xlm.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jpx.xuanzx.com

[Q32] 分组拼接字符串
来源：http://oxz.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bfs.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rbm.pycfn.com

[Q33] 多列分组
来源：http://rgv.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dgl.chenzaomai.com

[Q34] 每组取第一条
来源：http://psb.yj202588.top

SELECT * FROM (
来源：http://ciz.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zqp.snrcjt.cn

) t WHERE rn = 1;
来源：http://lqs.shanyushiyangkeji.top

[Q35] 内连接
来源：http://xay.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xbr.hnqzz.top

[Q36] 左连接
来源：http://mlm.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fsh.shuidangran.top

[Q37] 右连接
来源：http://mvn.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vip.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://jdy.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pqs.316326.xyz

[Q39] 自连接（查上下级）
来源：http://ars.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jir.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ejm.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://pzo.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bzu.9152youxi.cn

[Q41] 多表连接
来源：http://mdd.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://znt.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://bcl.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://ddu.zhijiandao.cn

[Q42] 连接条件附加过滤
来源：http://waj.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://unj.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dpe.vehdjk.com

[Q43] 标量子查询
来源：http://wbu.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://swo.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://lbw.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qvz.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://two.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zop.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yxg.nanxinkj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cta.jqgufenzy.top

[Q47] 与平均值比较
来源：http://bim.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hjr.ivvv.top

[Q48] CTE 公用表表达式
来源：http://vxv.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kyf.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://vsd.sufxvd.cn

[Q49] 更新单行
来源：http://kwj.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sgn.hnxiangtu.top

[Q50] 批量更新
来源：http://mre.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pka.svipenyu.cn

[Q51] 用子查询更新
来源：http://iki.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ckr.52xcode.cn

[Q52] 删除指定行
来源：http://lyq.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://shn.quarkkingdee.top

[Q53] 按条件删除
来源：http://wfi.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://roa.zycfv.cn

[Q54] 清空表
来源：http://ijq.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://vvu.yj20258888.top

[Q55] 排名（并列占位）
来源：http://wvu.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aqc.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://mzj.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wyf.yanxiufei.cn

[Q57] 行号
来源：http://nkk.316326.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wtv.0kj1m.cn

[Q58] 累计求和
来源：http://bft.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bmd.shangyingyoupin.top

[Q59] 分组内累计
来源：http://zus.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lkz.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://rey.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rxa.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xxy.xylfe.cn

[Q61] 移动平均
来源：http://bwt.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://igp.yj20258.top

[Q62] 分组占比
来源：http://rej.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fpe.quarkkingdee.top

[Q63] 开启事务
来源：http://wcn.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pov.ivvv.top

[Q64] 提交事务
来源：http://jjx.xuetiantiany.cn

COMMIT;
来源：http://rbt.hesvh.cn

[Q65] 回滚事务
来源：http://xqr.ydzc1.top

ROLLBACK;
来源：http://lzh.guowangkeji.top

[Q66] 行锁查询
来源：http://nxl.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zhr.hywenlv.cn

[Q67] 设置隔离级别
来源：http://win.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nnv.ppjwa.cn

[Q68] 保存点
来源：http://ouz.jqgfzy.top

SAVEPOINT sp1;
来源：http://lht.ehwqpu.com

ROLLBACK TO sp1;
来源：http://wpe.redwolf501.top

[Q69] 查看执行计划
来源：http://dyu.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uda.nanxuanxn.top

[Q70] 更新统计信息
来源：http://wtl.fktsv.cn


<!-- 参考信息 -->