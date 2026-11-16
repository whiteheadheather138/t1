代发 wailian999

================================================================================
来源：http://rdj.xylfe.cn

O. 并发与异步
来源：http://ekb.dashuyun.cn

================================================================================
来源：http://chp.hammf.cn

[O01] 启动一个线程
来源：http://med.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kde.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rcf.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ydb.yuxming.cn

TS:   // 同 JS
来源：http://prh.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://wdb.jqgufenzy.top

Go:   go f()
来源：http://udd.birdmap.top

Ruby: Thread.new { f }
来源：http://pto.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://guw.yuxming.cn

[O02] 使用线程池
来源：http://dlu.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tju.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hrp.epnwcf.com

JS:   // worker_threads 线程池
来源：http://qwz.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://nqb.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://fss.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dys.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://clb.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fpg.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://our.yj202588.top

Py:   with lock: shared += 1
来源：http://kqh.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://krd.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vju.316326.xyz

TS:   // 同 JS
来源：http://mnx.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://zqd.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://alv.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jcf.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://ros.xylfe.cn

[O04] 定义异步函数并等待
来源：http://sdu.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://zub.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://knr.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://vqt.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cmw.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyg.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pdn.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://nyx.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://koq.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://mre.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://zii.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rnl.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://jfp.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://tou.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://smh.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wzo.hesvh.cn

Ruby: threads.map(&:join)
来源：http://iql.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pyy.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://ybe.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fxw.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qbv.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://xkl.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://fyy.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xqh.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://taf.9152youxi.cn

Ruby: // fork 块
来源：http://qok.fehbvm.com

C#:   Parallel.For
来源：http://asg.pycfn.com

================================================================================
来源：http://jel.hongshengwenyu.top

P. 常用工具函数
来源：http://ksb.xingfuxueyuan.xyz

================================================================================
来源：http://mwf.svipenyu.cn

[P01] 生成 UUID
来源：http://tid.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://mhu.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://szc.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://snx.tanke756.top

TS:   crypto.randomUUID()
来源：http://cpk.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://gju.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://gjn.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://zii.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://mpe.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://fve.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://szo.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://dhu.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uwq.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cch.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bno.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xom.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zsk.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ubx.gotoacloud.top

[P03] 生成短随机字符串
来源：http://goj.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ndj.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zzg.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zzd.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grv.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ehd.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ahp.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wnx.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nrw.ehwqpu.com

[P04] 求长度
来源：http://hxp.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kda.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rgx.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fxv.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyv.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://zka.pycfn.com

Go:   len(arr);  len(m)
来源：http://cib.xuanzx.com

Ruby: x.length;  x.size
来源：http://dfb.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bot.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://yhp.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://dni.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yqr.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sch.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://skh.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tal.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://cxs.jianghu66.top

Ruby: a == b
来源：http://vdg.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mih.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fke.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lad.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://xfd.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jdu.fengsongda.top

TS:   if (x == null) {}
来源：http://ruv.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aqk.chenzaomai.com

Go:   if x == nil {}
来源：http://qyi.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hem.ppjwa.cn

C#:   if (x is null) {}
来源：http://qai.sxryk.cn

[P07] 防抖与节流
来源：http://axn.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://brh.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://pga.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gyl.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbr.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bfq.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ake.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qdo.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bph.mhx1999.top

[P08] 处理浮点精度问题
来源：http://zkh.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uwq.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgy.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://anm.xuetiantiany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jjc.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yjm.sufxvd.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dpa.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uxo.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bgk.kuanghao11.cn

================================================================================
来源：http://ppx.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://laf.ydjk.org.cn

================================================================================
来源：http://nrx.hysaishi.cn

[Q01] 创建表
来源：http://hzi.jianghu66.top

CREATE TABLE users (
来源：http://vsn.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cuz.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://idf.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://kav.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vap.sufxvd.cn

);
来源：http://snn.wangdashe.top

[Q02] 创建带外键的表
来源：http://niz.hammf.cn

CREATE TABLE orders (
来源：http://pmt.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ryc.fzhhl.top

user_id INT NOT NULL,
来源：http://mzk.cheryme.top

amount DECIMAL(10, 2),
来源：http://tcr.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lhd.xuetiantiany.cn

);
来源：http://hlc.gzhubu.top

[Q03] 增加列
来源：http://knj.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gso.cucudq.cn

[Q04] 修改列类型
来源：http://aig.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wyn.yvedp.cn

[Q05] 重命名列
来源：http://mva.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zum.sjlbkw.cn

[Q06] 删除列
来源：http://esk.xinyue.icu

ALTER TABLE users DROP COLUMN age;
来源：http://ilo.vqdsnc.cn

[Q07] 删除表
来源：http://xxy.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://qev.ydzc1.top

[Q08] 创建普通索引
来源：http://vfc.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cdk.sxryk.cn

[Q09] 创建唯一索引
来源：http://ibk.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ctg.hesvh.cn

[Q10] 插入单行
来源：http://fxi.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jnd.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://mln.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jzl.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://gwy.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://rjr.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dmw.vehdjk.com

[Q13] 忽略重复插入
来源：http://tgt.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lkh.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://mkc.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xds.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kyv.tanke756.top

[Q15] 查询全部
来源：http://uaw.yongpay.top

