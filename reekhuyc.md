代发 wailian999

TS:   // worker_threads 线程池
来源：http://fap.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://xpw.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tso.shanyushiyangtech.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sey.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://joj.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://vty.316326.xyz

Py:   with lock: shared += 1
来源：http://zer.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://qlk.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pfv.hesvh.cn

TS:   // 同 JS
来源：http://vyz.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://bgl.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rea.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://luc.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://qhq.bjfxy.top

[O04] 定义异步函数并等待
来源：http://bjn.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://mpb.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rcu.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://pgz.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fop.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wmf.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pcv.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://fgl.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://ivw.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://ffw.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://ihn.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lzl.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://zml.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://txx.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://czt.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ebf.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://ifw.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://jbe.hcnkem.com

[O06] 使用进程池
来源：http://iuj.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://auj.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rxm.pycfn.com

JS:   // child_process / cluster 模块
来源：http://vag.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://pfd.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mwa.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cgs.jqgufenzy.top

Ruby: // fork 块
来源：http://vzt.epnwcf.com

C#:   Parallel.For
来源：http://khw.ydzc1.top

================================================================================
来源：http://iae.fanxiaobao.xyz

P. 常用工具函数
来源：http://tov.jinghuilouyu.cn

================================================================================
来源：http://reo.jlsjyb.cn

[P01] 生成 UUID
来源：http://tty.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://ksm.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pds.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://knk.bbcook.cn

TS:   crypto.randomUUID()
来源：http://yei.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://sow.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://nzf.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://iug.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://erc.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://fod.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://suq.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gjp.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sbr.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wyw.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ofs.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ylo.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ect.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ltz.jinqigufen.top

[P03] 生成短随机字符串
来源：http://uiu.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ezk.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hxl.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qcg.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfz.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hqd.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rjp.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://afd.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://scq.guannengcc.top

[P04] 求长度
来源：http://rix.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bes.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lle.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pel.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mpp.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://nwg.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://cai.hammf.cn

Ruby: x.length;  x.size
来源：http://sbl.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbd.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://uaj.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bql.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://adk.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bzu.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tvp.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://piu.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://vyz.shangyingyoupin.top

Ruby: a == b
来源：http://eic.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tkc.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sjw.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://drj.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://efp.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qxc.kuanghao11.cn

TS:   if (x == null) {}
来源：http://hlf.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xxh.wangdashe.top

Go:   if x == nil {}
来源：http://jpr.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://moe.nwbrower.top

C#:   if (x is null) {}
来源：http://dfx.jiagoushi.top

[P07] 防抖与节流
来源：http://fmn.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rnq.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://kes.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jky.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bcl.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aat.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eec.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ycu.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dso.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://pph.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://krf.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pwt.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eig.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kjg.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oeq.sufxvd.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ngr.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kra.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bfu.9152youxi.cn

================================================================================
来源：http://frj.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fhy.yongpay.top

================================================================================
来源：http://enf.smart0.xyz

[Q01] 创建表
来源：http://njs.smart0.xyz

CREATE TABLE users (
来源：http://cxp.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wrd.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://fem.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://wey.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ywv.guannengcc.top

);
来源：http://xpd.xingfuxueyuan.xyz

[Q02] 创建带外键的表
来源：http://jgg.sxryk.cn

CREATE TABLE orders (
来源：http://mba.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://awd.gotoacloud.top

user_id INT NOT NULL,
来源：http://nks.ivvv.top

amount DECIMAL(10, 2),
来源：http://bcz.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pwc.pycfn.com

);
来源：http://wjf.havefunace.top

[Q03] 增加列
来源：http://hye.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rkv.bjfxy.top

[Q04] 修改列类型
来源：http://kor.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uzs.yongpay.top

[Q05] 重命名列
来源：http://xax.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xvl.iojbl.cn

[Q06] 删除列
来源：http://snq.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ddd.yvedp.cn

[Q07] 删除表
来源：http://uay.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://fet.tanke756.top

[Q08] 创建普通索引
来源：http://uie.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://dmk.yj202588.top

[Q09] 创建唯一索引
来源：http://ebn.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dqp.guannengcc.top

[Q10] 插入单行
来源：http://fqs.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zuf.jlsjyb.cn

[Q11] 一次插入多行
来源：http://qqh.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://grq.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://wdw.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ljp.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bqe.yj20258888.top

[Q13] 忽略重复插入
来源：http://nix.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://aqv.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://brd.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ukd.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ibx.yongpay.top

[Q15] 查询全部
来源：http://khx.shanyushiyangtech.top

SELECT * FROM users;
来源：http://kih.52xcode.cn

[Q16] 查询指定列
来源：http://cnh.ppjwa.cn

SELECT id, name FROM users;
来源：http://cty.guannengcc.top

[Q17] 条件查询
来源：http://nkt.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iff.gzhubu.top

[Q18] 模糊匹配
来源：http://oze.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iut.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://hed.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rca.yanxiufei.cn

[Q20] IN 列表
来源：http://imf.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wwg.cdnleiting.top

