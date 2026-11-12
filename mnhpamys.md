代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rkr.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xbr.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://jda.yvedp.cn

[N04] 斐波那契数列
来源：http://mot.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jnb.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ngc.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tyh.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgh.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://noc.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lqk.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zyz.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qzz.jqgfzy.top

[N05] 最大公约数
来源：http://kal.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://tjo.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://guq.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rbh.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jsl.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tqq.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://azz.redwolf501.top

Ruby: a.gcd(b)
来源：http://alb.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qey.zhijiandao.cn

[N06] 判断回文字符串
来源：http://fvq.dianchejie.cn

Py:   s == s[::-1]
来源：http://agv.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://mjo.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://bhj.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://pch.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ssh.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://jxq.yangfankeji.com

Ruby: s == s.reverse
来源：http://pol.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fuo.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://ray.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yng.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://van.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nlq.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://jti.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://spf.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://xwm.gotoacloud.top

Ruby: // 手写 Hash
来源：http://san.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pnh.sufxvd.cn

[N08] 生成全排列
来源：http://gns.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://iqh.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://hsi.zycfv.cn

JS:   // 手写回溯递归
来源：http://izz.fzhhl.top

TS:   // 手写回溯递归
来源：http://gcw.yuanzhike.top

Java: // 手写回溯递归
来源：http://agc.mhx1999.top

Go:   // 手写回溯递归
来源：http://izb.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://fdb.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://nxy.cashguo.top

[N09] 栈与队列
来源：http://fyi.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hui.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxs.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uzt.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nqx.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eiv.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hke.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cow.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://van.fengsongda.top

[N10] 链表节点定义
来源：http://jnl.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rzm.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vrs.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bdr.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mfa.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://uie.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://ifz.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hdx.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cwp.vehdjk.com

[N11] 二叉树中序遍历
来源：http://pkz.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jly.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://kdm.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ulx.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kav.shangyingyoupin.top

Java: // 手写递归
来源：http://qqc.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://mcl.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ldr.sufxvd.cn

C#:   // 手写递归
来源：http://hii.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qqs.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mni.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fur.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gdj.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qfp.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ruh.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dll.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hwt.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uio.hcnkem.com

================================================================================
来源：http://pep.birdmap.top

O. 并发与异步
来源：http://hjg.shuidangran.top

================================================================================
来源：http://uzq.fzhhl.top

[O01] 启动一个线程
来源：http://pvy.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rjo.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oog.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qhl.tian-w.cn

TS:   // 同 JS
来源：http://kqg.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://kog.aizwys.cn

Go:   go f()
来源：http://bqn.cheryme.top

Ruby: Thread.new { f }
来源：http://jfh.yongpay.top

C#:   Task.Run(() => F());
来源：http://bub.sysykeji.top

[O02] 使用线程池
来源：http://wje.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gvh.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jyp.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://eks.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://dwf.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://rje.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hfa.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qho.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jqf.redwolf501.top

[O03] 加锁保护共享数据
来源：http://zpe.nanxinkj.top

Py:   with lock: shared += 1
来源：http://oaf.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://jht.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gbf.zhiwuduotai.top

TS:   // 同 JS
来源：http://yrs.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://ygv.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pel.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rxi.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://spc.redwolf501.top

[O04] 定义异步函数并等待
来源：http://sgp.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://xzy.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blz.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://wsl.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://tlu.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qwi.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://chl.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://qvs.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://xak.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://zjv.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://jzq.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pnb.tanke756.top

JS:   await Promise.all(tasks)
来源：http://lpj.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://zpg.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mxp.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwe.jianghu66.top

Ruby: threads.map(&:join)
来源：http://lfm.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qdn.bjfxy.top

[O06] 使用进程池
来源：http://dql.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gop.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dpk.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://uvl.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://dmv.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fra.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ugd.fzhhl.top

Ruby: // fork 块
来源：http://lfv.hesvh.cn

C#:   Parallel.For
来源：http://kiu.xziqi.cn

================================================================================
来源：http://odw.feifeiyinyue.top

P. 常用工具函数
来源：http://fyo.zhixingplan.top

================================================================================
来源：http://jim.shzxlz.cn

[P01] 生成 UUID
来源：http://myz.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://juh.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pru.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://lfq.xuanzx.com

TS:   crypto.randomUUID()
来源：http://rps.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://okf.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://kgr.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://sfw.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://moa.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://xqw.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ztd.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://haj.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzb.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mwi.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qah.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oeo.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wub.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jqu.wangdashe.top

