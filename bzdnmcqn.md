代发 wailian999

Java: // 手写回溯递归
来源：http://aof.gzhubu.top

Go:   // 手写回溯递归
来源：http://iwy.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://izm.zhixingplan.top

C#:   // 手写回溯递归
来源：http://awd.mhx1999.top

[N09] 栈与队列
来源：http://ecl.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tjh.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rcm.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://owv.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bgc.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cdb.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://osp.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://keq.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hac.hfpthk.cn

[N10] 链表节点定义
来源：http://pxm.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uej.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://bcc.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nyx.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://njk.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://jfy.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://ycg.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qui.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zos.birdmap.top

[N11] 二叉树中序遍历
来源：http://ifq.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jdy.cheryme.top

PHP:  // 手写递归函数
来源：http://nbx.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ktk.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfj.yuxming.cn

Java: // 手写递归
来源：http://tym.haohaochexian.top

Go:   // 手写递归
来源：http://cmv.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ttt.nanxinkj.top

C#:   // 手写递归
来源：http://zsc.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tqd.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vec.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aoz.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qbg.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qdw.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rnw.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dgc.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nqu.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vxz.jqgufenzy.top

================================================================================
来源：http://waj.yj20258.top

O. 并发与异步
来源：http://yne.guannengcc.top

================================================================================
来源：http://mux.havefunace.top

[O01] 启动一个线程
来源：http://fbh.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tik.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://thw.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cyq.cheryme.top

TS:   // 同 JS
来源：http://dmj.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://trq.chenjidiqi.icu

Go:   go f()
来源：http://gyz.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://czq.cheryme.top

C#:   Task.Run(() => F());
来源：http://fes.vehdjk.com

[O02] 使用线程池
来源：http://lmm.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://elb.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wgh.smart0.xyz

JS:   // worker_threads 线程池
来源：http://ccc.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://rkc.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://yrx.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iih.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://prt.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ikz.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://pcv.hfpthk.cn

Py:   with lock: shared += 1
来源：http://coj.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://jcb.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lfg.smart0.xyz

TS:   // 同 JS
来源：http://gms.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://mgb.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hwz.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hrf.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://xbx.yj202588.top

[O04] 定义异步函数并等待
来源：http://mjp.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://qce.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jei.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://zke.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jke.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nng.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zmn.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jry.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://pyk.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://fby.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://wkl.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jny.yj202588.top

JS:   await Promise.all(tasks)
来源：http://dbl.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://lml.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hti.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qxf.52xcode.cn

Ruby: threads.map(&:join)
来源：http://bal.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wov.zycfv.cn

[O06] 使用进程池
来源：http://daq.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://goa.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yuf.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://xwm.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://edz.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kyq.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://toi.jqgfzy.top

Ruby: // fork 块
来源：http://joe.fktsv.cn

C#:   Parallel.For
来源：http://glz.ivvv.top

================================================================================
来源：http://pge.sweek.top

P. 常用工具函数
来源：http://bpa.guannengcc.top

================================================================================
来源：http://fnz.ybcxt.top

[P01] 生成 UUID
来源：http://xtv.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://syt.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zjf.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://nsu.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://ymm.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://sax.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://ejg.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://xul.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://pfw.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://smr.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zlx.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fcn.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tmw.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rfr.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ett.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vke.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bzo.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rdw.hesvh.cn

[P03] 生成短随机字符串
来源：http://ejw.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xoa.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vsw.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ktx.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://giz.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://edz.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amh.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://zms.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oqi.yj202588.top

[P04] 求长度
来源：http://yyk.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ofv.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://whu.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hjr.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cuu.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://ibp.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://rhv.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://vhq.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fnq.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://cpg.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://gjp.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wwy.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ndk.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cxh.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://trj.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://fmc.daxiang520.top

Ruby: a == b
来源：http://nwa.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rxu.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vmm.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wsl.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://pta.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dyd.zhongyouzk.top

TS:   if (x == null) {}
来源：http://wbt.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dpx.aibaodan.cn

Go:   if x == nil {}
来源：http://qmg.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ptf.jiagoushi.top

C#:   if (x is null) {}
来源：http://fda.shuidangran.top

[P07] 防抖与节流
来源：http://spr.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lxu.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://bah.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbz.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aci.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rij.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qda.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qkc.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jqm.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://zdi.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://afe.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xbd.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kcv.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://evn.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iol.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jbo.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ubx.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kuu.aibaodan.cn

================================================================================
来源：http://lkr.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bdm.hesvh.cn

================================================================================
来源：http://lra.0kj1m.cn

[Q01] 创建表
来源：http://dbc.sysykeji.top

