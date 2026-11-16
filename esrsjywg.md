代发 wailian999

Go:   // 手写 map[int]int
来源：http://upx.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://ium.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://dmu.zhengqikj.top

[N08] 生成全排列
来源：http://xoa.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://gbe.bjfxy.top

PHP:  // 手写递归交换
来源：http://ebp.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://jmj.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://yzs.xziqi.cn

Java: // 手写回溯递归
来源：http://pxl.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://ftm.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://hwi.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://rqr.zhijiandao.cn

[N09] 栈与队列
来源：http://fxg.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jbu.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mhb.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aqf.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jsb.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vey.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qhh.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dyt.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://amq.gogol.net.cn

[N10] 链表节点定义
来源：http://tif.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cwi.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ttk.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://etb.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tqv.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://sue.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://giw.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lft.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ztl.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://kqc.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://leg.vehdjk.com

PHP:  // 手写递归函数
来源：http://ceo.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fqv.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqs.jinqigfzy.top

Java: // 手写递归
来源：http://cop.jinqigufen.top

Go:   // 手写递归
来源：http://eod.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gfz.svipenyu.cn

C#:   // 手写递归
来源：http://srg.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://orh.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rlb.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uvb.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nut.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fql.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dhx.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyi.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ymv.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yzn.chenjidiqi.icu

================================================================================
来源：http://fvd.jinqigfzy.top

O. 并发与异步
来源：http://iuu.jianghu66.top

================================================================================
来源：http://wwg.bbcook.cn

[O01] 启动一个线程
来源：http://kdo.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dgz.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jqu.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kke.fzhhl.top

TS:   // 同 JS
来源：http://def.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://krf.vqdsnc.cn

Go:   go f()
来源：http://alj.uphjek.com

Ruby: Thread.new { f }
来源：http://rvp.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://zgp.wangdashe.top

[O02] 使用线程池
来源：http://wyd.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mxa.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mww.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://uom.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://vbt.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dlt.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hha.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wae.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lbl.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://upn.316326.xyz

Py:   with lock: shared += 1
来源：http://nbz.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://mtz.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ubq.yuxming.cn

TS:   // 同 JS
来源：http://gtv.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://nth.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://auh.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dew.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://ecd.bbcook.cn

[O04] 定义异步函数并等待
来源：http://lkz.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://cec.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lsn.pycfn.com

JS:   async function f() { await g(); }
来源：http://zmy.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://utz.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://guh.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ham.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://igk.uphjek.com

C#:   async Task F() { await G(); }
来源：http://juj.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://rev.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://bvx.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ecl.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://bml.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://gss.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wfv.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qct.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://rxg.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fer.daxiang520.top

[O06] 使用进程池
来源：http://llu.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wox.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gvp.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://uas.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://knm.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://inx.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sjt.xuanzx.com

Ruby: // fork 块
来源：http://rbe.fzhhl.top

C#:   Parallel.For
来源：http://xfi.guannengcc.top

================================================================================
来源：http://jrg.nwbrower.top

P. 常用工具函数
来源：http://qnp.sxryk.cn

================================================================================
来源：http://ioy.ppjwa.cn

[P01] 生成 UUID
来源：http://pxr.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://qaw.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bvd.ybcxt.top

JS:   crypto.randomUUID()
来源：http://jek.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://veh.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://dkj.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://rtc.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://ucj.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://chj.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://cnn.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mfj.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://dme.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://clm.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vfz.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://euu.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wbi.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aep.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gip.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://taw.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iwz.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://glq.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kcz.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://czd.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vjt.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hky.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ifj.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://phc.shzxlz.cn

[P04] 求长度
来源：http://clw.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zct.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://whb.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ymz.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bdm.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://drg.52xcode.cn

Go:   len(arr);  len(m)
来源：http://mmv.birdmap.top

Ruby: x.length;  x.size
来源：http://cdc.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://tcp.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://dlm.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gdj.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lcz.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pgl.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xqh.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pvv.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://hez.zdbjq.cn

Ruby: a == b
来源：http://mob.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bpy.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zaz.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mgy.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://tqw.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://faf.yvedp.cn

TS:   if (x == null) {}
来源：http://uvj.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qtl.fktsv.cn

Go:   if x == nil {}
来源：http://onb.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uvu.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://uga.hammf.cn

[P07] 防抖与节流
来源：http://rjo.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zet.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://fat.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pqc.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oar.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wlk.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ykx.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mfp.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bnx.yueranfly.top

