代发 wailian999

Go:   // 手写 map[int]int
来源：http://pha.daria6918.cn

Ruby: // 手写 Hash
来源：http://rdy.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://iqs.daria6918.cn

[N08] 生成全排列
来源：http://wxp.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://ilc.yj202588.top

PHP:  // 手写递归交换
来源：http://pye.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://upc.yfazqb.com

TS:   // 手写回溯递归
来源：http://ksy.cucudq.cn

Java: // 手写回溯递归
来源：http://axd.ppjwa.cn

Go:   // 手写回溯递归
来源：http://ezi.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://afv.xylfe.cn

C#:   // 手写回溯递归
来源：http://bok.cheryme.top

[N09] 栈与队列
来源：http://xic.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iua.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vir.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lqi.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ksf.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uvd.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qqx.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ews.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yoh.iojbl.cn

[N10] 链表节点定义
来源：http://baf.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oiu.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://owe.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bvg.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jfv.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://ghz.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://qwn.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zvk.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bql.yvedp.cn

[N11] 二叉树中序遍历
来源：http://rjl.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vdp.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://cye.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hmv.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xon.shzxlz.cn

Java: // 手写递归
来源：http://hms.zdbjq.cn

Go:   // 手写递归
来源：http://phj.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mai.yangfankeji.com

C#:   // 手写递归
来源：http://pyv.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hgc.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xqt.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lbt.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zmi.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rzj.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qps.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oxw.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dfq.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://njs.tian-w.cn

================================================================================
来源：http://bzs.birdmap.top

O. 并发与异步
来源：http://xia.sysykeji.top

================================================================================
来源：http://mqi.yangfankeji.com

[O01] 启动一个线程
来源：http://wvw.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uci.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rog.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fvt.havefunace.top

TS:   // 同 JS
来源：http://mbf.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://xee.xziqi.cn

Go:   go f()
来源：http://qae.zycfv.cn

Ruby: Thread.new { f }
来源：http://vme.daxiang520.top

C#:   Task.Run(() => F());
来源：http://dnw.xylfe.cn

[O02] 使用线程池
来源：http://jcv.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ssl.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ytj.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://bim.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://tnx.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gui.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bqw.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xqq.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iqq.xuanzx.com

[O03] 加锁保护共享数据
来源：http://kse.fktsv.cn

Py:   with lock: shared += 1
来源：http://ajh.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://xix.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cbf.nwbrower.top

TS:   // 同 JS
来源：http://jxu.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://atl.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ftj.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ipx.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://xgg.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://bnu.pycfn.com

Py:   async def f():⏎    await g()
来源：http://vry.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uba.sysykeji.top

JS:   async function f() { await g(); }
来源：http://gdv.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lcj.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wgr.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ims.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://srl.sweek.top

C#:   async Task F() { await G(); }
来源：http://zmh.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://aod.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://pwn.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ufm.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://onm.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://pyq.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ukv.birdmap.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://knl.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://zfs.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://eat.nanxuanxn.top

[O06] 使用进程池
来源：http://lim.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zjz.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dcj.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://mxc.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://rjb.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jea.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lxe.chenzaomai.com

Ruby: // fork 块
来源：http://ljj.316326.xyz

C#:   Parallel.For
来源：http://abw.cucudq.cn

================================================================================
来源：http://nvy.andypj.xyz

P. 常用工具函数
来源：http://fei.fehbvm.com

================================================================================
来源：http://utb.fktsv.cn

[P01] 生成 UUID
来源：http://izi.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://vjp.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fpd.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://sil.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://mns.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://udv.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://uap.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://zdn.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://oxm.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://lan.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vwn.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nev.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qdo.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://css.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hfq.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lyo.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lkv.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zfs.hywenlv.cn

[P03] 生成短随机字符串
来源：http://wdl.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ctg.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tst.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kyv.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dsh.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dal.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lnh.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yfs.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jyb.nwbrower.top

[P04] 求长度
来源：http://hqu.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blz.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hbr.zhongyouzk.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yoh.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zeq.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://vng.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://got.dianchejie.cn

Ruby: x.length;  x.size
来源：http://ukt.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vyc.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://cid.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tqn.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oeo.zycfv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qyu.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mzu.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rzc.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rht.jinghuilouyu.cn

Ruby: a == b
来源：http://afp.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uxu.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://skw.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rlt.316326.xyz

PHP:  if (empty($x)) {}
来源：http://jrj.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://suj.tarul.cn

TS:   if (x == null) {}
来源：http://gkv.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cqt.ivvv.top

Go:   if x == nil {}
来源：http://lxc.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xjk.sufxvd.cn

C#:   if (x is null) {}
来源：http://ujn.birdmap.top

