代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://pfm.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://pgf.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://dtm.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bgq.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xdm.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gjm.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kkj.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://sif.vehdjk.com

Ruby: arr.sort
来源：http://luw.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://afz.meibo888.top

[N03] 快速排序（分治示例）
来源：http://zmi.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ctz.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://uqd.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pcz.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ldx.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kap.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://quf.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uqd.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://htu.dashuyun.cn

[N04] 斐波那契数列
来源：http://qoo.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jvh.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jph.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wru.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eek.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wpl.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bho.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dpg.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oyz.ppjwa.cn

[N05] 最大公约数
来源：http://owt.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://yjm.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ebj.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yuy.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://heb.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bkz.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyy.daria6918.cn

Ruby: a.gcd(b)
来源：http://tre.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mqy.redwolf501.top

[N06] 判断回文字符串
来源：http://kux.havefunace.top

Py:   s == s[::-1]
来源：http://tqk.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://exn.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://sbc.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://ebh.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://els.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://lcq.epnwcf.com

Ruby: s == s.reverse
来源：http://ssy.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xzy.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://cui.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dpz.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xsy.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nxo.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://dzx.vqdsnc.cn

Java: // 手写 HashMap
来源：http://qrk.tian-w.cn

Go:   // 手写 map[int]int
来源：http://tfr.epnwcf.com

Ruby: // 手写 Hash
来源：http://jwu.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://xun.meibo888.top

[N08] 生成全排列
来源：http://kqp.tanke756.top

Py:   itertools.permutations(arr)
来源：http://orn.yongpay.top

PHP:  // 手写递归交换
来源：http://qoa.dashuyun.cn

JS:   // 手写回溯递归
来源：http://ynx.shzxlz.cn

TS:   // 手写回溯递归
来源：http://sfc.c1oappe.top

Java: // 手写回溯递归
来源：http://ask.sweek.top

Go:   // 手写回溯递归
来源：http://dio.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://yau.zdqjudy.top

C#:   // 手写回溯递归
来源：http://lgf.birdmap.top

[N09] 栈与队列
来源：http://jef.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://exd.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fjy.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rqj.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xkr.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aie.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kuc.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qdh.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kwq.iojbl.cn

[N10] 链表节点定义
来源：http://tof.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xfb.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://qqz.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tdq.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dts.birdmap.top

Java: class Node { int v; Node next; }
来源：http://vxl.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://zwd.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kgr.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://goc.wangdashe.top

[N11] 二叉树中序遍历
来源：http://lyj.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://agn.ehwqpu.com

PHP:  // 手写递归函数
来源：http://mxz.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://chw.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwp.zhaomingkeji.xyz

Java: // 手写递归
来源：http://bul.fengsongda.top

Go:   // 手写递归
来源：http://yxf.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://spb.sweek.top

C#:   // 手写递归
来源：http://unp.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzn.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aaa.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zgt.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iua.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fxj.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://izo.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sxl.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wrz.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xeu.chenjidiqi.icu

================================================================================
来源：http://lfk.yangfankeji.com

O. 并发与异步
来源：http://zbt.yj202588.top

================================================================================
来源：http://bee.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://gen.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ile.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zou.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://czp.fanxiaobao.xyz

TS:   // 同 JS
来源：http://vla.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://sqo.gaohongyu789.top

Go:   go f()
来源：http://syu.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://ugt.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://zri.bjfxy.top

[O02] 使用线程池
来源：http://hus.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kmx.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lnx.xylfe.cn

JS:   // worker_threads 线程池
来源：http://tgb.bbcook.cn

TS:   // worker_threads 线程池
来源：http://uef.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rrr.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kcg.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ikn.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://smg.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://ucx.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://cyc.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://cbx.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xzm.hysaishi.cn

TS:   // 同 JS
来源：http://rje.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://bic.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cea.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://don.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://izp.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://uht.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://rgs.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tsw.c1oappe.top

JS:   async function f() { await g(); }
来源：http://fxl.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://kiw.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yyh.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://non.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iwo.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://tiw.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://zta.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://upd.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zzm.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://qqs.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://dwi.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mgy.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rip.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://dlg.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://xsh.xinyue.icu

[O06] 使用进程池
来源：http://ltk.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mjj.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gjn.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://aop.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://lkn.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eqc.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://krz.0kj1m.cn

Ruby: // fork 块
来源：http://ztd.ydjk.org.cn

C#:   Parallel.For
来源：http://pcx.pycfn.com

