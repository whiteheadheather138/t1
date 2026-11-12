代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://twv.xziqi.cn

Go:   go f()
来源：http://cnr.zdbjq.cn

Ruby: Thread.new { f }
来源：http://opo.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://nvt.svipenyu.cn

[O02] 使用线程池
来源：http://wyv.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xwc.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://adq.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://uop.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://uap.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://pdf.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://exq.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yfy.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gil.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://wsf.c1oappe.top

Py:   with lock: shared += 1
来源：http://fah.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://ylv.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xdd.zycfv.cn

TS:   // 同 JS
来源：http://wkq.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://uqz.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://csx.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://obe.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://qtk.nwbrower.top

[O04] 定义异步函数并等待
来源：http://lff.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://qjc.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eoo.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://crq.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qxp.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uet.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://unv.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://azy.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://rtw.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://ujs.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://sdw.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oxk.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://jcx.pycfn.com

TS:   await Promise.all(tasks)
来源：http://rwi.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mjj.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iiy.xziqi.cn

Ruby: threads.map(&:join)
来源：http://ird.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nsy.fzhhl.top

[O06] 使用进程池
来源：http://rgc.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvv.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sxt.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://wcz.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://wmr.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://frf.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lvu.nwbrower.top

Ruby: // fork 块
来源：http://rxt.sxryk.cn

C#:   Parallel.For
来源：http://bas.chenzaomai.com

================================================================================
来源：http://qhn.snrcjt.cn

P. 常用工具函数
来源：http://cec.aibaodan.cn

================================================================================
来源：http://uka.gotoacloud.top

[P01] 生成 UUID
来源：http://vop.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://uui.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zuq.yj20258.top

JS:   crypto.randomUUID()
来源：http://pbg.316326.xyz

TS:   crypto.randomUUID()
来源：http://nzo.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://nmb.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://pva.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://yhd.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://sjt.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://bsn.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fea.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mmq.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zaq.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ibg.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ccq.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ltq.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nqx.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xeq.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://bvw.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fel.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kcl.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yhn.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oqm.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gpv.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://min.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bbb.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fwi.ydjk.org.cn

[P04] 求长度
来源：http://bam.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nkc.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgl.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gxb.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fjx.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://sfr.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://utj.yangfankeji.com

Ruby: x.length;  x.size
来源：http://iwz.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qbn.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://lnf.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kro.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ktn.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nhs.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tti.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pmt.fehbvm.com

Go:   reflect.DeepEqual(a, b)
来源：http://ylq.zhaomingkeji.xyz

Ruby: a == b
来源：http://lay.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xke.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hyc.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qyg.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://tqg.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kpb.epnwcf.com

TS:   if (x == null) {}
来源：http://dlr.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pkh.feifeiyinyue.top

Go:   if x == nil {}
来源：http://ghy.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oxk.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://wcf.ctjpmb.com

[P07] 防抖与节流
来源：http://pnc.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hob.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://hrn.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kqr.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zok.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hgc.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jeq.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ttb.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gfw.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://whe.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://spa.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://akh.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqv.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lle.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xde.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eou.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gyc.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wmf.9152youxi.cn

================================================================================
来源：http://qej.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tie.ybcxt.top

================================================================================
来源：http://jpm.uphjek.com

[Q01] 创建表
来源：http://wox.birdmap.top

CREATE TABLE users (
来源：http://vbo.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rrm.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://beu.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://eoa.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bcj.ppjwa.cn

);
来源：http://css.andypj.xyz

[Q02] 创建带外键的表
来源：http://hdm.epnwcf.com

CREATE TABLE orders (
来源：http://ooh.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://owx.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://wgh.yfazqb.com

amount DECIMAL(10, 2),
来源：http://gtm.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zyi.pengpengdd.cyou

);
来源：http://uvm.xuanzx.com

[Q03] 增加列
来源：http://yiz.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://woq.yangfankeji.com

[Q04] 修改列类型
来源：http://wle.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cnn.tarul.cn

[Q05] 重命名列
来源：http://wsq.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fva.yj202588.top

[Q06] 删除列
来源：http://ueh.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gza.sufxvd.cn

[Q07] 删除表
来源：http://nof.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://iyq.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://laa.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gkl.meibo888.top

[Q09] 创建唯一索引
来源：http://vlt.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jak.smart0.xyz

[Q10] 插入单行
来源：http://uqc.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://avk.fzhhl.top

[Q11] 一次插入多行
来源：http://zks.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qoo.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://bbu.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://ras.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ygk.gzhubu.top

[Q13] 忽略重复插入
来源：http://rlx.pengpengdd.cyou

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wks.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://rbe.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pbi.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kok.9152youxi.cn

[Q15] 查询全部
来源：http://wdf.cdnleiting.top

SELECT * FROM users;
来源：http://nsy.jiagoushi.top

[Q16] 查询指定列
来源：http://bxu.zycfv.cn

SELECT id, name FROM users;
来源：http://wgc.nanxuanxn.top

[Q17] 条件查询
来源：http://iro.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hrh.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://nsl.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xbf.chenjidiqi.icu

