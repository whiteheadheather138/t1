代发 wailian999

Go:   // 手写 map[int]int
来源：http://prr.jqgfzy.top

Ruby: // 手写 Hash
来源：http://dsi.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jgv.zhoulong.xyz

[N08] 生成全排列
来源：http://wpi.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://ubd.hcnkem.com

PHP:  // 手写递归交换
来源：http://izb.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://drc.hcnkem.com

TS:   // 手写回溯递归
来源：http://wuy.sysykeji.top

Java: // 手写回溯递归
来源：http://urr.cheryme.top

Go:   // 手写回溯递归
来源：http://jcm.cheryme.top

Ruby: arr.permutation.to_a
来源：http://qaw.guowangkeji.top

C#:   // 手写回溯递归
来源：http://ybj.hfpthk.cn

[N09] 栈与队列
来源：http://vfi.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tzg.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kho.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvd.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zno.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cwj.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lsw.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hwy.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvw.zhongyouzk.top

[N10] 链表节点定义
来源：http://xio.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhe.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lxa.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ezz.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ejv.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://phe.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dvj.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zwt.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fqz.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://vmg.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ulu.fehbvm.com

PHP:  // 手写递归函数
来源：http://xeg.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvy.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dtl.tarul.cn

Java: // 手写递归
来源：http://fwa.svipenyu.cn

Go:   // 手写递归
来源：http://rty.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zbk.aibaodan.cn

C#:   // 手写递归
来源：http://ixc.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kol.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hot.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zti.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgu.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vak.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tyr.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ggr.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zpp.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ocu.hcnkem.com

================================================================================
来源：http://pat.jianghu66.top

O. 并发与异步
来源：http://kbl.yj202588.top

================================================================================
来源：http://daw.9152youxi.cn

[O01] 启动一个线程
来源：http://bcp.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qew.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rjz.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qxv.yuanzhike.top

TS:   // 同 JS
来源：http://uig.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://wig.jinqigfzy.top

Go:   go f()
来源：http://dzk.guannengcc.top

Ruby: Thread.new { f }
来源：http://rgo.uphjek.com

C#:   Task.Run(() => F());
来源：http://vwk.yfazqb.com

[O02] 使用线程池
来源：http://cxp.mhx1999.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bhs.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bgv.yuxming.cn

JS:   // worker_threads 线程池
来源：http://esk.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://cnn.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://try.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://idr.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nab.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yoe.316326.xyz

[O03] 加锁保护共享数据
来源：http://fxs.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://yok.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://rkx.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kkd.zhiwuduotai.top

TS:   // 同 JS
来源：http://gsv.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://vuf.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zng.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oqv.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://uth.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://tfd.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://fom.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eqs.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://ucx.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://imw.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cil.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rdr.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aty.meibo888.top

C#:   async Task F() { await G(); }
来源：http://ues.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://vlt.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://rld.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yht.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://rvp.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://lip.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nta.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xnq.bjfxy.top

Ruby: threads.map(&:join)
来源：http://xhg.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yno.gotoacloud.top

[O06] 使用进程池
来源：http://jsu.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://opg.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nim.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://yhr.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://jnj.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vzk.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lqe.tarul.cn

Ruby: // fork 块
来源：http://bee.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://epu.daria6918.cn

================================================================================
来源：http://jay.jlsjyb.cn

P. 常用工具函数
来源：http://zaj.zhixingplan.top

================================================================================
来源：http://fbp.mhx1999.top

[P01] 生成 UUID
来源：http://iok.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://jnv.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sax.iojbl.cn

JS:   crypto.randomUUID()
来源：http://tmp.vehdjk.com

TS:   crypto.randomUUID()
来源：http://oew.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://owg.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://ioi.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://nym.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://utu.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://see.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ucr.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sqm.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vdt.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rqz.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gfd.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mdu.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gsg.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://enp.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://tta.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jcq.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pqu.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsw.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nfj.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vnq.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vzg.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lbv.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rih.shangyingyoupin.top

[P04] 求长度
来源：http://uaj.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zaj.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rsa.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqj.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ejd.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://gxs.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://kxb.nanxinkj.top

Ruby: x.length;  x.size
来源：http://ldq.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kpq.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://tbi.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jcm.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hyj.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fii.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jox.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dsb.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://tcd.ivvv.top

Ruby: a == b
来源：http://djm.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ojh.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ram.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vkn.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://nag.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ozn.yuanzhike.top

TS:   if (x == null) {}
来源：http://zah.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tul.yj20258888.top

Go:   if x == nil {}
来源：http://lsj.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ret.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://svc.nwbrower.top

