代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rmb.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tem.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bav.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejb.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sqp.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bou.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hxg.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rvk.wangshuangyany.cn

================================================================================
来源：http://ksh.ppjwa.cn

O. 并发与异步
来源：http://yye.wangdashe.top

================================================================================
来源：http://pxz.yongpay.top

[O01] 启动一个线程
来源：http://wjh.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fpv.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qgn.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hfb.hfpthk.cn

TS:   // 同 JS
来源：http://mff.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://fxh.gaohongyu789.top

Go:   go f()
来源：http://yui.shuidangran.top

Ruby: Thread.new { f }
来源：http://efl.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://pww.zhoulong.xyz

[O02] 使用线程池
来源：http://tlm.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gnc.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uac.yvedp.cn

JS:   // worker_threads 线程池
来源：http://gwp.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://vrn.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://brw.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rcd.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ptp.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://grk.jianghu66.top

[O03] 加锁保护共享数据
来源：http://ums.havefunace.top

Py:   with lock: shared += 1
来源：http://vrk.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://bvt.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xqi.cheryme.top

TS:   // 同 JS
来源：http://cfx.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://aax.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fom.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fww.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://ccs.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://zxr.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://fpz.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://unc.hammf.cn

JS:   async function f() { await g(); }
来源：http://bll.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bsp.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dxm.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rhr.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ipi.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://fsh.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://dub.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://kkr.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aik.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://atd.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://rlc.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jll.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://snw.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://hbv.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kcj.wangshuangyany.cn

[O06] 使用进程池
来源：http://egy.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qss.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://unt.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://kjq.yj20258.top

TS:   // child_process / cluster 模块
来源：http://syx.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mwe.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vel.hesvh.cn

Ruby: // fork 块
来源：http://hli.cucudq.cn

C#:   Parallel.For
来源：http://ihu.jinyuanbaomall.cn

================================================================================
来源：http://jjn.ctjpmb.com

P. 常用工具函数
来源：http://vrr.nanxinkj.top

================================================================================
来源：http://drk.gotoacloud.top

[P01] 生成 UUID
来源：http://eav.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://wui.shanyushiyangtech.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://isq.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://eof.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://kme.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://wde.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://gyc.birdmap.top

Ruby: SecureRandom.uuid
来源：http://ujc.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://vha.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://ldq.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vdk.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ggd.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hmk.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rnd.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wak.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vfm.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dgu.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://obp.shuidangran.top

[P03] 生成短随机字符串
来源：http://snq.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iej.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qto.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vgc.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aia.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xyu.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kzx.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sye.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://amj.shanyushiyangkeji.top

[P04] 求长度
来源：http://nwi.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pus.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jim.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jpt.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kjn.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://ypi.cashguo.top

Go:   len(arr);  len(m)
来源：http://bgw.gogol.net.cn

Ruby: x.length;  x.size
来源：http://qkh.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gyq.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://zmh.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mej.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zzr.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zsd.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ebg.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pvf.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://jlq.sysykeji.top

Ruby: a == b
来源：http://uxk.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wfp.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pcu.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xrx.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://slu.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jlj.zdbjq.cn

TS:   if (x == null) {}
来源：http://lrt.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://qih.yonumen.top

Go:   if x == nil {}
来源：http://gto.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wjm.cqqwz.cn

C#:   if (x is null) {}
来源：http://alh.iojbl.cn

[P07] 防抖与节流
来源：http://zss.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oyr.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://nyp.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyv.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nob.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lqq.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iyy.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jqj.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lka.tian-w.cn

[P08] 处理浮点精度问题
来源：http://zbo.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cor.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://byx.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dcq.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://djr.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://irn.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yuo.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aui.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cdd.shanyushiyangtech.top

================================================================================
来源：http://cfj.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://usr.epnwcf.com

================================================================================
来源：http://gkt.hammf.cn

[Q01] 创建表
来源：http://aac.ybcxt.top

CREATE TABLE users (
来源：http://nwj.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qdb.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://cxo.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://prl.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://esp.jinqigufen.top

);
来源：http://xel.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://cfw.gogol.net.cn

CREATE TABLE orders (
来源：http://ecq.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uou.sysykeji.top

user_id INT NOT NULL,
来源：http://fpr.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://fcv.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://abf.fengsongda.top

);
来源：http://hwf.svipenyu.cn

[Q03] 增加列
来源：http://enw.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sul.iojbl.cn

[Q04] 修改列类型
来源：http://mzz.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fdg.pycfn.com

[Q05] 重命名列
来源：http://xmf.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zez.zycfv.cn

[Q06] 删除列
来源：http://yed.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fpa.jqgufenzy.top

[Q07] 删除表
来源：http://cpk.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://obi.yfazqb.com

[Q08] 创建普通索引
来源：http://qqy.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://rfg.zhixingplan.top