================================================================================
来源：http://bbh.jqgfzy.top

P. 常用工具函数
来源：http://jha.9152youxi.cn

================================================================================
来源：http://agw.yfazqb.com

[P01] 生成 UUID
来源：http://hzf.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://qcm.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tfj.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://jll.yueranfly.top

TS:   crypto.randomUUID()
来源：http://ftf.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://lzp.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://ddu.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://ctc.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://rct.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://rur.andypj.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uzo.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eqy.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://odp.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://smr.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wcf.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tvz.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://quc.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nyi.nwbrower.top

[P03] 生成短随机字符串
来源：http://ciw.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://quj.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aru.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rfn.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://koq.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://alc.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sru.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lpk.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ztd.cqqwz.cn

[P04] 求长度
来源：http://jyb.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cug.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxk.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zwe.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jei.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://rgh.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://tgi.guowangkeji.top

Ruby: x.length;  x.size
来源：http://pdq.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pcz.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://jds.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mix.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wvo.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hvp.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ewg.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qcp.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tlh.mhx1999.top

Ruby: a == b
来源：http://yib.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ymh.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ray.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mfd.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://inm.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vbr.chenlongwang.top

TS:   if (x == null) {}
来源：http://tgp.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nrc.chenjidiqi.icu

Go:   if x == nil {}
来源：http://uhx.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uoc.hesvh.cn

C#:   if (x is null) {}
来源：http://ulq.xuanzx.com

[P07] 防抖与节流
来源：http://lzd.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vyz.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://cin.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nyp.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bho.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jgq.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://toa.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://iev.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://niw.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://bhz.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ksh.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jcm.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pfq.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ddy.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kxo.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sqy.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://paz.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zju.yj202588.top

================================================================================
来源：http://vho.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rsd.zycfv.cn

================================================================================
来源：http://auv.jinqigufen.top

[Q01] 创建表
来源：http://pzm.jlsjyb.cn

CREATE TABLE users (
来源：http://lpt.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nhc.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://hil.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://iyf.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tlb.mhx1999.top

);
来源：http://nzb.yj20258.top

[Q02] 创建带外键的表
来源：http://fmc.fengsongda.top

CREATE TABLE orders (
来源：http://vqn.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hxe.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://ivl.fengsongda.top

amount DECIMAL(10, 2),
来源：http://tjt.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vmu.yj202588.top

);
来源：http://soh.feifeiyinyue.top

[Q03] 增加列
来源：http://qmg.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://atn.yj20258888.top

[Q04] 修改列类型
来源：http://tsv.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://veh.shzxlz.cn

[Q05] 重命名列
来源：http://shy.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vfs.hesvh.cn

[Q06] 删除列
来源：http://ygb.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://izk.fktsv.cn

[Q07] 删除表
来源：http://tvt.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://ukm.zhoulong.xyz

[Q08] 创建普通索引
来源：http://huk.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jtl.sufxvd.cn

[Q09] 创建唯一索引
来源：http://ebq.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://izn.wangdashe.top

[Q10] 插入单行
来源：http://bbt.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ppb.hfpthk.cn

[Q11] 一次插入多行
来源：http://wkt.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zac.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://ilg.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://euw.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qjs.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://mxs.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oww.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://bkv.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ukd.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mtv.redwolf501.top

[Q15] 查询全部
来源：http://zpj.yongpay.top

SELECT * FROM users;
来源：http://uol.wangdashe.top

[Q16] 查询指定列
来源：http://ysb.nanxinkj.top

SELECT id, name FROM users;
来源：http://ouk.jianghu66.top

[Q17] 条件查询
来源：http://cvy.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://chx.yj202588.top

[Q18] 模糊匹配
来源：http://odk.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://abk.chenjidiqi.icu

[Q19] 范围查询
来源：http://wtu.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yae.hysaishi.cn

[Q20] IN 列表
来源：http://wdo.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zzd.vqdsnc.cn

[Q21] 空值判断
来源：http://gak.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://swr.snrcjt.cn

[Q22] 排序
来源：http://mmt.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bwb.svipenyu.cn

[Q23] 分页
来源：http://xwn.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kdv.vqdsnc.cn

[Q24] 去重
来源：http://cmk.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://qim.pycfn.com

[Q25] 只取前 N 条
来源：http://yxx.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yxa.hfpthk.cn

[Q26] 计数
来源：http://zaa.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://acs.fzhhl.top

[Q27] 条件计数
来源：http://lwi.xylfe.cn


<!-- 参考信息 -->