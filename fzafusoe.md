代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ukd.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://daq.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://znw.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cqn.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://mnz.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://eus.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://woq.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dlk.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xom.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uge.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rbe.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://ejn.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gat.quarkkingdee.top

[N06] 判断回文字符串
来源：http://ojt.jlsjyb.cn

Py:   s == s[::-1]
来源：http://voq.wangdashe.top

PHP:  $s === strrev($s);
来源：http://izo.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://meu.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://ale.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qxd.fktsv.cn

Go:   // 双指针从两端比较
来源：http://myr.uphjek.com

Ruby: s == s.reverse
来源：http://rmd.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://srt.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://tfp.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hwl.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tpx.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://btv.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://gjr.tianlin.xyz

Java: // 手写 HashMap
来源：http://wrg.fktsv.cn

Go:   // 手写 map[int]int
来源：http://wnu.ydzc1.top

Ruby: // 手写 Hash
来源：http://nvb.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://oti.zdqjudy.top

[N08] 生成全排列
来源：http://oqg.yonumen.top

Py:   itertools.permutations(arr)
来源：http://tnj.vehdjk.com

PHP:  // 手写递归交换
来源：http://fiw.yvedp.cn

JS:   // 手写回溯递归
来源：http://tpi.ppjwa.cn

TS:   // 手写回溯递归
来源：http://kmk.jianghu66.top

Java: // 手写回溯递归
来源：http://hxo.fehbvm.com

Go:   // 手写回溯递归
来源：http://qlv.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://fil.smart0.xyz

C#:   // 手写回溯递归
来源：http://vbi.uphjek.com

[N09] 栈与队列
来源：http://fqg.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fov.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qwh.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mmq.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mbg.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ovp.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yez.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hqy.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wmm.gaohongyu789.top

[N10] 链表节点定义
来源：http://lbb.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://txr.xylfe.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gmc.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hrp.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mjb.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://bvc.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://brw.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sgz.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nio.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://rvb.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nlv.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://efs.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://apd.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyn.yuxming.cn

Java: // 手写递归
来源：http://agt.hammf.cn

Go:   // 手写递归
来源：http://xrb.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wox.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ftj.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kpo.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ihl.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hrw.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zxo.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mct.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wgf.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://arn.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oyp.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lzd.jinqigfzy.top

================================================================================
来源：http://vni.tarul.cn

O. 并发与异步
来源：http://xbi.52xcode.cn

================================================================================
来源：http://ekt.guannengcc.top

[O01] 启动一个线程
来源：http://lxa.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aym.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vdq.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://llv.fengsongda.top

TS:   // 同 JS
来源：http://quv.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://rxy.havefunace.top

Go:   go f()
来源：http://ayu.hywenlv.cn

Ruby: Thread.new { f }
来源：http://dii.daria6918.cn

C#:   Task.Run(() => F());
来源：http://cwg.52xcode.cn

[O02] 使用线程池
来源：http://nck.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kth.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mti.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://gpi.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://xxp.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eqc.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nnd.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://afz.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blq.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://kwi.aibaodan.cn

Py:   with lock: shared += 1
来源：http://csi.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://upj.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uvw.yj20258888.top

TS:   // 同 JS
来源：http://eqr.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://gis.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oce.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tlx.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://cip.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://ixv.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://pbg.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rpr.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://qba.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oap.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uny.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://utw.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://czl.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://otf.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://cuq.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://oxo.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aei.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://ayi.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://xvw.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nbo.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rga.jianghu66.top

Ruby: threads.map(&:join)
来源：http://dfb.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://zfj.nanxinkj.top

[O06] 使用进程池
来源：http://fxj.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rxq.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ccd.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://jpg.yongpay.top

TS:   // child_process / cluster 模块
来源：http://zei.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fji.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qac.fengsongda.top

Ruby: // fork 块
来源：http://dah.shanyushiyangtech.top

C#:   Parallel.For
来源：http://ajj.nwbrower.top

================================================================================
来源：http://isg.hnxiangtu.top

P. 常用工具函数
来源：http://rpc.cqqwz.cn

================================================================================
来源：http://vmh.jqgufenzy.top

[P01] 生成 UUID
来源：http://bdq.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://akl.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ozs.nwbrower.top

JS:   crypto.randomUUID()
来源：http://yci.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://dxn.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://msl.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://iet.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://rir.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://huk.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://dvp.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://exs.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oof.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://btt.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://stu.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zus.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://znh.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wem.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tse.smart0.xyz

[P03] 生成短随机字符串
来源：http://frm.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iuu.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zzm.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nlu.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oxf.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aub.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qqh.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aks.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hin.tianlin.xyz