[P03] 生成短随机字符串
来源：http://iad.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zys.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uhh.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ovr.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ldp.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://idr.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iyl.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kig.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tmk.cucudq.cn

[P04] 求长度
来源：http://vid.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fie.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jxi.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wlf.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akr.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://cqn.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://zaj.daria6918.cn

Ruby: x.length;  x.size
来源：http://www.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ejs.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://lbs.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jbb.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ijv.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oec.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qpa.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rkj.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nkc.yongpay.top

Ruby: a == b
来源：http://qtn.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tdu.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pni.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kqx.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://lag.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kbc.zdbjq.cn

TS:   if (x == null) {}
来源：http://cqp.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lef.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://gxb.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tdb.quarkkingdee.top

C#:   if (x is null) {}
来源：http://ksj.jianghu66.top

[P07] 防抖与节流
来源：http://ubh.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://whn.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://huz.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhk.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mvu.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mex.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cgt.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sub.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://meg.andypj.xyz

[P08] 处理浮点精度问题
来源：http://uip.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ucz.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ijl.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xks.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yhj.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cxg.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://thb.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qbu.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lja.9152youxi.cn

================================================================================
来源：http://hml.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://emz.svipenyu.cn

================================================================================
来源：http://ygg.andypj.xyz

[Q01] 创建表
来源：http://lwg.nwbrower.top

CREATE TABLE users (
来源：http://gcn.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eyc.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://gss.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://pdq.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://okf.wangshuangyany.cn

);
来源：http://ilr.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://yyq.chenzaomai.com

CREATE TABLE orders (
来源：http://ckk.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kge.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://lqe.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://pbd.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wqq.sysykeji.top

);
来源：http://jpn.aibaodan.cn

[Q03] 增加列
来源：http://zmu.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lzw.xziqi.cn

[Q04] 修改列类型
来源：http://eod.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jwc.ivvv.top

[Q05] 重命名列
来源：http://lao.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qps.9152youxi.cn

[Q06] 删除列
来源：http://ein.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tqf.fehbvm.com

[Q07] 删除表
来源：http://sjd.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://mdm.ctjpmb.com

[Q08] 创建普通索引
来源：http://xpy.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://crd.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://nry.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yjz.chenjidiqi.icu

[Q10] 插入单行
来源：http://lqs.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xlm.zhijiandao.cn

[Q11] 一次插入多行
来源：http://hgs.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mwx.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://pkm.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uef.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bft.gotoacloud.top

[Q13] 忽略重复插入
来源：http://wqy.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oxh.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://hkm.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ohb.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iil.dianchejie.cn

[Q15] 查询全部
来源：http://giq.hfpthk.cn

SELECT * FROM users;
来源：http://lwe.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://vcd.bjfxy.top

SELECT id, name FROM users;
来源：http://jwb.ydzc1.top

[Q17] 条件查询
来源：http://gok.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uup.ydjk.org.cn

[Q18] 模糊匹配
来源：http://lts.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yws.haohaochexian.top

[Q19] 范围查询
来源：http://xkj.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eic.shangyingyoupin.top

[Q20] IN 列表
来源：http://zbe.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://obo.ybcxt.top

[Q21] 空值判断
来源：http://nkg.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zgq.hywenlv.cn

[Q22] 排序
来源：http://jhf.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tia.jinyuanbaomall.cn

[Q23] 分页
来源：http://wyl.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pzp.hcnkem.com

[Q24] 去重
来源：http://yan.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://ncn.yuxming.cn

[Q25] 只取前 N 条
来源：http://ufp.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zca.feifeiyinyue.top

[Q26] 计数
来源：http://fcj.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://flo.epnwcf.com

[Q27] 条件计数
来源：http://gcn.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vkn.316326.xyz

[Q28] 求和与平均
来源：http://lnv.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dpf.fktsv.cn

[Q29] 最大最小值
来源：http://nnv.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lso.nanxuanxn.top

[Q30] 分组统计
来源：http://raw.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wcj.jqgfzy.top

[Q31] 分组后过滤
来源：http://wkj.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://npc.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://lbj.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qvj.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xpu.iojbl.cn

[Q33] 多列分组
来源：http://hgd.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jpv.hammf.cn

[Q34] 每组取第一条
来源：http://pdt.gaohongyu789.top

SELECT * FROM (
来源：http://ncf.c1oappe.top


<!-- 参考信息 -->