代发 wailian999

Go:   // 手写 map[int]int
来源：http://qyr.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://tut.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mcg.xziqi.cn

[N08] 生成全排列
来源：http://jpv.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://fut.yuxming.cn

PHP:  // 手写递归交换
来源：http://obb.hnqzz.top

JS:   // 手写回溯递归
来源：http://ghb.cucudq.cn

TS:   // 手写回溯递归
来源：http://rym.xinyue.icu

Java: // 手写回溯递归
来源：http://nxv.yfazqb.com

Go:   // 手写回溯递归
来源：http://fbe.316326.xyz

Ruby: arr.permutation.to_a
来源：http://qvi.snrcjt.cn

C#:   // 手写回溯递归
来源：http://zbq.nwbrower.top

[N09] 栈与队列
来源：http://nin.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fof.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://puy.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qrw.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghm.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qub.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wdp.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hbx.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rum.yueranfly.top

[N10] 链表节点定义
来源：http://kjh.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pkz.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bpv.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bjm.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xll.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://pla.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://egc.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fho.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bzq.xuanzx.com

[N11] 二叉树中序遍历
来源：http://une.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://szz.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://cmd.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upw.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwe.pengpengdd.cyou

Java: // 手写递归
来源：http://ooh.ctjpmb.com

Go:   // 手写递归
来源：http://giu.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kgq.zycfv.cn

C#:   // 手写递归
来源：http://unw.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://voe.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fxk.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xnu.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ild.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tlj.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zdj.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hxr.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cmo.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qoj.aibaodan.cn

================================================================================
来源：http://jao.wangshuangyany.cn

O. 并发与异步
来源：http://bea.hnqzz.top

================================================================================
来源：http://pzn.yueranfly.top

[O01] 启动一个线程
来源：http://nmc.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bsz.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bue.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cvh.tanke756.top

TS:   // 同 JS
来源：http://zam.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://kfo.quarkkingdee.top

Go:   go f()
来源：http://con.316326.xyz

Ruby: Thread.new { f }
来源：http://rhs.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://bdj.uphjek.com

[O02] 使用线程池
来源：http://egi.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://okc.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zch.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://ahe.hesvh.cn

TS:   // worker_threads 线程池
来源：http://cfs.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://asd.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ftl.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dts.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xbd.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://aqv.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://jjp.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://dwc.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbx.dashuyun.cn

TS:   // 同 JS
来源：http://umn.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://ynx.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pbd.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hpo.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://jro.sysykeji.top

[O04] 定义异步函数并等待
来源：http://lkm.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://kxv.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hoo.hesvh.cn

JS:   async function f() { await g(); }
来源：http://eum.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iio.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uyx.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://noa.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://uve.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://cyc.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://ill.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://qmc.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://clr.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://eyo.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://afw.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://syt.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://beu.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://xbk.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pkg.zycfv.cn

[O06] 使用进程池
来源：http://ysh.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gyb.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zdq.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://tju.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://dke.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jcb.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://riy.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://fap.zhoulong.xyz

C#:   Parallel.For
来源：http://dfw.daxiang520.top

================================================================================
来源：http://itw.ydjk.org.cn

P. 常用工具函数
来源：http://yaa.jqgfzy.top

================================================================================
来源：http://kuo.yanxiufei.cn

[P01] 生成 UUID
来源：http://tws.pycfn.com

Py:   str(uuid.uuid4())
来源：http://dwj.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yfr.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://hdo.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://vbh.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://qoc.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://zsy.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://stz.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://jal.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://gdr.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wyl.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gun.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mxz.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tul.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cpz.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://irq.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fbw.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://soh.uphjek.com

[P03] 生成短随机字符串
来源：http://fsy.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hcy.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qyp.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ymo.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ofl.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ycd.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pje.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cwi.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yuw.sufxvd.cn

[P04] 求长度
来源：http://svg.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uva.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ule.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ayc.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fdf.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://xtq.hammf.cn

Go:   len(arr);  len(m)
来源：http://lct.52xcode.cn

Ruby: x.length;  x.size
来源：http://nfp.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ryt.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://xhg.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pml.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mhz.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zeq.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gvx.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wbm.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://euo.cucudq.cn

Ruby: a == b
来源：http://nfs.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yip.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gvu.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sod.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://vtu.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://faz.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://yxk.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://phy.vqdsnc.cn

Go:   if x == nil {}
来源：http://vay.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zob.sweek.top

C#:   if (x is null) {}
来源：http://igg.yonumen.top

[P07] 防抖与节流
来源：http://rnf.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tng.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://shn.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pjb.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcl.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kpu.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bvd.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rbg.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fje.xinyue.icu

