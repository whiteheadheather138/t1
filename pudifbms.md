代发 wailian999

================================================================================
来源：http://rjn.chenjidiqi.icu

O. 并发与异步
来源：http://kax.hnxiangtu.top

================================================================================
来源：http://tph.yj202588.top

[O01] 启动一个线程
来源：http://yur.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zbd.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ntg.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ceb.zhiwuduotai.top

TS:   // 同 JS
来源：http://vhe.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://cjk.xuetiantiany.cn

Go:   go f()
来源：http://wtz.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://yaz.316326.xyz

C#:   Task.Run(() => F());
来源：http://gga.sjlbkw.cn

[O02] 使用线程池
来源：http://bdy.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vsc.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://htp.cashguo.top

JS:   // worker_threads 线程池
来源：http://bva.guannengcc.top

TS:   // worker_threads 线程池
来源：http://gyw.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://gnj.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jec.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mit.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dqo.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://dly.daxiang520.top

Py:   with lock: shared += 1
来源：http://dvs.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://uwi.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gmi.shzxlz.cn

TS:   // 同 JS
来源：http://huy.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://xxx.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nsz.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qmy.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://chf.meibo888.top

[O04] 定义异步函数并等待
来源：http://xfc.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://ibk.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gbs.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://azz.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fec.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kjm.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fex.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ryw.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://wzb.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://xka.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://lgf.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ffi.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://rvj.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://nmw.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tdh.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bwy.xziqi.cn

Ruby: threads.map(&:join)
来源：http://afs.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jou.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://gci.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xci.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gtu.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://bqh.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://uou.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://acc.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xnq.shangyingyoupin.top

Ruby: // fork 块
来源：http://adk.nwbrower.top

C#:   Parallel.For
来源：http://alh.hammf.cn

================================================================================
来源：http://ayk.hnqzz.top

P. 常用工具函数
来源：http://uju.sweek.top

================================================================================
来源：http://ymo.bjfxy.top

[P01] 生成 UUID
来源：http://sce.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://dtw.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xse.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://wqg.fehbvm.com

TS:   crypto.randomUUID()
来源：http://okr.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://mzb.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://khr.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://oxt.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://nqo.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://kpg.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://esw.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://upl.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pgr.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lzf.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lkr.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ulf.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zkp.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gmq.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://wwx.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pqc.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vbq.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekh.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bet.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hgp.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lmd.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://yvm.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ipo.sjlbkw.cn

[P04] 求长度
来源：http://sxl.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rsd.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xcx.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jry.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jxd.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://egr.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://zux.mhx1999.top

Ruby: x.length;  x.size
来源：http://jyq.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fxd.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://mfu.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://tjz.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vqj.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rnp.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hgn.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kwn.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://wlq.ydjk.org.cn

Ruby: a == b
来源：http://jvu.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fmu.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://izr.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ytw.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://uvg.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xuk.fzhhl.top

TS:   if (x == null) {}
来源：http://bbp.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mdu.cdnleiting.top

Go:   if x == nil {}
来源：http://qvn.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ria.ydzc1.top

C#:   if (x is null) {}
来源：http://jhn.meibo888.top

[P07] 防抖与节流
来源：http://lpx.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zdf.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://cga.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycs.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbs.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eqo.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jqh.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qjc.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://psa.cucudq.cn

[P08] 处理浮点精度问题
来源：http://kct.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vkl.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vnv.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xsh.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wlh.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://itk.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ltj.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gqy.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tkf.yj20258.top

================================================================================
来源：http://zqi.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://skw.dianchejie.cn

================================================================================
来源：http://udk.shanyushiyangtech.top

[Q01] 创建表
来源：http://hpe.sxryk.cn

CREATE TABLE users (
来源：http://tlw.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://psf.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://htq.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://zwj.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zid.fanxiaobao.xyz

);
来源：http://qdc.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://dhf.yongpay.top

CREATE TABLE orders (
来源：http://xik.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://czq.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://pgj.shzxlz.cn

amount DECIMAL(10, 2),
来源：http://ohm.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nme.hnxiangtu.top

);
来源：http://eiz.redwolf501.top

[Q03] 增加列
来源：http://mhn.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tpj.zhijiandao.cn

[Q04] 修改列类型
来源：http://vvu.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ezo.daxiang520.top

[Q05] 重命名列
来源：http://hfm.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://usw.yonumen.top

[Q06] 删除列
来源：http://hpx.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://fal.feifeiyinyue.top

[Q07] 删除表
来源：http://rhw.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://yem.zhengqikj.top

[Q08] 创建普通索引
来源：http://hhz.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://frq.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://ypi.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wav.birdmap.top

[Q10] 插入单行
来源：http://tyx.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://flz.ctjpmb.com

[Q11] 一次插入多行
来源：http://aaq.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hgu.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://zcd.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bcb.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vqi.zhengqikj.top