[Q19] 范围查询
来源：http://yni.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://inp.jyoumei.cn

[Q20] IN 列表
来源：http://nxr.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wfi.shangyingyoupin.top

[Q21] 空值判断
来源：http://syj.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ewl.vqdsnc.cn

[Q22] 排序
来源：http://xlm.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zzd.tian-w.cn

[Q23] 分页
来源：http://tfa.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vvw.cdnleiting.top

[Q24] 去重
来源：http://xmf.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://nsy.dianchejie.cn

[Q25] 只取前 N 条
来源：http://wuz.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iyw.zhaomingkeji.xyz

[Q26] 计数
来源：http://cwd.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://mzc.fehbvm.com

[Q27] 条件计数
来源：http://fyi.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vhk.zhoulong.xyz

[Q28] 求和与平均
来源：http://grc.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pcs.9152youxi.cn

[Q29] 最大最小值
来源：http://itj.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://msa.birdmap.top

[Q30] 分组统计
来源：http://mqv.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tlc.ydzc1.top

[Q31] 分组后过滤
来源：http://zlc.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dbu.wangdashe.top

[Q32] 分组拼接字符串
来源：http://ton.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://onk.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cwt.gotoacloud.top

[Q33] 多列分组
来源：http://ucg.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wov.jiagoushi.top

[Q34] 每组取第一条
来源：http://bqj.zdqjudy.top

SELECT * FROM (
来源：http://jgt.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iua.ydzc1.top

) t WHERE rn = 1;
来源：http://dlo.hesvh.cn

[Q35] 内连接
来源：http://apu.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ogs.shzxlz.cn

[Q36] 左连接
来源：http://etq.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://enu.hfpthk.cn

[Q37] 右连接
来源：http://iby.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jui.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://mlg.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tsz.jlsjyb.cn

[Q39] 自连接（查上下级）
来源：http://dvu.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gpj.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wgn.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yos.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hqz.gaohongyu789.top

[Q41] 多表连接
来源：http://uon.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://lwo.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://aak.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://eta.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://yqr.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://zno.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tgb.tian-w.cn

[Q43] 标量子查询
来源：http://wyl.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gid.ehwqpu.com

[Q44] IN 子查询
来源：http://oku.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tkz.cheryme.top

[Q45] EXISTS 判断存在
来源：http://jkc.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zeh.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://jeh.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zfv.jqgufenzy.top

[Q47] 与平均值比较
来源：http://gqa.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ooi.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://vhn.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zee.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://ywo.vehdjk.com

[Q49] 更新单行
来源：http://yyx.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gla.daxiang520.top

[Q50] 批量更新
来源：http://aev.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://agn.smart0.xyz

[Q51] 用子查询更新
来源：http://cts.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://olx.cheryme.top

[Q52] 删除指定行
来源：http://sth.sufxvd.cn

DELETE FROM users WHERE id = 10;
来源：http://gbz.haohaochexian.top

[Q53] 按条件删除
来源：http://ujh.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sok.jiagoushi.top

[Q54] 清空表
来源：http://nqx.shuidangran.top

TRUNCATE TABLE logs;
来源：http://vet.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://inq.xingfuxueyuan.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tfn.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://htg.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ikr.ydzc1.top

[Q57] 行号
来源：http://rox.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vce.52xcode.cn

[Q58] 累计求和
来源：http://oms.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jxz.zdbjq.cn

[Q59] 分组内累计
来源：http://wqs.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xtg.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://omu.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oem.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wyj.zhongyouzk.top

[Q61] 移动平均
来源：http://vfd.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://clx.zdbjq.cn

[Q62] 分组占比
来源：http://fkb.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bkq.hfpthk.cn

[Q63] 开启事务
来源：http://yfa.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bdr.cucudq.cn

[Q64] 提交事务
来源：http://jta.ppjwa.cn

COMMIT;
来源：http://ojk.xuetiantiany.cn

[Q65] 回滚事务
来源：http://qey.bjfxy.top

ROLLBACK;
来源：http://ngv.zhiwuduotai.top

[Q66] 行锁查询
来源：http://tgo.mhx1999.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://puq.tianlin.xyz

[Q67] 设置隔离级别
来源：http://faf.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dvw.shangyingyoupin.top

[Q68] 保存点
来源：http://mvj.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://unk.hysaishi.cn

ROLLBACK TO sp1;
来源：http://yle.bbcook.cn

[Q69] 查看执行计划
来源：http://qyj.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cda.hnqzz.top

[Q70] 更新统计信息
来源：http://ywj.nwbrower.top

ANALYZE TABLE users;
来源：http://bvl.nwbrower.top

[Q71] 查看建表语句
来源：http://ojj.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cmp.hnxiangtu.top

[Q72] 查看索引
来源：http://yfl.sufxvd.cn

SHOW INDEX FROM users;
来源：http://igt.chenlongwang.top

[Q73] 查看表状态
来源：http://rgn.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rjg.yangfankeji.com

[Q74] 强制使用索引
来源：http://oyz.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uly.yonumen.top

[Q75] 日期格式化
来源：http://ghu.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gjb.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://prj.hfpthk.cn


<!-- 参考信息 -->