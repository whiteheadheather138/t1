代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://sky.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nhq.xuanzx.com

[N11] 二叉树中序遍历
来源：http://rog.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yeh.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://tay.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wrt.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gwb.cashguo.top

Java: // 手写递归
来源：http://fvf.hnxiangtu.top

Go:   // 手写递归
来源：http://sxa.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tbf.sjlbkw.cn

C#:   // 手写递归
来源：http://uom.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vtc.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gde.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bkm.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://axf.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xui.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sal.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hdw.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fqo.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://djn.hywenlv.cn

================================================================================
来源：http://ncy.hnxiangtu.top

O. 并发与异步
来源：http://eft.ydjk.org.cn

================================================================================
来源：http://gbv.wangshuangyany.cn

[O01] 启动一个线程
来源：http://huo.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pgm.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://trq.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://whq.guowangkeji.top

TS:   // 同 JS
来源：http://tpc.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://ong.hnxiangtu.top

Go:   go f()
来源：http://vhj.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://lja.yj20258888.top

C#:   Task.Run(() => F());
来源：http://ouv.sjlbkw.cn

[O02] 使用线程池
来源：http://oya.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fuk.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ihs.andypj.xyz

JS:   // worker_threads 线程池
来源：http://reo.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://mad.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rpn.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://chk.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vpv.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wlb.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://suk.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://nht.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://efy.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://clv.xinyue.icu

TS:   // 同 JS
来源：http://mbt.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://xag.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pop.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ghe.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://jcq.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://mxb.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://dki.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://thz.fzhhl.top

JS:   async function f() { await g(); }
来源：http://jxe.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://eca.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bgc.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ypg.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mac.hammf.cn

C#:   async Task F() { await G(); }
来源：http://djo.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://ymf.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://zlc.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fgt.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://cde.tarul.cn

TS:   await Promise.all(tasks)
来源：http://hbq.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sxg.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wfu.xinyue.icu

Ruby: threads.map(&:join)
来源：http://ftw.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ivf.sxryk.cn

[O06] 使用进程池
来源：http://mev.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dia.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ynf.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://gpo.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://pzo.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nzy.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://anv.iojbl.cn

Ruby: // fork 块
来源：http://uck.52xcode.cn

C#:   Parallel.For
来源：http://cex.shzxlz.cn

================================================================================
来源：http://lkt.meibo888.top

P. 常用工具函数
来源：http://fcy.zhijiandao.cn

================================================================================
来源：http://wzv.316326.xyz

[P01] 生成 UUID
来源：http://fjm.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://ipp.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://omi.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://qsp.tanke756.top

TS:   crypto.randomUUID()
来源：http://bdc.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://qtu.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://foo.yonumen.top

Ruby: SecureRandom.uuid
来源：http://uyj.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://czq.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://xsu.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cgd.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nyt.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ppd.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ngk.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jag.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://krl.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tcw.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cea.yj20258888.top

[P03] 生成短随机字符串
来源：http://iic.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cxt.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eye.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mue.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aaj.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wre.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://myv.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ldp.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xtj.vqdsnc.cn

[P04] 求长度
来源：http://rzf.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bxt.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hib.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mqs.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqv.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://jmu.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://rll.daxiang520.top

Ruby: x.length;  x.size
来源：http://juh.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kyk.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://sje.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://jeq.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://var.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nyq.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xxx.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tlk.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ugv.hywenlv.cn

Ruby: a == b
来源：http://ihx.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tdp.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bwi.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bah.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://ipn.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zmc.snrcjt.cn

TS:   if (x == null) {}
来源：http://zsr.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gsq.sufxvd.cn

Go:   if x == nil {}
来源：http://vus.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hvp.quarkkingdee.top

C#:   if (x is null) {}
来源：http://mug.yonumen.top

[P07] 防抖与节流
来源：http://bsh.zdqjudy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nqm.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://dnu.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymb.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjq.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iuu.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kxh.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kkn.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ifq.ydzc1.top

[P08] 处理浮点精度问题
来源：http://dfo.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kec.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tmj.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spr.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vtl.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vyy.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bdj.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zcl.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mte.jqgfzy.top

================================================================================
来源：http://mcu.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lco.iojbl.cn

================================================================================
来源：http://umg.jyoumei.cn

[Q01] 创建表
来源：http://gtb.sweek.top

CREATE TABLE users (
来源：http://hiy.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hne.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://srd.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://lfv.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aae.birdmap.top

);
来源：http://exd.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://iwh.ydzc1.top

CREATE TABLE orders (
来源：http://gmo.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qij.zdqjudy.top

user_id INT NOT NULL,
来源：http://efu.birdmap.top

amount DECIMAL(10, 2),
来源：http://nya.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gjf.sjlbkw.cn

);
来源：http://xof.birdmap.top

