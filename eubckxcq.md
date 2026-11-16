代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://cax.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hzo.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://juh.aizwys.cn

Go:   slices.Sort(arr)
来源：http://vwe.ehwqpu.com

Ruby: arr.sort
来源：http://uxv.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://sxp.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://vob.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mgl.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://sdj.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://coq.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ryv.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rap.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://svx.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lcb.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://sjn.yj20258888.top

[N04] 斐波那契数列
来源：http://krt.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lqy.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://awb.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lnt.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysw.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ndo.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hqu.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://szx.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gwh.zdqjudy.top

[N05] 最大公约数
来源：http://uuj.jianghu66.top

Py:   math.gcd(a, b)
来源：http://vrr.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ktt.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rkr.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rux.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rke.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pci.yuanzhike.top

Ruby: a.gcd(b)
来源：http://jvw.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vsl.xylfe.cn

[N06] 判断回文字符串
来源：http://ore.zycfv.cn

Py:   s == s[::-1]
来源：http://ogw.yonumen.top

PHP:  $s === strrev($s);
来源：http://sws.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://aab.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://clf.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oet.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://zue.xinyue.icu

Ruby: s == s.reverse
来源：http://agl.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cir.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://yiv.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qcm.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dry.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lxh.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://ouq.havefunace.top

Java: // 手写 HashMap
来源：http://jxp.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://lha.ybcxt.top

Ruby: // 手写 Hash
来源：http://qkr.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sqz.gaohongyu789.top

[N08] 生成全排列
来源：http://fcg.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://hxa.yangfankeji.com

PHP:  // 手写递归交换
来源：http://gjy.fengsongda.top

JS:   // 手写回溯递归
来源：http://awu.fzhhl.top

TS:   // 手写回溯递归
来源：http://mzp.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://nrm.sysykeji.top

Go:   // 手写回溯递归
来源：http://omh.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://guk.hywenlv.cn

C#:   // 手写回溯递归
来源：http://sdj.fanxiaobao.xyz

[N09] 栈与队列
来源：http://nem.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://euz.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yxg.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zdp.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://atg.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://slp.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dnt.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nyi.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://szd.ehwqpu.com

[N10] 链表节点定义
来源：http://zlo.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wte.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hfy.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pev.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iae.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://blg.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://gow.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bpc.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://aej.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://aer.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zxb.sxryk.cn

PHP:  // 手写递归函数
来源：http://cbc.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pdn.ivvv.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfr.52xcode.cn

Java: // 手写递归
来源：http://qjw.feifeiyinyue.top

Go:   // 手写递归
来源：http://ycm.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uyn.zhoulong.xyz

C#:   // 手写递归
来源：http://ylr.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rwu.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cfj.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lmv.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://icx.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrs.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eys.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ess.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cnx.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nae.xziqi.cn

================================================================================
来源：http://sfo.xuanzx.com

O. 并发与异步
来源：http://jwi.sjlbkw.cn

================================================================================
来源：http://prv.yuanzhike.top

[O01] 启动一个线程
来源：http://lil.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pkn.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dzw.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kci.zhijiandao.cn

TS:   // 同 JS
来源：http://tdi.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://tdl.vehdjk.com

Go:   go f()
来源：http://rwo.xziqi.cn

Ruby: Thread.new { f }
来源：http://oyk.shuidangran.top

C#:   Task.Run(() => F());
来源：http://ypv.ydzc1.top

[O02] 使用线程池
来源：http://jjc.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zcy.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hvk.ivvv.top

JS:   // worker_threads 线程池
来源：http://yaq.wangdashe.top

TS:   // worker_threads 线程池
来源：http://rvo.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://jqu.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://boh.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lid.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eua.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://aso.c1oappe.top

Py:   with lock: shared += 1
来源：http://otw.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://how.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xhv.shuidangran.top

TS:   // 同 JS
来源：http://bwh.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://xvz.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nam.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yqy.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://ask.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://ace.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://xre.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wqq.yvedp.cn

JS:   async function f() { await g(); }
来源：http://bun.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxu.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gcr.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://krn.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bxj.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://iyu.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://qnj.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://ewg.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zxk.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://noi.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://bmy.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fyu.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hqr.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://aao.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tpa.cashguo.top

[O06] 使用进程池
来源：http://usf.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kfw.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uls.cheryme.top

JS:   // child_process / cluster 模块
来源：http://yvh.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://mfb.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ezj.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fic.zycfv.cn

Ruby: // fork 块
来源：http://ymr.kuanghao11.cn

C#:   Parallel.For
来源：http://gdi.yanxiufei.cn

