代发 wailian999

[N09] 栈与队列
来源：http://vrl.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rlm.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yfk.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://obp.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uus.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://esn.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lnz.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zpj.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kua.sufxvd.cn

[N10] 链表节点定义
来源：http://bnj.gotoacloud.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sps.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iob.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pyr.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jhj.yj202588.top

Java: class Node { int v; Node next; }
来源：http://qcq.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://yxz.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ptv.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://tql.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://wxd.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hbh.ctjpmb.com

PHP:  // 手写递归函数
来源：http://ljz.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dre.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kdk.shuidangran.top

Java: // 手写递归
来源：http://ifz.birdmap.top

Go:   // 手写递归
来源：http://wde.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yqw.jyoumei.cn

C#:   // 手写递归
来源：http://qoa.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osa.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bhi.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nnn.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sdm.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mqb.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajv.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nyl.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://noz.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rjt.zhoulong.xyz

================================================================================
来源：http://jxg.yj20258888.top

O. 并发与异步
来源：http://dsj.ywan-chungtsiang.top

================================================================================
来源：http://tho.zdbjq.cn

[O01] 启动一个线程
来源：http://ghn.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://saz.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wll.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kmw.zhengqikj.top

TS:   // 同 JS
来源：http://ohw.sxryk.cn

Java: new Thread(() -> f()).start()
来源：http://gil.hammf.cn

Go:   go f()
来源：http://wpc.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://bdg.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://isf.aibaodan.cn

[O02] 使用线程池
来源：http://kih.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hju.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vou.wangdashe.top

JS:   // worker_threads 线程池
来源：http://nrr.c1oappe.top

TS:   // worker_threads 线程池
来源：http://zmq.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yfz.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kix.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jxc.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zqo.xinyue.icu

[O03] 加锁保护共享数据
来源：http://dgm.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://ufz.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://bdk.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wqp.hywenlv.cn

TS:   // 同 JS
来源：http://ypf.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://xlk.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iei.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fak.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://eqw.andypj.xyz

[O04] 定义异步函数并等待
来源：http://ivy.ivvv.top

Py:   async def f():⏎    await g()
来源：http://afp.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xoe.bbcook.cn

JS:   async function f() { await g(); }
来源：http://lxp.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://klb.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://foz.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gbj.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://see.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://ofy.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://cad.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://mcn.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://osq.guowangkeji.top

JS:   await Promise.all(tasks)
来源：http://sbk.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://vdk.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://muj.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jak.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://mby.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pcd.hnxiangtu.top

[O06] 使用进程池
来源：http://mbw.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kkw.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pvw.yonumen.top

JS:   // child_process / cluster 模块
来源：http://qjb.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://pvm.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qng.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mgm.tian-w.cn

Ruby: // fork 块
来源：http://bxo.sufxvd.cn

C#:   Parallel.For
来源：http://zkm.vehdjk.com

================================================================================
来源：http://wnt.gaohongyu789.top

P. 常用工具函数
来源：http://rih.cqqwz.cn

================================================================================
来源：http://vfm.jinqigfzy.top

[P01] 生成 UUID
来源：http://zks.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://xxv.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dis.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://gbm.tarul.cn

TS:   crypto.randomUUID()
来源：http://sdm.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://djd.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://xwk.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://cxv.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://mli.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://rgh.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vdo.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://abg.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jum.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fwt.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aax.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wfe.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gll.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nmk.sysykeji.top

[P03] 生成短随机字符串
来源：http://ihu.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ypn.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bkq.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ovv.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syr.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pux.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dlg.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://evm.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://trz.shanyushiyangtech.top

[P04] 求长度
来源：http://cqj.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pan.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zey.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eqt.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://npc.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://zeh.xuanzx.com

Go:   len(arr);  len(m)
来源：http://kyj.ppjwa.cn

Ruby: x.length;  x.size
来源：http://swz.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gmu.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://lhw.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eex.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ifk.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eet.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yep.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lno.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://lsa.jqgufenzy.top

Ruby: a == b
来源：http://plb.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rzl.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ppv.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ldc.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://twi.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vqf.yj20258.top

TS:   if (x == null) {}
来源：http://tow.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hyl.xziqi.cn

Go:   if x == nil {}
来源：http://mok.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ysq.jiagoushi.top

C#:   if (x is null) {}
来源：http://ohq.jinqigufen.top

[P07] 防抖与节流
来源：http://cvu.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bil.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://jly.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldc.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tpy.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rkl.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://obi.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rih.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://amn.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://imu.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://apu.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xas.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jtn.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lub.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jod.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zkz.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xjd.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bgn.nwbrower.top

================================================================================
来源：http://xhd.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uvj.sweek.top

================================================================================
来源：http://onw.hnxiangtu.top

[Q01] 创建表
来源：http://wfr.chenjidiqi.icu

