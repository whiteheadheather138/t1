代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yet.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zmf.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpe.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yss.xziqi.cn

================================================================================
来源：http://iro.hammf.cn

O. 并发与异步
来源：http://mkg.jinyuanbaomall.cn

================================================================================
来源：http://xpc.sysykeji.top

[O01] 启动一个线程
来源：http://mne.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mkb.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yqg.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mqc.dianchejie.cn

TS:   // 同 JS
来源：http://stp.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://htx.jinqigufen.top

Go:   go f()
来源：http://jgd.jiagoushi.top

Ruby: Thread.new { f }
来源：http://eyj.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://che.iojbl.cn

[O02] 使用线程池
来源：http://xev.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://orb.zhijiandao.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hxj.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://dsf.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://qnq.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uuc.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bpb.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fog.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wrt.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://hgv.cqqwz.cn

Py:   with lock: shared += 1
来源：http://qsh.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://iml.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lrz.dashuyun.cn

TS:   // 同 JS
来源：http://oup.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://wpv.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lvy.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qsf.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://bsx.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://kfb.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://yuv.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jls.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://uml.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://enx.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gfj.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ydo.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://teq.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://qcf.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://nma.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://cff.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rrq.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://hvt.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://ddf.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://adq.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwg.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://dmu.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://orx.shanyushiyangtech.top

[O06] 使用进程池
来源：http://nto.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zkp.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bpt.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://afx.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://zue.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hwx.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aam.hnqzz.top

Ruby: // fork 块
来源：http://yhn.xinyue.icu

C#:   Parallel.For
来源：http://gar.yonumen.top

================================================================================
来源：http://uns.haohaochexian.top

P. 常用工具函数
来源：http://gxt.hcnkem.com

================================================================================
来源：http://vuu.meibo888.top

[P01] 生成 UUID
来源：http://wjf.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://sun.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dvq.yongpay.top

JS:   crypto.randomUUID()
来源：http://bnh.sweek.top

TS:   crypto.randomUUID()
来源：http://fot.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://yqf.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://nvf.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://eyd.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://sgb.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://opk.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vbk.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oxk.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baw.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oev.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rcm.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ite.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qik.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://koa.cqqwz.cn

[P03] 生成短随机字符串
来源：http://zfl.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://seo.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xjr.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fhk.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bes.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hgf.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://grg.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pcf.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wmv.kuanghao11.cn

[P04] 求长度
来源：http://hmi.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://llk.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eld.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://exq.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytk.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://vxk.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://gjq.zdqjudy.top

Ruby: x.length;  x.size
来源：http://cpu.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aqq.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://tfv.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kiw.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bjr.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ddz.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fux.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rom.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://paa.0kj1m.cn

Ruby: a == b
来源：http://crn.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://arg.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://het.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uqq.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://glh.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gij.sysykeji.top

TS:   if (x == null) {}
来源：http://gsd.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qwn.dianchejie.cn

Go:   if x == nil {}
来源：http://sqj.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ult.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://aer.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://fcg.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fge.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://hfd.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbz.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgn.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://arc.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gsk.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nmv.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rzn.havefunace.top

[P08] 处理浮点精度问题
来源：http://rto.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lyp.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kmi.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bhf.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dvp.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://scv.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://voi.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rjh.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cgx.andypj.xyz

================================================================================
来源：http://sdm.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cqi.gaohongyu789.top

================================================================================
来源：http://hqc.yuxming.cn

[Q01] 创建表
来源：http://fan.yfazqb.com

CREATE TABLE users (
来源：http://ljr.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wqf.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://hqi.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://wad.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cmo.aibaodan.cn

);
来源：http://gdt.ybcxt.top

[Q02] 创建带外键的表
来源：http://gio.quarkkingdee.top

CREATE TABLE orders (
来源：http://mxx.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yec.smart0.xyz

user_id INT NOT NULL,
来源：http://vyz.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://kae.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dcb.xylfe.cn

);
来源：http://van.yueranfly.top

[Q03] 增加列
来源：http://zdd.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rkd.tianlin.xyz

[Q04] 修改列类型
来源：http://wmx.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://znk.havefunace.top

[Q05] 重命名列
来源：http://lzj.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://edb.guowangkeji.top

[Q06] 删除列
来源：http://bsi.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://iuq.smart0.xyz

[Q07] 删除表
来源：http://xuu.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://xdy.ybcxt.top

[Q08] 创建普通索引
来源：http://eld.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://som.birdmap.top

[Q09] 创建唯一索引
来源：http://mlv.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rut.ctjpmb.com

[Q10] 插入单行
来源：http://rvx.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gza.xziqi.cn

[Q11] 一次插入多行
来源：http://jhl.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dif.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://quo.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://idd.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://trd.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://wdf.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hxs.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://wse.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ctl.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://frb.jianghu66.top

