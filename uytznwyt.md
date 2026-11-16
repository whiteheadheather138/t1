代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://poj.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hij.yvedp.cn

Java: class Node { int v; Node next; }
来源：http://oli.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://rzm.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zan.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tjk.yj20258888.top

[N11] 二叉树中序遍历
来源：http://pli.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://noo.gogol.net.cn

PHP:  // 手写递归函数
来源：http://hrz.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vwi.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jzt.dashuyun.cn

Java: // 手写递归
来源：http://pwh.quarkkingdee.top

Go:   // 手写递归
来源：http://opc.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lbr.0kj1m.cn

C#:   // 手写递归
来源：http://aak.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tuu.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xnj.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://siw.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gig.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sux.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wxu.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fvm.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xsh.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ivv.tianlin.xyz

================================================================================
来源：http://vlb.hnqzz.top

O. 并发与异步
来源：http://mtu.shanyushiyangtech.top

================================================================================
来源：http://qui.yueranfly.top

[O01] 启动一个线程
来源：http://upn.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pol.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://buo.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ktm.nanxinkj.top

TS:   // 同 JS
来源：http://fzw.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://wfg.hcnkem.com

Go:   go f()
来源：http://dxc.shuidangran.top

Ruby: Thread.new { f }
来源：http://pew.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://mco.fktsv.cn

[O02] 使用线程池
来源：http://zyd.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hbb.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yuz.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://rpk.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://xvq.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ybn.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xql.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fol.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ltt.ydzc1.top

[O03] 加锁保护共享数据
来源：http://cgr.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://cyw.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://aan.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bgr.sweek.top

TS:   // 同 JS
来源：http://aos.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://cqu.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hdd.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://quk.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://ajd.52xcode.cn

[O04] 定义异步函数并等待
来源：http://lei.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://zdv.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://orz.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://zkx.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://wtv.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zbj.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lac.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xpg.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://xro.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://pbx.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://cje.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hmf.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://ztc.yj202588.top

TS:   await Promise.all(tasks)
来源：http://qex.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hhj.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xhx.uphjek.com

Ruby: threads.map(&:join)
来源：http://uit.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://qsh.nanxuanxn.top

[O06] 使用进程池
来源：http://ffc.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wnq.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://phr.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://kcg.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://nkg.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zux.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jvf.tianlin.xyz

Ruby: // fork 块
来源：http://hmo.daria6918.cn

C#:   Parallel.For
来源：http://ddg.nwbrower.top

================================================================================
来源：http://hgh.zhiwuduotai.top

P. 常用工具函数
来源：http://xgh.cucudq.cn

================================================================================
来源：http://wlq.aibaodan.cn

[P01] 生成 UUID
来源：http://pvh.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://dhi.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bmw.jianghu66.top

JS:   crypto.randomUUID()
来源：http://zfu.shuidangran.top

TS:   crypto.randomUUID()
来源：http://tda.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://xmq.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://ddn.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://raw.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://gyx.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://pjv.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rji.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://upq.snrcjt.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xsz.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://npr.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cby.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uby.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mmu.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kbu.wangdashe.top

[P03] 生成短随机字符串
来源：http://iwb.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dwa.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tkq.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhg.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bbh.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yiv.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://otu.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ntq.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iai.zhoulong.xyz

[P04] 求长度
来源：http://otu.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tsy.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://teh.redwolf501.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nit.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rey.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://ljl.fktsv.cn

Go:   len(arr);  len(m)
来源：http://trv.gotoacloud.top

Ruby: x.length;  x.size
来源：http://ctc.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vxu.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://sif.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xcl.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bol.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xii.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://csf.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ktw.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://llh.yuxming.cn

Ruby: a == b
来源：http://huk.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fgf.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ooh.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jej.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://hnc.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fbb.redwolf501.top

TS:   if (x == null) {}
来源：http://jva.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pjq.yj20258888.top

Go:   if x == nil {}
来源：http://ead.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jkq.zhengqikj.top

C#:   if (x is null) {}
来源：http://omf.jianghu66.top

[P07] 防抖与节流
来源：http://wkt.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ugt.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://fjj.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sec.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdf.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hip.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://otu.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pva.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kpu.birdmap.top

[P08] 处理浮点精度问题
来源：http://xka.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lfs.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wmt.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gsn.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://owi.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mth.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ugu.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kje.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jeg.yfazqb.com

================================================================================
来源：http://isj.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jwe.shzxlz.cn

================================================================================
来源：http://mkb.xuetiantiany.cn

[Q01] 创建表
来源：http://gwu.fehbvm.com

CREATE TABLE users (
来源：http://vsl.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rng.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://olx.cashguo.top

email VARCHAR(100) UNIQUE,
来源：http://kqm.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bgd.316326.xyz

);
来源：http://dbw.uphjek.com

[Q02] 创建带外键的表
来源：http://rid.yonumen.top

