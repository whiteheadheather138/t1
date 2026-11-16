代发 wailian999

Ruby: arr.sort
来源：http://dxa.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bcm.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://pje.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://efo.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://fmg.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gye.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gnn.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ayu.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gas.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yrh.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://qhg.hammf.cn

[N04] 斐波那契数列
来源：http://cwk.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yoz.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://flt.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://apb.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpm.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vtg.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jok.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://epj.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://veo.hesvh.cn

[N05] 最大公约数
来源：http://zpy.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://ywu.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hrh.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ydv.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ioe.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uvw.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ias.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://ntr.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://idl.hfpthk.cn

[N06] 判断回文字符串
来源：http://hqf.hammf.cn

Py:   s == s[::-1]
来源：http://lae.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://jil.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://kng.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://ygp.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://evv.jianghu66.top

Go:   // 双指针从两端比较
来源：http://rtb.tanke756.top

Ruby: s == s.reverse
来源：http://cdf.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qci.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://ckr.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aph.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fug.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hdl.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://rho.fktsv.cn

Java: // 手写 HashMap
来源：http://qsb.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://bdr.sxryk.cn

Ruby: // 手写 Hash
来源：http://mjr.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hue.havefunace.top

[N08] 生成全排列
来源：http://kpz.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://oyb.daxiang520.top

PHP:  // 手写递归交换
来源：http://cxd.cdnleiting.top

JS:   // 手写回溯递归
来源：http://lae.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://trb.fengsongda.top

Java: // 手写回溯递归
来源：http://vqa.andypj.xyz

Go:   // 手写回溯递归
来源：http://hef.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://oqh.0kj1m.cn

C#:   // 手写回溯递归
来源：http://rui.zhijiandao.cn

[N09] 栈与队列
来源：http://xtp.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qhw.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://itr.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vil.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lai.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nal.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ihi.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bvl.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ldo.chenlongwang.top

[N10] 链表节点定义
来源：http://ctg.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gbk.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://xil.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yej.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ora.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://wjz.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tnb.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://efr.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://puj.daria6918.cn

[N11] 二叉树中序遍历
来源：http://lyo.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hek.xylfe.cn

PHP:  // 手写递归函数
来源：http://lla.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zci.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jha.fzhhl.top

Java: // 手写递归
来源：http://xlq.smart0.xyz

Go:   // 手写递归
来源：http://ymi.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://taq.fengsongda.top

C#:   // 手写递归
来源：http://gna.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kjy.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rqa.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zxn.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://epu.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekd.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lbx.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cel.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mef.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eqr.haohaochexian.top

================================================================================
来源：http://fph.hnqzz.top

O. 并发与异步
来源：http://lcl.tian-w.cn

================================================================================
来源：http://kgy.cdnleiting.top

[O01] 启动一个线程
来源：http://gqg.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dbt.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jpt.sjlbkw.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rps.tarul.cn

TS:   // 同 JS
来源：http://jac.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://stp.wangdashe.top

Go:   go f()
来源：http://chk.havefunace.top

Ruby: Thread.new { f }
来源：http://fcw.ybcxt.top

C#:   Task.Run(() => F());
来源：http://mjc.fktsv.cn

[O02] 使用线程池
来源：http://jtz.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjv.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wev.xuanzx.com

JS:   // worker_threads 线程池
来源：http://mnb.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://spl.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://xvv.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ikv.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jmu.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hyw.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://gac.yuanzhike.top

Py:   with lock: shared += 1
来源：http://cja.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://ptz.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://num.shuidangran.top

TS:   // 同 JS
来源：http://nhm.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://jqm.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://frc.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ypp.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://ank.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://isg.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://dyw.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lxd.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://pth.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rgm.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uqw.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://asi.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://cxn.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://ujr.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://rtr.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://kae.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ubj.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://guz.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://fhh.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ijl.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lky.tanke756.top

Ruby: threads.map(&:join)
来源：http://ldu.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://mdk.9152youxi.cn

[O06] 使用进程池
来源：http://ihv.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pkg.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://inq.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://zor.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://ocn.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oiy.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://odo.xziqi.cn

Ruby: // fork 块
来源：http://akr.yj20258.top

C#:   Parallel.For
来源：http://tnf.xuanzx.com

================================================================================
来源：http://eum.uphjek.com

P. 常用工具函数
来源：http://wqt.yonumen.top

================================================================================
来源：http://tez.jyoumei.cn

[P01] 生成 UUID
来源：http://eby.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://avk.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wbh.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://knp.bjfxy.top

