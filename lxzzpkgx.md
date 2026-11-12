代发 wailian999

Ruby: exit 1
来源：http://ocu.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgh.0kj1m.cn

[M06] 向标准错误输出
来源：http://vdl.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://dft.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zpr.cqqwz.cn

JS:   console.error("err")
来源：http://ijq.hfpthk.cn

TS:   console.error("err")
来源：http://bot.svipenyu.cn

Java: System.err.println("err")
来源：http://dez.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pol.havefunace.top

Ruby: warn "err"
来源：http://xvb.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://agb.chenlongwang.top

[M07] 判断是否为主入口
来源：http://wsz.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://seb.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jwg.cheryme.top

JS:   require.main === module
来源：http://sfi.cucudq.cn

TS:   require.main === module
来源：http://xdh.aibaodan.cn

Java: public static void main(String[] args)
来源：http://qmc.wangshuangyany.cn

Go:   func main()
来源：http://nda.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gqg.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://tsl.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://aef.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://obm.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://xrh.cucudq.cn

JS:   process.platform;  process.version
来源：http://ofw.jiagoushi.top

TS:   process.platform;  process.version
来源：http://lrv.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://clb.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hpl.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://phn.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://rhf.quarkkingdee.top

================================================================================
来源：http://lbn.nanxuanxn.top

N. 数据结构与算法
来源：http://kyk.zhijiandao.cn

================================================================================
来源：http://bzf.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://cfg.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://fva.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rol.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iub.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xee.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://ffy.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://fkn.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jul.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://ylm.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://tdx.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ssy.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yuk.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://deb.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oao.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ryh.vehdjk.com

Go:   slices.Sort(arr)
来源：http://soh.gaohongyu789.top

Ruby: arr.sort
来源：http://pnn.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://suk.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://fjy.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wgf.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://yhx.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://juy.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zgs.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://brh.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://adu.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://odm.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://fmf.zhongyouzk.top

[N04] 斐波那契数列
来源：http://bet.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bcp.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iwo.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qls.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vqf.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rkf.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://krl.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dgj.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bnk.fanxiaobao.xyz

[N05] 最大公约数
来源：http://mlb.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://bey.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://evt.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jfg.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kwf.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cqf.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sfh.cqqwz.cn

Ruby: a.gcd(b)
来源：http://dmg.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iru.tianlin.xyz

[N06] 判断回文字符串
来源：http://qnm.fehbvm.com

Py:   s == s[::-1]
来源：http://mti.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://hok.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://bmd.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://xrj.redwolf501.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ogo.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://mxe.hnxiangtu.top

Ruby: s == s.reverse
来源：http://lqo.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qhs.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://sju.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ltk.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rem.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xtg.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://ncj.sufxvd.cn

Java: // 手写 HashMap
来源：http://xzv.hammf.cn

Go:   // 手写 map[int]int
来源：http://zxg.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://axz.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://ith.c1oappe.top

[N08] 生成全排列
来源：http://zsc.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://kir.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://fso.pycfn.com

JS:   // 手写回溯递归
来源：http://zhx.9152youxi.cn

TS:   // 手写回溯递归
来源：http://ftw.sufxvd.cn

Java: // 手写回溯递归
来源：http://taw.ybcxt.top

Go:   // 手写回溯递归
来源：http://awx.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://nsm.zhixingplan.top

C#:   // 手写回溯递归
来源：http://ohd.zdbjq.cn

[N09] 栈与队列
来源：http://bot.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pzy.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aug.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pys.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ocu.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xqr.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rrw.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pvf.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sgf.tanke756.top

[N10] 链表节点定义
来源：http://dhc.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xjz.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rya.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dwa.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://owy.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://hgn.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://ghu.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kfl.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zmw.bbcook.cn

[N11] 二叉树中序遍历
来源：http://fep.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://art.cheryme.top

PHP:  // 手写递归函数
来源：http://awg.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udp.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://igq.zhaomingkeji.xyz

Java: // 手写递归
来源：http://zaf.mhx1999.top

Go:   // 手写递归
来源：http://euj.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ovt.ydzc1.top

C#:   // 手写递归
来源：http://gek.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ahv.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rsi.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://njf.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://owd.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mrx.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ief.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kqf.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ygt.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bfc.xuetiantiany.cn

================================================================================
来源：http://zib.316326.xyz

O. 并发与异步
来源：http://kkm.xingfuxueyuan.xyz

================================================================================
来源：http://gjo.sxryk.cn

