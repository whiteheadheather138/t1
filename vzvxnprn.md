代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://alc.sufxvd.cn

Go:   go f()
来源：http://fyk.xuanzx.com

Ruby: Thread.new { f }
来源：http://yek.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://waz.jiagoushi.top

[O02] 使用线程池
来源：http://akh.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://giq.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jqp.wangdashe.top

JS:   // worker_threads 线程池
来源：http://umi.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://zzn.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://ciw.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mzx.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baf.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbw.tian-w.cn

[O03] 加锁保护共享数据
来源：http://coh.dashuyun.cn

Py:   with lock: shared += 1
来源：http://kwa.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://odd.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rot.jinghuilouyu.cn

TS:   // 同 JS
来源：http://ywx.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://rdj.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ruk.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xfe.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://nbf.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://mgl.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://fhj.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://okr.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://jgn.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tbp.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vgs.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fkh.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://wwk.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://jcn.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://ozt.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://tma.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://boz.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://gow.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://roa.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jyz.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kwo.gzhubu.top

Ruby: threads.map(&:join)
来源：http://olf.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wfm.chenjidiqi.icu

[O06] 使用进程池
来源：http://ori.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xam.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fin.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://dbq.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://ufx.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jox.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gkw.daria6918.cn

Ruby: // fork 块
来源：http://ldh.yongpay.top

C#:   Parallel.For
来源：http://xco.zhongyouzk.top

================================================================================
来源：http://nmx.chenzaomai.com

P. 常用工具函数
来源：http://gvs.chenlongwang.top

================================================================================
来源：http://mqw.uphjek.com

[P01] 生成 UUID
来源：http://fwr.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://jnc.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oow.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://dep.havefunace.top

TS:   crypto.randomUUID()
来源：http://cvm.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://nzo.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://lna.havefunace.top

Ruby: SecureRandom.uuid
来源：http://sts.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://hcm.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://pud.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ykh.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmu.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ekg.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mjw.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://drl.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kmh.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://grl.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fgm.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://ptu.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fli.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ixn.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://egp.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cmi.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://urj.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wnw.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://hcx.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hgy.sufxvd.cn

[P04] 求长度
来源：http://ndv.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://anv.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hvr.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nwl.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgj.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://qhm.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://ifb.aibaodan.cn

Ruby: x.length;  x.size
来源：http://ukz.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://eda.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://xxg.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tnv.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ufx.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oeb.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://igh.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zun.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://jzn.daria6918.cn

Ruby: a == b
来源：http://yfn.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xch.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wvq.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cng.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://mme.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tpr.hcnkem.com

TS:   if (x == null) {}
来源：http://cpn.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://adc.cqqwz.cn

Go:   if x == nil {}
来源：http://kkg.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://feg.yangfankeji.com

C#:   if (x is null) {}
来源：http://dpb.jyoumei.cn

[P07] 防抖与节流
来源：http://zrs.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bjc.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://ldi.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aul.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://okp.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://abk.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wqa.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://blh.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yed.aizwys.cn

[P08] 处理浮点精度问题
来源：http://rda.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pug.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://goy.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ahw.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zus.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ksp.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://shf.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iqb.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ruz.yfazqb.com

================================================================================
来源：http://msp.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tmy.guowangkeji.top

================================================================================
来源：http://qmx.yvedp.cn

[Q01] 创建表
来源：http://eps.zdqjudy.top

CREATE TABLE users (
来源：http://jle.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jrs.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://cwy.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://vgz.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jem.cashguo.top

);
来源：http://bsx.sweek.top

[Q02] 创建带外键的表
来源：http://yrw.fktsv.cn

CREATE TABLE orders (
来源：http://dgi.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://slf.svipenyu.cn

user_id INT NOT NULL,
来源：http://soe.bbcook.cn

amount DECIMAL(10, 2),
来源：http://bel.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://itq.hfpthk.cn

);
来源：http://ukf.jqgfzy.top

[Q03] 增加列
来源：http://oei.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jcf.shzxlz.cn

[Q04] 修改列类型
来源：http://huc.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qdx.jinqigufen.top

[Q05] 重命名列
来源：http://xoy.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://igy.epnwcf.com

[Q06] 删除列
来源：http://xcx.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://scx.zdqjudy.top

[Q07] 删除表
来源：http://rcd.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://teo.0kj1m.cn

[Q08] 创建普通索引
来源：http://vjm.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lpc.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://vps.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hom.ehwqpu.com

[Q10] 插入单行
来源：http://ufs.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bwr.yonumen.top

[Q11] 一次插入多行
来源：http://ksa.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rzf.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://heb.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://igs.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wfj.0kj1m.cn

[Q13] 忽略重复插入
来源：http://tgv.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fzh.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://fpa.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uum.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ses.zhengqikj.top

[Q15] 查询全部
来源：http://mjq.hywenlv.cn

SELECT * FROM users;
来源：http://eyx.yangfankeji.com

[Q16] 查询指定列
来源：http://voz.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://cjx.cqqwz.cn

[Q17] 条件查询
来源：http://guz.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zdy.dianchejie.cn

