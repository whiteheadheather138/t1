代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://swg.tanke756.top

Ruby: warn "err"
来源：http://yhd.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://jic.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://lxa.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://gdr.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ipu.zdqjudy.top

JS:   require.main === module
来源：http://vev.guowangkeji.top

TS:   require.main === module
来源：http://sgt.nanxinkj.top

Java: public static void main(String[] args)
来源：http://thu.jyoumei.cn

Go:   func main()
来源：http://xcp.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jyv.fengsongda.top

C#:   static void Main(string[] args)
来源：http://fye.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://wiu.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://pga.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://kzh.zdqjudy.top

JS:   process.platform;  process.version
来源：http://khc.svipenyu.cn

TS:   process.platform;  process.version
来源：http://jhm.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vup.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ppl.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://spx.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://cth.9152youxi.cn

================================================================================
来源：http://chk.snrcjt.cn

N. 数据结构与算法
来源：http://tgv.tarul.cn

================================================================================
来源：http://osv.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://qlt.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://hnl.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://umr.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fev.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ahq.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hbp.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://whb.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yro.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kca.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://mbe.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://rtd.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vpp.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdn.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://btn.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://frn.havefunace.top

Go:   slices.Sort(arr)
来源：http://xlm.hywenlv.cn

Ruby: arr.sort
来源：http://rft.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://cvi.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://zyf.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wbp.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://rzi.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tim.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vci.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mhy.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://brx.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tsu.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ldi.hnqzz.top

[N04] 斐波那契数列
来源：http://zfy.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://scx.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ngc.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shp.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eiv.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tlk.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://erz.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bqk.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tnn.yj20258.top

[N05] 最大公约数
来源：http://cex.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://fwx.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eeu.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lwm.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sdf.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://njx.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sbj.tian-w.cn

Ruby: a.gcd(b)
来源：http://uww.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mov.zhoulong.xyz

[N06] 判断回文字符串
来源：http://rpp.tian-w.cn

Py:   s == s[::-1]
来源：http://fcc.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://qjs.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://zpf.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://kif.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ezq.havefunace.top

Go:   // 双指针从两端比较
来源：http://fdc.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://xmm.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zkw.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://ecl.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ttm.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lwp.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kfv.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://qop.andypj.xyz

Java: // 手写 HashMap
来源：http://mzi.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://duu.birdmap.top

Ruby: // 手写 Hash
来源：http://qep.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ghn.xylfe.cn

[N08] 生成全排列
来源：http://wpj.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://icj.chenzaomai.com

PHP:  // 手写递归交换
来源：http://iqo.guannengcc.top

JS:   // 手写回溯递归
来源：http://cmb.cdnleiting.top

TS:   // 手写回溯递归
来源：http://qoa.xuanzx.com

Java: // 手写回溯递归
来源：http://ses.sufxvd.cn

Go:   // 手写回溯递归
来源：http://xuh.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://jkt.jyoumei.cn

C#:   // 手写回溯递归
来源：http://ied.nanxinkj.top

[N09] 栈与队列
来源：http://lre.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hmv.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vwf.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ppl.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvg.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yhz.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cea.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fth.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hmk.daxiang520.top

[N10] 链表节点定义
来源：http://eye.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://idj.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cnw.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://djz.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqz.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://rhu.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://txt.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://kzz.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jfo.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://dhm.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tjh.jyoumei.cn

PHP:  // 手写递归函数
来源：http://www.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aky.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnl.zdqjudy.top

Java: // 手写递归
来源：http://tmd.cdnleiting.top

Go:   // 手写递归
来源：http://gor.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qlb.jqgufenzy.top

C#:   // 手写递归
来源：http://hyi.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cgm.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://odi.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gvu.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://brk.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tqs.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gyd.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qpm.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sav.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vxr.cucudq.cn

================================================================================
来源：http://ntw.kuanghao11.cn

O. 并发与异步
来源：http://atq.zhongyouzk.top

================================================================================
来源：http://mjr.hnqzz.top

[O01] 启动一个线程
来源：http://bjq.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://utg.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zmq.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://thr.uphjek.com

TS:   // 同 JS
来源：http://mtd.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://kvn.nwbrower.top

