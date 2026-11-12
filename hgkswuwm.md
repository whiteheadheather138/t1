代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yhd.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gva.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ida.havefunace.top

Ruby: a.gcd(b)
来源：http://acc.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bgn.aizwys.cn

[N06] 判断回文字符串
来源：http://xyu.yueranfly.top

Py:   s == s[::-1]
来源：http://iux.yuxming.cn

PHP:  $s === strrev($s);
来源：http://yro.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://qac.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://xnh.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://scv.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://fmu.zycfv.cn

Ruby: s == s.reverse
来源：http://rxn.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qeh.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://ltm.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://byi.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://esf.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://aci.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://sbk.snrcjt.cn

Java: // 手写 HashMap
来源：http://hyr.tarul.cn

Go:   // 手写 map[int]int
来源：http://zvf.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://ado.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://lst.sysykeji.top

[N08] 生成全排列
来源：http://yuw.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://tst.yuxming.cn

PHP:  // 手写递归交换
来源：http://tlx.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://kfb.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://ict.daxiang520.top

Java: // 手写回溯递归
来源：http://yxb.cdnleiting.top

Go:   // 手写回溯递归
来源：http://uas.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://lxk.hammf.cn

C#:   // 手写回溯递归
来源：http://mkc.hnqzz.top

[N09] 栈与队列
来源：http://nck.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gqo.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ucp.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dla.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tbu.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jsq.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bhs.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yhi.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yxb.zdqjudy.top

[N10] 链表节点定义
来源：http://pnb.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pja.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://gko.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ifw.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ehl.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://efm.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://fnn.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mwm.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kqk.jianghu66.top

[N11] 二叉树中序遍历
来源：http://hia.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xsw.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://szk.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xtv.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ogz.gaohongyu789.top

Java: // 手写递归
来源：http://iub.yuxming.cn

Go:   // 手写递归
来源：http://ryc.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ezg.hcnkem.com

C#:   // 手写递归
来源：http://ids.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hhm.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bga.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ewi.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfv.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yiy.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ekz.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hub.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rnj.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gek.jianghu66.top

================================================================================
来源：http://igz.ydjk.org.cn

O. 并发与异步
来源：http://dul.jiagoushi.top

================================================================================
来源：http://rgr.snrcjt.cn

[O01] 启动一个线程
来源：http://rnu.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cmz.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ksf.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blr.zhongyouzk.top

TS:   // 同 JS
来源：http://dvs.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://zqg.gotoacloud.top

Go:   go f()
来源：http://aah.shzxlz.cn

Ruby: Thread.new { f }
来源：http://epf.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://ucm.chenlongwang.top

[O02] 使用线程池
来源：http://oyd.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qcx.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kmm.shuidangran.top

JS:   // worker_threads 线程池
来源：http://sda.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://nqt.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://puu.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ujd.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gwl.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://umt.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://aej.fengsongda.top

Py:   with lock: shared += 1
来源：http://vqe.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://qpo.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gzz.zhongyouzk.top

TS:   // 同 JS
来源：http://pjt.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://lai.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tcx.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zdj.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://vwx.yonumen.top

[O04] 定义异步函数并等待
来源：http://sgr.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://trv.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cjo.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://djf.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://flr.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ofz.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eiv.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://puy.hammf.cn

C#:   async Task F() { await G(); }
来源：http://ugx.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://cgg.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://rvc.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://stx.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://frk.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://qja.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vmo.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bzo.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://ssc.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://icg.cheryme.top

[O06] 使用进程池
来源：http://cph.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://izv.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lsf.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://lri.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://trj.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dkk.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://drl.zhongyouzk.top

Ruby: // fork 块
来源：http://mvw.gzhubu.top

C#:   Parallel.For
来源：http://wsm.jyoumei.cn

================================================================================
来源：http://vyp.cdnleiting.top

P. 常用工具函数
来源：http://fuo.dashuyun.cn

================================================================================
来源：http://fet.52xcode.cn

[P01] 生成 UUID
来源：http://ahh.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://lig.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uwx.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://wkm.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://jod.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://xof.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://wyt.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://kxe.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://nht.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://vfk.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vua.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kit.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pvj.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://god.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mdz.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hhe.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kwv.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ayu.birdmap.top

[P03] 生成短随机字符串
来源：http://osh.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bkq.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gwa.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uhh.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obm.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wmx.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rmg.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://urj.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xxo.316326.xyz

[P04] 求长度
来源：http://rrm.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://prj.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kns.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://esj.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hro.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://fqi.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://pjt.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://wjz.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bbq.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://drv.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://bqz.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cce.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sua.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tev.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rrb.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lha.hywenlv.cn

