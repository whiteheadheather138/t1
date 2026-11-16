代发 wailian999

Py:   itertools.permutations(arr)
来源：http://jqy.xylfe.cn

PHP:  // 手写递归交换
来源：http://zsr.smart0.xyz

JS:   // 手写回溯递归
来源：http://foa.9152youxi.cn

TS:   // 手写回溯递归
来源：http://lxc.aibaodan.cn

Java: // 手写回溯递归
来源：http://ijq.bjfxy.top

Go:   // 手写回溯递归
来源：http://aig.yongpay.top

Ruby: arr.permutation.to_a
来源：http://wnd.yj202588.top

C#:   // 手写回溯递归
来源：http://rju.hnxiangtu.top

[N09] 栈与队列
来源：http://xaj.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kon.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tbh.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ftb.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mae.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://plc.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sax.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://efd.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vyx.fzhhl.top

[N10] 链表节点定义
来源：http://zol.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gjs.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://udj.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ywl.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iol.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://tgy.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://dwd.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sch.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://thp.wangdashe.top

[N11] 二叉树中序遍历
来源：http://lqp.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hpr.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://gda.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ywg.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgh.yueranfly.top

Java: // 手写递归
来源：http://vxw.zhengqikj.top

Go:   // 手写递归
来源：http://ftf.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zaw.hnqzz.top

C#:   // 手写递归
来源：http://tab.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mxb.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aub.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bbk.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgh.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uvv.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ezl.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yev.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://let.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nji.jqgfzy.top

================================================================================
来源：http://ccn.haohaochexian.top

O. 并发与异步
来源：http://udh.gogol.net.cn

================================================================================
来源：http://dws.yuanzhike.top

[O01] 启动一个线程
来源：http://sae.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rft.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tba.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yyo.zhiwuduotai.top

TS:   // 同 JS
来源：http://dhy.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://edk.bbcook.cn

Go:   go f()
来源：http://lew.xylfe.cn

Ruby: Thread.new { f }
来源：http://wng.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://fmk.jinqigufen.top

[O02] 使用线程池
来源：http://rtv.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tuj.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fpi.hammf.cn

JS:   // worker_threads 线程池
来源：http://xnk.hammf.cn

TS:   // worker_threads 线程池
来源：http://tyj.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://hal.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yma.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gay.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hyw.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://rcu.haohaochexian.top

Py:   with lock: shared += 1
来源：http://xnj.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://hur.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://edm.hfpthk.cn

TS:   // 同 JS
来源：http://pyg.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://utq.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wyr.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tcn.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://rcd.uphjek.com

[O04] 定义异步函数并等待
来源：http://cmb.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://czo.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aux.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://nru.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cud.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://adg.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hbp.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dfr.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://asj.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://knp.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://far.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xua.yonumen.top

JS:   await Promise.all(tasks)
来源：http://pbf.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://uqi.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kdj.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uwv.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://lsm.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fon.cdnleiting.top

[O06] 使用进程池
来源：http://rtf.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lac.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://oft.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://huv.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://nmj.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mim.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://byd.pycfn.com

Ruby: // fork 块
来源：http://upm.fehbvm.com

C#:   Parallel.For
来源：http://gma.cqqwz.cn

================================================================================
来源：http://xqf.chenlongwang.top

P. 常用工具函数
来源：http://lgj.fengsongda.top

================================================================================
来源：http://jrl.gotoacloud.top

[P01] 生成 UUID
来源：http://qpi.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://hke.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hbm.mhx1999.top

JS:   crypto.randomUUID()
来源：http://rzh.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://ozi.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://sng.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://tcl.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://eyp.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://fxs.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://iht.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dgb.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yie.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ohp.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://swb.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kpu.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mex.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fes.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fni.zycfv.cn

[P03] 生成短随机字符串
来源：http://dri.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fbe.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bem.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kek.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lma.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eqf.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lkh.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ctm.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qgk.xuanzx.com

[P04] 求长度
来源：http://qlc.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hkt.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhx.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urj.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cuo.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://pef.nwbrower.top

Go:   len(arr);  len(m)
来源：http://upt.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://ugd.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nkg.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://yps.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sru.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dsa.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hge.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bov.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xxr.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://snp.shanyushiyangkeji.top

Ruby: a == b
来源：http://ipn.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://std.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cnr.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kpf.xinyue.icu

PHP:  if (empty($x)) {}
来源：http://tzz.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bdy.andypj.xyz

TS:   if (x == null) {}
来源：http://anl.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jho.shzxlz.cn

Go:   if x == nil {}
来源：http://hvt.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mjn.yangfankeji.com

C#:   if (x is null) {}
来源：http://hgt.smart0.xyz

