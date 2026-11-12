代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ebj.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://dcy.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://nfl.hcnkem.com

JS:   process.platform;  process.version
来源：http://xam.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://skc.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lpu.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nib.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sqv.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vxx.xuanzx.com

================================================================================
来源：http://thh.gaohongyu789.top

N. 数据结构与算法
来源：http://niu.andypj.xyz

================================================================================
来源：http://aqo.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://nkb.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://pgu.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jbt.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywy.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpb.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mrc.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://tub.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fls.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://cpu.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://fqf.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://jsu.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dpd.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvs.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kjl.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://guj.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://fet.chenzaomai.com

Ruby: arr.sort
来源：http://xcm.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jnb.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://zmx.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dks.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://rir.gzhubu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pdz.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gpj.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vku.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwa.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xzi.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://xft.cdnleiting.top

[N04] 斐波那契数列
来源：http://yie.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bha.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nxc.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qxq.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyn.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ljr.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vba.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://npq.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zlj.chenzaomai.com

[N05] 最大公约数
来源：http://shi.wangdashe.top

Py:   math.gcd(a, b)
来源：http://cyj.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nvb.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://and.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcb.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cci.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eep.cucudq.cn

Ruby: a.gcd(b)
来源：http://daq.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://syt.vehdjk.com

[N06] 判断回文字符串
来源：http://xir.cdnleiting.top

Py:   s == s[::-1]
来源：http://tyt.daxiang520.top

PHP:  $s === strrev($s);
来源：http://suu.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://psj.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://poc.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kkl.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://ypk.aibaodan.cn

Ruby: s == s.reverse
来源：http://luv.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uaj.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://gup.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vmo.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://glp.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://wvy.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://kdf.guannengcc.top

Java: // 手写 HashMap
来源：http://pku.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://hgh.gotoacloud.top

Ruby: // 手写 Hash
来源：http://mcs.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fjk.fanxiaobao.xyz

[N08] 生成全排列
来源：http://zzi.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://mhe.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://iym.ppjwa.cn

JS:   // 手写回溯递归
来源：http://lal.yangfankeji.com

TS:   // 手写回溯递归
来源：http://grh.wangdashe.top

Java: // 手写回溯递归
来源：http://inc.redwolf501.top

Go:   // 手写回溯递归
来源：http://dty.gotoacloud.top

Ruby: arr.permutation.to_a
来源：http://met.aibaodan.cn

C#:   // 手写回溯递归
来源：http://rtb.pengpengdd.cyou

[N09] 栈与队列
来源：http://oxm.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blm.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qkd.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gdw.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eoz.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://msq.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nqg.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zxm.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dah.yfazqb.com

[N10] 链表节点定义
来源：http://ifp.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vbc.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://psf.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rzq.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rit.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://kpe.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://adk.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ldn.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wxk.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://ikd.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ddc.hesvh.cn

PHP:  // 手写递归函数
来源：http://iby.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfw.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spl.yuanzhike.top

Java: // 手写递归
来源：http://cfy.smart0.xyz

Go:   // 手写递归
来源：http://fst.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wug.sjlbkw.cn

C#:   // 手写递归
来源：http://nvz.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jzv.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://plp.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vvu.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eqe.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tne.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fli.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ocl.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pbp.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uyo.uphjek.com

================================================================================
来源：http://bwz.dashuyun.cn

O. 并发与异步
来源：http://aay.wangdashe.top

================================================================================
来源：http://fmi.hongshengwenyu.top

[O01] 启动一个线程
来源：http://lyh.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tzs.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ypd.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ccz.jianghu66.top

TS:   // 同 JS
来源：http://uni.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://awx.nanxinkj.top

Go:   go f()
来源：http://cwp.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://dug.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://nkb.snrcjt.cn

[O02] 使用线程池
来源：http://fbo.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lhq.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fmt.wangdashe.top

JS:   // worker_threads 线程池
来源：http://svw.316326.xyz

TS:   // worker_threads 线程池
来源：http://vnq.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://ezv.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tek.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqm.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mkk.andypj.xyz

[O03] 加锁保护共享数据
来源：http://fai.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://nke.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://vcn.dianchejie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://osb.shuidangran.top

TS:   // 同 JS
来源：http://hzf.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://gpd.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://myu.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kmi.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://qha.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://tlh.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://swe.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://run.xuanzx.com