[P07] 防抖与节流
来源：http://byn.sufxvd.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kam.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://fyl.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oli.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ngq.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hap.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://koc.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://dsf.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqp.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://wnz.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://obn.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kin.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qes.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gez.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fsi.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uwm.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dcx.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aqc.xziqi.cn

================================================================================
来源：http://yel.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tdv.cheryme.top

================================================================================
来源：http://agr.shanyushiyangtech.top

[Q01] 创建表
来源：http://qod.guowangkeji.top

CREATE TABLE users (
来源：http://gqd.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wtn.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://vgc.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://lgk.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ftt.xuanzx.com

);
来源：http://jan.svipenyu.cn

[Q02] 创建带外键的表
来源：http://als.feifeiyinyue.top

CREATE TABLE orders (
来源：http://lsf.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kbf.xuanzx.com

user_id INT NOT NULL,
来源：http://qek.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://dxn.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cah.tianlin.xyz

);
来源：http://fms.jiagoushi.top

[Q03] 增加列
来源：http://zqj.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gel.sxryk.cn

[Q04] 修改列类型
来源：http://bqi.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kek.zhiwuduotai.top

[Q05] 重命名列
来源：http://ckh.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vnp.fanxiaobao.xyz

[Q06] 删除列
来源：http://rcp.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bwx.zycfv.cn

[Q07] 删除表
来源：http://jfi.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://yek.yfazqb.com

[Q08] 创建普通索引
来源：http://yxz.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hfu.epnwcf.com

[Q09] 创建唯一索引
来源：http://xpk.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://muh.yongpay.top

[Q10] 插入单行
来源：http://fwa.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qhi.aibaodan.cn

[Q11] 一次插入多行
来源：http://ljp.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fal.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://lni.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://mbt.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sno.ivvv.top

[Q13] 忽略重复插入
来源：http://bzm.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hkc.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://iee.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ldt.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zvp.xuanzx.com

[Q15] 查询全部
来源：http://qbx.sufxvd.cn

SELECT * FROM users;
来源：http://tkw.jqgfzy.top

[Q16] 查询指定列
来源：http://sbe.sweek.top

SELECT id, name FROM users;
来源：http://wnc.fehbvm.com

[Q17] 条件查询
来源：http://uyc.shzxlz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cfd.zhixingplan.top

[Q18] 模糊匹配
来源：http://oha.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ryj.birdmap.top

[Q19] 范围查询
来源：http://ozd.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://onc.jiagoushi.top

[Q20] IN 列表
来源：http://lej.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wek.tianlin.xyz

[Q21] 空值判断
来源：http://hyx.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lgt.jinqigfzy.top

[Q22] 排序
来源：http://ofn.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://paq.fanxiaobao.xyz

[Q23] 分页
来源：http://tph.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jke.hfpthk.cn

[Q24] 去重
来源：http://hwz.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://amo.hesvh.cn

[Q25] 只取前 N 条
来源：http://bct.svipenyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lno.zdqjudy.top

[Q26] 计数
来源：http://fha.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://dnt.zdbjq.cn

[Q27] 条件计数
来源：http://jqj.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rpm.zhengqikj.top

[Q28] 求和与平均
来源：http://taq.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lsx.sysykeji.top

[Q29] 最大最小值
来源：http://sbx.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://box.sysykeji.top

[Q30] 分组统计
来源：http://ypx.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://igu.epnwcf.com

[Q31] 分组后过滤
来源：http://hfq.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://chx.316326.xyz

[Q32] 分组拼接字符串
来源：http://iln.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vqy.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://quy.sufxvd.cn

[Q33] 多列分组
来源：http://gdz.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lnk.zycfv.cn

[Q34] 每组取第一条
来源：http://icf.shzxlz.cn

SELECT * FROM (
来源：http://wzb.cdnleiting.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fuf.nanxuanxn.top

) t WHERE rn = 1;
来源：http://job.jyoumei.cn

[Q35] 内连接
来源：http://yxi.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jsb.cqqwz.cn

[Q36] 左连接
来源：http://atj.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bif.fktsv.cn

[Q37] 右连接
来源：http://vjg.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qjv.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ybv.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yiw.uphjek.com

[Q39] 自连接（查上下级）
来源：http://xre.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://cgg.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nez.zhiwuduotai.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gtl.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://upt.bjfxy.top

[Q41] 多表连接
来源：http://twn.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wya.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://nxb.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://hey.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://avx.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://zsc.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ezo.zhiwuduotai.top

[Q43] 标量子查询
来源：http://doq.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bxr.ppjwa.cn

[Q44] IN 子查询
来源：http://ljm.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xol.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://qbd.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fmk.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://ukx.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ndz.andypj.xyz

[Q47] 与平均值比较
来源：http://sdq.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ogw.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://daa.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wzh.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://yuv.xinyue.icu

[Q49] 更新单行
来源：http://mhc.jinghuilouyu.cn


<!-- 参考信息 -->