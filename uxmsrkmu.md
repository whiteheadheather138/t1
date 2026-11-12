代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://aer.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zgk.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://rrq.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tlz.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://mlj.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbk.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cyt.jqgfzy.top

Java: // 手写递归
来源：http://cgl.kuanghao11.cn

Go:   // 手写递归
来源：http://kug.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ypy.dashuyun.cn

C#:   // 手写递归
来源：http://rno.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gmz.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://khk.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://liy.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://owt.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xeh.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bap.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oqz.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ptg.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zhw.xylfe.cn

================================================================================
来源：http://ycd.ehwqpu.com

O. 并发与异步
来源：http://fnk.sufxvd.cn

================================================================================
来源：http://hzn.ydjk.org.cn

[O01] 启动一个线程
来源：http://jtm.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://byu.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hlr.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vqq.ppjwa.cn

TS:   // 同 JS
来源：http://hky.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://dgj.yj20258888.top

Go:   go f()
来源：http://sih.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://nak.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://dkp.pengpengdd.cyou

[O02] 使用线程池
来源：http://jlq.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://itg.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ymg.yfazqb.com

JS:   // worker_threads 线程池
来源：http://lyo.c1oappe.top

TS:   // worker_threads 线程池
来源：http://mix.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://eom.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ebo.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nfy.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zih.tanke756.top

[O03] 加锁保护共享数据
来源：http://lzy.xziqi.cn

Py:   with lock: shared += 1
来源：http://oxg.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://jwu.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://olv.sufxvd.cn

TS:   // 同 JS
来源：http://kok.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://dcf.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://use.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uwi.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://bzb.yueranfly.top

[O04] 定义异步函数并等待
来源：http://xiu.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://byy.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gxh.epnwcf.com

JS:   async function f() { await g(); }
来源：http://eei.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bcp.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://beq.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bjl.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://mvn.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://bmr.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://zym.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://noo.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://txt.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://oxz.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://wps.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xhy.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dud.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://mag.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xop.daria6918.cn

[O06] 使用进程池
来源：http://kei.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mrx.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://san.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://jqp.yj202588.top

TS:   // child_process / cluster 模块
来源：http://dce.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yup.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uid.meibo888.top

Ruby: // fork 块
来源：http://mbk.guowangkeji.top

C#:   Parallel.For
来源：http://jhi.vehdjk.com

================================================================================
来源：http://cyg.jinghuilouyu.cn

P. 常用工具函数
来源：http://qmb.hnqzz.top

================================================================================
来源：http://xhh.yuanzhike.top

[P01] 生成 UUID
来源：http://xes.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://igu.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uqf.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://nso.yj20258888.top

TS:   crypto.randomUUID()
来源：http://vgg.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://ffm.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://qbs.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://vmr.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://blp.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://oia.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aaj.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lci.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wtx.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://niy.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wat.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qxt.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pyj.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blp.nwbrower.top

[P03] 生成短随机字符串
来源：http://ctx.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ibi.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gea.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://umm.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://abh.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mga.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yxn.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rcq.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pda.ctjpmb.com

[P04] 求长度
来源：http://zcb.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pdq.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://egj.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://atw.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zdv.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://gpt.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://jyd.52xcode.cn

Ruby: x.length;  x.size
来源：http://cpy.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dyh.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://wrv.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yjq.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://czk.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ftq.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ylg.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vvx.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://xgu.fktsv.cn

Ruby: a == b
来源：http://kvg.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tvl.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hrh.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sji.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://eni.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ppq.yj20258888.top

TS:   if (x == null) {}
来源：http://van.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://erz.yongpay.top

Go:   if x == nil {}
来源：http://frk.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfl.nanxuanxn.top

C#:   if (x is null) {}
来源：http://ywl.ivvv.top

[P07] 防抖与节流
来源：http://dkk.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mhd.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://mqh.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxl.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mzw.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ltp.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hhr.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vfm.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ifj.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://xmo.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xto.pengpengdd.cyou

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hrl.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bju.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rhe.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pbq.cqqwz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://szk.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qtn.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nrk.guannengcc.top

================================================================================
来源：http://joe.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ean.sweek.top

================================================================================
来源：http://ogp.hnqzz.top

[Q01] 创建表
来源：http://viz.kuanghao11.cn

CREATE TABLE users (
来源：http://moh.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfe.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://ohz.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://hza.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mja.sxryk.cn

);
来源：http://hlc.hysaishi.cn

[Q02] 创建带外键的表
来源：http://aqk.ppjwa.cn

CREATE TABLE orders (
来源：http://lyb.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzm.hnqzz.top

user_id INT NOT NULL,
来源：http://iwk.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://jpn.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bmo.tanke756.top

);
来源：http://jju.dianchejie.cn

