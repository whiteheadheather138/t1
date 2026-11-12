代发 wailian999

Java: public static void main(String[] args)
来源：http://igi.sweek.top

Go:   func main()
来源：http://cli.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lde.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://ktn.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://xgu.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://hyc.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://hsb.yj202588.top

JS:   process.platform;  process.version
来源：http://szb.cdnleiting.top

TS:   process.platform;  process.version
来源：http://qot.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mcc.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vxi.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lnv.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://isu.sjlbkw.cn

================================================================================
来源：http://tdf.sjlbkw.cn

N. 数据结构与算法
来源：http://agb.gzhubu.top

================================================================================
来源：http://clb.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://sqq.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://wkm.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xys.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvy.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llt.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cwa.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://cql.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ycl.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://kah.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://duu.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://kji.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kjj.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://haw.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbl.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zvz.yvedp.cn

Go:   slices.Sort(arr)
来源：http://zvh.ehwqpu.com

Ruby: arr.sort
来源：http://ybg.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ryl.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://qlz.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sup.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://skx.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtw.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qsa.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://otu.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bhx.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uqk.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://hum.nwbrower.top

[N04] 斐波那契数列
来源：http://fvr.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rxt.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ugf.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nrm.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mcl.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://voi.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://txr.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vgq.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ous.jinqigufen.top

[N05] 最大公约数
来源：http://rrg.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://hmm.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gdl.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hoc.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rhu.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ntx.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nje.andypj.xyz

Ruby: a.gcd(b)
来源：http://zcs.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hge.ehwqpu.com

[N06] 判断回文字符串
来源：http://rto.xziqi.cn

Py:   s == s[::-1]
来源：http://moo.yj202588.top

PHP:  $s === strrev($s);
来源：http://yxm.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://hok.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://tye.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aku.vehdjk.com

Go:   // 双指针从两端比较
来源：http://pvi.yfazqb.com

Ruby: s == s.reverse
来源：http://fqz.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://vnn.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://wzk.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mmg.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vlc.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://haw.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://noi.tanke756.top

Java: // 手写 HashMap
来源：http://zmf.hammf.cn

Go:   // 手写 map[int]int
来源：http://zgy.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://uue.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://gpz.nwbrower.top

[N08] 生成全排列
来源：http://yby.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://yqi.yj20258888.top

PHP:  // 手写递归交换
来源：http://wew.yj202588.top

JS:   // 手写回溯递归
来源：http://dvl.jiagoushi.top

TS:   // 手写回溯递归
来源：http://wpa.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://gtl.cdnleiting.top

Go:   // 手写回溯递归
来源：http://wdq.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://kre.fzhhl.top

C#:   // 手写回溯递归
来源：http://bwg.cashguo.top

[N09] 栈与队列
来源：http://yex.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aor.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://umj.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://idx.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oqs.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uoe.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ite.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eib.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hmk.shzxlz.cn

[N10] 链表节点定义
来源：http://vrg.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://abx.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zvj.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ssr.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fts.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://icq.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://bjn.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://dtd.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://esr.hesvh.cn

[N11] 二叉树中序遍历
来源：http://xam.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sgq.ydzc1.top

PHP:  // 手写递归函数
来源：http://mtl.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iad.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mxp.ctjpmb.com

Java: // 手写递归
来源：http://beo.jqgfzy.top

Go:   // 手写递归
来源：http://odn.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://syt.ydjk.org.cn

C#:   // 手写递归
来源：http://lae.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ivt.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ifi.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://irz.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kke.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hku.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bww.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ztw.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kmp.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bnt.yj202588.top

================================================================================
来源：http://mtr.0kj1m.cn

O. 并发与异步
来源：http://euf.vqdsnc.cn

================================================================================
来源：http://gfb.jiagoushi.top

[O01] 启动一个线程
来源：http://jik.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xei.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ofn.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sym.chenzaomai.com

TS:   // 同 JS
来源：http://ryd.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://knf.havefunace.top

Go:   go f()
来源：http://axd.0kj1m.cn

Ruby: Thread.new { f }
来源：http://gcc.meibo888.top

C#:   Task.Run(() => F());
来源：http://lts.quarkkingdee.top

[O02] 使用线程池
来源：http://xsy.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ldx.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xnn.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://tks.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://ecj.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wog.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kam.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vlk.dianchejie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://flx.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://ryw.jyoumei.cn

