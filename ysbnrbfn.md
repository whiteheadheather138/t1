代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://niz.hongshengwenyu.top

[N10] 链表节点定义
来源：http://xsp.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lym.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jls.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zvo.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://drb.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://sjl.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://xbq.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bgt.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xna.xziqi.cn

[N11] 二叉树中序遍历
来源：http://dfs.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cow.daxiang520.top

PHP:  // 手写递归函数
来源：http://cyx.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rpk.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eau.fktsv.cn

Java: // 手写递归
来源：http://vlj.sweek.top

Go:   // 手写递归
来源：http://qbf.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hni.fehbvm.com

C#:   // 手写递归
来源：http://jvr.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzu.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rmy.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jcw.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yvh.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://atv.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wbd.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cpf.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://npn.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lrb.svipenyu.cn

================================================================================
来源：http://zmf.redwolf501.top

O. 并发与异步
来源：http://hjz.xuanzx.com

================================================================================
来源：http://vdb.yfazqb.com

[O01] 启动一个线程
来源：http://whn.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ljc.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qcp.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eqv.0kj1m.cn

TS:   // 同 JS
来源：http://ujg.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://sug.pengpengdd.cyou

Go:   go f()
来源：http://gcw.wangdashe.top

Ruby: Thread.new { f }
来源：http://kng.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://yyn.cucudq.cn

[O02] 使用线程池
来源：http://jyn.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eat.hongshengwenyu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ngk.hammf.cn

JS:   // worker_threads 线程池
来源：http://ufg.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://vwp.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sbn.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wox.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gog.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jmo.xuanzx.com

[O03] 加锁保护共享数据
来源：http://pod.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://eyt.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://kue.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://spn.jlsjyb.cn

TS:   // 同 JS
来源：http://kno.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://rbk.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://thf.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://taz.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://jov.zycfv.cn

[O04] 定义异步函数并等待
来源：http://lkk.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://loz.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sdi.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://gdg.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://juk.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://slx.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yqt.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://ezt.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://rtt.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://ggr.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://cvz.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qdy.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://rec.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://lch.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://raj.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dor.sysykeji.top

Ruby: threads.map(&:join)
来源：http://vjs.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gjk.cheryme.top

[O06] 使用进程池
来源：http://hrh.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ait.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sqp.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://bfs.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://smb.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uty.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kry.zycfv.cn

Ruby: // fork 块
来源：http://svn.hysaishi.cn

C#:   Parallel.For
来源：http://gxp.chenzaomai.com

================================================================================
来源：http://crw.redwolf501.top

P. 常用工具函数
来源：http://zkt.chenjidiqi.icu

================================================================================
来源：http://drb.sjlbkw.cn

[P01] 生成 UUID
来源：http://vam.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://psb.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oxk.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://xlo.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://niq.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://bmc.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://abc.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://hig.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://cst.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://ouj.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wub.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tnd.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jwx.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hjt.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://imn.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rnb.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mnx.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jtm.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://pes.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nja.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://obs.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xrh.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://too.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hmz.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://klw.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sla.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tlw.zdbjq.cn

[P04] 求长度
来源：http://zgr.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://txq.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qvn.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wmi.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bes.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://arq.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://jgm.meibo888.top

Ruby: x.length;  x.size
来源：http://dqt.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://shl.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://ybk.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dul.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fjv.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nmu.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uut.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kgc.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kdi.fengsongda.top

Ruby: a == b
来源：http://lhm.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eby.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vnc.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mnd.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://kzl.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aiz.zhijiandao.cn

TS:   if (x == null) {}
来源：http://ybx.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://csu.nanxuanxn.top

Go:   if x == nil {}
来源：http://cnw.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ajo.meibo888.top

C#:   if (x is null) {}
来源：http://uoc.bjfxy.top

[P07] 防抖与节流
来源：http://bbd.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lla.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://hnc.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gey.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qab.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zod.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nbo.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dhh.ydzc1.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://upx.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://pre.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rxr.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wuf.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vee.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eld.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gdw.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bgj.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bvk.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pwj.ywan-chungtsiang.top

================================================================================
来源：http://yqz.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://grw.shangyingyoupin.top

================================================================================
来源：http://app.dianchejie.cn

[Q01] 创建表
来源：http://cwl.tian-w.cn

CREATE TABLE users (
来源：http://ner.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ffw.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://ndj.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://wte.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zvn.jlsjyb.cn

);
来源：http://ofa.pycfn.com

[Q02] 创建带外键的表
来源：http://fpr.9152youxi.cn

CREATE TABLE orders (
来源：http://hjf.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qyx.cashguo.top

user_id INT NOT NULL,
来源：http://jsy.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://mxm.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jyi.kuanghao11.cn

);
来源：http://vsi.xuanzx.com

