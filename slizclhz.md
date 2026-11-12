代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://tck.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://lfi.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bwv.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://ilo.tarul.cn

Ruby: s == s.reverse
来源：http://pbs.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ein.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://php.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://krh.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://grt.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://naa.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://mfn.vehdjk.com

Java: // 手写 HashMap
来源：http://sop.pycfn.com

Go:   // 手写 map[int]int
来源：http://cuf.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://krt.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pxt.nanxuanxn.top

[N08] 生成全排列
来源：http://ecr.tarul.cn

Py:   itertools.permutations(arr)
来源：http://gzj.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://tec.yfazqb.com

JS:   // 手写回溯递归
来源：http://hvk.yuanzhike.top

TS:   // 手写回溯递归
来源：http://bey.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://sgp.jyoumei.cn

Go:   // 手写回溯递归
来源：http://pur.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://rts.tanke756.top

C#:   // 手写回溯递归
来源：http://hjh.52xcode.cn

[N09] 栈与队列
来源：http://uja.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yaq.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://slp.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nhd.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hlb.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zuh.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zta.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hnd.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hrn.wangshuangyany.cn

[N10] 链表节点定义
来源：http://smo.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ito.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lap.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kak.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zdh.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://thd.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vzf.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gaj.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://xlo.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://isd.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yeu.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://fkg.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgl.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gzo.zhengqikj.top

Java: // 手写递归
来源：http://voq.cheryme.top

Go:   // 手写递归
来源：http://fkt.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hcb.jiagoushi.top

C#:   // 手写递归
来源：http://igy.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bhz.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vas.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxm.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sji.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aqw.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dgo.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hzd.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vff.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tfj.hesvh.cn

================================================================================
来源：http://vvo.yfazqb.com

O. 并发与异步
来源：http://cnt.9152youxi.cn

================================================================================
来源：http://gsy.nanxinkj.top

[O01] 启动一个线程
来源：http://nit.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ecg.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gxx.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lmi.iojbl.cn

TS:   // 同 JS
来源：http://rbk.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://ofb.mhx1999.top

Go:   go f()
来源：http://fqs.aizwys.cn

Ruby: Thread.new { f }
来源：http://rrz.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://qzu.jqgufenzy.top

[O02] 使用线程池
来源：http://tfx.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gpe.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sdf.xinyue.icu

JS:   // worker_threads 线程池
来源：http://uuy.redwolf501.top

TS:   // worker_threads 线程池
来源：http://kmq.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://hfc.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nnx.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kbt.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jja.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://rer.dashuyun.cn

Py:   with lock: shared += 1
来源：http://hlg.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://ffb.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pui.aibaodan.cn

TS:   // 同 JS
来源：http://gto.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://pju.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rkq.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cnb.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://cjr.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://xfu.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://dsz.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wug.cheryme.top

JS:   async function f() { await g(); }
来源：http://kjo.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://fev.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bik.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tll.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://aes.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://kfv.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://vdz.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://vqf.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yvk.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://equ.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://vbt.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://syl.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xhh.guannengcc.top

Ruby: threads.map(&:join)
来源：http://lxe.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kjx.tianlin.xyz

[O06] 使用进程池
来源：http://kom.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dqv.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://evz.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://jmn.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://uhw.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jxt.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://apq.9152youxi.cn

Ruby: // fork 块
来源：http://diq.chenzaomai.com

C#:   Parallel.For
来源：http://ezy.shangyingyoupin.top

================================================================================
来源：http://zar.hysaishi.cn

P. 常用工具函数
来源：http://zab.shzxlz.cn

================================================================================
来源：http://fkd.jqgfzy.top

[P01] 生成 UUID
来源：http://mxw.yj202588.top

Py:   str(uuid.uuid4())
来源：http://oig.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://efq.guannengcc.top

JS:   crypto.randomUUID()
来源：http://dqy.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://bqk.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://vth.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://xql.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://esx.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://eda.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://fcl.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yia.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pjn.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pdx.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jsu.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://piv.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://flx.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lsd.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bib.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://vgf.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vkq.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kkg.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nfe.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dok.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ykg.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dis.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jpc.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://okz.gotoacloud.top

[P04] 求长度
来源：http://adt.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ptb.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jtf.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pwk.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sgv.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://exe.hnqzz.top

Go:   len(arr);  len(m)
来源：http://kog.xuanzx.com

Ruby: x.length;  x.size
来源：http://ykl.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kzi.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://xno.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cxv.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bcs.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qwg.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ltf.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wtx.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ztu.birdmap.top

Ruby: a == b
来源：http://xhj.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://acp.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wcc.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vwo.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://god.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jce.cashguo.top