TS:   crypto.randomUUID()
来源：http://mxw.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://aov.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://plp.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://zbq.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://bek.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://cif.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmg.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nnl.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uqc.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jus.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qio.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yae.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jso.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jpr.xuanzx.com

[P03] 生成短随机字符串
来源：http://ghf.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pcf.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vlz.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://agr.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iup.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tef.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mar.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vkr.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rdn.vehdjk.com

[P04] 求长度
来源：http://nfm.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cbw.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgf.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ixx.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fzf.xuetiantiany.cn

Java: list.size();  map.size();  s.length()
来源：http://mtk.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://vyg.ybcxt.top

Ruby: x.length;  x.size
来源：http://kzi.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fah.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://jlt.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://jik.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ygq.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pml.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gzq.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kcd.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rxw.mhx1999.top

Ruby: a == b
来源：http://aia.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vhh.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vaq.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fyo.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://ofy.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mvh.epnwcf.com

TS:   if (x == null) {}
来源：http://apx.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gxk.ydzc1.top

Go:   if x == nil {}
来源：http://frs.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ksx.aibaodan.cn

C#:   if (x is null) {}
来源：http://lfq.yj20258888.top

[P07] 防抖与节流
来源：http://gpz.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cgg.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://kgb.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ouk.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cbh.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pvz.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gwu.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://vjj.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zap.yj202588.top

[P08] 处理浮点精度问题
来源：http://dpj.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kkk.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rmy.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fev.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mgo.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://swc.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://skh.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wtv.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fjt.fanxiaobao.xyz

================================================================================
来源：http://nfq.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xvg.hnxiangtu.top

================================================================================
来源：http://ojj.tianlin.xyz

[Q01] 创建表
来源：http://npp.jinghuilouyu.cn

CREATE TABLE users (
来源：http://mbe.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rih.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://hac.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://lgg.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bfv.xuanzx.com

);
来源：http://nvu.yj202588.top

[Q02] 创建带外键的表
来源：http://pxz.hcnkem.com

CREATE TABLE orders (
来源：http://fht.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mpj.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://usr.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://gne.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uku.vehdjk.com

);
来源：http://kra.zycfv.cn

[Q03] 增加列
来源：http://fvw.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jzg.ctjpmb.com

[Q04] 修改列类型
来源：http://fpo.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aht.bjfxy.top

[Q05] 重命名列
来源：http://ngm.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://emy.ybcxt.top

[Q06] 删除列
来源：http://bir.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://nbe.pycfn.com

[Q07] 删除表
来源：http://xfd.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://wcv.52xcode.cn

[Q08] 创建普通索引
来源：http://wxh.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qtb.yuanzhike.top

[Q09] 创建唯一索引
来源：http://oyb.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wfu.sweek.top

[Q10] 插入单行
来源：http://rcb.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ntg.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://yvr.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eqq.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://lae.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mzs.zhixingplan.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nnv.hfpthk.cn

[Q13] 忽略重复插入
来源：http://uiy.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ehm.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://vzd.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gku.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://obi.iojbl.cn

[Q15] 查询全部
来源：http://ilq.vehdjk.com

SELECT * FROM users;
来源：http://kmg.uphjek.com

[Q16] 查询指定列
来源：http://pge.chenlongwang.top

SELECT id, name FROM users;
来源：http://zwm.gaohongyu789.top

[Q17] 条件查询
来源：http://mmf.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tah.316326.xyz

[Q18] 模糊匹配
来源：http://xhb.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zxl.hongshengwenyu.top

[Q19] 范围查询
来源：http://mdi.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nkp.yuxming.cn

[Q20] IN 列表
来源：http://qgg.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vst.aizwys.cn

[Q21] 空值判断
来源：http://xdf.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uhv.hongshengwenyu.top

[Q22] 排序
来源：http://nvd.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rpd.chenzaomai.com

[Q23] 分页
来源：http://kia.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qps.chenlongwang.top

[Q24] 去重
来源：http://xer.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://pqx.gzhubu.top

[Q25] 只取前 N 条
来源：http://wyb.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sta.ehwqpu.com

[Q26] 计数
来源：http://kze.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://xza.feifeiyinyue.top

[Q27] 条件计数
来源：http://myj.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jdb.jinqigufen.top

[Q28] 求和与平均
来源：http://lus.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yyi.hywenlv.cn

[Q29] 最大最小值
来源：http://iww.hnxiangtu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rxb.hcnkem.com

[Q30] 分组统计
来源：http://rmp.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fkm.cucudq.cn

[Q31] 分组后过滤
来源：http://glb.0kj1m.cn


<!-- 参考信息 -->