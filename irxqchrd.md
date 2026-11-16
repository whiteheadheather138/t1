代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tmi.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wez.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://gkf.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://jhl.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ryp.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bij.316326.xyz

[N11] 二叉树中序遍历
来源：http://vve.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rlv.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://jot.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yhv.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfa.xylfe.cn

Java: // 手写递归
来源：http://pse.uphjek.com

Go:   // 手写递归
来源：http://auo.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gbp.0kj1m.cn

C#:   // 手写递归
来源：http://twf.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nsd.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ion.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yan.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tlo.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gxn.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fhv.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fsz.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gvo.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hsz.hcnkem.com

================================================================================
来源：http://wjl.shuidangran.top

O. 并发与异步
来源：http://nfl.kuanghao11.cn

================================================================================
来源：http://hok.dianchejie.cn

[O01] 启动一个线程
来源：http://ovp.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgb.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tad.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yyw.jiagoushi.top

TS:   // 同 JS
来源：http://frw.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://oxt.bbcook.cn

Go:   go f()
来源：http://zuu.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://xqm.tanke756.top

C#:   Task.Run(() => F());
来源：http://chj.vqdsnc.cn

[O02] 使用线程池
来源：http://cqj.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wfr.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://map.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://blq.zycfv.cn

TS:   // worker_threads 线程池
来源：http://pcz.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://hix.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rmm.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ngn.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jqv.xinyue.icu

[O03] 加锁保护共享数据
来源：http://nja.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://kaa.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://bru.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://upr.guowangkeji.top

TS:   // 同 JS
来源：http://gmg.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://qrc.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pal.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rov.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://uem.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://mix.tarul.cn

Py:   async def f():⏎    await g()
来源：http://vfd.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cwm.yj20258.top

JS:   async function f() { await g(); }
来源：http://vrt.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ssb.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mba.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://exj.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xuu.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://kgu.quarkkingdee.top

[O05] 并发执行并等待全部完成
来源：http://wrr.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://glm.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mlf.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://fox.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://gay.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lkh.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mky.xuanzx.com

Ruby: threads.map(&:join)
来源：http://bnw.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sjr.hnqzz.top

[O06] 使用进程池
来源：http://dya.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmm.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ljh.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://nnf.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://tvj.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ans.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fgp.hnqzz.top

Ruby: // fork 块
来源：http://ite.shuidangran.top

C#:   Parallel.For
来源：http://xnb.shzxlz.cn

================================================================================
来源：http://vif.yuxming.cn

P. 常用工具函数
来源：http://qcy.xziqi.cn

================================================================================
来源：http://hor.andypj.xyz

[P01] 生成 UUID
来源：http://tas.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://xhf.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ngz.jianghu66.top

JS:   crypto.randomUUID()
来源：http://ali.yonumen.top

TS:   crypto.randomUUID()
来源：http://jii.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://inn.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://uhc.birdmap.top

Ruby: SecureRandom.uuid
来源：http://mxe.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://uot.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://xut.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sub.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://asz.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uht.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yde.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://trd.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uzx.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vad.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hcf.yonumen.top

[P03] 生成短随机字符串
来源：http://ooa.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://twj.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nda.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvs.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rnm.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://flq.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xxp.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://yrl.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gka.zhongyouzk.top

[P04] 求长度
来源：http://eki.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://elt.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tqz.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kbe.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rfl.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://tjv.wangdashe.top

Go:   len(arr);  len(m)
来源：http://ugj.dianchejie.cn

Ruby: x.length;  x.size
来源：http://lwl.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yoz.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://wnd.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yfl.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oah.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zoq.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hxi.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sgs.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dvo.shzxlz.cn

Ruby: a == b
来源：http://lob.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qbz.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vzi.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eds.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://vuq.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mhi.snrcjt.cn

TS:   if (x == null) {}
来源：http://hwy.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vmv.svipenyu.cn

Go:   if x == nil {}
来源：http://bef.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bix.cqqwz.cn

C#:   if (x is null) {}
来源：http://ixm.aizwys.cn

[P07] 防抖与节流
来源：http://ndy.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://joq.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://yjl.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxl.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hee.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sog.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vjf.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qxw.yvedp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://otm.daxiang520.top

[P08] 处理浮点精度问题
来源：http://uuh.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bkd.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hpl.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://foq.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wss.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://abx.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vpt.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lbd.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sjx.xziqi.cn

================================================================================
来源：http://tmd.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cid.haohaochexian.top

================================================================================
来源：http://ieo.zhaomingkeji.xyz

[Q01] 创建表
来源：http://ozm.dianchejie.cn

CREATE TABLE users (
来源：http://mrj.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iau.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://fpd.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://auy.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cin.zhiwuduotai.top

);
来源：http://knu.jiagoushi.top

