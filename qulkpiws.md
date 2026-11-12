代发 wailian999

Go:   // 手写递归
来源：http://hrl.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rjz.zycfv.cn

C#:   // 手写递归
来源：http://ngs.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zdx.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ynn.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qdn.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hlw.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hpm.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dbr.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yht.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lse.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bje.uphjek.com

================================================================================
来源：http://dzo.zhijiandao.cn

O. 并发与异步
来源：http://lvr.yj20258888.top

================================================================================
来源：http://wqj.chenjidiqi.icu

[O01] 启动一个线程
来源：http://sxh.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cyt.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bpf.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qhq.ivvv.top

TS:   // 同 JS
来源：http://ahk.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://aul.haohaochexian.top

Go:   go f()
来源：http://qis.aizwys.cn

Ruby: Thread.new { f }
来源：http://lnt.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://foz.9152youxi.cn

[O02] 使用线程池
来源：http://rth.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://orr.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pnm.hnqzz.top

JS:   // worker_threads 线程池
来源：http://vqe.birdmap.top

TS:   // worker_threads 线程池
来源：http://nys.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vij.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wqb.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ydm.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hvk.vehdjk.com

[O03] 加锁保护共享数据
来源：http://ygw.gogol.net.cn

Py:   with lock: shared += 1
来源：http://frd.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://rzo.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yca.kuanghao11.cn

TS:   // 同 JS
来源：http://aiv.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://hil.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bcx.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zoz.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://nas.mhx1999.top

[O04] 定义异步函数并等待
来源：http://vro.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://ufr.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfl.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://loa.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vgs.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://coe.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mce.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://uoz.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://emr.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://xjf.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://lan.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://njl.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://sxj.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://ozr.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mls.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rcy.aizwys.cn

Ruby: threads.map(&:join)
来源：http://jva.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xla.svipenyu.cn

[O06] 使用进程池
来源：http://cag.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://haq.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cnb.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://lhg.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://dos.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cmf.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://imd.yvedp.cn

Ruby: // fork 块
来源：http://vny.xuetiantiany.cn

C#:   Parallel.For
来源：http://kmb.ywan-chungtsiang.top

================================================================================
来源：http://olc.iojbl.cn

P. 常用工具函数
来源：http://zzg.jinghuilouyu.cn

================================================================================
来源：http://csh.52xcode.cn

[P01] 生成 UUID
来源：http://gul.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://azs.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gud.meibo888.top

JS:   crypto.randomUUID()
来源：http://wpn.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://sqw.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://ekk.jianghu66.top

Go:   // 用 github.com/google/uuid
来源：http://uyh.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://dea.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://hlv.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://btl.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fyx.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sln.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qxg.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qef.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rwf.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hdg.xziqi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ren.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vib.zhixingplan.top

[P03] 生成短随机字符串
来源：http://ama.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mbw.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mvh.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mnj.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xph.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uli.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://why.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rgi.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gak.jinyuanbaomall.cn

[P04] 求长度
来源：http://prq.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://avm.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://caq.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfe.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vid.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://pne.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://gnd.cdnleiting.top

Ruby: x.length;  x.size
来源：http://ute.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://imw.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://ugq.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ydd.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wfv.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nsu.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nbh.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oxx.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://wxr.9152youxi.cn

Ruby: a == b
来源：http://nwx.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://msb.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gca.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://exb.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://sya.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lir.yj202588.top

TS:   if (x == null) {}
来源：http://xwt.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kll.hfpthk.cn

Go:   if x == nil {}
来源：http://clc.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wtg.0kj1m.cn

C#:   if (x is null) {}
来源：http://jnx.wangdashe.top

[P07] 防抖与节流
来源：http://jks.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://edg.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://cwk.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyy.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kjc.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mwz.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zbt.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jmg.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uvb.vehdjk.com

[P08] 处理浮点精度问题
来源：http://ipo.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aip.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nlm.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dqo.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nng.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bsd.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fcr.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://skn.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tid.guowangkeji.top

================================================================================
来源：http://csh.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rqh.fktsv.cn

================================================================================
来源：http://gsp.yfazqb.com

[Q01] 创建表
来源：http://qzd.chenlongwang.top

CREATE TABLE users (
来源：http://lku.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iko.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://nsg.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://izo.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rvo.jinqigfzy.top

);
来源：http://iss.chenzaomai.com

[Q02] 创建带外键的表
来源：http://xjd.epnwcf.com

CREATE TABLE orders (
来源：http://wtb.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hln.redwolf501.top

user_id INT NOT NULL,
来源：http://sif.epnwcf.com

amount DECIMAL(10, 2),
来源：http://qfk.xingfuxueyuan.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hqe.zhongyouzk.top

);
来源：http://tvt.hywenlv.cn

[Q03] 增加列
来源：http://abg.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jgi.ybcxt.top

[Q04] 修改列类型
来源：http://lii.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://exf.gotoacloud.top