[P07] 防抖与节流
来源：http://ykn.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://skh.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://wwx.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bmu.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swz.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nkd.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rnu.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qod.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jnm.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://qzj.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://huh.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ysu.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://abv.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xub.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wbr.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hhx.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dae.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jui.jlsjyb.cn

================================================================================
来源：http://bni.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kon.yonumen.top

================================================================================
来源：http://aum.zhijiandao.cn

[Q01] 创建表
来源：http://omr.jqgufenzy.top

CREATE TABLE users (
来源：http://eyg.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfc.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://jiv.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://sbp.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vmx.fzhhl.top

);
来源：http://ngd.yfazqb.com

[Q02] 创建带外键的表
来源：http://sdx.zhiwuduotai.top

CREATE TABLE orders (
来源：http://njq.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyp.andypj.xyz

user_id INT NOT NULL,
来源：http://uld.tarul.cn

amount DECIMAL(10, 2),
来源：http://lpb.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cvg.jinqigfzy.top

);
来源：http://kdt.cucudq.cn

[Q03] 增加列
来源：http://nam.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qcr.shzxlz.cn

[Q04] 修改列类型
来源：http://faq.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://epq.aizwys.cn

[Q05] 重命名列
来源：http://ftz.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vai.guannengcc.top

[Q06] 删除列
来源：http://mlw.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kru.gaohongyu789.top

[Q07] 删除表
来源：http://rua.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://jsj.yonumen.top

[Q08] 创建普通索引
来源：http://jgl.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xux.xziqi.cn

[Q09] 创建唯一索引
来源：http://era.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ywi.havefunace.top

[Q10] 插入单行
来源：http://qzj.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://snr.vehdjk.com

[Q11] 一次插入多行
来源：http://rgc.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tsc.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://llc.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://vlu.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pax.zhixingplan.top

[Q13] 忽略重复插入
来源：http://ubz.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eax.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://rkb.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cbm.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qzi.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://vlg.gotoacloud.top

SELECT * FROM users;
来源：http://hiq.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://jqv.xinyue.icu

SELECT id, name FROM users;
来源：http://vve.0kj1m.cn

[Q17] 条件查询
来源：http://ktn.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vnq.zdqjudy.top

[Q18] 模糊匹配
来源：http://kqr.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zlu.tanke756.top

[Q19] 范围查询
来源：http://lxe.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vnw.jinghuilouyu.cn

[Q20] IN 列表
来源：http://bfb.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zih.zycfv.cn

[Q21] 空值判断
来源：http://fji.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vzm.zhoulong.xyz

[Q22] 排序
来源：http://ybc.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hht.meibo888.top

[Q23] 分页
来源：http://mfa.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kyg.52xcode.cn

[Q24] 去重
来源：http://sve.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://omv.zhengqikj.top

[Q25] 只取前 N 条
来源：http://byv.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kxk.tianlin.xyz

[Q26] 计数
来源：http://amz.nwbrower.top

SELECT COUNT(*) FROM users;
来源：http://dtz.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://vll.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vmi.cucudq.cn

[Q28] 求和与平均
来源：http://ylv.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rfq.aizwys.cn

[Q29] 最大最小值
来源：http://dyy.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ura.ehwqpu.com

[Q30] 分组统计
来源：http://wyy.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xrl.yanxiufei.cn

[Q31] 分组后过滤
来源：http://jqx.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zmm.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://qir.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lng.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lzr.haohaochexian.top

[Q33] 多列分组
来源：http://fhs.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://czb.quarkkingdee.top

[Q34] 每组取第一条
来源：http://rko.jinghuilouyu.cn

SELECT * FROM (
来源：http://kjy.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fqy.tian-w.cn

) t WHERE rn = 1;
来源：http://shl.yongpay.top

[Q35] 内连接
来源：http://irj.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iad.havefunace.top

[Q36] 左连接
来源：http://djz.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ezu.jyoumei.cn

[Q37] 右连接
来源：http://fgz.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rnt.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xrk.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qwo.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://vzz.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cyn.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xcg.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hkk.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ros.quarkkingdee.top

[Q41] 多表连接
来源：http://rym.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://xns.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://hiz.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://bxi.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://tsx.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://qio.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mym.sxryk.cn

[Q43] 标量子查询
来源：http://zuq.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ipj.pengpengdd.cyou

[Q44] IN 子查询
来源：http://ugj.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://agw.tanke756.top

[Q45] EXISTS 判断存在
来源：http://otv.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uql.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://rjf.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ops.bbcook.cn

[Q47] 与平均值比较
来源：http://blz.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kzs.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://zsv.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wmr.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://sdh.cucudq.cn

[Q49] 更新单行
来源：http://pda.chenjidiqi.icu


<!-- 参考信息 -->