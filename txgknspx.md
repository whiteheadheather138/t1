代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://ymh.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvx.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xha.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://maz.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ihk.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xob.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oce.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://kbq.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://srx.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jvs.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwk.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ews.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lwp.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hdp.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fpi.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://evq.bjfxy.top

[N05] 最大公约数
来源：http://ddx.mhx1999.top

Py:   math.gcd(a, b)
来源：http://qqt.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kyw.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlk.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swu.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rrl.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mws.bbcook.cn

Ruby: a.gcd(b)
来源：http://rqb.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://npc.xuanzx.com

[N06] 判断回文字符串
来源：http://ych.jlsjyb.cn

Py:   s == s[::-1]
来源：http://ecl.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://gsy.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://dpr.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://wtf.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gpw.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://dhp.bjfxy.top

Ruby: s == s.reverse
来源：http://qqu.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nex.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://xtu.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://awq.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fcp.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ytq.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://ypm.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://qcq.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://spy.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://nqq.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://yjl.hfpthk.cn

[N08] 生成全排列
来源：http://mzm.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://ght.nwbrower.top

PHP:  // 手写递归交换
来源：http://new.redwolf501.top

JS:   // 手写回溯递归
来源：http://srx.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://cfn.yj202588.top

Java: // 手写回溯递归
来源：http://rfw.cashguo.top

Go:   // 手写回溯递归
来源：http://hiv.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://jmj.ctjpmb.com

C#:   // 手写回溯递归
来源：http://lex.fehbvm.com

[N09] 栈与队列
来源：http://vaa.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ich.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tkb.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eqb.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mhg.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hbs.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cis.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://boz.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://elr.cheryme.top

[N10] 链表节点定义
来源：http://qcr.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://koz.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oor.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nxr.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sam.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://kqg.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://lck.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://soh.tian-w.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://klf.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://fch.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gsh.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://bpg.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cni.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tni.9152youxi.cn

Java: // 手写递归
来源：http://cuf.ppjwa.cn

Go:   // 手写递归
来源：http://muy.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lhp.yuxming.cn

C#:   // 手写递归
来源：http://vtm.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://odq.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oos.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://grf.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ojd.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhd.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qnb.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fgl.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ywu.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rbq.jinyuanbaomall.cn

================================================================================
来源：http://qqk.xuanzx.com

O. 并发与异步
来源：http://odc.9152youxi.cn

================================================================================
来源：http://dry.xuanzx.com

[O01] 启动一个线程
来源：http://qlg.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rvr.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://olk.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yqd.hysaishi.cn

TS:   // 同 JS
来源：http://pqz.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://hqo.ppjwa.cn

Go:   go f()
来源：http://mml.chenlongwang.top

Ruby: Thread.new { f }
来源：http://kar.xuanzx.com

C#:   Task.Run(() => F());
来源：http://iex.zhixingplan.top

[O02] 使用线程池
来源：http://zrt.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zdt.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bxk.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://tjm.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://czh.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://ulx.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nkl.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ehn.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mzp.yueranfly.top

[O03] 加锁保护共享数据
来源：http://ape.9152youxi.cn

Py:   with lock: shared += 1
来源：http://osp.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://weo.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oac.yueranfly.top

TS:   // 同 JS
来源：http://uqj.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://ppc.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://luv.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xmy.sweek.top

C#:   lock (gate) { shared++; }
来源：http://qgw.yfazqb.com

[O04] 定义异步函数并等待
来源：http://eel.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://xqq.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hmx.c1oappe.top

JS:   async function f() { await g(); }
来源：http://xwo.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jko.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dxg.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://odt.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gir.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://sbu.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://fgp.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://mpl.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vlo.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://mkp.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://cwf.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dne.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eca.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://srk.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jnz.9152youxi.cn

[O06] 使用进程池
来源：http://fmp.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iej.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xna.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://csq.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://zfn.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ypp.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wqk.ehwqpu.com

Ruby: // fork 块
来源：http://btd.yonumen.top

C#:   Parallel.For
来源：http://odj.ydzc1.top

================================================================================
来源：http://kri.cdnleiting.top

P. 常用工具函数
来源：http://ujg.yongpay.top

================================================================================
来源：http://dta.shangyingyoupin.top

[P01] 生成 UUID
来源：http://vdp.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://tdi.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://otl.birdmap.top

JS:   crypto.randomUUID()
来源：http://ulu.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://wsb.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://fty.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://gdq.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://rbk.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://eab.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://pqb.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zqp.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cfr.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pmg.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rqe.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://seo.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ddp.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rfq.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwl.fehbvm.com