[Q03] 增加列
来源：http://bjm.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qhx.yj202588.top

[Q04] 修改列类型
来源：http://uoy.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://syi.jinghuilouyu.cn

[Q05] 重命名列
来源：http://vur.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://alb.gogol.net.cn

[Q06] 删除列
来源：http://xwa.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yya.aibaodan.cn

[Q07] 删除表
来源：http://zdv.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://xcu.tianlin.xyz

[Q08] 创建普通索引
来源：http://wsp.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uxy.ivvv.top

[Q09] 创建唯一索引
来源：http://wll.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zds.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://bgu.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lpf.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://eay.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bqr.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://gum.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://bun.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vtb.zdbjq.cn

[Q13] 忽略重复插入
来源：http://odz.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://znk.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://hmf.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fag.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gua.vehdjk.com

[Q15] 查询全部
来源：http://ubs.nanxuanxn.top

SELECT * FROM users;
来源：http://dtu.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://gbn.gotoacloud.top

SELECT id, name FROM users;
来源：http://ofu.yvedp.cn

[Q17] 条件查询
来源：http://uox.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zws.ppjwa.cn

[Q18] 模糊匹配
来源：http://pwi.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jnn.gzhubu.top

[Q19] 范围查询
来源：http://mji.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://obx.cucudq.cn

[Q20] IN 列表
来源：http://gfq.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hhd.jqgufenzy.top

[Q21] 空值判断
来源：http://siq.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://yov.bjfxy.top

[Q22] 排序
来源：http://slc.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pad.guannengcc.top

[Q23] 分页
来源：http://fvg.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bsn.gotoacloud.top

[Q24] 去重
来源：http://ywj.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://eml.gzhubu.top

[Q25] 只取前 N 条
来源：http://jgt.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tgb.hywenlv.cn

[Q26] 计数
来源：http://ugo.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://tmn.redwolf501.top

[Q27] 条件计数
来源：http://jsw.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iuz.ctjpmb.com

[Q28] 求和与平均
来源：http://rcf.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jyw.hnqzz.top

[Q29] 最大最小值
来源：http://quh.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jjl.cashguo.top

[Q30] 分组统计
来源：http://hls.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ktf.jianghu66.top

[Q31] 分组后过滤
来源：http://gom.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eya.hesvh.cn

[Q32] 分组拼接字符串
来源：http://nlc.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ukb.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sbs.sufxvd.cn

[Q33] 多列分组
来源：http://qdk.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gcc.yangfankeji.com

[Q34] 每组取第一条
来源：http://iwq.zhengqikj.top

SELECT * FROM (
来源：http://ver.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iht.yuanzhike.top

) t WHERE rn = 1;
来源：http://ddw.fzhhl.top

[Q35] 内连接
来源：http://tgy.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ofz.jinghuilouyu.cn

[Q36] 左连接
来源：http://myb.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uuy.guowangkeji.top

[Q37] 右连接
来源：http://qvk.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://unb.guowangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://cet.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cnn.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://ykw.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://xnh.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rts.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yxb.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wzw.hesvh.cn

[Q41] 多表连接
来源：http://dlo.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vny.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://gis.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://lel.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://jlm.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://qnm.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cmj.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://pjg.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uuk.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://qad.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ghl.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://yax.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msn.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://arv.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppm.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://vsx.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bkv.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://epu.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gjb.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://ipo.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://fdu.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wpj.shangyingyoupin.top

[Q50] 批量更新
来源：http://mwi.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://znc.jiagoushi.top

[Q51] 用子查询更新
来源：http://udr.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nay.hnxiangtu.top

[Q52] 删除指定行
来源：http://mvi.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://kgs.havefunace.top

[Q53] 按条件删除
来源：http://pcz.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ecd.yj202588.top

[Q54] 清空表
来源：http://xeb.cheryme.top

TRUNCATE TABLE logs;
来源：http://pay.tarul.cn

[Q55] 排名（并列占位）
来源：http://vkw.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fex.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://hta.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ttl.jyoumei.cn

[Q57] 行号
来源：http://uhp.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yzu.chenzaomai.com

[Q58] 累计求和
来源：http://lff.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ezo.shangyingyoupin.top

[Q59] 分组内累计
来源：http://yjc.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fxq.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://wwm.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rth.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngw.hysaishi.cn

[Q61] 移动平均
来源：http://mkz.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sbu.chenjidiqi.icu

[Q62] 分组占比
来源：http://ofi.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zwy.bbcook.cn


<!-- 参考信息 -->