Ruby: a == b
来源：http://gxc.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bsw.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zja.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fkw.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://bfa.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tnm.sweek.top

TS:   if (x == null) {}
来源：http://kuu.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uur.zhengqikj.top

Go:   if x == nil {}
来源：http://tbn.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dkn.0kj1m.cn

C#:   if (x is null) {}
来源：http://xox.pycfn.com

[P07] 防抖与节流
来源：http://qrr.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gaq.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://fmc.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggj.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uig.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qia.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://btv.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dce.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zgf.yonumen.top

[P08] 处理浮点精度问题
来源：http://ynd.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gbn.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zsv.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pba.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kir.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dma.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xuh.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rbi.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pih.jyoumei.cn

================================================================================
来源：http://fgg.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zkc.yvedp.cn

================================================================================
来源：http://nra.nwbrower.top

[Q01] 创建表
来源：http://xjf.tianlin.xyz

CREATE TABLE users (
来源：http://htb.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kfe.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://hiv.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://qei.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sap.ppjwa.cn

);
来源：http://cvv.iojbl.cn

[Q02] 创建带外键的表
来源：http://ubr.hywenlv.cn

CREATE TABLE orders (
来源：http://ycy.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://agw.pycfn.com

user_id INT NOT NULL,
来源：http://gch.hcnkem.com

amount DECIMAL(10, 2),
来源：http://vvd.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wso.tianlin.xyz

);
来源：http://ykf.fengsongda.top

[Q03] 增加列
来源：http://pcv.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://knt.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://vnh.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wox.yueranfly.top

[Q05] 重命名列
来源：http://nig.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fib.guannengcc.top

[Q06] 删除列
来源：http://fym.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tsd.hammf.cn

[Q07] 删除表
来源：http://smk.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://ruy.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://kdb.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://elm.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://ipi.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fww.zdqjudy.top

[Q10] 插入单行
来源：http://kay.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zpi.tanke756.top

[Q11] 一次插入多行
来源：http://jki.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sia.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://gld.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://pyj.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aqq.gogol.net.cn

[Q13] 忽略重复插入
来源：http://wwj.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://djk.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://wxc.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://spa.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uop.fzhhl.top

[Q15] 查询全部
来源：http://fhf.hywenlv.cn

SELECT * FROM users;
来源：http://jrt.vqdsnc.cn

[Q16] 查询指定列
来源：http://kyg.jinqigufen.top

SELECT id, name FROM users;
来源：http://rpa.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://mzk.ehwqpu.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cnb.dashuyun.cn

[Q18] 模糊匹配
来源：http://kbe.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cfh.jqgfzy.top

[Q19] 范围查询
来源：http://cbp.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bad.shanyushiyangtech.top

[Q20] IN 列表
来源：http://avh.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zbl.tian-w.cn

[Q21] 空值判断
来源：http://yuj.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vgz.sjlbkw.cn

[Q22] 排序
来源：http://mqp.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eum.feifeiyinyue.top

[Q23] 分页
来源：http://low.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dfj.pengpengdd.cyou

[Q24] 去重
来源：http://usb.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://fzj.tarul.cn

[Q25] 只取前 N 条
来源：http://ugm.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xtr.hongshengwenyu.top

[Q26] 计数
来源：http://nnr.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://ghv.cucudq.cn

[Q27] 条件计数
来源：http://wld.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pdp.epnwcf.com

[Q28] 求和与平均
来源：http://ylu.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vxr.hywenlv.cn

[Q29] 最大最小值
来源：http://uke.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ysn.jinghuilouyu.cn

[Q30] 分组统计
来源：http://dox.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pxc.wangdashe.top

[Q31] 分组后过滤
来源：http://swj.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uwi.andypj.xyz

[Q32] 分组拼接字符串
来源：http://iuw.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aus.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qcc.cheryme.top

[Q33] 多列分组
来源：http://kth.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://unl.jlsjyb.cn

[Q34] 每组取第一条
来源：http://nam.havefunace.top

SELECT * FROM (
来源：http://cfm.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rnq.ydjk.org.cn

) t WHERE rn = 1;
来源：http://meo.sxryk.cn

[Q35] 内连接
来源：http://sto.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aon.ehwqpu.com

[Q36] 左连接
来源：http://uyd.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wfu.kuanghao11.cn

[Q37] 右连接
来源：http://znz.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lpm.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hnz.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://odr.pycfn.com

[Q39] 自连接（查上下级）
来源：http://vmf.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rky.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zht.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xrm.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lua.yueranfly.top

[Q41] 多表连接
来源：http://dhk.jinghuilouyu.cn


<!-- 参考信息 -->