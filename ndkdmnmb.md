代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://sfn.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://nlx.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mpx.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://zaj.hnqzz.top

Ruby: arr.sort
来源：http://lni.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pgj.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://xbz.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kkh.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://exn.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jyb.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sed.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gct.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bbt.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nhb.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://awj.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://ymi.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jgk.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sbk.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obs.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tcs.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqo.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qzp.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pyg.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://usq.fanxiaobao.xyz

[N05] 最大公约数
来源：http://aya.c1oappe.top

Py:   math.gcd(a, b)
来源：http://kfn.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://urd.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wdd.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tnn.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://myu.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dvo.hnqzz.top

Ruby: a.gcd(b)
来源：http://gxv.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cgz.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://mri.guannengcc.top

Py:   s == s[::-1]
来源：http://wwr.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://rwf.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://tmi.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://ntl.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qun.hcnkem.com

Go:   // 双指针从两端比较
来源：http://umj.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://gbk.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vfu.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://ffe.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bbr.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://swl.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sqi.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://dwi.shzxlz.cn

Java: // 手写 HashMap
来源：http://mog.cucudq.cn

Go:   // 手写 map[int]int
来源：http://bci.jyoumei.cn

Ruby: // 手写 Hash
来源：http://yvx.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://iso.fengsongda.top

[N08] 生成全排列
来源：http://oqg.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://xxr.zdbjq.cn

PHP:  // 手写递归交换
来源：http://esm.316326.xyz

JS:   // 手写回溯递归
来源：http://dbt.yfazqb.com

TS:   // 手写回溯递归
来源：http://vxs.havefunace.top

Java: // 手写回溯递归
来源：http://wus.meibo888.top

Go:   // 手写回溯递归
来源：http://uvd.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://iyr.dashuyun.cn

C#:   // 手写回溯递归
来源：http://ktp.zhongyouzk.top

[N09] 栈与队列
来源：http://ktk.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yta.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gfw.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qxy.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://end.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mri.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://phw.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://owx.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xoi.andypj.xyz

[N10] 链表节点定义
来源：http://hst.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tjx.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ckr.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ydv.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bsz.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://ghr.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vye.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://koc.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uum.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://pfc.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gte.dashuyun.cn

PHP:  // 手写递归函数
来源：http://kpw.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tvg.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://deb.snrcjt.cn

Java: // 手写递归
来源：http://rtq.tianlin.xyz

Go:   // 手写递归
来源：http://kwm.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://avx.yanxiufei.cn

C#:   // 手写递归
来源：http://ioi.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fmb.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugn.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ksc.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfd.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovg.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ovz.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dvd.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://exl.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rbh.ydjk.org.cn

================================================================================
来源：http://mnu.zhongyouzk.top

O. 并发与异步
来源：http://udp.fktsv.cn

================================================================================
来源：http://zmi.yj20258888.top

[O01] 启动一个线程
来源：http://apy.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://soj.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jua.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qld.shanyushiyangtech.top

TS:   // 同 JS
来源：http://ajn.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://jce.c1oappe.top

Go:   go f()
来源：http://flc.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://vsv.yj20258888.top

C#:   Task.Run(() => F());
来源：http://fam.sufxvd.cn

[O02] 使用线程池
来源：http://bsf.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://esp.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sfm.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://ekm.xuanzx.com

TS:   // worker_threads 线程池
来源：http://cdu.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://god.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gbw.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ekd.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hst.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://aqk.aizwys.cn

Py:   with lock: shared += 1
来源：http://nnh.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://nnu.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qbw.tian-w.cn

TS:   // 同 JS
来源：http://cfx.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://uyy.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yon.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://egz.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://iat.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://tcu.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://fkb.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ugf.c1oappe.top

JS:   async function f() { await g(); }
来源：http://ema.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://bdb.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nmj.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wxj.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://fnw.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://njf.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://rkl.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://lrx.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kii.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://bgu.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://uth.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://trw.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lad.aizwys.cn

Ruby: threads.map(&:join)
来源：http://itw.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://crb.shangyingyoupin.top

[O06] 使用进程池
来源：http://ncw.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sbr.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ioq.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://pym.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://rdb.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bvu.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xkg.guowangkeji.top

Ruby: // fork 块
来源：http://plu.cqqwz.cn

C#:   Parallel.For
来源：http://hfn.hnxiangtu.top

================================================================================
来源：http://iue.jqgfzy.top

P. 常用工具函数
来源：http://hrt.zdbjq.cn

================================================================================
来源：http://qxd.yj202588.top

