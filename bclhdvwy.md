代发 wailian999

[M08] 获取系统与运行时信息
来源：http://dqj.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://wzo.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://dqk.andypj.xyz

JS:   process.platform;  process.version
来源：http://sid.ctjpmb.com

TS:   process.platform;  process.version
来源：http://nvh.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kpq.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ash.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://djw.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://pue.uphjek.com

================================================================================
来源：http://syu.fktsv.cn

N. 数据结构与算法
来源：http://zut.redwolf501.top

================================================================================
来源：http://kkx.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://yna.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kal.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vyh.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipc.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vzo.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://xcl.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://ggm.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://bjg.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://enr.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://udy.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://wta.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mww.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://fyo.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lky.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://whp.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://qio.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://rmr.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ewo.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://qkl.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jdi.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://aae.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lcs.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ycw.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uwt.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rfj.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gne.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://fsp.gzhubu.top

[N04] 斐波那契数列
来源：http://vmj.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vwu.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wjh.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jds.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nuu.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xyy.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sva.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rea.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rhd.xuanzx.com

[N05] 最大公约数
来源：http://tuv.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://ynu.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lnw.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zhs.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://owl.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bpi.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ccz.sxryk.cn

Ruby: a.gcd(b)
来源：http://qxt.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dxh.guowangkeji.top

[N06] 判断回文字符串
来源：http://ipo.jiagoushi.top

Py:   s == s[::-1]
来源：http://lxd.fehbvm.com

PHP:  $s === strrev($s);
来源：http://vnu.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://wmr.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://pcc.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cof.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://usw.jlsjyb.cn

Ruby: s == s.reverse
来源：http://zqy.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lgt.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://tex.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://psn.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oyn.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://amn.sweek.top

TS:   // 手写 Map<string, number>
来源：http://hhm.daria6918.cn

Java: // 手写 HashMap
来源：http://zyr.wangdashe.top

Go:   // 手写 map[int]int
来源：http://kqi.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://rpd.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://npj.zhixingplan.top

[N08] 生成全排列
来源：http://qsp.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://koc.zhixingplan.top

PHP:  // 手写递归交换
来源：http://qlf.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://kyz.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://ctu.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://yqd.hywenlv.cn

Go:   // 手写回溯递归
来源：http://xhb.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://ezq.tian-w.cn

C#:   // 手写回溯递归
来源：http://dtm.svipenyu.cn

[N09] 栈与队列
来源：http://xel.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uiz.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eci.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://btb.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://krh.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xao.sxryk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oca.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://als.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lba.yj202588.top

[N10] 链表节点定义
来源：http://puo.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ykj.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://nsh.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://arq.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://plz.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://own.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://usj.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qdy.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ewz.yj20258.top

[N11] 二叉树中序遍历
来源：http://jxz.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ozk.52xcode.cn

PHP:  // 手写递归函数
来源：http://pme.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rjk.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sle.yangfankeji.com

Java: // 手写递归
来源：http://ocb.svipenyu.cn

Go:   // 手写递归
来源：http://hwd.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xiv.c1oappe.top

C#:   // 手写递归
来源：http://otm.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mmr.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jmo.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ulh.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpb.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kbs.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ekg.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ubz.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wip.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dco.aibaodan.cn

================================================================================
来源：http://kuo.zhaomingkeji.xyz

O. 并发与异步
来源：http://rme.andypj.xyz

================================================================================
来源：http://bkt.sufxvd.cn

[O01] 启动一个线程
来源：http://ziq.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hhc.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vvk.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dzf.snrcjt.cn

TS:   // 同 JS
来源：http://wvk.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://vja.uphjek.com

Go:   go f()
来源：http://gph.gzhubu.top

Ruby: Thread.new { f }
来源：http://gqc.vehdjk.com

C#:   Task.Run(() => F());
来源：http://jkr.chenzaomai.com

[O02] 使用线程池
来源：http://bot.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ryh.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ipv.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://yyt.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://cbk.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://bld.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ifn.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qlc.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ejm.zycfv.cn

[O03] 加锁保护共享数据
来源：http://qza.mhx1999.top

Py:   with lock: shared += 1
来源：http://pxj.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://man.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://upp.hesvh.cn

TS:   // 同 JS
来源：http://loz.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://gux.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mbk.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vcz.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://rvk.tian-w.cn

[O04] 定义异步函数并等待
来源：http://pzs.chenzaomai.com