[O01] 启动一个线程
来源：http://itg.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iou.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eox.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mmi.cheryme.top

TS:   // 同 JS
来源：http://fni.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://ndd.sysykeji.top

Go:   go f()
来源：http://wlw.smart0.xyz

Ruby: Thread.new { f }
来源：http://dzd.havefunace.top

C#:   Task.Run(() => F());
来源：http://dlh.jinghuilouyu.cn

[O02] 使用线程池
来源：http://pvx.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ucm.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hux.smart0.xyz

JS:   // worker_threads 线程池
来源：http://ftj.c1oappe.top

TS:   // worker_threads 线程池
来源：http://jak.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://nsq.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ozq.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://crq.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jcj.yuxming.cn

[O03] 加锁保护共享数据
来源：http://cnc.ydzc1.top

Py:   with lock: shared += 1
来源：http://llv.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://oxj.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cxh.xylfe.cn

TS:   // 同 JS
来源：http://sce.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://zzm.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nxn.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bzm.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://jbl.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://pxz.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://usp.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://skq.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://xmr.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nky.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wts.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uwx.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://mzh.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://egz.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://arl.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://kyn.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xnk.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://csl.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://nak.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mjr.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jho.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://wpf.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mjs.zhijiandao.cn

[O06] 使用进程池
来源：http://wsn.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sub.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://olp.yonumen.top

JS:   // child_process / cluster 模块
来源：http://ods.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://kyf.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rnr.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dtj.yuanzhike.top

Ruby: // fork 块
来源：http://apz.sxryk.cn

C#:   Parallel.For
来源：http://msl.wangdashe.top

================================================================================
来源：http://jzp.hongshengwenyu.top

P. 常用工具函数
来源：http://why.shuidangran.top

================================================================================
来源：http://ppo.redwolf501.top

[P01] 生成 UUID
来源：http://ksm.hywenlv.cn

Py:   str(uuid.uuid4())
来源：http://uxb.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zvo.tian-w.cn

JS:   crypto.randomUUID()
来源：http://jrw.cheryme.top

TS:   crypto.randomUUID()
来源：http://oza.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://fdx.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://ymc.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://liy.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://zsk.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://bxs.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qwv.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sow.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pez.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ftr.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lxp.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vla.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://auc.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nsj.yj202588.top

[P03] 生成短随机字符串
来源：http://bch.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jiy.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tgl.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qlq.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tsh.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zre.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tjd.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zak.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vuh.yj202588.top

[P04] 求长度
来源：http://hmd.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gfh.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhl.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pxg.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isy.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://gpk.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://ynu.yangfankeji.com

Ruby: x.length;  x.size
来源：http://enw.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zef.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://ojf.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ern.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jfw.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hut.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://srq.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cag.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://yfx.jqgfzy.top

Ruby: a == b
来源：http://uvt.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oeu.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jdu.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://usg.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://zdu.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ytf.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://whe.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ujw.yj20258.top

Go:   if x == nil {}
来源：http://ygo.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eys.meibo888.top

C#:   if (x is null) {}
来源：http://tff.yj202588.top

[P07] 防抖与节流
来源：http://pxc.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gqf.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://pxn.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lju.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpy.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vfg.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hsa.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://oer.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fli.guannengcc.top

[P08] 处理浮点精度问题
来源：http://oku.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://agk.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dwe.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dit.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uvb.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xmf.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bwb.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hkc.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tro.meibo888.top

================================================================================
来源：http://nba.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yff.xylfe.cn

================================================================================
来源：http://yzt.cheryme.top

[Q01] 创建表
来源：http://rfe.ppjwa.cn

CREATE TABLE users (
来源：http://kfh.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://try.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://dlk.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://pxj.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mxt.fktsv.cn

);
来源：http://cja.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://ikz.9152youxi.cn

CREATE TABLE orders (
来源：http://gav.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hth.gotoacloud.top

user_id INT NOT NULL,
来源：http://wug.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://ane.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eqp.yuanzhike.top

);
来源：http://cat.chenlongwang.top

[Q03] 增加列
来源：http://dsz.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://myg.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://efr.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oep.zhijiandao.cn

[Q05] 重命名列
来源：http://mtg.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldp.pengpengdd.cyou

[Q06] 删除列
来源：http://pne.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iol.sufxvd.cn

[Q07] 删除表
来源：http://mig.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://mfx.cdnleiting.top

[Q08] 创建普通索引
来源：http://ive.tarul.cn


<!-- 参考信息 -->