[Q05] 重命名列
来源：http://bwy.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hsz.tianlin.xyz

[Q06] 删除列
来源：http://kfg.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://oqv.sufxvd.cn

[Q07] 删除表
来源：http://jyl.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://gsq.hysaishi.cn

[Q08] 创建普通索引
来源：http://iud.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wyj.xziqi.cn

[Q09] 创建唯一索引
来源：http://slj.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://klo.uphjek.com

[Q10] 插入单行
来源：http://nuh.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jxf.ivvv.top

[Q11] 一次插入多行
来源：http://zoq.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ueb.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://cqw.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nyv.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rbf.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://say.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jsg.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://mfe.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kbx.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yqo.haohaochexian.top

[Q15] 查询全部
来源：http://fnx.birdmap.top

SELECT * FROM users;
来源：http://uhj.zdbjq.cn

[Q16] 查询指定列
来源：http://zft.yanxiufei.cn

SELECT id, name FROM users;
来源：http://ffl.jinqigfzy.top

[Q17] 条件查询
来源：http://hng.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qhj.yj20258.top

[Q18] 模糊匹配
来源：http://zzx.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ckf.hcnkem.com

[Q19] 范围查询
来源：http://chb.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xgn.ppjwa.cn

[Q20] IN 列表
来源：http://ybx.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fgk.jqgfzy.top

[Q21] 空值判断
来源：http://axd.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wjf.shangyingyoupin.top

[Q22] 排序
来源：http://adq.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fhp.ydjk.org.cn

[Q23] 分页
来源：http://qku.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ijj.yfazqb.com

[Q24] 去重
来源：http://iun.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://wlo.tarul.cn

[Q25] 只取前 N 条
来源：http://vqy.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zgk.gogol.net.cn

[Q26] 计数
来源：http://etu.sweek.top

SELECT COUNT(*) FROM users;
来源：http://lel.wangdashe.top

[Q27] 条件计数
来源：http://ict.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pjw.xziqi.cn

[Q28] 求和与平均
来源：http://usl.aibaodan.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bad.xinyue.icu

[Q29] 最大最小值
来源：http://viq.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hyy.guowangkeji.top

[Q30] 分组统计
来源：http://tvk.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://puu.tanke756.top

[Q31] 分组后过滤
来源：http://pdj.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pqh.c1oappe.top

[Q32] 分组拼接字符串
来源：http://xpk.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kfa.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dbr.yuxming.cn

[Q33] 多列分组
来源：http://tmt.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gve.tanke756.top

[Q34] 每组取第一条
来源：http://iji.zhongyouzk.top

SELECT * FROM (
来源：http://rqy.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rht.kuanghao11.cn

) t WHERE rn = 1;
来源：http://mqv.nanxuanxn.top

[Q35] 内连接
来源：http://beo.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yvh.jinqigfzy.top

[Q36] 左连接
来源：http://prs.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ooy.yueranfly.top

[Q37] 右连接
来源：http://tix.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ynp.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://zib.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sno.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://ihz.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://jer.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lig.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fnh.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eon.jlsjyb.cn

[Q41] 多表连接
来源：http://yzt.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://anb.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://vgx.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://tzk.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://tha.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://fpo.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xsi.meibo888.top

[Q43] 标量子查询
来源：http://ykb.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qwl.xuanzx.com

[Q44] IN 子查询
来源：http://iiz.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ddj.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://dil.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pva.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://anp.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxf.sysykeji.top

[Q47] 与平均值比较
来源：http://gkw.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uac.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://xam.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jyd.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://vhr.nwbrower.top

[Q49] 更新单行
来源：http://jra.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mou.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://fjv.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dup.jianghu66.top

[Q51] 用子查询更新
来源：http://erv.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rgj.jianghu66.top

[Q52] 删除指定行
来源：http://ikk.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://fjj.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://zas.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mlj.meibo888.top

[Q54] 清空表
来源：http://zvw.shuidangran.top

TRUNCATE TABLE logs;
来源：http://oxr.cashguo.top

[Q55] 排名（并列占位）
来源：http://hoj.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cbp.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://sut.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rnd.jyoumei.cn

[Q57] 行号
来源：http://zmi.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qli.dianchejie.cn

[Q58] 累计求和
来源：http://sbs.bjfxy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://egd.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://nhs.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xqk.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://wxp.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://imn.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxf.meibo888.top

[Q61] 移动平均
来源：http://frw.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cnu.dianchejie.cn

[Q62] 分组占比
来源：http://sda.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mgk.quarkkingdee.top

[Q63] 开启事务
来源：http://hed.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bhb.shzxlz.cn

[Q64] 提交事务
来源：http://zsc.yanxiufei.cn

COMMIT;
来源：http://cjf.cdnleiting.top

[Q65] 回滚事务
来源：http://aqz.52xcode.cn

ROLLBACK;
来源：http://ocn.0kj1m.cn

[Q66] 行锁查询
来源：http://red.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eix.cqqwz.cn


<!-- 参考信息 -->