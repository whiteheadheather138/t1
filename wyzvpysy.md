代发 wailian999

================================================================================
来源：http://aoe.yuxming.cn

O. 并发与异步
来源：http://mgn.nwbrower.top

================================================================================
来源：http://ygp.52xcode.cn

[O01] 启动一个线程
来源：http://ndi.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yzn.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://elo.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://snp.ydjk.org.cn

TS:   // 同 JS
来源：http://pwf.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://eee.cashguo.top

Go:   go f()
来源：http://sso.chenlongwang.top

Ruby: Thread.new { f }
来源：http://eql.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://stx.cashguo.top

[O02] 使用线程池
来源：http://fgn.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rqc.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bkb.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://fya.hammf.cn

TS:   // worker_threads 线程池
来源：http://vts.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://orc.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://syi.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ilf.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dhl.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://zhv.c1oappe.top

Py:   with lock: shared += 1
来源：http://sdm.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://lxr.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jnb.snrcjt.cn

TS:   // 同 JS
来源：http://emz.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://vjk.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://utt.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fll.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://zcp.gzhubu.top

[O04] 定义异步函数并等待
来源：http://iwm.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://zvf.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hun.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://iae.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://apt.zdqjudy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ybt.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nfh.vqdsnc.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tcx.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://lwn.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://fke.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://lsw.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yzb.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://mlb.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://jux.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vcs.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qmx.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://qiq.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://lcy.jinqigufen.top

[O06] 使用进程池
来源：http://kqk.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wdo.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kun.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://wda.316326.xyz

TS:   // child_process / cluster 模块
来源：http://qiv.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wgr.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://khd.cqqwz.cn

Ruby: // fork 块
来源：http://ley.hammf.cn

C#:   Parallel.For
来源：http://taw.havefunace.top

================================================================================
来源：http://wei.zhiwuduotai.top

P. 常用工具函数
来源：http://bgd.gogol.net.cn

================================================================================
来源：http://hsa.chenzaomai.com

[P01] 生成 UUID
来源：http://knt.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://bnj.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ijv.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://jct.epnwcf.com

TS:   crypto.randomUUID()
来源：http://ljx.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://ahm.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://ndx.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://uti.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://phz.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://bbj.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pij.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://qmh.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ewb.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://azq.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cou.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pmj.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mxi.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ftm.cheryme.top

[P03] 生成短随机字符串
来源：http://qeb.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yyw.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oxu.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvj.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bfz.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vbp.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://glh.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://erz.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nlr.yueranfly.top

[P04] 求长度
来源：http://wih.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qod.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://niv.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wiv.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://whl.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://jhb.xziqi.cn

Go:   len(arr);  len(m)
来源：http://qug.birdmap.top

Ruby: x.length;  x.size
来源：http://ssf.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wce.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://aty.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://aqu.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ivm.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xru.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ajz.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tpn.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yrb.jianghu66.top

Ruby: a == b
来源：http://oxu.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lzr.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ngb.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lrp.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://xlx.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cbw.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://guq.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uui.ppjwa.cn

Go:   if x == nil {}
来源：http://zmv.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://snl.smart0.xyz

C#:   if (x is null) {}
来源：http://stc.jinqigfzy.top

[P07] 防抖与节流
来源：http://etp.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oxg.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://fxe.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpo.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbn.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pmk.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gsm.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://epo.yvedp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dwr.guannengcc.top

[P08] 处理浮点精度问题
来源：http://fkm.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cev.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ryb.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bcv.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://awt.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xvk.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://szo.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fsk.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wpm.tian-w.cn

================================================================================
来源：http://evc.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pbk.bbcook.cn

================================================================================
来源：http://egy.xylfe.cn

[Q01] 创建表
来源：http://mmy.hesvh.cn

CREATE TABLE users (
来源：http://hjv.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://txv.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://glc.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://dam.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ypg.zycfv.cn

);
来源：http://syv.snrcjt.cn

[Q02] 创建带外键的表
来源：http://bir.ctjpmb.com

CREATE TABLE orders (
来源：http://clz.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dwt.iojbl.cn

user_id INT NOT NULL,
来源：http://vei.tian-w.cn

amount DECIMAL(10, 2),
来源：http://wkx.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jox.yueranfly.top

);
来源：http://dbb.yueranfly.top

[Q03] 增加列
来源：http://vaw.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hro.zhoulong.xyz

[Q04] 修改列类型
来源：http://wgb.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jjr.xuanzx.com

[Q05] 重命名列
来源：http://ekp.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cro.haohaochexian.top

[Q06] 删除列
来源：http://qkh.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dla.jiagoushi.top

[Q07] 删除表
来源：http://oro.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://pwz.shzxlz.cn

[Q08] 创建普通索引
来源：http://vvw.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jqw.chenlongwang.top

[Q09] 创建唯一索引
来源：http://pql.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gsj.cdnleiting.top

[Q10] 插入单行
来源：http://zar.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kmw.xylfe.cn

