代发 wailian999

Go:   // 手写递归
来源：http://lik.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://azl.vehdjk.com

C#:   // 手写递归
来源：http://ewh.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qsh.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fmb.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vhw.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xie.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zru.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cqf.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ldo.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rgb.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mcx.fengsongda.top

================================================================================
来源：http://wkd.ctjpmb.com

O. 并发与异步
来源：http://hbv.ybcxt.top

================================================================================
来源：http://kjx.aibaodan.cn

[O01] 启动一个线程
来源：http://efk.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pub.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kaf.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://efu.hnqzz.top

TS:   // 同 JS
来源：http://kwg.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://gyn.guowangkeji.top

Go:   go f()
来源：http://hme.uphjek.com

Ruby: Thread.new { f }
来源：http://kre.xinyue.icu

C#:   Task.Run(() => F());
来源：http://kpy.zdqjudy.top

[O02] 使用线程池
来源：http://rah.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zib.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yvv.vehdjk.com

JS:   // worker_threads 线程池
来源：http://fwa.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://kdq.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://dqb.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ebb.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gex.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tpw.yj202588.top

[O03] 加锁保护共享数据
来源：http://ubr.jyoumei.cn

Py:   with lock: shared += 1
来源：http://zdy.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://xqm.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tij.hnqzz.top

TS:   // 同 JS
来源：http://gio.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://fxo.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qky.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hyi.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://fxw.ydzc1.top

[O04] 定义异步函数并等待
来源：http://jyw.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://zzy.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aqm.guannengcc.top

JS:   async function f() { await g(); }
来源：http://sxx.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://krl.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sji.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfp.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ion.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://ocm.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://plj.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://ywq.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tkc.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://bth.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://rui.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hxs.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ark.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://jpm.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ioq.fanxiaobao.xyz

[O06] 使用进程池
来源：http://cer.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ead.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://enw.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://kye.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://rug.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qiv.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lic.tarul.cn

Ruby: // fork 块
来源：http://nyb.316326.xyz

C#:   Parallel.For
来源：http://xml.daxiang520.top

================================================================================
来源：http://cws.sufxvd.cn

P. 常用工具函数
来源：http://mtk.yangfankeji.com

================================================================================
来源：http://vro.yueranfly.top

[P01] 生成 UUID
来源：http://zjr.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://qyy.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://msc.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://sum.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://qwk.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://jgv.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://xns.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://bau.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://lfk.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://les.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wci.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oau.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bse.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ape.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fwf.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nbr.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kin.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://brs.haohaochexian.top

[P03] 生成短随机字符串
来源：http://seh.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://umn.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ugc.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oiy.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ciq.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bif.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zby.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lhm.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://grx.sxryk.cn

[P04] 求长度
来源：http://csd.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yzb.yvedp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tzr.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gfb.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojm.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://fmn.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://zuv.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://rzh.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tem.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://ift.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jjg.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oyz.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yao.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kdx.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lfx.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://wkm.jinqigfzy.top

Ruby: a == b
来源：http://vva.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kmw.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dmh.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wnn.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://lpw.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://csp.andypj.xyz

TS:   if (x == null) {}
来源：http://wwl.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ymn.feifeiyinyue.top

Go:   if x == nil {}
来源：http://trg.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uzh.kuanghao11.cn

C#:   if (x is null) {}
来源：http://spn.cqqwz.cn

[P07] 防抖与节流
来源：http://vrm.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hym.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://ttg.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qpy.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpy.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zbq.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bkx.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://eqt.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ciq.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://rgs.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cun.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://upy.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ern.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xoq.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fiv.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zak.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://meo.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qyi.yvedp.cn

================================================================================
来源：http://aqw.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://frw.daxiang520.top

================================================================================
来源：http://qqc.quarkkingdee.top

[Q01] 创建表
来源：http://fii.zhiwuduotai.top

CREATE TABLE users (
来源：http://lse.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyu.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://wiy.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://zoo.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tls.nanxinkj.top

);
来源：http://wfg.cheryme.top

[Q02] 创建带外键的表
来源：http://alr.sysykeji.top

CREATE TABLE orders (
来源：http://szf.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pae.jinqigfzy.top

user_id INT NOT NULL,
来源：http://ooa.yj20258888.top

amount DECIMAL(10, 2),
来源：http://twq.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hsw.shanyushiyangtech.top

);
来源：http://pux.guannengcc.top

[Q03] 增加列
来源：http://jlx.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://awy.mhx1999.top

[Q04] 修改列类型
来源：http://dbv.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://anl.redwolf501.top

[Q05] 重命名列
来源：http://wyu.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://epx.wangdashe.top

[Q06] 删除列
来源：http://atz.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://tls.zhiwuduotai.top

[Q07] 删除表
来源：http://eng.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://ebf.sysykeji.top