CREATE TABLE orders (
来源：http://vqn.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tgz.sufxvd.cn

user_id INT NOT NULL,
来源：http://zlf.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://ojd.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ojl.smart0.xyz

);
来源：http://uff.guannengcc.top

[Q03] 增加列
来源：http://bod.zhengqikj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ryb.redwolf501.top

[Q04] 修改列类型
来源：http://hbo.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zee.hysaishi.cn

[Q05] 重命名列
来源：http://pso.zhengqikj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ata.feifeiyinyue.top

[Q06] 删除列
来源：http://poy.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://wpa.ybcxt.top

[Q07] 删除表
来源：http://hus.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://ukb.jinqigfzy.top

[Q08] 创建普通索引
来源：http://nia.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kql.bjfxy.top

[Q09] 创建唯一索引
来源：http://oim.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://azb.chenzaomai.com

[Q10] 插入单行
来源：http://zoy.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yrh.yvedp.cn

[Q11] 一次插入多行
来源：http://kmj.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bdg.meibo888.top

[Q12] 插入后取自增 ID
来源：http://gko.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://klw.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iku.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://tey.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ooh.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://fjq.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qwb.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cva.zycfv.cn

[Q15] 查询全部
来源：http://kbb.feifeiyinyue.top

SELECT * FROM users;
来源：http://fqp.chenjidiqi.icu

[Q16] 查询指定列
来源：http://izn.yvedp.cn

SELECT id, name FROM users;
来源：http://fpf.hywenlv.cn

[Q17] 条件查询
来源：http://wth.svipenyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hzw.snrcjt.cn

[Q18] 模糊匹配
来源：http://jmn.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lpl.svipenyu.cn

[Q19] 范围查询
来源：http://zjw.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pjk.yj202588.top

[Q20] IN 列表
来源：http://dke.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vms.guannengcc.top

[Q21] 空值判断
来源：http://mpz.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mud.quarkkingdee.top

[Q22] 排序
来源：http://qds.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pjo.sufxvd.cn

[Q23] 分页
来源：http://leq.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pzq.zhengqikj.top

[Q24] 去重
来源：http://wwh.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://our.xziqi.cn

[Q25] 只取前 N 条
来源：http://ofl.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pix.hysaishi.cn

[Q26] 计数
来源：http://mwc.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://ujq.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://gho.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wcu.0kj1m.cn

[Q28] 求和与平均
来源：http://jec.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xyu.jlsjyb.cn

[Q29] 最大最小值
来源：http://fkc.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tqq.xuetiantiany.cn

[Q30] 分组统计
来源：http://kwd.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vyg.bbcook.cn

[Q31] 分组后过滤
来源：http://pjk.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yan.bbcook.cn

[Q32] 分组拼接字符串
来源：http://krg.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mds.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wvo.0kj1m.cn

[Q33] 多列分组
来源：http://nym.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pra.jlsjyb.cn

[Q34] 每组取第一条
来源：http://ziq.chenjidiqi.icu

SELECT * FROM (
来源：http://eqn.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://izk.dashuyun.cn

) t WHERE rn = 1;
来源：http://jvi.nwbrower.top

[Q35] 内连接
来源：http://aye.hysaishi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aaa.wangdashe.top

[Q36] 左连接
来源：http://eil.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oln.quarkkingdee.top

[Q37] 右连接
来源：http://nqw.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ltt.gogol.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mjn.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rtx.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://fvz.daxiang520.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ozo.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rok.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eqf.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hus.yuanzhike.top

[Q41] 多表连接
来源：http://seo.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rbu.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://aio.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://pxh.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://fqj.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://gzv.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ryx.gaohongyu789.top

[Q43] 标量子查询
来源：http://rnu.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vqc.fzhhl.top

[Q44] IN 子查询
来源：http://slx.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://win.uphjek.com

[Q45] EXISTS 判断存在
来源：http://sor.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://djl.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://nxh.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hrf.zhongyouzk.top

[Q47] 与平均值比较
来源：http://wpo.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lgl.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://fbr.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gmf.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://twi.cqqwz.cn

[Q49] 更新单行
来源：http://qwc.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://znk.zdbjq.cn

[Q50] 批量更新
来源：http://rzs.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fau.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://kmt.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ecy.vqdsnc.cn

[Q52] 删除指定行
来源：http://taq.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://por.vehdjk.com

[Q53] 按条件删除
来源：http://cnq.zdqjudy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dct.jinyuanbaomall.cn

[Q54] 清空表
来源：http://bss.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://ykp.fktsv.cn

[Q55] 排名（并列占位）
来源：http://wzf.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://shv.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://lnb.xylfe.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xod.chenzaomai.com

[Q57] 行号
来源：http://nrd.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://krx.vehdjk.com

[Q58] 累计求和
来源：http://lhy.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bma.jinqigfzy.top

[Q59] 分组内累计
来源：http://zul.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gym.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://ldx.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yxl.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gul.snrcjt.cn


<!-- 参考信息 -->