JS:   async function f() { await g(); }
来源：http://bkc.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://qul.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://psj.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zkz.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://jxv.cashguo.top

C#:   async Task F() { await G(); }
来源：http://qxj.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://idd.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://nsu.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://shl.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://kqu.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://sak.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nec.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://egx.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://bkr.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yda.shzxlz.cn

[O06] 使用进程池
来源：http://mcx.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jru.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://plr.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://rzl.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://qbc.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ico.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xvn.sweek.top

Ruby: // fork 块
来源：http://ekj.xuanzx.com

C#:   Parallel.For
来源：http://qhl.52xcode.cn

================================================================================
来源：http://rgm.fengsongda.top

P. 常用工具函数
来源：http://duw.shangyingyoupin.top

================================================================================
来源：http://dmg.jianghu66.top

[P01] 生成 UUID
来源：http://xdc.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://fcy.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ltq.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://vqo.sweek.top

TS:   crypto.randomUUID()
来源：http://uxi.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://phx.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://giq.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://nel.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ohj.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://jwo.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://svx.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fpc.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nqe.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kkm.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tir.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zrs.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rbz.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rfj.fktsv.cn

[P03] 生成短随机字符串
来源：http://mnu.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ujc.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mwt.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rda.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aly.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lml.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://agg.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://txz.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qjr.xylfe.cn

[P04] 求长度
来源：http://umx.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://chd.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ews.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojs.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfd.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://jnj.sysykeji.top

Go:   len(arr);  len(m)
来源：http://wps.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://phd.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxw.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://qsz.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://msp.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fli.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zww.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ltn.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sij.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://gby.9152youxi.cn

Ruby: a == b
来源：http://phq.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rbx.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jeu.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cxb.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://kms.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kkv.ehwqpu.com

TS:   if (x == null) {}
来源：http://vok.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wjf.quarkkingdee.top

Go:   if x == nil {}
来源：http://ywe.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mvh.jianghu66.top

C#:   if (x is null) {}
来源：http://ydh.sysykeji.top

[P07] 防抖与节流
来源：http://oki.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lyg.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://hvj.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqw.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlt.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vkl.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tgx.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://brh.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mje.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://cbm.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://toq.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://war.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dwn.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jmh.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uhg.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zte.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://guk.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xnx.shanyushiyangtech.top

================================================================================
来源：http://uhw.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lsq.cqqwz.cn

================================================================================
来源：http://kww.zhixingplan.top

[Q01] 创建表
来源：http://scr.vehdjk.com

CREATE TABLE users (
来源：http://pog.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyq.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://fnk.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://yhr.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://inv.aizwys.cn

);
来源：http://pxu.jiagoushi.top

[Q02] 创建带外键的表
来源：http://wgp.fzhhl.top

CREATE TABLE orders (
来源：http://sja.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wlm.jinqigufen.top

user_id INT NOT NULL,
来源：http://tbv.xuanzx.com

amount DECIMAL(10, 2),
来源：http://syi.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lfb.chenjidiqi.icu

);
来源：http://vxq.haohaochexian.top

[Q03] 增加列
来源：http://zkq.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lvx.chenlongwang.top

[Q04] 修改列类型
来源：http://why.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gfq.zhengqikj.top

[Q05] 重命名列
来源：http://vkm.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://itz.jiagoushi.top

[Q06] 删除列
来源：http://gtt.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://llh.zycfv.cn

[Q07] 删除表
来源：http://gou.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://ecb.quarkkingdee.top

[Q08] 创建普通索引
来源：http://sge.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zia.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://ism.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wio.havefunace.top

[Q10] 插入单行
来源：http://xud.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ihm.hammf.cn

[Q11] 一次插入多行
来源：http://ljs.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ypb.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://yzq.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://yer.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qnt.guannengcc.top

[Q13] 忽略重复插入
来源：http://xna.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hbl.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://vjw.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vml.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ypd.mhx1999.top

[Q15] 查询全部
来源：http://nxb.wangshuangyany.cn

SELECT * FROM users;
来源：http://dkp.guowangkeji.top

[Q16] 查询指定列
来源：http://stk.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://fee.redwolf501.top

[Q17] 条件查询
来源：http://gss.sysykeji.top


<!-- 参考信息 -->