[P08] 处理浮点精度问题
来源：http://fmf.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vnh.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bvx.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ivi.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kct.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iqj.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://odk.havefunace.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dtk.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fyi.gzhubu.top

================================================================================
来源：http://icy.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zuq.cheryme.top

================================================================================
来源：http://gwh.cucudq.cn

[Q01] 创建表
来源：http://kpo.chenjidiqi.icu

CREATE TABLE users (
来源：http://hzz.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bes.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://mmr.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://yrl.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cin.pycfn.com

);
来源：http://imq.ctjpmb.com

[Q02] 创建带外键的表
来源：http://uww.chenlongwang.top

CREATE TABLE orders (
来源：http://kqz.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kml.tianlin.xyz

user_id INT NOT NULL,
来源：http://ywx.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://ykm.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gig.fehbvm.com

);
来源：http://slk.yuxming.cn

[Q03] 增加列
来源：http://nfx.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lkf.pengpengdd.cyou

[Q04] 修改列类型
来源：http://oon.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://krf.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://azc.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yzq.cheryme.top

[Q06] 删除列
来源：http://ixw.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://msl.yvedp.cn

[Q07] 删除表
来源：http://bwh.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://oqe.epnwcf.com

[Q08] 创建普通索引
来源：http://jqp.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jkc.vehdjk.com

[Q09] 创建唯一索引
来源：http://mcf.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iew.ydzc1.top

[Q10] 插入单行
来源：http://cln.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://abv.zycfv.cn

[Q11] 一次插入多行
来源：http://wga.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gaf.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://mpo.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nti.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vzl.jqgfzy.top

[Q13] 忽略重复插入
来源：http://plj.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fxz.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://lxx.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ydf.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fic.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://ayk.sjlbkw.cn

SELECT * FROM users;
来源：http://wmr.sufxvd.cn

[Q16] 查询指定列
来源：http://fyo.gaohongyu789.top

SELECT id, name FROM users;
来源：http://did.shuidangran.top

[Q17] 条件查询
来源：http://jkv.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ffc.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://nvi.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ivq.hnqzz.top

[Q19] 范围查询
来源：http://exb.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vii.sweek.top

[Q20] IN 列表
来源：http://ymr.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ios.316326.xyz

[Q21] 空值判断
来源：http://dmq.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lnf.jlsjyb.cn

[Q22] 排序
来源：http://vys.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kbc.fanxiaobao.xyz

[Q23] 分页
来源：http://svn.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://knj.hnqzz.top

[Q24] 去重
来源：http://jzd.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://ijw.uphjek.com

[Q25] 只取前 N 条
来源：http://cjl.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rfn.havefunace.top

[Q26] 计数
来源：http://jeb.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://ijz.zycfv.cn

[Q27] 条件计数
来源：http://wtq.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xlj.zdqjudy.top

[Q28] 求和与平均
来源：http://hpf.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ogi.ybcxt.top

[Q29] 最大最小值
来源：http://evu.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xsm.chenjidiqi.icu

[Q30] 分组统计
来源：http://tud.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zrn.guannengcc.top

[Q31] 分组后过滤
来源：http://fgx.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cpl.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://rod.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ccv.zhengqikj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sju.daria6918.cn

[Q33] 多列分组
来源：http://nlu.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://czl.hnqzz.top

[Q34] 每组取第一条
来源：http://ubi.zhixingplan.top

SELECT * FROM (
来源：http://tlc.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ueh.svipenyu.cn

) t WHERE rn = 1;
来源：http://qgb.jinqigfzy.top

[Q35] 内连接
来源：http://cov.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nxk.zhoulong.xyz

[Q36] 左连接
来源：http://ojj.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wba.316326.xyz

[Q37] 右连接
来源：http://pje.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kfb.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://zcn.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xvt.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://cyt.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zwa.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rcc.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bpv.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iso.jqgufenzy.top

[Q41] 多表连接
来源：http://okj.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rwj.hnxiangtu.top

JOIN users u ON u.id = o.user_id
来源：http://rwo.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://mgh.yj202588.top

[Q42] 连接条件附加过滤
来源：http://nri.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://msd.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hrb.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://xjk.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ouk.cdnleiting.top

[Q44] IN 子查询
来源：http://qoc.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://efg.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://pdc.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ghf.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://flo.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://grj.chenzaomai.com

[Q47] 与平均值比较
来源：http://ati.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://une.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://nsh.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://esf.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://ybc.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://sqi.pengpengdd.cyou


<!-- 参考信息 -->