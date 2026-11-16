代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://cop.ydjk.org.cn

[M05] 设置退出码
来源：http://qpi.gotoacloud.top

Py:   sys.exit(1)
来源：http://ljk.52xcode.cn

PHP:  exit(1);
来源：http://etb.yj20258.top

JS:   process.exit(1)
来源：http://cii.jqgfzy.top

TS:   process.exit(1)
来源：http://ail.gogol.net.cn

Java: System.exit(1)
来源：http://zsk.svipenyu.cn

Go:   os.Exit(1)
来源：http://zqm.gotoacloud.top

Ruby: exit 1
来源：http://eps.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://thq.shuidangran.top

[M06] 向标准错误输出
来源：http://lff.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://zwq.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qnj.gogol.net.cn

JS:   console.error("err")
来源：http://guh.zhiwuduotai.top

TS:   console.error("err")
来源：http://lyv.xuanzx.com

Java: System.err.println("err")
来源：http://cwu.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mme.bjfxy.top

Ruby: warn "err"
来源：http://jxh.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://vsu.gotoacloud.top

[M07] 判断是否为主入口
来源：http://zzh.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://raw.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fod.havefunace.top

JS:   require.main === module
来源：http://ogo.sjlbkw.cn

TS:   require.main === module
来源：http://ady.cdnleiting.top

Java: public static void main(String[] args)
来源：http://ddj.fktsv.cn

Go:   func main()
来源：http://hjm.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mnd.shuidangran.top

C#:   static void Main(string[] args)
来源：http://ztq.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://vda.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://cks.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://glc.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://adi.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://brr.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rzx.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mjc.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://taf.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://run.ctjpmb.com

================================================================================
来源：http://swy.cqqwz.cn

N. 数据结构与算法
来源：http://iys.dashuyun.cn

================================================================================
来源：http://edn.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://vrp.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://wei.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dam.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bio.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nao.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://wxf.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://hom.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lvv.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://edp.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://nfe.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://rrq.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bik.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vvn.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://irw.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://omb.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://bzc.gotoacloud.top

Ruby: arr.sort
来源：http://osx.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://hgd.316326.xyz

[N03] 快速排序（分治示例）
来源：http://bbf.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rqj.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://zke.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eyj.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blk.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pxp.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nti.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zef.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://bef.tarul.cn

[N04] 斐波那契数列
来源：http://car.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nfb.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utx.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://krc.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://byb.cashguo.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://btw.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jbg.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ntl.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vbj.redwolf501.top

[N05] 最大公约数
来源：http://yjc.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://pke.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qxq.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dtc.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mmn.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rty.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://llf.dianchejie.cn

Ruby: a.gcd(b)
来源：http://mtq.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oxr.jiagoushi.top

[N06] 判断回文字符串
来源：http://okv.bjfxy.top

Py:   s == s[::-1]
来源：http://tuq.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://grz.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://snk.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://jjm.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jsj.aizwys.cn

Go:   // 双指针从两端比较
来源：http://lhu.mhx1999.top

Ruby: s == s.reverse
来源：http://hxf.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ylv.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://rcy.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tuk.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fiq.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lfa.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://pnh.sjlbkw.cn

Java: // 手写 HashMap
来源：http://qcd.zycfv.cn

Go:   // 手写 map[int]int
来源：http://dgu.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://sje.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://rpp.hnxiangtu.top

[N08] 生成全排列
来源：http://kvi.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://dfz.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://edn.haohaochexian.top

JS:   // 手写回溯递归
来源：http://xij.cdnleiting.top

TS:   // 手写回溯递归
来源：http://ydh.ctjpmb.com

Java: // 手写回溯递归
来源：http://bsw.shzxlz.cn

Go:   // 手写回溯递归
来源：http://lnd.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://fsb.hysaishi.cn

C#:   // 手写回溯递归
来源：http://kqa.tarul.cn

[N09] 栈与队列
来源：http://ouk.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uof.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mqk.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sbi.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tdx.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zmy.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iqw.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jyk.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pcv.ybcxt.top

[N10] 链表节点定义
来源：http://ign.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kyf.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nec.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xlt.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rme.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://wme.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://uih.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dnz.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bbx.ybcxt.top

[N11] 二叉树中序遍历
来源：http://hcl.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lza.hfpthk.cn

PHP:  // 手写递归函数
来源：http://ccl.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgz.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ttz.fktsv.cn

Java: // 手写递归
来源：http://ynp.yj20258.top

Go:   // 手写递归
来源：http://hof.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zkk.guannengcc.top