SELECT * FROM users;
来源：http://fpw.fehbvm.com

[Q16] 查询指定列
来源：http://aeo.fehbvm.com

SELECT id, name FROM users;
来源：http://xzy.tanke756.top

[Q17] 条件查询
来源：http://dsd.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kpw.cqqwz.cn

[Q18] 模糊匹配
来源：http://rzi.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yyb.fktsv.cn

[Q19] 范围查询
来源：http://rxt.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mru.yj20258.top

[Q20] IN 列表
来源：http://yec.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jou.bbcook.cn

[Q21] 空值判断
来源：http://ebe.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vjq.epnwcf.com

[Q22] 排序
来源：http://xod.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sqv.ivvv.top

[Q23] 分页
来源：http://aff.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gkg.wangshuangyany.cn

[Q24] 去重
来源：http://qnl.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://fqi.yonumen.top

[Q25] 只取前 N 条
来源：http://hrf.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xjk.0kj1m.cn

[Q26] 计数
来源：http://skb.shanyushiyangtech.top

SELECT COUNT(*) FROM users;
来源：http://xcj.0kj1m.cn

[Q27] 条件计数
来源：http://kat.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hsl.aibaodan.cn

[Q28] 求和与平均
来源：http://mog.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zdu.xinyue.icu

[Q29] 最大最小值
来源：http://pfk.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ktw.hongshengwenyu.top

[Q30] 分组统计
来源：http://nji.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vdr.zdqjudy.top

[Q31] 分组后过滤
来源：http://kzr.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cxk.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://qgj.gogol.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wxn.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rik.meibo888.top

[Q33] 多列分组
来源：http://tig.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://atk.bbcook.cn

[Q34] 每组取第一条
来源：http://spk.ywan-chungtsiang.top

SELECT * FROM (
来源：http://lol.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zwd.zdqjudy.top

) t WHERE rn = 1;
来源：http://mtu.snrcjt.cn

[Q35] 内连接
来源：http://vbi.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://end.ydjk.org.cn

[Q36] 左连接
来源：http://gfd.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://beg.fktsv.cn

[Q37] 右连接
来源：http://meo.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vyj.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qox.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nla.havefunace.top

[Q39] 自连接（查上下级）
来源：http://ziz.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gck.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gxc.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://uwi.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://osb.ivvv.top

[Q41] 多表连接
来源：http://dvb.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ivl.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://cxx.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://ekm.meibo888.top

[Q42] 连接条件附加过滤
来源：http://gcm.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://hgk.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zxc.andypj.xyz

[Q43] 标量子查询
来源：http://oiv.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vzh.epnwcf.com

[Q44] IN 子查询
来源：http://mpi.yj202588.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wem.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://yyd.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cuv.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://fky.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://btj.sufxvd.cn

[Q47] 与平均值比较
来源：http://fab.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://exs.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://iut.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sjv.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://hqr.zhongyouzk.top

[Q49] 更新单行
来源：http://nwp.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mxe.zhengqikj.top

[Q50] 批量更新
来源：http://nhm.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hmm.sjlbkw.cn

[Q51] 用子查询更新
来源：http://jac.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cyy.hammf.cn

[Q52] 删除指定行
来源：http://lls.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://ejz.shuidangran.top

[Q53] 按条件删除
来源：http://npy.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nds.zhiwuduotai.top

[Q54] 清空表
来源：http://ufx.shuidangran.top

TRUNCATE TABLE logs;
来源：http://jqk.vehdjk.com

[Q55] 排名（并列占位）
来源：http://ikr.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cwm.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://omq.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://css.birdmap.top

[Q57] 行号
来源：http://aui.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fuz.yuxming.cn

[Q58] 累计求和
来源：http://auk.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qir.dashuyun.cn

[Q59] 分组内累计
来源：http://zjo.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cow.shanyushiyangkeji.top

[Q60] 取上一行 / 下一行
来源：http://gpf.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://upq.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vrp.epnwcf.com

[Q61] 移动平均
来源：http://ani.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eea.aizwys.cn

[Q62] 分组占比
来源：http://lpf.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xze.hesvh.cn

[Q63] 开启事务
来源：http://xii.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://mjo.zhixingplan.top

[Q64] 提交事务
来源：http://wno.jinqigufen.top

COMMIT;
来源：http://ooe.316326.xyz

[Q65] 回滚事务
来源：http://uqf.pycfn.com

ROLLBACK;
来源：http://gws.cdnleiting.top

[Q66] 行锁查询
来源：http://cfq.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://woe.yongpay.top

[Q67] 设置隔离级别
来源：http://nmu.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yzp.zhaomingkeji.xyz

[Q68] 保存点
来源：http://ynk.yuxming.cn

SAVEPOINT sp1;
来源：http://fwd.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://jee.hcnkem.com

[Q69] 查看执行计划
来源：http://xid.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mvf.c1oappe.top

[Q70] 更新统计信息
来源：http://lxy.gzhubu.top

ANALYZE TABLE users;
来源：http://loo.shuidangran.top

[Q71] 查看建表语句
来源：http://liq.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lcl.zhengqikj.top

[Q72] 查看索引
来源：http://bdw.fzhhl.top


<!-- 参考信息 -->