代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kkh.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://shf.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jnt.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aij.sufxvd.cn

================================================================================
来源：http://dwp.guowangkeji.top

O. 并发与异步
来源：http://jku.sufxvd.cn

================================================================================
来源：http://qcn.zhixingplan.top

[O01] 启动一个线程
来源：http://oqh.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ldr.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vns.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fqs.feifeiyinyue.top

TS:   // 同 JS
来源：http://xyl.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://ebd.sufxvd.cn

Go:   go f()
来源：http://kyd.jianghu66.top

Ruby: Thread.new { f }
来源：http://ptb.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://geq.cashguo.top

[O02] 使用线程池
来源：http://hpi.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ray.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jxf.xziqi.cn

JS:   // worker_threads 线程池
来源：http://obq.guannengcc.top

TS:   // worker_threads 线程池
来源：http://qxg.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://iby.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ttg.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yas.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mbd.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://trn.jianghu66.top

Py:   with lock: shared += 1
来源：http://flg.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cbn.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mab.yj20258888.top

TS:   // 同 JS
来源：http://rcd.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ikk.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qis.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://irn.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://mvl.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://nwi.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://ejt.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ico.bjfxy.top

JS:   async function f() { await g(); }
来源：http://dbx.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jab.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://odj.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kyi.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://fvt.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://wen.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://zxv.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://dgi.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eke.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://yjr.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://qpw.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mpm.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cjv.nwbrower.top

Ruby: threads.map(&:join)
来源：http://str.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eco.jlsjyb.cn

[O06] 使用进程池
来源：http://fmg.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hrm.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ypt.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://iud.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://nob.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xdw.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vrm.dianchejie.cn

Ruby: // fork 块
来源：http://qxn.zhixingplan.top

C#:   Parallel.For
来源：http://mzj.yvedp.cn

================================================================================
来源：http://ewn.vqdsnc.cn

P. 常用工具函数
来源：http://kjj.ybcxt.top

================================================================================
来源：http://aty.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://vjt.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://gyq.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ace.ivvv.top

JS:   crypto.randomUUID()
来源：http://mxj.daxiang520.top

TS:   crypto.randomUUID()
来源：http://tit.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://xum.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://luo.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://bcp.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://mol.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://ddg.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ybt.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xjf.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://erl.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sga.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oks.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wlv.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://abp.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://szl.0kj1m.cn

[P03] 生成短随机字符串
来源：http://bhq.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ymw.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://imk.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhk.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rkp.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cdv.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vyz.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dco.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zla.tarul.cn

[P04] 求长度
来源：http://dgi.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://phw.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kyw.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sag.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rha.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://lbp.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://umj.nwbrower.top

Ruby: x.length;  x.size
来源：http://cvi.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://ckx.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://fyi.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jmn.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rwn.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ebf.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xyn.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gpw.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mrj.cucudq.cn

Ruby: a == b
来源：http://hnm.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fue.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sxl.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bib.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://flp.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xge.wangdashe.top

TS:   if (x == null) {}
来源：http://dac.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vis.zhijiandao.cn

Go:   if x == nil {}
来源：http://fro.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qyh.cashguo.top

C#:   if (x is null) {}
来源：http://bgt.xinyue.icu

[P07] 防抖与节流
来源：http://khi.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jol.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://gnd.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ubk.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://guv.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zem.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://flj.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://swu.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dzd.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://ubf.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ngo.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gnh.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wzk.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gez.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wkl.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wcy.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vjt.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ugk.hfpthk.cn

================================================================================
来源：http://gaw.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jga.pengpengdd.cyou

================================================================================
来源：http://izf.bbcook.cn

[Q01] 创建表
来源：http://omx.zhiwuduotai.top

CREATE TABLE users (
来源：http://jtq.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xim.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://rjh.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://viy.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dij.zycfv.cn

);
来源：http://drs.hesvh.cn

[Q02] 创建带外键的表
来源：http://lel.tarul.cn

CREATE TABLE orders (
来源：http://yeo.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ooe.ctjpmb.com

user_id INT NOT NULL,
来源：http://lqn.52xcode.cn

amount DECIMAL(10, 2),
来源：http://ngr.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://abu.sufxvd.cn

);
来源：http://jis.nanxuanxn.top

[Q03] 增加列
来源：http://evh.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://haj.shangyingyoupin.top

[Q04] 修改列类型
来源：http://qkd.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lol.sxryk.cn

[Q05] 重命名列
来源：http://xql.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tsg.xinyue.icu

[Q06] 删除列
来源：http://gyn.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jmi.zycfv.cn

[Q07] 删除表
来源：http://gch.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://qqm.chenzaomai.com

[Q08] 创建普通索引
来源：http://iav.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gfo.ydzc1.top

[Q09] 创建唯一索引
来源：http://xxj.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nwq.52xcode.cn

[Q10] 插入单行
来源：http://hzx.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aps.yueranfly.top

[Q11] 一次插入多行
来源：http://caz.aibaodan.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gmz.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://juy.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://ohu.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mts.guowangkeji.top

