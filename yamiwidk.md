代发 wailian999

Py:   itertools.permutations(arr)
来源：http://kzm.yj20258.top

PHP:  // 手写递归交换
来源：http://plw.yj20258.top

JS:   // 手写回溯递归
来源：http://xwe.aibaodan.cn

TS:   // 手写回溯递归
来源：http://hsc.pycfn.com

Java: // 手写回溯递归
来源：http://hwo.daria6918.cn

Go:   // 手写回溯递归
来源：http://ooc.sweek.top

Ruby: arr.permutation.to_a
来源：http://ubd.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://ule.hcnkem.com

[N09] 栈与队列
来源：http://ccq.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vhn.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pnm.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vwe.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gym.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iaf.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lem.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qwh.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qxs.gzhubu.top

[N10] 链表节点定义
来源：http://jsc.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ceh.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hxe.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://txa.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ctg.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://ntj.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lbz.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://cxv.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dsc.tanke756.top

[N11] 二叉树中序遍历
来源：http://jzx.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vhk.jqgfzy.top

PHP:  // 手写递归函数
来源：http://bsc.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://unx.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jbv.uphjek.com

Java: // 手写递归
来源：http://rox.guannengcc.top

Go:   // 手写递归
来源：http://hdj.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tle.yfazqb.com

C#:   // 手写递归
来源：http://tzm.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zox.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fma.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://liw.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ppb.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcg.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://clr.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://non.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dkg.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aoh.c1oappe.top

================================================================================
来源：http://rxd.yvedp.cn

O. 并发与异步
来源：http://waq.wangdashe.top

================================================================================
来源：http://pde.tianlin.xyz

[O01] 启动一个线程
来源：http://tnt.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lnn.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bab.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zrx.sxryk.cn

TS:   // 同 JS
来源：http://doz.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://cze.wangdashe.top

Go:   go f()
来源：http://cjs.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://nch.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://jhf.0kj1m.cn

[O02] 使用线程池
来源：http://vox.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yjt.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ydp.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://ydi.smart0.xyz

TS:   // worker_threads 线程池
来源：http://kwm.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eyl.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://csa.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iky.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dwg.yvedp.cn

[O03] 加锁保护共享数据
来源：http://qah.jiagoushi.top

Py:   with lock: shared += 1
来源：http://mwm.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://oqp.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rmw.mhx1999.top

TS:   // 同 JS
来源：http://tdl.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://vhh.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://erw.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kvr.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://oru.shuidangran.top

[O04] 定义异步函数并等待
来源：http://jrq.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://iub.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jms.gzhubu.top

JS:   async function f() { await g(); }
来源：http://lix.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://krn.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mpm.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eoy.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pqv.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://gjr.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://zwf.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://hfz.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://unt.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://ftx.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://nkh.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pmu.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xcf.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://pez.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jki.cucudq.cn

[O06] 使用进程池
来源：http://bla.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zgc.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iza.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://mbb.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://ieq.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zlt.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://joz.xylfe.cn

Ruby: // fork 块
来源：http://wwv.xinyue.icu

C#:   Parallel.For
来源：http://dvw.jyoumei.cn

================================================================================
来源：http://pvp.shanyushiyangtech.top

P. 常用工具函数
来源：http://ugt.zhoulong.xyz

================================================================================
来源：http://kzz.yj20258888.top

[P01] 生成 UUID
来源：http://vir.uphjek.com

Py:   str(uuid.uuid4())
来源：http://zao.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mms.mhx1999.top

JS:   crypto.randomUUID()
来源：http://wwr.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://mrs.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://toh.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://fto.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://yje.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://eyw.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://oyx.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ohi.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://syt.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aas.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qsm.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hjq.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ccg.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fec.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://epv.sweek.top

[P03] 生成短随机字符串
来源：http://eng.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gyv.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hju.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vri.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rng.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://edn.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cry.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://awn.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgi.xziqi.cn

[P04] 求长度
来源：http://vfp.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ajc.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pya.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zen.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jui.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://tyi.hnqzz.top

Go:   len(arr);  len(m)
来源：http://spo.sysykeji.top

Ruby: x.length;  x.size
来源：http://uvc.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://afh.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://vsh.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://asj.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pfb.zycfv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kwc.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gic.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zai.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ocg.yvedp.cn

Ruby: a == b
来源：http://dkc.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ckq.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sau.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bws.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://nov.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vse.vehdjk.com

TS:   if (x == null) {}
来源：http://xsm.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ujd.meibo888.top

Go:   if x == nil {}
来源：http://owg.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://abe.316326.xyz

C#:   if (x is null) {}
来源：http://ifn.xinyue.icu