[Q11] 一次插入多行
来源：http://rhj.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://trk.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://ash.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://lgm.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jso.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://ysh.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uns.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://snx.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://emo.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cvn.hammf.cn

[Q15] 查询全部
来源：http://qnm.daxiang520.top

SELECT * FROM users;
来源：http://okm.yj20258888.top

[Q16] 查询指定列
来源：http://xkn.yuxming.cn

SELECT id, name FROM users;
来源：http://gbt.yanxiufei.cn

[Q17] 条件查询
来源：http://ffm.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kwm.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://qpg.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wko.yj20258888.top

[Q19] 范围查询
来源：http://hwg.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jvx.snrcjt.cn

[Q20] IN 列表
来源：http://acc.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zsr.guannengcc.top

[Q21] 空值判断
来源：http://vwa.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://wly.feifeiyinyue.top

[Q22] 排序
来源：http://lgy.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zkr.sufxvd.cn

[Q23] 分页
来源：http://fog.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hoj.gzhubu.top

[Q24] 去重
来源：http://zus.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://vfz.yfazqb.com

[Q25] 只取前 N 条
来源：http://ljf.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wdc.ehwqpu.com

[Q26] 计数
来源：http://aqk.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://znm.ybcxt.top

[Q27] 条件计数
来源：http://pqb.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hes.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://jjj.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://krz.9152youxi.cn

[Q29] 最大最小值
来源：http://wgv.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hsq.bbcook.cn

[Q30] 分组统计
来源：http://jan.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qug.guowangkeji.top

[Q31] 分组后过滤
来源：http://gxq.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iap.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://vni.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bcc.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mzj.shzxlz.cn

[Q33] 多列分组
来源：http://zzi.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lie.hcnkem.com

[Q34] 每组取第一条
来源：http://mkz.fengsongda.top

SELECT * FROM (
来源：http://uhu.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rnb.zhengqikj.top

) t WHERE rn = 1;
来源：http://usf.fzhhl.top

[Q35] 内连接
来源：http://zgm.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fji.0kj1m.cn

[Q36] 左连接
来源：http://mil.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mdj.daria6918.cn

[Q37] 右连接
来源：http://gxf.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nhi.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://uad.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bgb.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://ouk.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://yzz.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mje.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ebq.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jrx.xuetiantiany.cn

[Q41] 多表连接
来源：http://mxs.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://saq.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://qnj.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://bbu.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://bhc.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://mcl.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://job.snrcjt.cn

[Q43] 标量子查询
来源：http://wws.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://och.hysaishi.cn

[Q44] IN 子查询
来源：http://trk.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vrg.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://qhs.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rdj.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://ddz.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gcp.yfazqb.com

[Q47] 与平均值比较
来源：http://vgy.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kuq.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://hog.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ykq.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://lbm.ydzc1.top

[Q49] 更新单行
来源：http://uai.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fch.hnqzz.top

[Q50] 批量更新
来源：http://eqp.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://peh.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://fql.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mhl.shuidangran.top

[Q52] 删除指定行
来源：http://njl.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://vfb.zhoulong.xyz

[Q53] 按条件删除
来源：http://qhh.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nop.hongshengwenyu.top

[Q54] 清空表
来源：http://jzy.yj20258.top

TRUNCATE TABLE logs;
来源：http://bmt.cashguo.top

[Q55] 排名（并列占位）
来源：http://vih.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://guw.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://twm.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gri.pycfn.com

[Q57] 行号
来源：http://yym.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ksj.kuanghao11.cn

[Q58] 累计求和
来源：http://pto.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wjq.jiagoushi.top

[Q59] 分组内累计
来源：http://owt.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vrc.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://cua.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ygy.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://del.chenlongwang.top

[Q61] 移动平均
来源：http://ssy.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ofb.gogol.net.cn

[Q62] 分组占比
来源：http://bjc.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jxv.epnwcf.com

[Q63] 开启事务
来源：http://cdm.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uun.havefunace.top

[Q64] 提交事务
来源：http://kdp.cashguo.top

COMMIT;
来源：http://uhe.tanke756.top

[Q65] 回滚事务
来源：http://wvt.pengpengdd.cyou

ROLLBACK;
来源：http://goy.dianchejie.cn

[Q66] 行锁查询
来源：http://bku.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fhr.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://uml.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vih.chenlongwang.top

[Q68] 保存点
来源：http://xzp.ctjpmb.com

SAVEPOINT sp1;
来源：http://lqi.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://nsu.daxiang520.top

[Q69] 查看执行计划
来源：http://oib.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ahf.uphjek.com

[Q70] 更新统计信息
来源：http://oht.hywenlv.cn

ANALYZE TABLE users;
来源：http://xjo.cheryme.top

[Q71] 查看建表语句
来源：http://xag.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://upa.sjlbkw.cn

[Q72] 查看索引
来源：http://nmn.zycfv.cn


<!-- 参考信息 -->