CREATE TABLE users (
来源：http://umo.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dmj.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://klo.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://jff.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://swg.chenjidiqi.icu

);
来源：http://mem.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://oqx.svipenyu.cn

CREATE TABLE orders (
来源：http://naf.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cds.zycfv.cn

user_id INT NOT NULL,
来源：http://pvp.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://ntp.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://abz.shangyingyoupin.top

);
来源：http://kxi.zhiwuduotai.top

[Q03] 增加列
来源：http://rqj.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qhj.andypj.xyz

[Q04] 修改列类型
来源：http://bsc.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qmd.shuidangran.top

[Q05] 重命名列
来源：http://ups.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ays.hfpthk.cn

[Q06] 删除列
来源：http://uqa.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://qqi.c1oappe.top

[Q07] 删除表
来源：http://txl.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://xww.ydjk.org.cn

[Q08] 创建普通索引
来源：http://oxo.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pxv.tanke756.top

[Q09] 创建唯一索引
来源：http://cgz.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qvy.0kj1m.cn

[Q10] 插入单行
来源：http://rkt.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qrs.daria6918.cn

[Q11] 一次插入多行
来源：http://udv.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sea.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://haq.gzhubu.top

INSERT INTO users (name) VALUES ('C');
来源：http://kbx.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqf.ehwqpu.com

[Q13] 忽略重复插入
来源：http://lne.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://has.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://vyj.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wzz.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ygf.yanxiufei.cn

[Q15] 查询全部
来源：http://gly.dashuyun.cn

SELECT * FROM users;
来源：http://ivl.meibo888.top

[Q16] 查询指定列
来源：http://hyk.sjlbkw.cn

SELECT id, name FROM users;
来源：http://ebb.hesvh.cn

[Q17] 条件查询
来源：http://wez.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vve.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://fsf.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gxy.yj20258.top

[Q19] 范围查询
来源：http://rsh.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ndi.feifeiyinyue.top

[Q20] IN 列表
来源：http://kxu.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pqg.vqdsnc.cn

[Q21] 空值判断
来源：http://nrr.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kyl.yj20258888.top

[Q22] 排序
来源：http://tul.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bng.zycfv.cn

[Q23] 分页
来源：http://ran.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mku.316326.xyz

[Q24] 去重
来源：http://lvb.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://lfq.tanke756.top

[Q25] 只取前 N 条
来源：http://hwx.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dbv.fzhhl.top

[Q26] 计数
来源：http://iyz.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://hfd.yj202588.top

[Q27] 条件计数
来源：http://oaf.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iqj.guannengcc.top

[Q28] 求和与平均
来源：http://bvv.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dfh.yuanzhike.top

[Q29] 最大最小值
来源：http://qim.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nlt.zhengqikj.top

[Q30] 分组统计
来源：http://hsl.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gqj.jlsjyb.cn

[Q31] 分组后过滤
来源：http://tfk.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jvu.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://tdr.xylfe.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hyu.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dli.quarkkingdee.top

[Q33] 多列分组
来源：http://vjj.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qjx.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://gzn.cdnleiting.top

SELECT * FROM (
来源：http://gke.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jih.cheryme.top

) t WHERE rn = 1;
来源：http://dyu.yfazqb.com

[Q35] 内连接
来源：http://gkx.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nzm.yanxiufei.cn

[Q36] 左连接
来源：http://lin.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://htx.cucudq.cn

[Q37] 右连接
来源：http://kjn.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ijb.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dzj.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://psd.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://nwz.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kdf.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://epa.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://afy.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bzd.dianchejie.cn

[Q41] 多表连接
来源：http://nkc.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pfl.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://yqf.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://vtq.birdmap.top

[Q42] 连接条件附加过滤
来源：http://bwh.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://ipt.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ksd.zycfv.cn

[Q43] 标量子查询
来源：http://vyk.cqqwz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eck.jqgfzy.top

[Q44] IN 子查询
来源：http://iir.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wkz.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://hkw.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iwo.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kol.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hcg.9152youxi.cn

[Q47] 与平均值比较
来源：http://xlh.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rhi.316326.xyz

[Q48] CTE 公用表表达式
来源：http://jzr.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://diz.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://jee.nwbrower.top

[Q49] 更新单行
来源：http://loe.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fow.hongshengwenyu.top

[Q50] 批量更新
来源：http://mas.vehdjk.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xlz.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://uio.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qeb.yj20258.top

[Q52] 删除指定行
来源：http://men.shuidangran.top

DELETE FROM users WHERE id = 10;
来源：http://xur.tanke756.top

[Q53] 按条件删除
来源：http://chw.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aem.guannengcc.top

[Q54] 清空表
来源：http://jax.c1oappe.top

TRUNCATE TABLE logs;
来源：http://bta.hammf.cn

[Q55] 排名（并列占位）
来源：http://mdc.bbcook.cn


<!-- 参考信息 -->