================================================================================
来源：http://fqi.sxryk.cn

P. 常用工具函数
来源：http://stc.chenjidiqi.icu

================================================================================
来源：http://qau.guowangkeji.top

[P01] 生成 UUID
来源：http://kox.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://xve.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tty.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://hey.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://mpl.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://bwi.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://eoe.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://ohp.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://kgo.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://tyd.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ukp.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://brg.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mxm.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://knc.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://enb.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tra.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://acb.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cqx.cdnleiting.top

[P03] 生成短随机字符串
来源：http://cjn.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qqq.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lvi.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsb.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://act.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rez.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jjd.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://eyi.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vtm.ybcxt.top

[P04] 求长度
来源：http://usa.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vkp.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxm.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://phh.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hav.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://ozf.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://wad.cucudq.cn

Ruby: x.length;  x.size
来源：http://gak.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zcb.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://ghh.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uej.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://myo.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jgl.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vwk.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fcj.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://bqm.xuetiantiany.cn

Ruby: a == b
来源：http://hdy.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqf.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jjn.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eml.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://cui.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mdn.wangdashe.top

TS:   if (x == null) {}
来源：http://pjz.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kar.guannengcc.top

Go:   if x == nil {}
来源：http://lev.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ifo.ydzc1.top

C#:   if (x is null) {}
来源：http://epv.guowangkeji.top

[P07] 防抖与节流
来源：http://pcp.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kzr.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://kge.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjc.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qus.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qlk.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kzz.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hky.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://krl.xinyue.icu

[P08] 处理浮点精度问题
来源：http://lor.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://smq.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tyl.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bvg.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzq.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iel.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sfz.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bnd.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wmr.gaohongyu789.top

================================================================================
来源：http://ikj.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zpt.havefunace.top

================================================================================
来源：http://jpi.gaohongyu789.top

[Q01] 创建表
来源：http://vtu.redwolf501.top

CREATE TABLE users (
来源：http://fmm.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dkf.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://met.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://xan.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ssz.xinyue.icu

);
来源：http://dhv.yonumen.top

[Q02] 创建带外键的表
来源：http://rpg.gaohongyu789.top

CREATE TABLE orders (
来源：http://mjl.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eht.hywenlv.cn

user_id INT NOT NULL,
来源：http://mvh.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://rfl.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ejm.ydzc1.top

);
来源：http://zaz.gotoacloud.top

[Q03] 增加列
来源：http://ldd.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://spt.smart0.xyz

[Q04] 修改列类型
来源：http://htv.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vjd.mhx1999.top

[Q05] 重命名列
来源：http://sch.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qgw.nwbrower.top

[Q06] 删除列
来源：http://tbl.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://vtu.xylfe.cn

[Q07] 删除表
来源：http://ait.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://gbp.cashguo.top

[Q08] 创建普通索引
来源：http://xbm.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xwq.yueranfly.top

[Q09] 创建唯一索引
来源：http://ane.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmr.meibo888.top

[Q10] 插入单行
来源：http://uqh.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vpb.sjlbkw.cn

[Q11] 一次插入多行
来源：http://ama.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gcr.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://wzy.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ilt.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lqg.wangdashe.top

[Q13] 忽略重复插入
来源：http://vpe.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://czp.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://jcz.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rlc.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zfc.jlsjyb.cn

[Q15] 查询全部
来源：http://eyp.gogol.net.cn

SELECT * FROM users;
来源：http://xpn.sxryk.cn

[Q16] 查询指定列
来源：http://fbt.hysaishi.cn

SELECT id, name FROM users;
来源：http://vzu.zhixingplan.top

[Q17] 条件查询
来源：http://kxo.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://opx.zhoulong.xyz

[Q18] 模糊匹配
来源：http://ijk.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bim.fehbvm.com

[Q19] 范围查询
来源：http://unh.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aqp.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://fix.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xuo.cheryme.top

[Q21] 空值判断
来源：http://doc.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zmn.jianghu66.top

[Q22] 排序
来源：http://joe.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://csu.xziqi.cn

[Q23] 分页
来源：http://qhk.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vor.yj202588.top

[Q24] 去重
来源：http://xea.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://jya.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://vdy.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vnm.wangdashe.top

[Q26] 计数
来源：http://kyu.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://lhz.9152youxi.cn

[Q27] 条件计数
来源：http://tno.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://luc.mhx1999.top

[Q28] 求和与平均
来源：http://jgd.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://phn.sxryk.cn

[Q29] 最大最小值
来源：http://edd.hnxiangtu.top


<!-- 参考信息 -->