[Q18] 模糊匹配
来源：http://bfi.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qgt.daria6918.cn

[Q19] 范围查询
来源：http://whk.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://peq.xuetiantiany.cn

[Q20] IN 列表
来源：http://fcg.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ofm.c1oappe.top

[Q21] 空值判断
来源：http://vzx.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mxc.havefunace.top

[Q22] 排序
来源：http://whp.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kwx.guannengcc.top

[Q23] 分页
来源：http://qug.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vab.havefunace.top

[Q24] 去重
来源：http://cri.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://lot.ydzc1.top

[Q25] 只取前 N 条
来源：http://rfr.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xaj.jinghuilouyu.cn

[Q26] 计数
来源：http://jfr.nwbrower.top

SELECT COUNT(*) FROM users;
来源：http://xrt.xinyue.icu

[Q27] 条件计数
来源：http://tti.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rdw.ehwqpu.com

[Q28] 求和与平均
来源：http://drl.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zix.pengpengdd.cyou

[Q29] 最大最小值
来源：http://ikz.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xwi.cdnleiting.top

[Q30] 分组统计
来源：http://qbx.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wly.zhongyouzk.top

[Q31] 分组后过滤
来源：http://ban.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rkr.redwolf501.top

[Q32] 分组拼接字符串
来源：http://imr.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dgy.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ikd.xingfuxueyuan.xyz

[Q33] 多列分组
来源：http://rvm.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tsn.52xcode.cn

[Q34] 每组取第一条
来源：http://lgq.hammf.cn

SELECT * FROM (
来源：http://gkx.bjfxy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vyc.hesvh.cn

) t WHERE rn = 1;
来源：http://lhs.uphjek.com

[Q35] 内连接
来源：http://hox.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wre.sysykeji.top

[Q36] 左连接
来源：http://pcl.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://trw.kuanghao11.cn

[Q37] 右连接
来源：http://vca.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://obu.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://mik.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://und.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://uel.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdj.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oml.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iwd.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eiv.zdbjq.cn

[Q41] 多表连接
来源：http://teu.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cxe.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://ijv.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://pmz.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://uxo.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://lqc.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gth.fehbvm.com

[Q43] 标量子查询
来源：http://awx.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tbb.tarul.cn

[Q44] IN 子查询
来源：http://pfs.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://omd.havefunace.top

[Q45] EXISTS 判断存在
来源：http://aqi.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://elz.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://sii.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cbu.chenzaomai.com

[Q47] 与平均值比较
来源：http://frg.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yhh.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://smn.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://toa.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://eny.jqgfzy.top

[Q49] 更新单行
来源：http://auj.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mep.snrcjt.cn

[Q50] 批量更新
来源：http://ssp.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zqf.ydjk.org.cn

[Q51] 用子查询更新
来源：http://lhf.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yzv.nanxinkj.top

[Q52] 删除指定行
来源：http://loy.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://tss.fktsv.cn

[Q53] 按条件删除
来源：http://kdg.jinqigfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fux.shanyushiyangtech.top

[Q54] 清空表
来源：http://ycs.yj20258888.top

TRUNCATE TABLE logs;
来源：http://xqp.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://bvy.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zhc.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://fdx.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zqo.shanyushiyangtech.top

[Q57] 行号
来源：http://hdr.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://slf.jqgfzy.top

[Q58] 累计求和
来源：http://gco.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nai.ybcxt.top

[Q59] 分组内累计
来源：http://nzn.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cxe.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://udk.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gie.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://krc.hammf.cn

[Q61] 移动平均
来源：http://ouf.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fbi.tianlin.xyz

[Q62] 分组占比
来源：http://qhv.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://esh.yuxming.cn

[Q63] 开启事务
来源：http://ijo.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uzx.chenzaomai.com

[Q64] 提交事务
来源：http://rhb.hcnkem.com

COMMIT;
来源：http://qdd.tianlin.xyz

[Q65] 回滚事务
来源：http://dbz.hongshengwenyu.top

ROLLBACK;
来源：http://wys.316326.xyz

[Q66] 行锁查询
来源：http://obf.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vsw.xinyue.icu

[Q67] 设置隔离级别
来源：http://yba.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mxe.yj20258888.top

[Q68] 保存点
来源：http://efv.kuanghao11.cn

SAVEPOINT sp1;
来源：http://xws.svipenyu.cn

ROLLBACK TO sp1;
来源：http://vvf.chenzaomai.com

[Q69] 查看执行计划
来源：http://isr.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gxy.daxiang520.top

[Q70] 更新统计信息
来源：http://osm.ctjpmb.com

ANALYZE TABLE users;
来源：http://wzk.jqgufenzy.top

[Q71] 查看建表语句
来源：http://stq.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wjj.jiagoushi.top

[Q72] 查看索引
来源：http://bxm.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://zqw.daxiang520.top

[Q73] 查看表状态
来源：http://xfo.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uhx.haohaochexian.top

[Q74] 强制使用索引
来源：http://acl.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cxj.zhongyouzk.top

[Q75] 日期格式化
来源：http://uve.pengpengdd.cyou

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jlt.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mty.jqgufenzy.top


<!-- 参考信息 -->