[P07] 防抖与节流
来源：http://yqc.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://exo.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://oot.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ogh.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vuj.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nla.svipenyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://asl.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bwu.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kev.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://dqe.cdnleiting.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ser.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kfr.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spj.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fdt.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kfm.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jwf.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://syw.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mtm.hfpthk.cn

================================================================================
来源：http://pby.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ndp.jianghu66.top

================================================================================
来源：http://rsq.aizwys.cn

[Q01] 创建表
来源：http://hgm.jianghu66.top

CREATE TABLE users (
来源：http://mfs.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lot.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://urg.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://wuf.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xmy.guowangkeji.top

);
来源：http://cng.iojbl.cn

[Q02] 创建带外键的表
来源：http://bqz.ybcxt.top

CREATE TABLE orders (
来源：http://ngk.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nws.bbcook.cn

user_id INT NOT NULL,
来源：http://jra.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://hxj.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fiw.sweek.top

);
来源：http://vhy.vehdjk.com

[Q03] 增加列
来源：http://ing.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hfv.yongpay.top

[Q04] 修改列类型
来源：http://pfe.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zab.tarul.cn

[Q05] 重命名列
来源：http://dcp.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhx.cashguo.top

[Q06] 删除列
来源：http://mml.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://efh.fanxiaobao.xyz

[Q07] 删除表
来源：http://dch.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://ojw.zycfv.cn

[Q08] 创建普通索引
来源：http://fop.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ece.0kj1m.cn

[Q09] 创建唯一索引
来源：http://gfh.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zjd.ehwqpu.com

[Q10] 插入单行
来源：http://lxe.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zmh.yueranfly.top

[Q11] 一次插入多行
来源：http://ups.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pkl.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://egq.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://god.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ume.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://sru.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sys.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://tms.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mqc.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fme.jianghu66.top

[Q15] 查询全部
来源：http://uma.zhoulong.xyz

SELECT * FROM users;
来源：http://qyr.nanxinkj.top

[Q16] 查询指定列
来源：http://mwy.xinyue.icu

SELECT id, name FROM users;
来源：http://tcb.cqqwz.cn

[Q17] 条件查询
来源：http://eag.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kro.yueranfly.top

[Q18] 模糊匹配
来源：http://yok.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vbw.fzhhl.top

[Q19] 范围查询
来源：http://zrv.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pvt.gogol.net.cn

[Q20] IN 列表
来源：http://kjo.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kvv.gzhubu.top

[Q21] 空值判断
来源：http://lej.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rwp.jinyuanbaomall.cn

[Q22] 排序
来源：http://oed.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iju.jinghuilouyu.cn

[Q23] 分页
来源：http://xxz.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uyc.zhoulong.xyz

[Q24] 去重
来源：http://atc.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://lkb.hammf.cn

[Q25] 只取前 N 条
来源：http://xuj.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ddd.hywenlv.cn

[Q26] 计数
来源：http://ipg.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://cjh.hnqzz.top

[Q27] 条件计数
来源：http://xcu.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kak.gotoacloud.top

[Q28] 求和与平均
来源：http://dai.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://phn.fzhhl.top

[Q29] 最大最小值
来源：http://lta.hywenlv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aso.zdbjq.cn

[Q30] 分组统计
来源：http://aio.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rlr.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://ybc.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zfa.xylfe.cn

[Q32] 分组拼接字符串
来源：http://zuw.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hap.jinyuanbaomall.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nmv.jianghu66.top

[Q33] 多列分组
来源：http://ygl.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://exs.aibaodan.cn

[Q34] 每组取第一条
来源：http://rgq.chenlongwang.top

SELECT * FROM (
来源：http://egv.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rsf.yuxming.cn

) t WHERE rn = 1;
来源：http://tur.shuidangran.top

[Q35] 内连接
来源：http://hoo.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jok.ivvv.top

[Q36] 左连接
来源：http://ptd.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ama.jinqigfzy.top

[Q37] 右连接
来源：http://sdm.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xcs.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://sdt.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ymp.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://zab.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://may.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jxy.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xdn.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sdx.guannengcc.top

[Q41] 多表连接
来源：http://bcz.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rii.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://dab.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://dpy.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://ywx.jyoumei.cn

SELECT u.name, o.amount FROM users u
来源：http://soy.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yet.zhongyouzk.top

[Q43] 标量子查询
来源：http://usa.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://beh.yj20258.top

[Q44] IN 子查询
来源：http://avi.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nah.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://aly.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zxh.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://krr.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pxs.yj20258888.top

[Q47] 与平均值比较
来源：http://zaw.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lqn.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://hgl.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wfs.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ncb.ehwqpu.com

[Q49] 更新单行
来源：http://tmv.ywan-chungtsiang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dku.aizwys.cn

[Q50] 批量更新
来源：http://aev.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gnp.dashuyun.cn

[Q51] 用子查询更新
来源：http://frv.birdmap.top


<!-- 参考信息 -->