[Q03] 增加列
来源：http://uet.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ggt.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://riy.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cet.jinghuilouyu.cn

[Q05] 重命名列
来源：http://eco.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lbw.sweek.top

[Q06] 删除列
来源：http://cbl.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yuy.ppjwa.cn

[Q07] 删除表
来源：http://xes.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://liq.nanxinkj.top

[Q08] 创建普通索引
来源：http://poz.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://dtr.sxryk.cn

[Q09] 创建唯一索引
来源：http://qhm.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fnr.jyoumei.cn

[Q10] 插入单行
来源：http://rcj.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://opd.jqgfzy.top

[Q11] 一次插入多行
来源：http://nvx.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aeb.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://xwf.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mpw.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cee.zdqjudy.top

[Q13] 忽略重复插入
来源：http://txk.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oae.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://qau.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jjc.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qzm.haohaochexian.top

[Q15] 查询全部
来源：http://kht.mhx1999.top

SELECT * FROM users;
来源：http://hgl.guowangkeji.top

[Q16] 查询指定列
来源：http://pqt.fehbvm.com

SELECT id, name FROM users;
来源：http://tui.tianlin.xyz

[Q17] 条件查询
来源：http://alm.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://akr.chenlongwang.top

[Q18] 模糊匹配
来源：http://epm.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tyc.316326.xyz

[Q19] 范围查询
来源：http://tzh.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zjz.shzxlz.cn

[Q20] IN 列表
来源：http://xlt.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mbh.tarul.cn

[Q21] 空值判断
来源：http://dda.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gog.aibaodan.cn

[Q22] 排序
来源：http://ejr.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bfn.yfazqb.com

[Q23] 分页
来源：http://rma.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jnb.ydjk.org.cn

[Q24] 去重
来源：http://tsi.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://cnm.aibaodan.cn

[Q25] 只取前 N 条
来源：http://dod.svipenyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jql.yangfankeji.com

[Q26] 计数
来源：http://wha.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://ppp.hysaishi.cn

[Q27] 条件计数
来源：http://kaw.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xxc.chenlongwang.top

[Q28] 求和与平均
来源：http://gsp.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://myu.ppjwa.cn

[Q29] 最大最小值
来源：http://fdn.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vpg.ydjk.org.cn

[Q30] 分组统计
来源：http://tle.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ohh.nanxuanxn.top

[Q31] 分组后过滤
来源：http://pto.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qbb.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://zyn.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sip.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://msh.guannengcc.top

[Q33] 多列分组
来源：http://zlx.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wns.hfpthk.cn

[Q34] 每组取第一条
来源：http://pib.fengsongda.top

SELECT * FROM (
来源：http://slj.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pru.ehwqpu.com

) t WHERE rn = 1;
来源：http://rmc.shanyushiyangkeji.top

[Q35] 内连接
来源：http://hzf.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://byu.jyoumei.cn

[Q36] 左连接
来源：http://emx.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rob.yj20258.top

[Q37] 右连接
来源：http://xio.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yrr.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://eir.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wcf.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://vjx.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bjd.xuetiantiany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://axr.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qbg.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://trt.tianlin.xyz

[Q41] 多表连接
来源：http://ihb.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bvu.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://fxu.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://bah.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://pjb.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://lgd.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pno.cheryme.top

[Q43] 标量子查询
来源：http://vxy.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yye.quarkkingdee.top

[Q44] IN 子查询
来源：http://acu.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://egm.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://dph.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://btp.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://atx.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wvt.wangdashe.top

[Q47] 与平均值比较
来源：http://ciq.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tpb.tarul.cn

[Q48] CTE 公用表表达式
来源：http://hce.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pcs.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://qjo.ydjk.org.cn

[Q49] 更新单行
来源：http://yon.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vxo.zhixingplan.top

[Q50] 批量更新
来源：http://zqk.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ayh.dianchejie.cn

[Q51] 用子查询更新
来源：http://fva.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nyo.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://voq.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://vvl.xuetiantiany.cn

[Q53] 按条件删除
来源：http://bjp.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zdi.vehdjk.com

[Q54] 清空表
来源：http://esr.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://ooy.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://ciu.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dbw.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://qgv.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ifh.chenzaomai.com

[Q57] 行号
来源：http://uub.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oqi.nanxuanxn.top

[Q58] 累计求和
来源：http://gos.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ufq.xylfe.cn

[Q59] 分组内累计
来源：http://rxf.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oxc.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://brn.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rit.zdbjq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://afc.zhijiandao.cn

[Q61] 移动平均
来源：http://vgd.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://srk.ybcxt.top

[Q62] 分组占比
来源：http://xmr.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vky.chenjidiqi.icu


<!-- 参考信息 -->