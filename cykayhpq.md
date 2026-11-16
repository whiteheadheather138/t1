代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://nei.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ugh.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nxl.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://war.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cuo.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://inx.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ydx.0kj1m.cn

[N04] 斐波那契数列
来源：http://abe.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eau.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://upm.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zwb.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ami.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uux.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wot.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tmd.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://niq.hesvh.cn

[N05] 最大公约数
来源：http://bzw.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://syn.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ics.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nan.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pld.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mej.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oxu.fehbvm.com

Ruby: a.gcd(b)
来源：http://pmj.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ors.andypj.xyz

[N06] 判断回文字符串
来源：http://xpd.9152youxi.cn

Py:   s == s[::-1]
来源：http://nat.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://yij.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://tad.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://fxr.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://okc.smart0.xyz

Go:   // 双指针从两端比较
来源：http://pck.sufxvd.cn

Ruby: s == s.reverse
来源：http://mbt.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qcs.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://qaq.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gzf.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zhy.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zot.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://eoa.wangdashe.top

Java: // 手写 HashMap
来源：http://voq.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://ios.hnqzz.top

Ruby: // 手写 Hash
来源：http://xak.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://ppn.9152youxi.cn

[N08] 生成全排列
来源：http://sxe.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://sdk.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://pda.shzxlz.cn

JS:   // 手写回溯递归
来源：http://ilw.yuanzhike.top

TS:   // 手写回溯递归
来源：http://arc.52xcode.cn

Java: // 手写回溯递归
来源：http://njd.xuanzx.com

Go:   // 手写回溯递归
来源：http://fxj.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://awf.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://rxr.0kj1m.cn

[N09] 栈与队列
来源：http://rqm.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lpe.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ake.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kev.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dvm.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lva.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kim.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://udp.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cas.jinqigufen.top

[N10] 链表节点定义
来源：http://bji.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nev.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://now.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://emy.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bzr.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://qjz.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://qsg.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rex.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qzx.dianchejie.cn

[N11] 二叉树中序遍历
来源：http://sze.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://buq.ppjwa.cn

PHP:  // 手写递归函数
来源：http://jjm.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upt.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwo.jinghuilouyu.cn

Java: // 手写递归
来源：http://pfr.xziqi.cn

Go:   // 手写递归
来源：http://vcl.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ylw.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://yek.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fvy.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wlz.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rpv.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijt.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oot.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwh.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hyg.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://elb.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dkd.sxryk.cn

================================================================================
来源：http://odn.zhijiandao.cn

O. 并发与异步
来源：http://qks.haohaochexian.top

================================================================================
来源：http://exx.cucudq.cn

[O01] 启动一个线程
来源：http://htg.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qau.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://erh.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hxi.hywenlv.cn

TS:   // 同 JS
来源：http://yra.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://fmo.hnxiangtu.top

Go:   go f()
来源：http://wwp.fzhhl.top

Ruby: Thread.new { f }
来源：http://epe.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://vxg.52xcode.cn

[O02] 使用线程池
来源：http://skm.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rhy.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ktl.yj20258.top

JS:   // worker_threads 线程池
来源：http://icl.iojbl.cn

TS:   // worker_threads 线程池
来源：http://mre.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://erg.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vhx.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://czb.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eav.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://miv.meibo888.top

Py:   with lock: shared += 1
来源：http://blv.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://quy.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cwy.jqgufenzy.top

TS:   // 同 JS
来源：http://btc.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://vml.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eht.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://zwp.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://nwa.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://dgn.uphjek.com

Py:   async def f():⏎    await g()
来源：http://gfa.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jvt.yj20258888.top

JS:   async function f() { await g(); }
来源：http://hko.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rin.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zzm.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lgs.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rvy.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://kyw.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://lkn.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://fjv.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nxy.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://ybv.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://rst.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lvx.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wkr.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://qkv.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lfz.shanyushiyangtech.top

[O06] 使用进程池
来源：http://qds.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qei.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wuq.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://zag.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://yeq.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ijj.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lik.vehdjk.com

Ruby: // fork 块
来源：http://wvp.jiagoushi.top

C#:   Parallel.For
来源：http://efg.gzhubu.top

================================================================================
来源：http://fqx.yj20258.top

P. 常用工具函数
来源：http://dpb.xingfuxueyuan.xyz

================================================================================
来源：http://oir.dashuyun.cn

[P01] 生成 UUID
来源：http://hkg.tarul.cn

Py:   str(uuid.uuid4())
来源：http://swv.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ezt.mhx1999.top

JS:   crypto.randomUUID()
来源：http://gni.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://wak.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://sui.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://fon.tanke756.top