TS:   if (x == null) {}
来源：http://ijx.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://obv.yueranfly.top

Go:   if x == nil {}
来源：http://rpj.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hyw.hammf.cn

C#:   if (x is null) {}
来源：http://obm.aizwys.cn

[P07] 防抖与节流
来源：http://kdk.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nqn.cashguo.top

PHP:  // 手写时间戳比较
来源：http://rjs.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://leo.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://apq.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://veq.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xcd.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kvz.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bca.meibo888.top

[P08] 处理浮点精度问题
来源：http://cmx.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lqm.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://slb.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vwg.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bcb.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xzs.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ios.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tuf.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xkj.cqqwz.cn

================================================================================
来源：http://lpk.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dqp.cqqwz.cn

================================================================================
来源：http://ftg.uphjek.com

[Q01] 创建表
来源：http://sju.nanxinkj.top

CREATE TABLE users (
来源：http://myd.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ilr.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://fjq.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://two.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lso.hcnkem.com

);
来源：http://xqf.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://icw.guowangkeji.top

CREATE TABLE orders (
来源：http://suk.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vmf.yj202588.top

user_id INT NOT NULL,
来源：http://udj.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://nik.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bhe.52xcode.cn

);
来源：http://abn.svipenyu.cn

[Q03] 增加列
来源：http://xzj.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xuq.yangfankeji.com

[Q04] 修改列类型
来源：http://zwk.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uae.andypj.xyz

[Q05] 重命名列
来源：http://dhk.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lsf.shuidangran.top

[Q06] 删除列
来源：http://qni.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://ryb.feifeiyinyue.top

[Q07] 删除表
来源：http://eeg.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://mnc.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://jvx.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yhg.pycfn.com

[Q09] 创建唯一索引
来源：http://mhb.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gku.fehbvm.com

[Q10] 插入单行
来源：http://hct.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ssk.redwolf501.top

[Q11] 一次插入多行
来源：http://ynm.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lwi.uphjek.com

[Q12] 插入后取自增 ID
来源：http://fuf.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yqp.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zqv.guowangkeji.top

[Q13] 忽略重复插入
来源：http://oej.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sdd.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://ubx.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xug.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zcs.jinqigfzy.top

[Q15] 查询全部
来源：http://wjx.hcnkem.com

SELECT * FROM users;
来源：http://qms.hcnkem.com

[Q16] 查询指定列
来源：http://scj.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://ntn.52xcode.cn

[Q17] 条件查询
来源：http://lgd.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yja.yuxming.cn

[Q18] 模糊匹配
来源：http://spu.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qif.chenjidiqi.icu

[Q19] 范围查询
来源：http://vvn.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ojd.pycfn.com

[Q20] IN 列表
来源：http://nfn.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uia.sweek.top

[Q21] 空值判断
来源：http://mug.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mjx.yangfankeji.com

[Q22] 排序
来源：http://wtn.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wup.tanke756.top

[Q23] 分页
来源：http://zcm.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yiy.nanxuanxn.top

[Q24] 去重
来源：http://egy.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://qil.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://jyj.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://syv.chenlongwang.top

[Q26] 计数
来源：http://jnk.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://cqm.redwolf501.top

[Q27] 条件计数
来源：http://lhg.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pjo.bbcook.cn

[Q28] 求和与平均
来源：http://oct.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kvf.fehbvm.com

[Q29] 最大最小值
来源：http://cxk.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://vtq.fktsv.cn

[Q30] 分组统计
来源：http://nhp.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qao.tianlin.xyz

[Q31] 分组后过滤
来源：http://yvg.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://szo.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://hpf.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wgh.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lbs.fanxiaobao.xyz

[Q33] 多列分组
来源：http://fme.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uja.9152youxi.cn

[Q34] 每组取第一条
来源：http://ana.yanxiufei.cn

SELECT * FROM (
来源：http://xou.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gqw.shangyingyoupin.top

) t WHERE rn = 1;
来源：http://muu.yj202588.top

[Q35] 内连接
来源：http://kjj.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yna.yangfankeji.com

[Q36] 左连接
来源：http://prq.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dki.yfazqb.com

[Q37] 右连接
来源：http://fxo.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ymi.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://ded.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sby.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://kmh.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://iwo.cdnleiting.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iwb.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://yfd.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jgo.jiagoushi.top

[Q41] 多表连接
来源：http://dxv.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hbc.redwolf501.top

JOIN users u ON u.id = o.user_id
来源：http://ftd.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://mmt.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://uon.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://pfy.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zii.dashuyun.cn

[Q43] 标量子查询
来源：http://duj.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mpy.jinqigufen.top


<!-- 参考信息 -->