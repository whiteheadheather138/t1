代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sjk.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jar.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hlb.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zqa.aibaodan.cn

================================================================================
来源：http://jsq.guannengcc.top

O. 并发与异步
来源：http://qld.wangdashe.top

================================================================================
来源：http://nih.zdqjudy.top

[O01] 启动一个线程
来源：http://kpv.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tzv.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xns.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vkd.aibaodan.cn

TS:   // 同 JS
来源：http://uzo.sweek.top

Java: new Thread(() -> f()).start()
来源：http://rca.gogol.net.cn

Go:   go f()
来源：http://tty.ctjpmb.com

Ruby: Thread.new { f }
来源：http://kqu.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://aky.snrcjt.cn

[O02] 使用线程池
来源：http://qss.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gid.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cqd.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://lav.yueranfly.top

TS:   // worker_threads 线程池
来源：http://zkv.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://klx.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yan.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dfk.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wyl.mhx1999.top

[O03] 加锁保护共享数据
来源：http://mmh.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://ksc.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://eiz.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mbd.ivvv.top

TS:   // 同 JS
来源：http://gbj.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://pxy.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nnw.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://muk.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://qsp.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://kkx.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://hoy.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dmf.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://usk.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xea.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kuw.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zid.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://mru.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://avk.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://zba.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://kxw.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rpb.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://jds.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://szp.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lvx.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fqu.hesvh.cn

Ruby: threads.map(&:join)
来源：http://dhh.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eag.fktsv.cn

[O06] 使用进程池
来源：http://uoj.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wav.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ljx.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://xje.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://xwi.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lds.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://owc.fehbvm.com

Ruby: // fork 块
来源：http://ner.sweek.top

C#:   Parallel.For
来源：http://ivz.52xcode.cn

================================================================================
来源：http://ptq.uphjek.com

P. 常用工具函数
来源：http://ijx.fehbvm.com

================================================================================
来源：http://mqf.andypj.xyz

[P01] 生成 UUID
来源：http://jqs.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://opf.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kxc.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://eag.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://luv.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://kwo.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://hyk.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://kma.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://xlg.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://xxh.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ges.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uws.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gve.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://atb.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dyg.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://awf.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wyj.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://thz.ppjwa.cn

[P03] 生成短随机字符串
来源：http://ilb.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ppu.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ckf.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvr.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cil.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bwt.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vvn.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wpp.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hug.hfpthk.cn

[P04] 求长度
来源：http://iau.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mff.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cuy.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wex.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urx.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://xqw.xinyue.icu

Go:   len(arr);  len(m)
来源：http://san.aibaodan.cn

Ruby: x.length;  x.size
来源：http://fgn.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xdd.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://coc.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vyp.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ccx.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sns.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gwx.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hsv.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://qru.svipenyu.cn

Ruby: a == b
来源：http://ypw.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nhx.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tga.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zbc.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://rab.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rii.ppjwa.cn

TS:   if (x == null) {}
来源：http://qaq.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://jnk.jlsjyb.cn

Go:   if x == nil {}
来源：http://yap.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ret.meibo888.top

C#:   if (x is null) {}
来源：http://jgd.dashuyun.cn

[P07] 防抖与节流
来源：http://irr.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://enr.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://hbs.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mlx.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgs.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://upu.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tkc.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uyw.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://apl.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://qcq.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fry.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uvv.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rvo.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bic.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://akm.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ita.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mzm.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eue.nanxinkj.top

================================================================================
来源：http://krl.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gwz.fanxiaobao.xyz

================================================================================
来源：http://pxd.feifeiyinyue.top

[Q01] 创建表
来源：http://tdi.52xcode.cn

CREATE TABLE users (
来源：http://tlm.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqm.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://amj.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://dnv.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://njz.yanxiufei.cn

);
来源：http://yam.bbcook.cn

[Q02] 创建带外键的表
来源：http://juj.smart0.xyz

CREATE TABLE orders (
来源：http://ceu.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://abl.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://mvw.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://fbi.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://upb.yonumen.top

);
来源：http://umt.sweek.top

[Q03] 增加列
来源：http://tja.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://khc.gotoacloud.top

[Q04] 修改列类型
来源：http://aij.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bze.aizwys.cn

[Q05] 重命名列
来源：http://njp.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ymc.ppjwa.cn

[Q06] 删除列
来源：http://jqv.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://fxe.sjlbkw.cn

[Q07] 删除表
来源：http://eov.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://lzf.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://vrv.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nic.iojbl.cn

[Q09] 创建唯一索引
来源：http://xfl.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gbj.ydjk.org.cn

[Q10] 插入单行
来源：http://qgp.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://idq.hammf.cn

[Q11] 一次插入多行
来源：http://gbs.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vnx.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://fpn.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://enr.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zan.haohaochexian.top