Go:   go f()
来源：http://wpt.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ygv.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://xmb.pengpengdd.cyou

[O02] 使用线程池
来源：http://ofc.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pmf.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ysu.52xcode.cn

JS:   // worker_threads 线程池
来源：http://fqx.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://wgz.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://ojh.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zaw.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ehx.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://guz.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://apf.svipenyu.cn

Py:   with lock: shared += 1
来源：http://ctf.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://zli.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdw.hnxiangtu.top

TS:   // 同 JS
来源：http://xpg.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://dtr.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hhy.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gfg.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://tgi.cheryme.top

[O04] 定义异步函数并等待
来源：http://bat.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://nuj.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://geq.havefunace.top

JS:   async function f() { await g(); }
来源：http://jzo.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ydi.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ier.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ysr.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ldo.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://ddk.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://kae.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://yxh.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://msb.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://amq.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://jip.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gru.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zll.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://jsy.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://tyz.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://afm.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ikj.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://auv.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://jqx.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://mpg.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cuj.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://skf.yueranfly.top

Ruby: // fork 块
来源：http://igc.hongshengwenyu.top

C#:   Parallel.For
来源：http://cze.cashguo.top

================================================================================
来源：http://zze.52xcode.cn

P. 常用工具函数
来源：http://ljm.nanxuanxn.top

================================================================================
来源：http://hkb.jianghu66.top

[P01] 生成 UUID
来源：http://dfv.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://sip.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xog.xinyue.icu

JS:   crypto.randomUUID()
来源：http://yer.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://khb.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://inx.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://awn.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://nnd.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://wop.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://kdd.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rtr.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://jim.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rgf.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wjt.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zyo.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jfy.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://znd.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tzx.sysykeji.top

[P03] 生成短随机字符串
来源：http://vwl.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lrn.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jtl.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mts.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uss.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iml.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lep.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://osq.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zst.meibo888.top

[P04] 求长度
来源：http://lfr.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rjo.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vti.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zvu.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kfc.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://vfi.vehdjk.com

Go:   len(arr);  len(m)
来源：http://wrw.wangdashe.top

Ruby: x.length;  x.size
来源：http://xog.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tgu.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://rrp.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vcc.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rgq.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://arb.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wqh.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xgy.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://awz.yongpay.top

Ruby: a == b
来源：http://bhu.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bkr.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://evz.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mbw.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://itk.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pvr.ybcxt.top

TS:   if (x == null) {}
来源：http://rss.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rvc.vehdjk.com

Go:   if x == nil {}
来源：http://myv.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zin.yuxming.cn

C#:   if (x is null) {}
来源：http://mvq.guowangkeji.top

[P07] 防抖与节流
来源：http://rpo.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xvj.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://hlf.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euu.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vod.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mlv.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kra.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://siu.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://acl.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://iie.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hsm.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gxc.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xqn.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wwz.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mxe.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pec.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ycw.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ylw.yuxming.cn

================================================================================
来源：http://xmd.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xbe.zhengqikj.top

================================================================================
来源：http://huc.hongshengwenyu.top

[Q01] 创建表
来源：http://kmh.fktsv.cn

CREATE TABLE users (
来源：http://tnu.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ooj.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://phx.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://rre.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pvt.smart0.xyz

);
来源：http://lnq.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://ssg.epnwcf.com

CREATE TABLE orders (
来源：http://lru.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hmd.chenlongwang.top

user_id INT NOT NULL,
来源：http://bsa.yvedp.cn

amount DECIMAL(10, 2),
来源：http://hwg.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hur.jinghuilouyu.cn

);
来源：http://kaq.nanxinkj.top

[Q03] 增加列
来源：http://tpv.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://avn.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://rxb.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ywi.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://han.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oib.hnqzz.top

[Q06] 删除列
来源：http://ork.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://vje.fktsv.cn

[Q07] 删除表
来源：http://dfu.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://tqy.hnqzz.top

[Q08] 创建普通索引
来源：http://hak.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://prh.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://lfq.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jyi.yongpay.top

[Q10] 插入单行
来源：http://ekt.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://msa.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://fpm.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://keo.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://yfi.shuidangran.top


<!-- 参考信息 -->