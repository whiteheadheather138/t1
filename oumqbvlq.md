代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://apx.redwolf501.top

[N10] 链表节点定义
来源：http://blf.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kxc.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nij.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://byk.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ggp.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://fre.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://don.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pcz.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://aqf.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://ejt.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://npz.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://ele.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hyo.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eka.nwbrower.top

Java: // 手写递归
来源：http://pto.snrcjt.cn

Go:   // 手写递归
来源：http://dex.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qzf.sufxvd.cn

C#:   // 手写递归
来源：http://rpk.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bgt.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ror.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dqm.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aef.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xlg.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://atv.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uoa.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tqx.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ujd.tianlin.xyz

================================================================================
来源：http://rby.ctjpmb.com

O. 并发与异步
来源：http://hwl.shangyingyoupin.top

================================================================================
来源：http://rhp.zhixingplan.top

[O01] 启动一个线程
来源：http://bkf.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xte.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aqs.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://csb.gzhubu.top

TS:   // 同 JS
来源：http://krm.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://alg.vqdsnc.cn

Go:   go f()
来源：http://vyb.xziqi.cn

Ruby: Thread.new { f }
来源：http://ccj.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://fxk.0kj1m.cn

[O02] 使用线程池
来源：http://lkh.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bcx.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://owc.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://rca.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://gnt.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gpd.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://skb.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pku.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://waf.cashguo.top

[O03] 加锁保护共享数据
来源：http://lte.jianghu66.top

Py:   with lock: shared += 1
来源：http://vvo.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xdm.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ksj.sufxvd.cn

TS:   // 同 JS
来源：http://zot.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://wxs.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cle.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://orv.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://jvl.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://esj.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://cza.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eww.cucudq.cn

JS:   async function f() { await g(); }
来源：http://mqm.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kff.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwb.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eot.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://kba.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://thj.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://dlx.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://kej.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qki.ivvv.top

JS:   await Promise.all(tasks)
来源：http://hsq.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://sqc.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uek.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jdt.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://qmc.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://guy.jinghuilouyu.cn

[O06] 使用进程池
来源：http://oad.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ttw.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bgf.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://jvi.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://zfc.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dra.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aoo.cheryme.top

Ruby: // fork 块
来源：http://oqi.quarkkingdee.top

C#:   Parallel.For
来源：http://rls.snrcjt.cn

================================================================================
来源：http://blq.sjlbkw.cn

P. 常用工具函数
来源：http://ssx.vehdjk.com

================================================================================
来源：http://ezz.yj20258.top

[P01] 生成 UUID
来源：http://ehz.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://nog.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ftb.yfazqb.com

JS:   crypto.randomUUID()
来源：http://eal.tarul.cn

TS:   crypto.randomUUID()
来源：http://jhz.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://bzo.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://rgu.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://xeo.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://afn.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://uih.cdnleiting.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://njp.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vaw.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rfu.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wkz.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bkp.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yfz.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://syw.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://azb.c1oappe.top

[P03] 生成短随机字符串
来源：http://uqf.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cse.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rbp.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://str.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zzh.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wwm.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qwa.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rgh.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qla.pengpengdd.cyou

[P04] 求长度
来源：http://var.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://swn.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmq.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xoa.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lsz.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://lud.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://uie.hcnkem.com

Ruby: x.length;  x.size
来源：http://lun.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mwk.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://kra.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rxf.dianchejie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yvw.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rfq.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cmb.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aau.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://qbd.zhixingplan.top

Ruby: a == b
来源：http://wgr.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cab.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rqq.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dmy.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://cei.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kmz.shuidangran.top

TS:   if (x == null) {}
来源：http://ztz.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uyj.svipenyu.cn

Go:   if x == nil {}
来源：http://pak.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yer.yanxiufei.cn

C#:   if (x is null) {}
来源：http://bxq.wangshuangyany.cn

[P07] 防抖与节流
来源：http://xtw.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vpl.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://hbw.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fuh.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ode.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ttf.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nrw.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vnn.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nxn.hesvh.cn

[P08] 处理浮点精度问题
来源：http://let.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ldo.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bdg.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yyo.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dun.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nxi.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yep.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zun.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rht.daria6918.cn

================================================================================
来源：http://yfw.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tvv.sysykeji.top

================================================================================
来源：http://dut.tarul.cn

[Q01] 创建表
来源：http://ptb.0kj1m.cn

CREATE TABLE users (
来源：http://env.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iif.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://gve.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://ldg.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hqo.gotoacloud.top

);
来源：http://zjo.wangdashe.top

[Q02] 创建带外键的表
来源：http://bwl.shzxlz.cn