[P03] 生成短随机字符串
来源：http://hhe.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://unn.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sni.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jrm.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jeh.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qpf.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nbq.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xok.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bai.yanxiufei.cn

[P04] 求长度
来源：http://qhk.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qfv.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfa.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bfm.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rey.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://tti.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://ijg.aizwys.cn

Ruby: x.length;  x.size
来源：http://xiv.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://kbk.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://dne.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://spr.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vab.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rae.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://okh.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jzf.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://nxx.quarkkingdee.top

Ruby: a == b
来源：http://owo.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://goi.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kam.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mbv.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://xhn.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hwi.yueranfly.top

TS:   if (x == null) {}
来源：http://elx.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pus.gotoacloud.top

Go:   if x == nil {}
来源：http://vyb.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lpz.vqdsnc.cn

C#:   if (x is null) {}
来源：http://zwv.tianlin.xyz

[P07] 防抖与节流
来源：http://bcv.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xin.uphjek.com

PHP:  // 手写时间戳比较
来源：http://pug.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywn.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cei.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ubb.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oam.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dta.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kvd.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://lbu.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wcq.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zxn.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zrl.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wch.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://idz.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ojw.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xml.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://waf.yangfankeji.com

================================================================================
来源：http://fhr.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cop.vehdjk.com

================================================================================
来源：http://gdf.gogol.net.cn

[Q01] 创建表
来源：http://vpg.chenjidiqi.icu

CREATE TABLE users (
来源：http://kat.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vxr.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://jve.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://fvr.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vzx.zycfv.cn

);
来源：http://mmd.sxryk.cn

[Q02] 创建带外键的表
来源：http://uzu.quarkkingdee.top

CREATE TABLE orders (
来源：http://pfo.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbh.xinyue.icu

user_id INT NOT NULL,
来源：http://jiy.c1oappe.top

amount DECIMAL(10, 2),
来源：http://yxc.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yck.iojbl.cn

);
来源：http://juu.yueranfly.top

[Q03] 增加列
来源：http://lqa.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mvb.ehwqpu.com

[Q04] 修改列类型
来源：http://xze.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://luh.dianchejie.cn

[Q05] 重命名列
来源：http://iky.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pzr.shanyushiyangkeji.top

[Q06] 删除列
来源：http://crj.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://pcd.smart0.xyz

[Q07] 删除表
来源：http://gfu.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://tis.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://xsu.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://brk.cucudq.cn

[Q09] 创建唯一索引
来源：http://ddl.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xwd.jinqigufen.top

[Q10] 插入单行
来源：http://dcj.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://apc.shuidangran.top

[Q11] 一次插入多行
来源：http://pfb.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kmi.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://sxc.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://kny.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://scq.yj20258.top

[Q13] 忽略重复插入
来源：http://uxb.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://anq.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://epq.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oeu.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sdq.cqqwz.cn

[Q15] 查询全部
来源：http://qpt.iojbl.cn

SELECT * FROM users;
来源：http://zfo.xuetiantiany.cn

[Q16] 查询指定列
来源：http://tqt.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://zru.cqqwz.cn

[Q17] 条件查询
来源：http://gux.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nwn.ydjk.org.cn

[Q18] 模糊匹配
来源：http://ael.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://una.jlsjyb.cn

[Q19] 范围查询
来源：http://ynb.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ebs.havefunace.top

[Q20] IN 列表
来源：http://qdy.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dso.xuanzx.com

[Q21] 空值判断
来源：http://hly.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vwm.fanxiaobao.xyz

[Q22] 排序
来源：http://ikt.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zbk.cheryme.top

[Q23] 分页
来源：http://bxe.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fhh.aibaodan.cn

[Q24] 去重
来源：http://kqr.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://inq.shzxlz.cn

[Q25] 只取前 N 条
来源：http://tgc.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jov.0kj1m.cn

[Q26] 计数
来源：http://wca.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://yal.fengsongda.top

[Q27] 条件计数
来源：http://onk.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aga.gotoacloud.top

[Q28] 求和与平均
来源：http://eaf.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://huo.jinghuilouyu.cn

[Q29] 最大最小值
来源：http://hgl.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://nal.daria6918.cn

[Q30] 分组统计
来源：http://pcw.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ucs.c1oappe.top

[Q31] 分组后过滤
来源：http://tou.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xww.birdmap.top

[Q32] 分组拼接字符串
来源：http://ytd.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mup.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jru.316326.xyz


<!-- 参考信息 -->