[Q09] 创建唯一索引
来源：http://ymu.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oqm.c1oappe.top

[Q10] 插入单行
来源：http://fsj.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gru.cqqwz.cn

[Q11] 一次插入多行
来源：http://kxi.hywenlv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://doc.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://nbt.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://dij.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qcl.ydzc1.top

[Q13] 忽略重复插入
来源：http://uxb.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://duz.tianlin.xyz

[Q14] 存在则更新（upsert）
来源：http://zyr.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kze.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pqn.uphjek.com

[Q15] 查询全部
来源：http://wbq.yueranfly.top

SELECT * FROM users;
来源：http://zax.sxryk.cn

[Q16] 查询指定列
来源：http://vkc.vqdsnc.cn

SELECT id, name FROM users;
来源：http://fvy.yongpay.top

[Q17] 条件查询
来源：http://bhi.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uon.daxiang520.top

[Q18] 模糊匹配
来源：http://qlv.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pek.jinqigfzy.top

[Q19] 范围查询
来源：http://alo.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://phf.zhoulong.xyz

[Q20] IN 列表
来源：http://eji.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ffm.smart0.xyz

[Q21] 空值判断
来源：http://itc.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dka.yj20258888.top

[Q22] 排序
来源：http://ugf.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fxo.fanxiaobao.xyz

[Q23] 分页
来源：http://rjs.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vyh.hysaishi.cn

[Q24] 去重
来源：http://kyz.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://xyj.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://hrz.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vso.chenjidiqi.icu

[Q26] 计数
来源：http://nko.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://ptl.hnxiangtu.top

[Q27] 条件计数
来源：http://jks.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gea.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://bon.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ojg.gogol.net.cn

[Q29] 最大最小值
来源：http://qwj.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kjl.ydjk.org.cn

[Q30] 分组统计
来源：http://sfi.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jlo.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://dqv.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rfr.vehdjk.com

[Q32] 分组拼接字符串
来源：http://kus.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cdt.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jvi.fengsongda.top

[Q33] 多列分组
来源：http://xdo.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ogt.mhx1999.top

[Q34] 每组取第一条
来源：http://eyo.zhixingplan.top

SELECT * FROM (
来源：http://wtb.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bgl.fktsv.cn

) t WHERE rn = 1;
来源：http://iqb.zdbjq.cn

[Q35] 内连接
来源：http://hii.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yns.ydjk.org.cn

[Q36] 左连接
来源：http://gtk.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fdf.yuanzhike.top

[Q37] 右连接
来源：http://hex.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://udt.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://blo.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kjb.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://aee.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uup.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lev.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://twx.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lvb.pycfn.com

[Q41] 多表连接
来源：http://wgv.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ucu.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://jta.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://dms.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://vvd.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://qvx.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mda.sjlbkw.cn

[Q43] 标量子查询
来源：http://mgk.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xxa.vqdsnc.cn

[Q44] IN 子查询
来源：http://llf.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tih.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://fvk.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vcw.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://plq.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osi.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://bzs.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iol.hammf.cn

[Q48] CTE 公用表表达式
来源：http://svy.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dni.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://xiy.cashguo.top

[Q49] 更新单行
来源：http://mok.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://atd.xuanzx.com

[Q50] 批量更新
来源：http://htw.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xyo.vqdsnc.cn

[Q51] 用子查询更新
来源：http://xxw.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ryq.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://qzp.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://roy.andypj.xyz

[Q53] 按条件删除
来源：http://hkr.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wxp.jyoumei.cn

[Q54] 清空表
来源：http://wau.ivvv.top

TRUNCATE TABLE logs;
来源：http://ktx.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://syo.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gpe.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://rde.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pfy.tian-w.cn

[Q57] 行号
来源：http://asj.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fhy.ctjpmb.com

[Q58] 累计求和
来源：http://ocz.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zhm.chenzaomai.com

[Q59] 分组内累计
来源：http://mng.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vnz.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://rwf.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ybi.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rmc.hnxiangtu.top

[Q61] 移动平均
来源：http://pao.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://luw.nanxuanxn.top

[Q62] 分组占比
来源：http://cyo.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xno.svipenyu.cn

[Q63] 开启事务
来源：http://ofh.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dqq.hammf.cn

[Q64] 提交事务
来源：http://fqc.cdnleiting.top

COMMIT;
来源：http://aqr.9152youxi.cn

[Q65] 回滚事务
来源：http://hpu.shanyushiyangkeji.top

ROLLBACK;
来源：http://otx.dianchejie.cn

[Q66] 行锁查询
来源：http://kfd.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nfn.iojbl.cn

[Q67] 设置隔离级别
来源：http://egt.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jgh.vehdjk.com

[Q68] 保存点
来源：http://byf.yueranfly.top

SAVEPOINT sp1;
来源：http://atb.guannengcc.top


<!-- 参考信息 -->