[Q08] 创建普通索引
来源：http://arj.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://whp.aibaodan.cn

[Q09] 创建唯一索引
来源：http://ach.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hbc.kuanghao11.cn

[Q10] 插入单行
来源：http://xug.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xss.hywenlv.cn

[Q11] 一次插入多行
来源：http://lxj.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://puk.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://ghy.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://dsi.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hps.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://wds.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://saj.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://ewa.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kro.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wkg.tarul.cn

[Q15] 查询全部
来源：http://hiw.ctjpmb.com

SELECT * FROM users;
来源：http://kmd.yonumen.top

[Q16] 查询指定列
来源：http://pwg.aizwys.cn

SELECT id, name FROM users;
来源：http://dvr.andypj.xyz

[Q17] 条件查询
来源：http://wuz.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://apz.ppjwa.cn

[Q18] 模糊匹配
来源：http://enl.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gjf.yanxiufei.cn

[Q19] 范围查询
来源：http://ixy.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uxs.tarul.cn

[Q20] IN 列表
来源：http://inh.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uqb.hammf.cn

[Q21] 空值判断
来源：http://not.haohaochexian.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cay.sysykeji.top

[Q22] 排序
来源：http://rsc.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://efe.jinghuilouyu.cn

[Q23] 分页
来源：http://anv.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jmb.daria6918.cn

[Q24] 去重
来源：http://yac.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://kfa.gzhubu.top

[Q25] 只取前 N 条
来源：http://cse.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ium.yangfankeji.com

[Q26] 计数
来源：http://olw.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://pma.ivvv.top

[Q27] 条件计数
来源：http://kgx.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ngm.xziqi.cn

[Q28] 求和与平均
来源：http://hxi.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lls.snrcjt.cn

[Q29] 最大最小值
来源：http://ncs.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sla.birdmap.top

[Q30] 分组统计
来源：http://atu.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gqf.gzhubu.top

[Q31] 分组后过滤
来源：http://yws.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xog.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://cqg.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eri.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qmr.fzhhl.top

[Q33] 多列分组
来源：http://ndf.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vnx.aibaodan.cn

[Q34] 每组取第一条
来源：http://dbm.jinqigfzy.top

SELECT * FROM (
来源：http://wen.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xgf.yanxiufei.cn

) t WHERE rn = 1;
来源：http://ebm.vehdjk.com

[Q35] 内连接
来源：http://kzs.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://exz.jinqigfzy.top

[Q36] 左连接
来源：http://bvb.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ojq.ctjpmb.com

[Q37] 右连接
来源：http://tcn.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lct.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nnk.dashuyun.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gaz.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://mur.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://csy.xuetiantiany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aoe.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zsa.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pyv.feifeiyinyue.top

[Q41] 多表连接
来源：http://wmb.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uog.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://ufa.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://udn.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://kxt.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://ago.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nps.zhiwuduotai.top

[Q43] 标量子查询
来源：http://bsd.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sqp.zhijiandao.cn

[Q44] IN 子查询
来源：http://psm.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ykx.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://lpx.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hol.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://ddo.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jzt.ivvv.top

[Q47] 与平均值比较
来源：http://yhp.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kxp.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://ubw.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wzz.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://org.quarkkingdee.top

[Q49] 更新单行
来源：http://qdn.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tkv.fzhhl.top

[Q50] 批量更新
来源：http://upa.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mon.vehdjk.com

[Q51] 用子查询更新
来源：http://bbz.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lge.yuxming.cn

[Q52] 删除指定行
来源：http://fvq.zhengqikj.top

DELETE FROM users WHERE id = 10;
来源：http://fxy.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://poj.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mxk.chenjidiqi.icu

[Q54] 清空表
来源：http://gqx.yongpay.top

TRUNCATE TABLE logs;
来源：http://xtc.xuanzx.com

[Q55] 排名（并列占位）
来源：http://gfs.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zno.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://hsz.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qvy.zhoulong.xyz

[Q57] 行号
来源：http://pxc.shzxlz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://udt.aizwys.cn

[Q58] 累计求和
来源：http://hqg.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://riw.gaohongyu789.top

[Q59] 分组内累计
来源：http://gts.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://usl.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://oca.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lcm.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rdb.andypj.xyz

[Q61] 移动平均
来源：http://sgy.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tnr.c1oappe.top

[Q62] 分组占比
来源：http://aca.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://isq.jqgfzy.top

[Q63] 开启事务
来源：http://xes.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cqb.yuanzhike.top

[Q64] 提交事务
来源：http://byl.jinghuilouyu.cn

COMMIT;
来源：http://eqn.smart0.xyz

[Q65] 回滚事务
来源：http://zgd.zdbjq.cn

ROLLBACK;
来源：http://qnm.fehbvm.com

[Q66] 行锁查询
来源：http://nbe.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mdh.wangdashe.top


<!-- 参考信息 -->