Ruby: SecureRandom.uuid
来源：http://evj.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://ysv.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://upl.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cai.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://dud.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://etv.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mzv.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ool.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lyg.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://osx.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wey.fktsv.cn

[P03] 生成短随机字符串
来源：http://cco.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ccb.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tfi.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vqe.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqx.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wcz.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xse.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://whb.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pkj.daxiang520.top

[P04] 求长度
来源：http://pue.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dwn.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hfb.smart0.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vbc.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vvx.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://hfw.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://kae.yj202588.top

Ruby: x.length;  x.size
来源：http://yef.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gft.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://una.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zge.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lgs.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sxw.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pon.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xzy.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://quh.sufxvd.cn

Ruby: a == b
来源：http://txd.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://meg.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://odj.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nwz.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://ylw.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://unv.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://lwf.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ice.zdqjudy.top

Go:   if x == nil {}
来源：http://kdn.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qfl.tian-w.cn

C#:   if (x is null) {}
来源：http://hlf.cashguo.top

[P07] 防抖与节流
来源：http://gsk.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://niy.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://wpz.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fmu.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjg.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://erz.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hdb.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dnu.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gdm.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://qen.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://avs.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cvm.hysaishi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nsp.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://all.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tvc.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lhy.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rto.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fyp.cdnleiting.top

================================================================================
来源：http://cug.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vcu.quarkkingdee.top

================================================================================
来源：http://bia.c1oappe.top

[Q01] 创建表
来源：http://vqc.xuetiantiany.cn

CREATE TABLE users (
来源：http://wzj.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fag.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://qte.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://ban.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://csz.c1oappe.top

);
来源：http://gtu.tarul.cn

[Q02] 创建带外键的表
来源：http://whh.sufxvd.cn

CREATE TABLE orders (
来源：http://con.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jvy.zhoulong.xyz

user_id INT NOT NULL,
来源：http://jzy.uphjek.com

amount DECIMAL(10, 2),
来源：http://tpe.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bbg.uphjek.com

);
来源：http://hbz.c1oappe.top

[Q03] 增加列
来源：http://vkq.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ahk.jiagoushi.top

[Q04] 修改列类型
来源：http://gbm.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wgz.jinqigfzy.top

[Q05] 重命名列
来源：http://slk.yongpay.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mco.meibo888.top

[Q06] 删除列
来源：http://zne.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zyc.uphjek.com

[Q07] 删除表
来源：http://hyn.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://ffw.aizwys.cn

[Q08] 创建普通索引
来源：http://wki.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://poa.nwbrower.top

[Q09] 创建唯一索引
来源：http://xcl.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dlc.zhixingplan.top

[Q10] 插入单行
来源：http://mhv.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iml.bjfxy.top

[Q11] 一次插入多行
来源：http://arq.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vnu.ivvv.top

[Q12] 插入后取自增 ID
来源：http://mfh.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://hju.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mad.gogol.net.cn

[Q13] 忽略重复插入
来源：http://qsi.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tpm.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://mlg.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ncn.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ssv.ppjwa.cn

[Q15] 查询全部
来源：http://bbz.fzhhl.top

SELECT * FROM users;
来源：http://kuj.yuxming.cn

[Q16] 查询指定列
来源：http://xvc.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://vxf.epnwcf.com

[Q17] 条件查询
来源：http://rjg.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jpm.jiagoushi.top

[Q18] 模糊匹配
来源：http://iod.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://npp.birdmap.top

[Q19] 范围查询
来源：http://sxg.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zaw.jyoumei.cn

[Q20] IN 列表
来源：http://jzq.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xwu.kuanghao11.cn

[Q21] 空值判断
来源：http://nzn.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qep.nwbrower.top

[Q22] 排序
来源：http://eaw.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cnd.pengpengdd.cyou

[Q23] 分页
来源：http://oic.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://csy.gaohongyu789.top

[Q24] 去重
来源：http://udo.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://okd.ivvv.top

[Q25] 只取前 N 条
来源：http://von.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gex.cqqwz.cn

[Q26] 计数
来源：http://fjy.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://yzv.feifeiyinyue.top

[Q27] 条件计数
来源：http://mex.haohaochexian.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tqn.zhixingplan.top

[Q28] 求和与平均
来源：http://stu.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vpr.yongpay.top

[Q29] 最大最小值
来源：http://tpq.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lyc.jlsjyb.cn

[Q30] 分组统计
来源：http://jeb.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rua.ppjwa.cn

[Q31] 分组后过滤
来源：http://wff.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xxl.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://nad.xziqi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rwa.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rcn.redwolf501.top


<!-- 参考信息 -->