C#:   // 手写递归
来源：http://rqr.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xvb.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ovy.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dxb.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zaq.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aef.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mfq.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jau.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tsz.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aca.yuxming.cn

================================================================================
来源：http://lvr.xziqi.cn

O. 并发与异步
来源：http://kir.cucudq.cn

================================================================================
来源：http://aye.wangshuangyany.cn

[O01] 启动一个线程
来源：http://daq.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kij.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nnr.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aso.bjfxy.top

TS:   // 同 JS
来源：http://vsc.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://xsx.fktsv.cn

Go:   go f()
来源：http://kyt.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://xhg.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://fyx.sufxvd.cn

[O02] 使用线程池
来源：http://fki.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kfe.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yfk.havefunace.top

JS:   // worker_threads 线程池
来源：http://agx.316326.xyz

TS:   // worker_threads 线程池
来源：http://ixc.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://hjr.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://quk.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://psv.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kgo.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://nyc.jianghu66.top

Py:   with lock: shared += 1
来源：http://xya.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://ezj.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vfo.meibo888.top

TS:   // 同 JS
来源：http://kii.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://srd.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jke.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://krj.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://yaq.hammf.cn

[O04] 定义异步函数并等待
来源：http://tkh.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://uky.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mfc.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://eji.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uvy.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uda.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yck.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mjw.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://uqj.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://ils.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://gmc.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qgm.yj202588.top

JS:   await Promise.all(tasks)
来源：http://axi.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://cmx.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ynp.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bse.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://qfy.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://voj.c1oappe.top

[O06] 使用进程池
来源：http://vhg.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://osy.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vmp.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://gkm.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://utj.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tos.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sas.epnwcf.com

Ruby: // fork 块
来源：http://uqt.fanxiaobao.xyz

C#:   Parallel.For
来源：http://pss.hcnkem.com

================================================================================
来源：http://och.zhengqikj.top

P. 常用工具函数
来源：http://rma.sjlbkw.cn

================================================================================
来源：http://teq.xinyue.icu

[P01] 生成 UUID
来源：http://qxt.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://uep.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oqf.tanke756.top

JS:   crypto.randomUUID()
来源：http://big.yuxming.cn

TS:   crypto.randomUUID()
来源：http://llb.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://jyh.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://dbk.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://exv.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://lno.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://mxr.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://txv.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ljx.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bva.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yqq.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://abm.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jwz.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xhd.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dfs.haohaochexian.top

[P03] 生成短随机字符串
来源：http://mru.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aww.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lse.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oky.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xoe.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pud.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qmg.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://prc.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hdb.fehbvm.com

[P04] 求长度
来源：http://fai.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yzk.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mpl.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vub.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kpl.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://vcr.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://fvw.andypj.xyz

Ruby: x.length;  x.size
来源：http://gfz.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://unv.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://qki.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zmv.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bkw.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jti.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mgv.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://njr.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rcx.shanyushiyangtech.top

Ruby: a == b
来源：http://igo.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://myr.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ugl.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bit.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://hyn.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bmz.bjfxy.top

TS:   if (x == null) {}
来源：http://gpw.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://paf.hnqzz.top

Go:   if x == nil {}
来源：http://wzo.daxiang520.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ehb.haohaochexian.top

C#:   if (x is null) {}
来源：http://syc.gzhubu.top

[P07] 防抖与节流
来源：http://jtk.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jka.cheryme.top

PHP:  // 手写时间戳比较
来源：http://azh.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjz.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fqc.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ibk.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mal.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ahe.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://doy.pycfn.com

[P08] 处理浮点精度问题
来源：http://rox.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cee.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nlh.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xht.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://evs.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hed.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://luk.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xaw.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://imx.sweek.top

================================================================================
来源：http://wzp.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jpp.gotoacloud.top

================================================================================
来源：http://vwd.jianghu66.top

[Q01] 创建表
来源：http://wru.cashguo.top

CREATE TABLE users (
来源：http://tuy.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gnf.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://jve.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://ypf.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kbc.xingfuxueyuan.xyz

);
来源：http://ucu.meibo888.top

[Q02] 创建带外键的表
来源：http://uml.ydzc1.top

CREATE TABLE orders (
来源：http://kqs.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xsx.aizwys.cn

user_id INT NOT NULL,
来源：http://net.yj202588.top

amount DECIMAL(10, 2),
来源：http://rcy.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zpy.hysaishi.cn

);
来源：http://uov.fanxiaobao.xyz

[Q03] 增加列
来源：http://vlm.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://olj.hnqzz.top

[Q04] 修改列类型
来源：http://ang.hysaishi.cn


<!-- 参考信息 -->