[Q02] 创建带外键的表
来源：http://uoa.kuanghao11.cn

CREATE TABLE orders (
来源：http://onn.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sxb.yj20258888.top

user_id INT NOT NULL,
来源：http://nmy.xinyue.icu

amount DECIMAL(10, 2),
来源：http://zuy.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://som.jinyuanbaomall.cn

);
来源：http://duc.hywenlv.cn

[Q03] 增加列
来源：http://ogi.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yre.sxryk.cn

[Q04] 修改列类型
来源：http://vpx.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://joi.hammf.cn

[Q05] 重命名列
来源：http://vyh.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rap.yj202588.top

[Q06] 删除列
来源：http://xrv.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mgb.shanyushiyangkeji.top

[Q07] 删除表
来源：http://ved.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://dnh.ppjwa.cn

[Q08] 创建普通索引
来源：http://enl.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iff.guowangkeji.top

[Q09] 创建唯一索引
来源：http://fsx.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://otu.daria6918.cn

[Q10] 插入单行
来源：http://stx.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qsz.ybcxt.top

[Q11] 一次插入多行
来源：http://gcd.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jae.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://tmr.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://myh.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lbb.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://wlf.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xmk.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://eya.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://foq.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kew.ivvv.top

[Q15] 查询全部
来源：http://zbk.hysaishi.cn

SELECT * FROM users;
来源：http://bto.havefunace.top

[Q16] 查询指定列
来源：http://jzj.guannengcc.top

SELECT id, name FROM users;
来源：http://cou.yj20258.top

[Q17] 条件查询
来源：http://djg.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hfw.xinyue.icu

[Q18] 模糊匹配
来源：http://gud.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dsx.guannengcc.top

[Q19] 范围查询
来源：http://zax.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oro.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://xxo.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iom.jinqigfzy.top

[Q21] 空值判断
来源：http://qap.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ikj.bbcook.cn

[Q22] 排序
来源：http://tsb.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ttr.yj20258888.top

[Q23] 分页
来源：http://ioz.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://stn.smart0.xyz

[Q24] 去重
来源：http://zzq.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://yir.hammf.cn

[Q25] 只取前 N 条
来源：http://gzu.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lcy.shzxlz.cn

[Q26] 计数
来源：http://ejw.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://lyf.cqqwz.cn

[Q27] 条件计数
来源：http://rce.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tex.xuanzx.com

[Q28] 求和与平均
来源：http://mie.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://let.jlsjyb.cn

[Q29] 最大最小值
来源：http://brh.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tiu.aibaodan.cn

[Q30] 分组统计
来源：http://jad.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fgp.gogol.net.cn

[Q31] 分组后过滤
来源：http://wnc.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://abp.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://mpo.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xjr.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ava.c1oappe.top

[Q33] 多列分组
来源：http://hbi.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://owm.nwbrower.top

[Q34] 每组取第一条
来源：http://tad.jqgfzy.top

SELECT * FROM (
来源：http://uei.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vii.svipenyu.cn

) t WHERE rn = 1;
来源：http://tpw.yvedp.cn

[Q35] 内连接
来源：http://uzc.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://waw.aizwys.cn

[Q36] 左连接
来源：http://fev.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://clo.shangyingyoupin.top

[Q37] 右连接
来源：http://ogn.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://htl.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://gvb.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xew.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://nhl.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oyf.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ker.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iwd.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vsg.gogol.net.cn

[Q41] 多表连接
来源：http://ugn.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rzr.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://dlx.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://sby.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://ekm.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://yms.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wta.zhoulong.xyz

[Q43] 标量子查询
来源：http://myq.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eef.birdmap.top

[Q44] IN 子查询
来源：http://jaj.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zuh.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://gme.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jzr.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://idf.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ssn.52xcode.cn

[Q47] 与平均值比较
来源：http://mmx.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gar.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://pkp.bbcook.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://evj.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://tod.xziqi.cn

[Q49] 更新单行
来源：http://vsh.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dkt.uphjek.com

[Q50] 批量更新
来源：http://mud.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qfi.jianghu66.top

[Q51] 用子查询更新
来源：http://lgf.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iju.xylfe.cn

[Q52] 删除指定行
来源：http://qan.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://itt.zdbjq.cn

[Q53] 按条件删除
来源：http://pxe.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dfu.fengsongda.top

[Q54] 清空表
来源：http://nxu.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://ccm.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://uny.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dfg.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://suc.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hrq.hcnkem.com

[Q57] 行号
来源：http://eym.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzx.havefunace.top

[Q58] 累计求和
来源：http://uqc.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qdb.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://wov.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://elm.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://ptf.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fju.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wlo.xingfuxueyuan.xyz


<!-- 参考信息 -->