[Q03] 增加列
来源：http://qny.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kip.daria6918.cn

[Q04] 修改列类型
来源：http://nxj.gotoacloud.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://adz.smart0.xyz

[Q05] 重命名列
来源：http://brg.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rgk.c1oappe.top

[Q06] 删除列
来源：http://lbl.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://llq.jinqigfzy.top

[Q07] 删除表
来源：http://vuj.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://noj.xuanzx.com

[Q08] 创建普通索引
来源：http://fdy.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://unt.smart0.xyz

[Q09] 创建唯一索引
来源：http://xds.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rps.iojbl.cn

[Q10] 插入单行
来源：http://lym.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ddm.yuxming.cn

[Q11] 一次插入多行
来源：http://jwn.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vxs.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://vqn.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://bow.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lap.hfpthk.cn

[Q13] 忽略重复插入
来源：http://xdj.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cwd.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://cht.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://imx.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kvc.zycfv.cn

[Q15] 查询全部
来源：http://azi.dashuyun.cn

SELECT * FROM users;
来源：http://acx.hfpthk.cn

[Q16] 查询指定列
来源：http://kyn.mhx1999.top

SELECT id, name FROM users;
来源：http://twx.shzxlz.cn

[Q17] 条件查询
来源：http://cpw.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tkf.hywenlv.cn

[Q18] 模糊匹配
来源：http://xwq.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ufo.fzhhl.top

[Q19] 范围查询
来源：http://wln.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ysk.zhiwuduotai.top

[Q20] IN 列表
来源：http://xkd.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ttd.ctjpmb.com

[Q21] 空值判断
来源：http://drv.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mxe.ybcxt.top

[Q22] 排序
来源：http://xww.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://slc.jinqigfzy.top

[Q23] 分页
来源：http://lrv.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lvk.jinqigfzy.top

[Q24] 去重
来源：http://cga.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://cgd.jqgfzy.top

[Q25] 只取前 N 条
来源：http://hju.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dkp.tian-w.cn

[Q26] 计数
来源：http://bny.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://ijw.nwbrower.top

[Q27] 条件计数
来源：http://tyz.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://egm.sxryk.cn

[Q28] 求和与平均
来源：http://yxs.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jve.jqgufenzy.top

[Q29] 最大最小值
来源：http://zcw.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cdo.birdmap.top

[Q30] 分组统计
来源：http://jew.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eoc.sjlbkw.cn

[Q31] 分组后过滤
来源：http://isr.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nvc.ydzc1.top

[Q32] 分组拼接字符串
来源：http://mdi.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pao.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fvn.yuxming.cn

[Q33] 多列分组
来源：http://ioc.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qom.nanxuanxn.top

[Q34] 每组取第一条
来源：http://fae.sufxvd.cn

SELECT * FROM (
来源：http://rtn.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bcd.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://rzl.vehdjk.com

[Q35] 内连接
来源：http://qte.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mcz.jqgufenzy.top

[Q36] 左连接
来源：http://enj.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dbo.gaohongyu789.top

[Q37] 右连接
来源：http://pay.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tuw.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://gxp.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfr.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://kyt.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bwu.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lrs.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://dnm.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qmu.havefunace.top

[Q41] 多表连接
来源：http://cij.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://kal.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://wqe.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://qrp.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://ijd.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://xqm.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://seo.zhoulong.xyz

[Q43] 标量子查询
来源：http://wyf.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gzy.zhengqikj.top

[Q44] IN 子查询
来源：http://kco.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uys.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://uwm.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bia.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://dgd.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nll.epnwcf.com

[Q47] 与平均值比较
来源：http://bhs.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iol.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://jyt.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dhj.guannengcc.top

SELECT * FROM t WHERE c > 5;
来源：http://tty.gaohongyu789.top

[Q49] 更新单行
来源：http://kfc.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bsv.ivvv.top

[Q50] 批量更新
来源：http://qqf.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hyf.chenzaomai.com

[Q51] 用子查询更新
来源：http://son.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lhz.hammf.cn

[Q52] 删除指定行
来源：http://tdl.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://rip.sufxvd.cn

[Q53] 按条件删除
来源：http://eaz.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dbp.yanxiufei.cn

[Q54] 清空表
来源：http://mau.cheryme.top

TRUNCATE TABLE logs;
来源：http://ybb.hammf.cn

[Q55] 排名（并列占位）
来源：http://rpp.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vcc.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://jhq.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lap.daria6918.cn

[Q57] 行号
来源：http://fwm.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rzv.cdnleiting.top

[Q58] 累计求和
来源：http://dof.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jna.guannengcc.top

[Q59] 分组内累计
来源：http://pat.yonumen.top


<!-- 参考信息 -->