[P07] 防抖与节流
来源：http://nie.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aoi.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://ifz.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsq.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nbo.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uyp.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rnr.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://onv.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://off.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://xnc.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uug.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lrg.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jhc.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aih.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://abi.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mzn.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://glm.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qxn.vehdjk.com

================================================================================
来源：http://ega.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zqf.ivvv.top

================================================================================
来源：http://dgp.fanxiaobao.xyz

[Q01] 创建表
来源：http://xqa.ydjk.org.cn

CREATE TABLE users (
来源：http://mol.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fyq.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://cpb.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://uzv.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nuu.cqqwz.cn

);
来源：http://dni.shzxlz.cn

[Q02] 创建带外键的表
来源：http://nnl.hnxiangtu.top

CREATE TABLE orders (
来源：http://tsn.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ktb.aibaodan.cn

user_id INT NOT NULL,
来源：http://knu.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://jhy.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ndo.yuanzhike.top

);
来源：http://xta.jqgfzy.top

[Q03] 增加列
来源：http://uhx.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nck.ctjpmb.com

[Q04] 修改列类型
来源：http://bjl.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ngz.yongpay.top

[Q05] 重命名列
来源：http://wzi.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tpu.zhongyouzk.top

[Q06] 删除列
来源：http://oxz.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zhm.wangdashe.top

[Q07] 删除表
来源：http://fxw.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://soc.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://jcp.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://guu.yj202588.top

[Q09] 创建唯一索引
来源：http://qcv.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uph.zhoulong.xyz

[Q10] 插入单行
来源：http://rci.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://osq.hfpthk.cn

[Q11] 一次插入多行
来源：http://meo.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lzh.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://joh.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://kex.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ypq.jianghu66.top

[Q13] 忽略重复插入
来源：http://zet.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nrt.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://oal.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cud.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://znm.xuetiantiany.cn

[Q15] 查询全部
来源：http://mhh.zdbjq.cn

SELECT * FROM users;
来源：http://tgz.havefunace.top

[Q16] 查询指定列
来源：http://lau.sjlbkw.cn

SELECT id, name FROM users;
来源：http://hxq.hfpthk.cn

[Q17] 条件查询
来源：http://hkp.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uio.fktsv.cn

[Q18] 模糊匹配
来源：http://mto.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://voo.snrcjt.cn

[Q19] 范围查询
来源：http://evb.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dbq.uphjek.com

[Q20] IN 列表
来源：http://elm.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ugf.hesvh.cn

[Q21] 空值判断
来源：http://ulb.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://jdu.bjfxy.top

[Q22] 排序
来源：http://qru.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://igv.dashuyun.cn

[Q23] 分页
来源：http://avz.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://duc.zhiwuduotai.top

[Q24] 去重
来源：http://wpo.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://sld.haohaochexian.top

[Q25] 只取前 N 条
来源：http://haz.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rjr.meibo888.top

[Q26] 计数
来源：http://lqe.nwbrower.top

SELECT COUNT(*) FROM users;
来源：http://tjn.tian-w.cn

[Q27] 条件计数
来源：http://zqb.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bxe.jqgufenzy.top

[Q28] 求和与平均
来源：http://zqr.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://geh.zhoulong.xyz

[Q29] 最大最小值
来源：http://amh.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jgo.fehbvm.com

[Q30] 分组统计
来源：http://clk.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cyj.yuanzhike.top

[Q31] 分组后过滤
来源：http://ruq.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xzo.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://chk.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://emn.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bgi.jinqigufen.top

[Q33] 多列分组
来源：http://mop.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ygh.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://bcy.zdbjq.cn

SELECT * FROM (
来源：http://bbv.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xux.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://ucg.shuidangran.top

[Q35] 内连接
来源：http://obg.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pli.andypj.xyz

[Q36] 左连接
来源：http://vot.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hvc.sysykeji.top

[Q37] 右连接
来源：http://cco.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zkw.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://wnz.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bjo.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://fcu.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://gbo.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jri.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lfk.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ywi.uphjek.com

[Q41] 多表连接
来源：http://pfe.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://emk.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://ugj.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://unt.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://kqm.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://alr.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bkn.xylfe.cn

[Q43] 标量子查询
来源：http://fze.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sji.fktsv.cn

[Q44] IN 子查询
来源：http://okv.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zjs.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://dfi.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tpv.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xal.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhv.guannengcc.top

[Q47] 与平均值比较
来源：http://niq.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://chr.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://bux.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://moc.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://kya.snrcjt.cn

[Q49] 更新单行
来源：http://wxa.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rcx.yanxiufei.cn

[Q50] 批量更新
来源：http://xxb.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ivc.tanke756.top

[Q51] 用子查询更新
来源：http://axp.ppjwa.cn


<!-- 参考信息 -->