[Q13] 忽略重复插入
来源：http://lpv.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xsm.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://uct.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xjv.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cel.jinqigfzy.top

[Q15] 查询全部
来源：http://ljc.hammf.cn

SELECT * FROM users;
来源：http://itj.ydzc1.top

[Q16] 查询指定列
来源：http://mac.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://sie.wangdashe.top

[Q17] 条件查询
来源：http://gzr.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rpr.hnxiangtu.top

[Q18] 模糊匹配
来源：http://dmr.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ahq.pycfn.com

[Q19] 范围查询
来源：http://azl.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvb.daria6918.cn

[Q20] IN 列表
来源：http://gnt.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xwr.guannengcc.top

[Q21] 空值判断
来源：http://blb.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iqa.kuanghao11.cn

[Q22] 排序
来源：http://plt.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dqw.wangdashe.top

[Q23] 分页
来源：http://rxp.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xmv.zhixingplan.top

[Q24] 去重
来源：http://abo.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://uyx.aizwys.cn

[Q25] 只取前 N 条
来源：http://ekx.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pha.cqqwz.cn

[Q26] 计数
来源：http://wom.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://omm.smart0.xyz

[Q27] 条件计数
来源：http://kos.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hvl.mhx1999.top

[Q28] 求和与平均
来源：http://oic.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ybz.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://cyd.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ioy.hywenlv.cn

[Q30] 分组统计
来源：http://jbl.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pwk.ivvv.top

[Q31] 分组后过滤
来源：http://tuc.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aww.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://vot.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ijr.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jme.daria6918.cn

[Q33] 多列分组
来源：http://hiw.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dcc.zhongyouzk.top

[Q34] 每组取第一条
来源：http://uuv.xuetiantiany.cn

SELECT * FROM (
来源：http://pwa.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rek.vehdjk.com

) t WHERE rn = 1;
来源：http://ige.nanxinkj.top

[Q35] 内连接
来源：http://nbw.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dtr.yfazqb.com

[Q36] 左连接
来源：http://dvr.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gmb.zhijiandao.cn

[Q37] 右连接
来源：http://bol.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nhv.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hah.sjlbkw.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eiu.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://xch.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eut.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qep.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rsl.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tud.fanxiaobao.xyz

[Q41] 多表连接
来源：http://dap.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wtr.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://ami.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://fhj.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://tyl.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://nxk.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ksi.52xcode.cn

[Q43] 标量子查询
来源：http://skm.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://swy.yuxming.cn

[Q44] IN 子查询
来源：http://kmc.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jxb.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://pki.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gjr.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rbz.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nux.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://pkh.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uic.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://hqt.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yoe.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://wnq.zhixingplan.top

[Q49] 更新单行
来源：http://sbe.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oiq.ppjwa.cn

[Q50] 批量更新
来源：http://lad.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zyg.mhx1999.top

[Q51] 用子查询更新
来源：http://vqg.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ohj.zycfv.cn

[Q52] 删除指定行
来源：http://ydq.tianlin.xyz

DELETE FROM users WHERE id = 10;
来源：http://bfn.sweek.top

[Q53] 按条件删除
来源：http://mrg.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://suc.xingfuxueyuan.xyz

[Q54] 清空表
来源：http://vdq.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://kju.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://pmj.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yqz.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://eih.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sjo.xingfuxueyuan.xyz

[Q57] 行号
来源：http://dci.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://msi.gaohongyu789.top

[Q58] 累计求和
来源：http://wbz.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ryj.ydzc1.top

[Q59] 分组内累计
来源：http://thm.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cdm.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://ybb.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ahr.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://orh.jqgufenzy.top

[Q61] 移动平均
来源：http://gjj.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pdi.fktsv.cn

[Q62] 分组占比
来源：http://tbh.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nln.yonumen.top

[Q63] 开启事务
来源：http://aoy.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://get.pycfn.com

[Q64] 提交事务
来源：http://qck.fktsv.cn

COMMIT;
来源：http://jgy.pengpengdd.cyou

[Q65] 回滚事务
来源：http://ndy.tanke756.top

ROLLBACK;
来源：http://sjn.wangshuangyany.cn

[Q66] 行锁查询
来源：http://fur.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eve.fengsongda.top

[Q67] 设置隔离级别
来源：http://lps.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mer.vqdsnc.cn

[Q68] 保存点
来源：http://vpf.ehwqpu.com

SAVEPOINT sp1;
来源：http://vmm.birdmap.top

ROLLBACK TO sp1;
来源：http://uzd.zhoulong.xyz

[Q69] 查看执行计划
来源：http://dns.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hgw.yj202588.top

[Q70] 更新统计信息
来源：http://joi.yfazqb.com

ANALYZE TABLE users;
来源：http://zra.hnqzz.top

[Q71] 查看建表语句
来源：http://vnt.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fxg.zdqjudy.top

[Q72] 查看索引
来源：http://ifu.jinghuilouyu.cn


<!-- 参考信息 -->