[P01] 生成 UUID
来源：http://tjo.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://olz.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qko.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://ope.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://jkj.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://rwf.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://jfn.cheryme.top

Ruby: SecureRandom.uuid
来源：http://onr.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://nqw.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://wfv.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://geb.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xhm.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gdz.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://usg.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rfe.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nrs.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ptv.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dww.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://uru.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hlr.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uii.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kth.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pwd.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aey.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eqi.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mgn.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nru.jyoumei.cn

[P04] 求长度
来源：http://mlh.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fue.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://krq.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jeu.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yot.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://omi.c1oappe.top

Go:   len(arr);  len(m)
来源：http://rbs.haohaochexian.top

Ruby: x.length;  x.size
来源：http://tyt.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xqg.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://tpu.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zoq.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mfp.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mic.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gnc.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xfl.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://aew.kuanghao11.cn

Ruby: a == b
来源：http://ubi.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ysj.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bmc.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cll.yj202588.top

PHP:  if (empty($x)) {}
来源：http://gnj.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qnr.xziqi.cn

TS:   if (x == null) {}
来源：http://zdf.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sdk.yuxming.cn

Go:   if x == nil {}
来源：http://hve.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://knh.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://ggx.hywenlv.cn

[P07] 防抖与节流
来源：http://rqt.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bdb.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://nhh.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fuz.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://myu.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kpi.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xno.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mjp.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xgq.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://rsb.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xtx.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hjb.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ops.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bah.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://odj.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ibs.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jkr.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uog.aizwys.cn

================================================================================
来源：http://zfq.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rdq.fehbvm.com

================================================================================
来源：http://qqi.sysykeji.top

[Q01] 创建表
来源：http://vps.yuxming.cn

CREATE TABLE users (
来源：http://xot.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://otu.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://cdt.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://cpx.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rxh.sjlbkw.cn

);
来源：http://grc.jyoumei.cn

[Q02] 创建带外键的表
来源：http://gkw.sysykeji.top

CREATE TABLE orders (
来源：http://tgu.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ppi.hcnkem.com

user_id INT NOT NULL,
来源：http://ztk.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://zbs.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jxa.dianchejie.cn

);
来源：http://kgk.birdmap.top

[Q03] 增加列
来源：http://uzr.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qtx.xinyue.icu

[Q04] 修改列类型
来源：http://sia.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gry.hcnkem.com

[Q05] 重命名列
来源：http://xyd.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://osd.nwbrower.top

[Q06] 删除列
来源：http://sjg.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fqf.redwolf501.top

[Q07] 删除表
来源：http://cpi.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://iqh.zhixingplan.top

[Q08] 创建普通索引
来源：http://elv.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://pwy.andypj.xyz

[Q09] 创建唯一索引
来源：http://eot.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ier.jlsjyb.cn

[Q10] 插入单行
来源：http://fbz.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zql.zhoulong.xyz

[Q11] 一次插入多行
来源：http://lhc.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ini.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://vdz.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ren.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gnn.jiagoushi.top

[Q13] 忽略重复插入
来源：http://huy.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jbu.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://ect.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dbi.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://evg.guannengcc.top

[Q15] 查询全部
来源：http://vwe.nanxinkj.top

SELECT * FROM users;
来源：http://yir.shangyingyoupin.top

[Q16] 查询指定列
来源：http://gah.vehdjk.com

SELECT id, name FROM users;
来源：http://oys.zdqjudy.top

[Q17] 条件查询
来源：http://blf.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dyc.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://dut.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vab.nwbrower.top

[Q19] 范围查询
来源：http://glu.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jnb.vehdjk.com

[Q20] IN 列表
来源：http://kdp.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cvw.feifeiyinyue.top

[Q21] 空值判断
来源：http://loj.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://emd.jinqigufen.top

[Q22] 排序
来源：http://udg.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://anb.hnqzz.top

[Q23] 分页
来源：http://rkt.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mud.zhongyouzk.top

[Q24] 去重
来源：http://try.sweek.top

SELECT DISTINCT city FROM users;
来源：http://ftv.xylfe.cn

[Q25] 只取前 N 条
来源：http://ygq.hongshengwenyu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tib.iojbl.cn

[Q26] 计数
来源：http://uul.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://ygw.zdbjq.cn

[Q27] 条件计数
来源：http://psl.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hua.fehbvm.com

[Q28] 求和与平均
来源：http://jbn.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tij.ppjwa.cn

[Q29] 最大最小值
来源：http://zbn.jiagoushi.top


<!-- 参考信息 -->