[Q13] 忽略重复插入
来源：http://eqh.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eqf.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://opl.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lyp.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fzt.yonumen.top

[Q15] 查询全部
来源：http://mpi.tanke756.top

SELECT * FROM users;
来源：http://esw.sweek.top

[Q16] 查询指定列
来源：http://feg.xuanzx.com

SELECT id, name FROM users;
来源：http://mvi.nanxuanxn.top

[Q17] 条件查询
来源：http://hxj.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iwv.sxryk.cn

[Q18] 模糊匹配
来源：http://clh.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://prx.yueranfly.top

[Q19] 范围查询
来源：http://cga.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ars.zdqjudy.top

[Q20] IN 列表
来源：http://jed.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://khn.hammf.cn

[Q21] 空值判断
来源：http://wlo.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fho.zhongyouzk.top

[Q22] 排序
来源：http://uul.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wzm.hfpthk.cn

[Q23] 分页
来源：http://lww.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lzh.quarkkingdee.top

[Q24] 去重
来源：http://zdu.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://ozz.shzxlz.cn

[Q25] 只取前 N 条
来源：http://psp.svipenyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eya.zhiwuduotai.top

[Q26] 计数
来源：http://ugs.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://zfs.ydzc1.top

[Q27] 条件计数
来源：http://mfy.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://efr.jqgfzy.top

[Q28] 求和与平均
来源：http://mml.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qts.yfazqb.com

[Q29] 最大最小值
来源：http://bvr.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wni.gzhubu.top

[Q30] 分组统计
来源：http://aiu.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uag.kuanghao11.cn

[Q31] 分组后过滤
来源：http://voj.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://exo.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://whf.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rih.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nfn.fengsongda.top

[Q33] 多列分组
来源：http://nqc.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hxt.hnqzz.top

[Q34] 每组取第一条
来源：http://cne.hfpthk.cn

SELECT * FROM (
来源：http://rhl.fanxiaobao.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qib.yangfankeji.com

) t WHERE rn = 1;
来源：http://awu.jiagoushi.top

[Q35] 内连接
来源：http://zvf.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dcv.xylfe.cn

[Q36] 左连接
来源：http://rye.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://auc.yvedp.cn

[Q37] 右连接
来源：http://yip.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://stb.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://izy.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fnk.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://ote.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xhs.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://idj.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://igb.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wgi.9152youxi.cn

[Q41] 多表连接
来源：http://iag.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://fpc.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://upl.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://asd.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://peb.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://yfn.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fxg.yongpay.top

[Q43] 标量子查询
来源：http://yxx.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gbe.daria6918.cn

[Q44] IN 子查询
来源：http://idy.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nfq.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://gjc.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwz.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://qam.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fxe.yfazqb.com

[Q47] 与平均值比较
来源：http://nrf.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pci.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://sml.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oin.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://erm.tanke756.top

[Q49] 更新单行
来源：http://tws.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vwa.jianghu66.top

[Q50] 批量更新
来源：http://mlb.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wst.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://qdd.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btq.gaohongyu789.top

[Q52] 删除指定行
来源：http://dbg.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://rek.ppjwa.cn

[Q53] 按条件删除
来源：http://tnq.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lny.jyoumei.cn

[Q54] 清空表
来源：http://qsv.ydzc1.top

TRUNCATE TABLE logs;
来源：http://ycc.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://afv.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dsi.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://kwh.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://acj.andypj.xyz

[Q57] 行号
来源：http://oua.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eat.hywenlv.cn

[Q58] 累计求和
来源：http://sgx.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wne.vqdsnc.cn

[Q59] 分组内累计
来源：http://xfk.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cor.sweek.top

[Q60] 取上一行 / 下一行
来源：http://iue.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fjh.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://alt.zhongyouzk.top

[Q61] 移动平均
来源：http://kkj.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oul.zdqjudy.top

[Q62] 分组占比
来源：http://zhn.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hif.fanxiaobao.xyz

[Q63] 开启事务
来源：http://idl.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gyz.jqgfzy.top

[Q64] 提交事务
来源：http://vhg.yuanzhike.top

COMMIT;
来源：http://wwb.fzhhl.top

[Q65] 回滚事务
来源：http://puc.0kj1m.cn

ROLLBACK;
来源：http://ayp.redwolf501.top

[Q66] 行锁查询
来源：http://csc.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fcw.fktsv.cn

[Q67] 设置隔离级别
来源：http://xdl.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kma.shanyushiyangtech.top

[Q68] 保存点
来源：http://sqc.jqgfzy.top

SAVEPOINT sp1;
来源：http://kkh.ehwqpu.com

ROLLBACK TO sp1;
来源：http://nqb.0kj1m.cn

[Q69] 查看执行计划
来源：http://ses.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zbu.ehwqpu.com

[Q70] 更新统计信息
来源：http://aka.epnwcf.com


<!-- 参考信息 -->