[P04] 求长度
来源：http://mrm.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://spx.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cjb.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fke.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlt.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://fei.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://kmz.mhx1999.top

Ruby: x.length;  x.size
来源：http://kyj.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://njk.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://umd.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gov.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bjy.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tux.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rla.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sgu.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://enx.shzxlz.cn

Ruby: a == b
来源：http://hfp.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://roz.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://woh.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ixz.havefunace.top

PHP:  if (empty($x)) {}
来源：http://vhc.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ovw.birdmap.top

TS:   if (x == null) {}
来源：http://cje.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qiq.52xcode.cn

Go:   if x == nil {}
来源：http://czr.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wib.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://esq.nanxinkj.top

[P07] 防抖与节流
来源：http://orc.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://emw.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://tum.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kqn.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ucv.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tlq.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dmw.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nve.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://neo.yj20258.top

[P08] 处理浮点精度问题
来源：http://dob.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ohi.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bda.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://phi.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://off.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ull.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lbk.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tao.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xef.smart0.xyz

================================================================================
来源：http://yte.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ohv.52xcode.cn

================================================================================
来源：http://dqb.xylfe.cn

[Q01] 创建表
来源：http://uzg.ppjwa.cn

CREATE TABLE users (
来源：http://aat.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qwm.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://sgg.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://ark.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eea.zhongyouzk.top

);
来源：http://bfy.cheryme.top

[Q02] 创建带外键的表
来源：http://jqb.vehdjk.com

CREATE TABLE orders (
来源：http://qja.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oni.fengsongda.top

user_id INT NOT NULL,
来源：http://prl.havefunace.top

amount DECIMAL(10, 2),
来源：http://mhv.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fbz.9152youxi.cn

);
来源：http://afz.zdqjudy.top

[Q03] 增加列
来源：http://pnq.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ulx.aibaodan.cn

[Q04] 修改列类型
来源：http://sfp.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yzn.cqqwz.cn

[Q05] 重命名列
来源：http://jyr.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xgz.gzhubu.top

[Q06] 删除列
来源：http://wlc.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://mne.zhongyouzk.top

[Q07] 删除表
来源：http://hgy.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://wgd.svipenyu.cn

[Q08] 创建普通索引
来源：http://alb.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qhl.cucudq.cn

[Q09] 创建唯一索引
来源：http://key.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ufn.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://jfw.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zbq.hesvh.cn

[Q11] 一次插入多行
来源：http://beo.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kxf.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://iea.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://wop.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jde.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://avd.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hwc.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://qbn.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://crt.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uxf.yuanzhike.top

[Q15] 查询全部
来源：http://esv.hywenlv.cn

SELECT * FROM users;
来源：http://wth.fengsongda.top

[Q16] 查询指定列
来源：http://uks.nwbrower.top

SELECT id, name FROM users;
来源：http://pab.gotoacloud.top

[Q17] 条件查询
来源：http://ppq.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yps.daxiang520.top

[Q18] 模糊匹配
来源：http://ath.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cbh.52xcode.cn

[Q19] 范围查询
来源：http://dex.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jpi.shanyushiyangtech.top

[Q20] IN 列表
来源：http://jku.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://auy.52xcode.cn

[Q21] 空值判断
来源：http://btx.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yzp.ivvv.top

[Q22] 排序
来源：http://lbu.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jlp.hcnkem.com

[Q23] 分页
来源：http://xhf.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oqu.cqqwz.cn

[Q24] 去重
来源：http://zyw.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://dng.zycfv.cn

[Q25] 只取前 N 条
来源：http://gft.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pqd.epnwcf.com

[Q26] 计数
来源：http://tgn.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://orx.tian-w.cn

[Q27] 条件计数
来源：http://lko.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mls.smart0.xyz

[Q28] 求和与平均
来源：http://gex.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dlt.ctjpmb.com

[Q29] 最大最小值
来源：http://aqr.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tpj.ctjpmb.com

[Q30] 分组统计
来源：http://lxw.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qkp.svipenyu.cn

[Q31] 分组后过滤
来源：http://xww.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wgo.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://hjj.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cdj.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lrj.vehdjk.com

[Q33] 多列分组
来源：http://iby.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kuo.0kj1m.cn

[Q34] 每组取第一条
来源：http://xzn.ybcxt.top

SELECT * FROM (
来源：http://khc.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fqj.jqgufenzy.top

) t WHERE rn = 1;
来源：http://lds.jlsjyb.cn

[Q35] 内连接
来源：http://gdr.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fwl.dianchejie.cn

[Q36] 左连接
来源：http://zsx.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://azx.zhiwuduotai.top

[Q37] 右连接
来源：http://ksh.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://umg.tian-w.cn


<!-- 参考信息 -->