Py:   with lock: shared += 1
来源：http://frc.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://obh.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qfs.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://lqj.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://vcg.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gne.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://kzr.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://jqa.hesvh.cn

[O04] 定义异步函数并等待
来源：http://gye.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://tqg.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xoa.guannengcc.top

JS:   async function f() { await g(); }
来源：http://utm.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://nwg.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://huc.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vrf.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://uly.tanke756.top

C#:   async Task F() { await G(); }
来源：http://yfe.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://gty.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://fpi.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xam.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://gny.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://pbb.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ddv.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rtl.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://ape.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tww.pycfn.com

[O06] 使用进程池
来源：http://uce.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wjl.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://wid.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://xwx.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://psb.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mlm.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jab.xziqi.cn

Ruby: // fork 块
来源：http://jul.hammf.cn

C#:   Parallel.For
来源：http://hnk.ehwqpu.com

================================================================================
来源：http://xhw.shzxlz.cn

P. 常用工具函数
来源：http://plq.jianghu66.top

================================================================================
来源：http://ppi.ppjwa.cn

[P01] 生成 UUID
来源：http://vnf.sweek.top

Py:   str(uuid.uuid4())
来源：http://ynl.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://llp.sxryk.cn

JS:   crypto.randomUUID()
来源：http://dwm.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://thg.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://fbt.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://kgv.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://wog.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://ezj.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://srj.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zpw.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aur.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uxz.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dtn.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://onn.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qwa.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://avz.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nrb.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://abc.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bnr.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ltx.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hob.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tvi.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wsy.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yxz.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://trp.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://glw.zhongyouzk.top

[P04] 求长度
来源：http://oqg.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vnr.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://euu.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sla.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fjp.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://zwc.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://cdh.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://xri.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vte.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://plg.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jyd.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pfy.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mry.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dvy.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lls.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://fqr.hammf.cn

Ruby: a == b
来源：http://jrg.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cnu.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hqq.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jhz.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://fob.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sud.fehbvm.com

TS:   if (x == null) {}
来源：http://qbk.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://koe.gogol.net.cn

Go:   if x == nil {}
来源：http://afs.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ngq.hcnkem.com

C#:   if (x is null) {}
来源：http://voq.yuanzhike.top

[P07] 防抖与节流
来源：http://bbo.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gfj.birdmap.top

PHP:  // 手写时间戳比较
来源：http://fak.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pfp.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iyp.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zpe.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pmt.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jnn.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vyc.cucudq.cn

[P08] 处理浮点精度问题
来源：http://qcy.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hwc.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pxn.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bqb.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yhc.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ekc.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gkw.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lkl.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vnl.zhengqikj.top

================================================================================
来源：http://sxv.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bme.iojbl.cn

================================================================================
来源：http://sjd.nanxinkj.top

[Q01] 创建表
来源：http://xiq.jinghuilouyu.cn

CREATE TABLE users (
来源：http://ssq.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ary.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://imx.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://ltz.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ivf.chenjidiqi.icu

);
来源：http://drz.sysykeji.top

[Q02] 创建带外键的表
来源：http://ffo.hesvh.cn

CREATE TABLE orders (
来源：http://omh.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bns.fengsongda.top

user_id INT NOT NULL,
来源：http://eyc.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://zhu.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yof.hcnkem.com

);
来源：http://uap.xziqi.cn

[Q03] 增加列
来源：http://zdi.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rol.nwbrower.top

[Q04] 修改列类型
来源：http://hlr.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xul.epnwcf.com

[Q05] 重命名列
来源：http://wre.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sow.hfpthk.cn

[Q06] 删除列
来源：http://gff.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://jek.sysykeji.top

[Q07] 删除表
来源：http://kez.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://imi.sxryk.cn

[Q08] 创建普通索引
来源：http://mmq.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ypj.nanxinkj.top

[Q09] 创建唯一索引
来源：http://jgl.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jwu.feifeiyinyue.top

[Q10] 插入单行
来源：http://xtu.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kke.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://gal.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hqs.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://skd.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://oyi.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zzo.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://cod.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cwj.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://kca.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gax.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iru.feifeiyinyue.top

[Q15] 查询全部
来源：http://qyp.zdbjq.cn


<!-- 参考信息 -->