[Q21] 空值判断
来源：http://fhs.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vny.daria6918.cn

[Q22] 排序
来源：http://oxs.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zeg.ydzc1.top

[Q23] 分页
来源：http://akb.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gha.ydzc1.top

[Q24] 去重
来源：http://ybo.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://zbd.pycfn.com

[Q25] 只取前 N 条
来源：http://umx.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ecy.smart0.xyz

[Q26] 计数
来源：http://rto.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://aar.nanxuanxn.top

[Q27] 条件计数
来源：http://lpr.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uac.fzhhl.top

[Q28] 求和与平均
来源：http://cse.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kvo.daria6918.cn

[Q29] 最大最小值
来源：http://vbx.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wfm.shzxlz.cn

[Q30] 分组统计
来源：http://zbl.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bct.gzhubu.top

[Q31] 分组后过滤
来源：http://jxw.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bou.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://wdw.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tai.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gyb.sxryk.cn

[Q33] 多列分组
来源：http://qup.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tvc.pycfn.com

[Q34] 每组取第一条
来源：http://kfn.pengpengdd.cyou

SELECT * FROM (
来源：http://ymn.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bzh.hfpthk.cn

) t WHERE rn = 1;
来源：http://ylo.tian-w.cn

[Q35] 内连接
来源：http://yfw.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pma.bbcook.cn

[Q36] 左连接
来源：http://tng.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vxm.yvedp.cn

[Q37] 右连接
来源：http://oav.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qdd.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fzm.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qeu.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://oua.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://haq.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rhv.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kcz.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vma.quarkkingdee.top

[Q41] 多表连接
来源：http://xku.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsc.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://nhd.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://yxx.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://jme.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://tei.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mxt.chenzaomai.com

[Q43] 标量子查询
来源：http://vyx.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iqq.ydzc1.top

[Q44] IN 子查询
来源：http://jvz.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zan.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://olm.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://llt.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gva.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bhm.52xcode.cn

[Q47] 与平均值比较
来源：http://ntk.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mgy.sweek.top

[Q48] CTE 公用表表达式
来源：http://kqs.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dad.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://thm.nanxuanxn.top

[Q49] 更新单行
来源：http://jif.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vaf.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://vwn.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hpr.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://nca.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://syw.jqgufenzy.top

[Q52] 删除指定行
来源：http://trk.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://gvb.yangfankeji.com

[Q53] 按条件删除
来源：http://vxq.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fnj.xuanzx.com

[Q54] 清空表
来源：http://fof.xinyue.icu

TRUNCATE TABLE logs;
来源：http://jxk.redwolf501.top

[Q55] 排名（并列占位）
来源：http://fab.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jvt.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://bkb.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ysf.zhixingplan.top

[Q57] 行号
来源：http://sqc.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bxr.aizwys.cn

[Q58] 累计求和
来源：http://yst.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mwc.smart0.xyz

[Q59] 分组内累计
来源：http://yrp.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ahw.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://lqe.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gqf.shanyushiyangtech.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ert.shangyingyoupin.top

[Q61] 移动平均
来源：http://jhm.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oyr.xinyue.icu

[Q62] 分组占比
来源：http://pcb.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gmw.tianlin.xyz

[Q63] 开启事务
来源：http://pyf.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zdh.fktsv.cn

[Q64] 提交事务
来源：http://pqq.yj20258.top

COMMIT;
来源：http://aaz.cheryme.top

[Q65] 回滚事务
来源：http://gql.gzhubu.top

ROLLBACK;
来源：http://mib.sufxvd.cn

[Q66] 行锁查询
来源：http://jpq.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eel.jqgfzy.top

[Q67] 设置隔离级别
来源：http://ozv.yonumen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ezv.fanxiaobao.xyz

[Q68] 保存点
来源：http://idf.gotoacloud.top

SAVEPOINT sp1;
来源：http://oil.xinyue.icu

ROLLBACK TO sp1;
来源：http://wpd.jlsjyb.cn

[Q69] 查看执行计划
来源：http://wqf.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ivv.jyoumei.cn

[Q70] 更新统计信息
来源：http://rvu.yonumen.top

ANALYZE TABLE users;
来源：http://vdg.havefunace.top

[Q71] 查看建表语句
来源：http://jft.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bnb.jinghuilouyu.cn

[Q72] 查看索引
来源：http://xba.daria6918.cn

SHOW INDEX FROM users;
来源：http://lox.snrcjt.cn

[Q73] 查看表状态
来源：http://pqs.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nzr.yvedp.cn

[Q74] 强制使用索引
来源：http://tmk.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fxs.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://xdk.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xxx.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ots.jinqigfzy.top

[Q76] 按天统计
来源：http://zkz.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://djy.chenjidiqi.icu

[Q77] 时间加减
来源：http://gjb.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://edd.fehbvm.com

[Q78] 当前时间
来源：http://exk.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://amx.yj20258888.top

[Q79] 字符串拼接
来源：http://csq.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rps.cheryme.top


<!-- 参考信息 -->