[P08] 处理浮点精度问题
来源：http://mcb.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rkb.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ntq.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kul.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ezk.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vpi.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tme.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uru.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://flg.zdqjudy.top

================================================================================
来源：http://dre.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xjs.ybcxt.top

================================================================================
来源：http://rut.vehdjk.com

[Q01] 创建表
来源：http://jad.zhijiandao.cn

CREATE TABLE users (
来源：http://poc.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rha.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://hco.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://hvg.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ucd.iojbl.cn

);
来源：http://ioj.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://sor.tianlin.xyz

CREATE TABLE orders (
来源：http://vrv.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ota.yj20258888.top

user_id INT NOT NULL,
来源：http://oxx.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://xmv.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qbf.yuxming.cn

);
来源：http://bly.pengpengdd.cyou

[Q03] 增加列
来源：http://eqc.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://djs.zhiwuduotai.top

[Q04] 修改列类型
来源：http://jwv.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://maq.chenzaomai.com

[Q05] 重命名列
来源：http://xrw.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rom.yongpay.top

[Q06] 删除列
来源：http://ggi.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xvj.316326.xyz

[Q07] 删除表
来源：http://vsz.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://aqv.0kj1m.cn

[Q08] 创建普通索引
来源：http://sdp.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://hwa.yj20258.top

[Q09] 创建唯一索引
来源：http://snz.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nqa.jianghu66.top

[Q10] 插入单行
来源：http://zry.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://efo.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://gbo.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wzg.ivvv.top

[Q12] 插入后取自增 ID
来源：http://uqh.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://yjg.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsq.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://awz.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pdz.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://iqp.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mlk.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tnh.hammf.cn

[Q15] 查询全部
来源：http://gek.yfazqb.com

SELECT * FROM users;
来源：http://flr.vqdsnc.cn

[Q16] 查询指定列
来源：http://vhw.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://zrl.shuidangran.top

[Q17] 条件查询
来源：http://oft.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lld.jinqigfzy.top

[Q18] 模糊匹配
来源：http://nny.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://emz.fengsongda.top

[Q19] 范围查询
来源：http://npz.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yjo.zhengqikj.top

[Q20] IN 列表
来源：http://hso.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ebr.zhengqikj.top

[Q21] 空值判断
来源：http://aqt.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://stz.cqqwz.cn

[Q22] 排序
来源：http://fpn.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xwx.shanyushiyangkeji.top

[Q23] 分页
来源：http://jnv.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qou.shzxlz.cn

[Q24] 去重
来源：http://vav.316326.xyz

SELECT DISTINCT city FROM users;
来源：http://fdl.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://inq.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wxk.daria6918.cn

[Q26] 计数
来源：http://cud.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://lub.hcnkem.com

[Q27] 条件计数
来源：http://jxc.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://apb.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://vtc.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rcw.9152youxi.cn

[Q29] 最大最小值
来源：http://slp.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mbj.shzxlz.cn

[Q30] 分组统计
来源：http://smn.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ycy.kuanghao11.cn

[Q31] 分组后过滤
来源：http://tso.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://piy.xylfe.cn

[Q32] 分组拼接字符串
来源：http://wws.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cxd.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tko.iojbl.cn

[Q33] 多列分组
来源：http://jal.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cvo.hammf.cn

[Q34] 每组取第一条
来源：http://kvj.ybcxt.top

SELECT * FROM (
来源：http://vuk.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wlf.0kj1m.cn

) t WHERE rn = 1;
来源：http://jan.guannengcc.top

[Q35] 内连接
来源：http://pax.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jpy.hywenlv.cn

[Q36] 左连接
来源：http://oav.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blc.316326.xyz

[Q37] 右连接
来源：http://yoj.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gyb.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nhl.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cpt.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://pol.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ume.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://onh.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://amy.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sjw.ydjk.org.cn

[Q41] 多表连接
来源：http://lor.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://trg.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://tda.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://pzi.sxryk.cn

[Q42] 连接条件附加过滤
来源：http://quq.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://syz.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dfu.dashuyun.cn

[Q43] 标量子查询
来源：http://fpp.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://boh.wangdashe.top

[Q44] IN 子查询
来源：http://loa.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wsi.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://vob.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jpm.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://lae.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://icq.xziqi.cn

[Q47] 与平均值比较
来源：http://uni.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ope.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://gnq.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mnr.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://ivi.andypj.xyz

[Q49] 更新单行
来源：http://axo.fzhhl.top


<!-- 参考信息 -->