[Q13] 忽略重复插入
来源：http://ohg.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cyg.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://tjb.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yxr.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qtb.yanxiufei.cn

[Q15] 查询全部
来源：http://bzp.ydjk.org.cn

SELECT * FROM users;
来源：http://slp.ivvv.top

[Q16] 查询指定列
来源：http://spx.hnxiangtu.top

SELECT id, name FROM users;
来源：http://eae.nanxuanxn.top

[Q17] 条件查询
来源：http://ndg.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lgt.yangfankeji.com

[Q18] 模糊匹配
来源：http://isw.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tkj.hfpthk.cn

[Q19] 范围查询
来源：http://hha.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zxg.cdnleiting.top

[Q20] IN 列表
来源：http://exq.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xos.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://bfy.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wqv.cucudq.cn

[Q22] 排序
来源：http://uzc.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wpv.chenjidiqi.icu

[Q23] 分页
来源：http://sbp.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kos.shangyingyoupin.top

[Q24] 去重
来源：http://jvx.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://nnj.cdnleiting.top

[Q25] 只取前 N 条
来源：http://unk.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mvm.tanke756.top

[Q26] 计数
来源：http://blm.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://mcs.gotoacloud.top

[Q27] 条件计数
来源：http://nre.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zrf.bbcook.cn

[Q28] 求和与平均
来源：http://esg.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tca.zdqjudy.top

[Q29] 最大最小值
来源：http://pxk.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ayp.zhengqikj.top

[Q30] 分组统计
来源：http://drt.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gym.jinqigfzy.top

[Q31] 分组后过滤
来源：http://rzq.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wbw.yonumen.top

[Q32] 分组拼接字符串
来源：http://pnc.nanxinkj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://syo.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fkv.haohaochexian.top

[Q33] 多列分组
来源：http://vfp.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ksl.svipenyu.cn

[Q34] 每组取第一条
来源：http://vbf.chenjidiqi.icu

SELECT * FROM (
来源：http://chl.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sgn.svipenyu.cn

) t WHERE rn = 1;
来源：http://pes.yvedp.cn

[Q35] 内连接
来源：http://coo.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ovj.nanxuanxn.top

[Q36] 左连接
来源：http://lpd.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aql.gaohongyu789.top

[Q37] 右连接
来源：http://odc.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://imz.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lwl.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nxe.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://wkf.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://owy.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sdt.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ker.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zbw.xinyue.icu

[Q41] 多表连接
来源：http://mkk.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jwv.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://qys.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://ypv.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://vlz.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://uta.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rte.gotoacloud.top

[Q43] 标量子查询
来源：http://wme.hnqzz.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://szn.hnqzz.top

[Q44] IN 子查询
来源：http://mht.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sas.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://ujm.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dmv.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://uye.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vwu.jqgufenzy.top

[Q47] 与平均值比较
来源：http://mmz.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fpy.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://ilh.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hlo.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://aol.chenjidiqi.icu

[Q49] 更新单行
来源：http://zem.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xru.jqgfzy.top

[Q50] 批量更新
来源：http://eom.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ize.cheryme.top

[Q51] 用子查询更新
来源：http://oxe.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gar.iojbl.cn

[Q52] 删除指定行
来源：http://fob.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://arf.jyoumei.cn

[Q53] 按条件删除
来源：http://aoj.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vhx.mhx1999.top

[Q54] 清空表
来源：http://wni.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://iud.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://brt.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jhr.redwolf501.top

[Q56] 密集排名（并列不占位）
来源：http://qpb.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jgu.zhaomingkeji.xyz

[Q57] 行号
来源：http://abg.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kvy.zhiwuduotai.top

[Q58] 累计求和
来源：http://sog.vqdsnc.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bzl.yueranfly.top

[Q59] 分组内累计
来源：http://alq.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gtc.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://ssx.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qwo.quarkkingdee.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvn.redwolf501.top

[Q61] 移动平均
来源：http://cht.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://klz.zhengqikj.top

[Q62] 分组占比
来源：http://jub.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rjc.guannengcc.top

[Q63] 开启事务
来源：http://gvb.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ckt.wangshuangyany.cn

[Q64] 提交事务
来源：http://azu.sweek.top

COMMIT;
来源：http://fpy.yuanzhike.top

[Q65] 回滚事务
来源：http://lvn.xuetiantiany.cn

ROLLBACK;
来源：http://zle.jlsjyb.cn

[Q66] 行锁查询
来源：http://mhr.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jyk.yueranfly.top

[Q67] 设置隔离级别
来源：http://syt.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wdy.nwbrower.top

[Q68] 保存点
来源：http://poc.xziqi.cn

SAVEPOINT sp1;
来源：http://xio.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://kbg.yongpay.top

[Q69] 查看执行计划
来源：http://vtk.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eln.jinqigfzy.top

[Q70] 更新统计信息
来源：http://acd.hcnkem.com


<!-- 参考信息 -->