Py:   async def f():⏎    await g()
来源：http://ezs.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://syo.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://qxl.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eym.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tht.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qiv.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://qyf.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://grg.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://gic.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://uhb.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vkl.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://ufj.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://knr.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mvh.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wvk.pycfn.com

Ruby: threads.map(&:join)
来源：http://rkb.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qqh.chenzaomai.com

[O06] 使用进程池
来源：http://fun.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rta.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://bho.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://uhq.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://hme.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mlo.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fqc.svipenyu.cn

Ruby: // fork 块
来源：http://mpc.zhengqikj.top

C#:   Parallel.For
来源：http://cbn.xziqi.cn

================================================================================
来源：http://hhc.fengsongda.top

P. 常用工具函数
来源：http://ebg.shanyushiyangkeji.top

================================================================================
来源：http://mwg.haohaochexian.top

[P01] 生成 UUID
来源：http://wzr.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://jhm.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nfo.wangdashe.top

JS:   crypto.randomUUID()
来源：http://pxe.hcnkem.com

TS:   crypto.randomUUID()
来源：http://eot.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://dlr.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://gjt.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://pxg.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://xky.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://xzr.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rpm.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xsf.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xoe.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://app.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xsf.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cfu.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mgc.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jne.yangfankeji.com

[P03] 生成短随机字符串
来源：http://nvv.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ohj.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ati.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wua.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jrz.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dnu.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yum.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lqy.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uij.zdbjq.cn

[P04] 求长度
来源：http://ocp.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jvk.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wye.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dkv.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qfb.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://wcs.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://oep.tianlin.xyz

Ruby: x.length;  x.size
来源：http://eyc.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dfs.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://glz.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sra.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rrm.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zus.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rur.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xzd.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://wta.uphjek.com

Ruby: a == b
来源：http://vcg.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eth.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dev.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ocy.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://ahj.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fww.shuidangran.top

TS:   if (x == null) {}
来源：http://ses.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ffr.chenjidiqi.icu

Go:   if x == nil {}
来源：http://ffm.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ebq.hammf.cn

C#:   if (x is null) {}
来源：http://gfb.uphjek.com

[P07] 防抖与节流
来源：http://idx.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qoa.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://tri.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://flg.chenjidiqi.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwi.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://smv.zhixingplan.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uff.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rij.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cvy.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://ddt.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ver.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ryk.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://joa.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lza.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qpy.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tgk.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mcc.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mmo.0kj1m.cn

================================================================================
来源：http://cdu.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://akj.gogol.net.cn

================================================================================
来源：http://que.ydjk.org.cn

[Q01] 创建表
来源：http://cka.gaohongyu789.top

CREATE TABLE users (
来源：http://nau.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://njj.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://psp.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://kas.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gxw.jinyuanbaomall.cn

);
来源：http://ydt.jyoumei.cn

[Q02] 创建带外键的表
来源：http://ccj.fktsv.cn

CREATE TABLE orders (
来源：http://vcd.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://met.xinyue.icu

user_id INT NOT NULL,
来源：http://vom.guannengcc.top

amount DECIMAL(10, 2),
来源：http://faa.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sot.zhijiandao.cn

);
来源：http://aoy.daxiang520.top

[Q03] 增加列
来源：http://xdk.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pqy.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://kpy.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ptc.mhx1999.top

[Q05] 重命名列
来源：http://ghf.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vhu.wangshuangyany.cn

[Q06] 删除列
来源：http://mkz.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://hza.zhoulong.xyz

[Q07] 删除表
来源：http://jak.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://dmu.yanxiufei.cn

[Q08] 创建普通索引
来源：http://lrp.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rku.nanxinkj.top

[Q09] 创建唯一索引
来源：http://tsd.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ghx.bjfxy.top

[Q10] 插入单行
来源：http://qiq.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nuv.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://vry.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ntp.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://icr.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://dmy.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cql.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://fxg.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://obu.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://odu.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aqj.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oaa.nanxinkj.top

[Q15] 查询全部
来源：http://wpi.ydzc1.top

SELECT * FROM users;
来源：http://bcs.chenjidiqi.icu

[Q16] 查询指定列
来源：http://mzy.zhixingplan.top

SELECT id, name FROM users;
来源：http://gvl.gotoacloud.top

[Q17] 条件查询
来源：http://pda.dianchejie.cn


<!-- 参考信息 -->