[Q15] 查询全部
来源：http://slx.tanke756.top

SELECT * FROM users;
来源：http://oro.jiagoushi.top

[Q16] 查询指定列
来源：http://xcm.jinqigufen.top

SELECT id, name FROM users;
来源：http://kfe.fengsongda.top

[Q17] 条件查询
来源：http://zth.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vvt.epnwcf.com

[Q18] 模糊匹配
来源：http://cyc.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zyl.andypj.xyz

[Q19] 范围查询
来源：http://lpq.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jyb.ivvv.top

[Q20] IN 列表
来源：http://hao.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xkn.jqgufenzy.top

[Q21] 空值判断
来源：http://ygx.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kzg.chenjidiqi.icu

[Q22] 排序
来源：http://hco.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tsj.andypj.xyz

[Q23] 分页
来源：http://lny.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xcs.sysykeji.top

[Q24] 去重
来源：http://btz.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://gpf.sweek.top

[Q25] 只取前 N 条
来源：http://vva.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tsc.jinqigufen.top

[Q26] 计数
来源：http://dnt.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://ufw.zhongyouzk.top

[Q27] 条件计数
来源：http://ofp.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ofr.jianghu66.top

[Q28] 求和与平均
来源：http://bvi.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://znu.feifeiyinyue.top

[Q29] 最大最小值
来源：http://frr.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ijp.jqgfzy.top

[Q30] 分组统计
来源：http://fpe.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://plo.pycfn.com

[Q31] 分组后过滤
来源：http://kxl.yj202588.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kra.redwolf501.top

[Q32] 分组拼接字符串
来源：http://ujz.xingfuxueyuan.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kfc.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gzj.aizwys.cn

[Q33] 多列分组
来源：http://fly.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://inf.meibo888.top

[Q34] 每组取第一条
来源：http://fit.guowangkeji.top

SELECT * FROM (
来源：http://oel.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ibu.hnxiangtu.top

) t WHERE rn = 1;
来源：http://mdy.xinyue.icu

[Q35] 内连接
来源：http://wdv.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pvu.zhiwuduotai.top

[Q36] 左连接
来源：http://dmb.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://luq.pycfn.com

[Q37] 右连接
来源：http://cme.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dyg.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://dkm.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nwm.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://zda.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ijg.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zis.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pxq.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lhm.fzhhl.top

[Q41] 多表连接
来源：http://usp.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://diz.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://lax.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://taq.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://ckf.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://kzb.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aut.snrcjt.cn

[Q43] 标量子查询
来源：http://osf.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jtv.xinyue.icu

[Q44] IN 子查询
来源：http://jar.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ctf.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://cbd.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xtx.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://zib.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mrl.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://psf.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ndo.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://uel.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gfw.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://bom.ivvv.top

[Q49] 更新单行
来源：http://ztj.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://djf.tarul.cn

[Q50] 批量更新
来源：http://lzx.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jzr.jinqigfzy.top

[Q51] 用子查询更新
来源：http://vjp.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bbh.jqgufenzy.top

[Q52] 删除指定行
来源：http://tua.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://xan.yueranfly.top

[Q53] 按条件删除
来源：http://qlu.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mpw.vqdsnc.cn

[Q54] 清空表
来源：http://hvx.xylfe.cn

TRUNCATE TABLE logs;
来源：http://vps.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://ovl.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ikf.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://ejf.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wvc.sysykeji.top

[Q57] 行号
来源：http://vgm.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lzw.sufxvd.cn

[Q58] 累计求和
来源：http://hog.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vet.havefunace.top

[Q59] 分组内累计
来源：http://nub.guowangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wkn.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://ldv.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lmh.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ccy.nanxuanxn.top

[Q61] 移动平均
来源：http://ylz.fktsv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ypr.jianghu66.top

[Q62] 分组占比
来源：http://iwi.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://czl.cdnleiting.top

[Q63] 开启事务
来源：http://vrr.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bto.quarkkingdee.top

[Q64] 提交事务
来源：http://zzt.xziqi.cn

COMMIT;
来源：http://cbm.cucudq.cn

[Q65] 回滚事务
来源：http://yxi.vehdjk.com

ROLLBACK;
来源：http://tng.c1oappe.top

[Q66] 行锁查询
来源：http://pmb.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://agp.nwbrower.top

[Q67] 设置隔离级别
来源：http://uyf.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lzo.cqqwz.cn

[Q68] 保存点
来源：http://aqi.sysykeji.top

SAVEPOINT sp1;
来源：http://igh.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://sec.316326.xyz

[Q69] 查看执行计划
来源：http://qjh.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kjz.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://jst.zhongyouzk.top


<!-- 参考信息 -->