CREATE TABLE orders (
来源：http://jbv.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cqj.jinqigfzy.top

user_id INT NOT NULL,
来源：http://qci.bbcook.cn

amount DECIMAL(10, 2),
来源：http://mwy.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wel.xylfe.cn

);
来源：http://kmr.nanxuanxn.top

[Q03] 增加列
来源：http://xzk.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ibn.jqgfzy.top

[Q04] 修改列类型
来源：http://gow.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jzk.nanxuanxn.top

[Q05] 重命名列
来源：http://nxt.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cva.shanyushiyangkeji.top

[Q06] 删除列
来源：http://cbp.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pqh.jlsjyb.cn

[Q07] 删除表
来源：http://hgk.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://oia.sxryk.cn

[Q08] 创建普通索引
来源：http://pjc.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ehv.shuidangran.top

[Q09] 创建唯一索引
来源：http://bbg.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://opu.aizwys.cn

[Q10] 插入单行
来源：http://lcv.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qev.jinqigfzy.top

[Q11] 一次插入多行
来源：http://iva.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://llu.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://qaf.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fzt.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tdk.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://prt.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jki.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://kex.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wum.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://syq.cashguo.top

[Q15] 查询全部
来源：http://glt.tarul.cn

SELECT * FROM users;
来源：http://hib.zhijiandao.cn

[Q16] 查询指定列
来源：http://ief.yongpay.top

SELECT id, name FROM users;
来源：http://cfj.zycfv.cn

[Q17] 条件查询
来源：http://oqh.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ijp.shuidangran.top

[Q18] 模糊匹配
来源：http://tyb.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mzs.shzxlz.cn

[Q19] 范围查询
来源：http://poh.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qaz.dianchejie.cn

[Q20] IN 列表
来源：http://nxf.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oup.aizwys.cn

[Q21] 空值判断
来源：http://aux.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://usu.hesvh.cn

[Q22] 排序
来源：http://yia.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hyd.jqgfzy.top

[Q23] 分页
来源：http://eop.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rgf.hfpthk.cn

[Q24] 去重
来源：http://ocu.sweek.top

SELECT DISTINCT city FROM users;
来源：http://lah.sweek.top

[Q25] 只取前 N 条
来源：http://vbs.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://igz.jinyuanbaomall.cn

[Q26] 计数
来源：http://rpk.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://rdr.9152youxi.cn

[Q27] 条件计数
来源：http://bfb.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bbv.jqgfzy.top

[Q28] 求和与平均
来源：http://lwu.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xqc.jinqigfzy.top

[Q29] 最大最小值
来源：http://hvl.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xar.jinghuilouyu.cn

[Q30] 分组统计
来源：http://hfc.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yip.shzxlz.cn

[Q31] 分组后过滤
来源：http://jlb.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nbh.tarul.cn

[Q32] 分组拼接字符串
来源：http://vla.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jnk.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yiu.zhiwuduotai.top

[Q33] 多列分组
来源：http://zgj.zycfv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cuo.aibaodan.cn

[Q34] 每组取第一条
来源：http://wro.shuidangran.top

SELECT * FROM (
来源：http://xov.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://spm.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://koj.bjfxy.top

[Q35] 内连接
来源：http://pzq.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pdi.jqgufenzy.top

[Q36] 左连接
来源：http://vof.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tzi.ppjwa.cn

[Q37] 右连接
来源：http://xcr.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://paa.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://amh.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bho.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://dcb.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://myq.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://osr.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rzj.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qxm.yongpay.top

[Q41] 多表连接
来源：http://cvx.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kyd.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://aor.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://tpo.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://jwj.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://pbc.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xbq.meibo888.top

[Q43] 标量子查询
来源：http://zum.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bvr.pengpengdd.cyou

[Q44] IN 子查询
来源：http://iec.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lmg.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://hrg.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xla.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nlk.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hnn.zhoulong.xyz

[Q47] 与平均值比较
来源：http://git.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zst.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://ajb.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dso.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://bto.yj20258888.top

[Q49] 更新单行
来源：http://hrv.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lgv.jqgfzy.top

[Q50] 批量更新
来源：http://gew.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eaj.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://avj.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blz.birdmap.top

[Q52] 删除指定行
来源：http://hro.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://xyd.andypj.xyz

[Q53] 按条件删除
来源：http://jxs.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hlx.xuanzx.com

[Q54] 清空表
来源：http://jwz.nwbrower.top

TRUNCATE TABLE logs;
来源：http://ebk.yuxming.cn

[Q55] 排名（并列占位）
来源：http://muu.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pmr.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://jsf.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lmt.shanyushiyangkeji.top

[Q57] 行号
来源：http://ohn.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wdo.52xcode.cn

[Q58] 累计求和
来源：http://dkw.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gbd.sxryk.cn

[Q59] 分组内累计
来源：http://fvs.sweek.top


<!-- 参考信息 -->