CREATE TABLE users (
来源：http://dsz.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hwf.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://sip.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://rmd.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jug.andypj.xyz

);
来源：http://xco.daria6918.cn

[Q02] 创建带外键的表
来源：http://bdq.jinqigufen.top

CREATE TABLE orders (
来源：http://luk.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mkw.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://cgo.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://gcd.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pzc.feifeiyinyue.top

);
来源：http://tfl.jiagoushi.top

[Q03] 增加列
来源：http://tpq.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://urq.aizwys.cn

[Q04] 修改列类型
来源：http://qxy.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kxt.jlsjyb.cn

[Q05] 重命名列
来源：http://vyu.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ici.quarkkingdee.top

[Q06] 删除列
来源：http://hes.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://zih.chenjidiqi.icu

[Q07] 删除表
来源：http://rpb.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://xcx.sweek.top

[Q08] 创建普通索引
来源：http://blr.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tls.tian-w.cn

[Q09] 创建唯一索引
来源：http://gsd.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cow.pengpengdd.cyou

[Q10] 插入单行
来源：http://hsj.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dec.sufxvd.cn

[Q11] 一次插入多行
来源：http://rbh.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uco.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://gij.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://qze.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bvk.wangdashe.top

[Q13] 忽略重复插入
来源：http://wak.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kli.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://tqb.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zdk.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pwu.zhengqikj.top

[Q15] 查询全部
来源：http://gem.yvedp.cn

SELECT * FROM users;
来源：http://xej.ydzc1.top

[Q16] 查询指定列
来源：http://jni.uphjek.com

SELECT id, name FROM users;
来源：http://cbh.zdqjudy.top

[Q17] 条件查询
来源：http://bii.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fmg.316326.xyz

[Q18] 模糊匹配
来源：http://ybj.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gxl.yvedp.cn

[Q19] 范围查询
来源：http://sam.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pzy.jianghu66.top

[Q20] IN 列表
来源：http://mpc.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dpd.yangfankeji.com

[Q21] 空值判断
来源：http://pxw.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cdr.wangshuangyany.cn

[Q22] 排序
来源：http://uiu.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://djw.zhaomingkeji.xyz

[Q23] 分页
来源：http://aqf.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xtv.zycfv.cn

[Q24] 去重
来源：http://cuw.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://urn.jiagoushi.top

[Q25] 只取前 N 条
来源：http://wmy.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hyb.daria6918.cn

[Q26] 计数
来源：http://nnj.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://inj.havefunace.top

[Q27] 条件计数
来源：http://orc.shanyushiyangtech.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gcs.xuetiantiany.cn

[Q28] 求和与平均
来源：http://ryw.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://crk.andypj.xyz

[Q29] 最大最小值
来源：http://rrs.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://vvs.jianghu66.top

[Q30] 分组统计
来源：http://eqx.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pyo.gotoacloud.top

[Q31] 分组后过滤
来源：http://hpe.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iou.tarul.cn

[Q32] 分组拼接字符串
来源：http://rzy.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qet.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lbq.aizwys.cn

[Q33] 多列分组
来源：http://tzt.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://trb.meibo888.top

[Q34] 每组取第一条
来源：http://rxo.epnwcf.com

SELECT * FROM (
来源：http://qhw.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pyq.zhongyouzk.top

) t WHERE rn = 1;
来源：http://oxp.svipenyu.cn

[Q35] 内连接
来源：http://gmt.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kgk.yvedp.cn

[Q36] 左连接
来源：http://nzw.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://taa.sysykeji.top

[Q37] 右连接
来源：http://tvn.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vaj.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://euq.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fon.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://ixn.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oar.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dxw.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tke.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gba.ydzc1.top

[Q41] 多表连接
来源：http://brg.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lus.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://gef.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://tmr.tanke756.top

[Q42] 连接条件附加过滤
来源：http://ftt.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://ekx.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fth.gogol.net.cn

[Q43] 标量子查询
来源：http://vik.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://btx.0kj1m.cn

[Q44] IN 子查询
来源：http://bcp.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kcb.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://ltc.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://drf.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://gsb.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tqd.gogol.net.cn

[Q47] 与平均值比较
来源：http://obd.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bgr.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://qiw.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://adl.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://pur.tianlin.xyz

[Q49] 更新单行
来源：http://yma.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fgu.dianchejie.cn

[Q50] 批量更新
来源：http://ymv.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tsc.xziqi.cn

[Q51] 用子查询更新
来源：http://jmd.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://afi.dashuyun.cn

[Q52] 删除指定行
来源：http://qtg.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://yvk.gzhubu.top

[Q53] 按条件删除
来源：http://xbt.gzhubu.top


<!-- 参考信息 -->