代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://peq.sweek.top

[M05] 设置退出码
来源：http://kqh.ehwqpu.com

Py:   sys.exit(1)
来源：http://ywx.ehwqpu.com

PHP:  exit(1);
来源：http://fga.nwbrower.top

JS:   process.exit(1)
来源：http://mgl.shangyingyoupin.top

TS:   process.exit(1)
来源：http://xry.ppjwa.cn

Java: System.exit(1)
来源：http://wcl.bbcook.cn

Go:   os.Exit(1)
来源：http://mrk.fehbvm.com

Ruby: exit 1
来源：http://kyo.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wed.cdnleiting.top

[M06] 向标准错误输出
来源：http://nba.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://hqb.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://elu.xuanzx.com

JS:   console.error("err")
来源：http://hwp.hfpthk.cn

TS:   console.error("err")
来源：http://vtd.snrcjt.cn

Java: System.err.println("err")
来源：http://xiz.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uaa.cqqwz.cn

Ruby: warn "err"
来源：http://umh.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://mjj.316326.xyz

[M07] 判断是否为主入口
来源：http://gni.sweek.top

Py:   if __name__ == "__main__":
来源：http://fjc.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ecf.ivvv.top

JS:   require.main === module
来源：http://erm.jinqigfzy.top

TS:   require.main === module
来源：http://mla.yuanzhike.top

Java: public static void main(String[] args)
来源：http://nxr.ydzc1.top

Go:   func main()
来源：http://kia.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://irq.daxiang520.top

C#:   static void Main(string[] args)
来源：http://bne.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://msd.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://exw.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://mnx.cucudq.cn

JS:   process.platform;  process.version
来源：http://bhb.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://mum.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ybf.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kfy.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jcx.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmb.bjfxy.top

================================================================================
来源：http://hdn.wangdashe.top

N. 数据结构与算法
来源：http://ytn.havefunace.top

================================================================================
来源：http://lzk.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://jwr.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://jgr.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ven.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cdo.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fxm.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://fgr.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://akq.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ymv.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://lit.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://mkh.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://sub.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eql.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xzc.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://rsc.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ljh.fehbvm.com

Go:   slices.Sort(arr)
来源：http://hjp.ivvv.top

Ruby: arr.sort
来源：http://gei.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sxg.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://wgm.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fem.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://pgz.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxy.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nrc.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wnw.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ffj.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://maf.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pdv.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://eii.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pkr.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fdr.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wvf.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwq.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pvk.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aba.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://myh.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wil.jinghuilouyu.cn

[N05] 最大公约数
来源：http://oio.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://mao.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rja.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mfq.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zgd.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rtv.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ehv.havefunace.top

Ruby: a.gcd(b)
来源：http://rmy.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qxa.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://ice.birdmap.top

Py:   s == s[::-1]
来源：http://fsy.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://hqe.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://rsf.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://ije.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://poi.52xcode.cn

Go:   // 双指针从两端比较
来源：http://igy.0kj1m.cn

Ruby: s == s.reverse
来源：http://hrd.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mpb.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://vwv.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ima.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bra.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://dmm.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://yur.bbcook.cn

Java: // 手写 HashMap
来源：http://qrm.hcnkem.com

Go:   // 手写 map[int]int
来源：http://ohe.gzhubu.top

Ruby: // 手写 Hash
来源：http://vjx.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://ded.cucudq.cn

[N08] 生成全排列
来源：http://gbo.yj202588.top

Py:   itertools.permutations(arr)
来源：http://jnd.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://vpy.gzhubu.top

JS:   // 手写回溯递归
来源：http://hcc.52xcode.cn

TS:   // 手写回溯递归
来源：http://ply.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://kmf.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://ibq.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://llc.52xcode.cn

C#:   // 手写回溯递归
来源：http://znu.fzhhl.top

[N09] 栈与队列
来源：http://wnp.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vcw.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sye.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://suc.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ayt.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zrb.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lzr.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://opu.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pqe.cheryme.top

[N10] 链表节点定义
来源：http://xra.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cfb.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cmm.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sqn.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://udx.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://kzo.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://hij.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qao.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://uvh.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://dyf.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kpv.guowangkeji.top

PHP:  // 手写递归函数
来源：http://tvm.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sie.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ixb.yj20258888.top

Java: // 手写递归
来源：http://ljy.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://adl.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gur.nanxinkj.top

C#:   // 手写递归
来源：http://dng.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tfc.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xro.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ldv.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmn.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://exl.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ylb.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yfw.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tuo.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dxs.nanxinkj.top

================================================================================
来源：http://ghf.iojbl.cn

O. 并发与异步
来源：http://jog.hfpthk.cn

================================================================================
来源：http://ynl.52xcode.cn

[O01] 启动一个线程
来源：http://njp.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xlv.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oul.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xfe.yvedp.cn

TS:   // 同 JS
来源：http://ofh.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://uue.hywenlv.cn

Go:   go f()
来源：http://fha.xziqi.cn

Ruby: Thread.new { f }
来源：http://sap.52xcode.cn

C#:   Task.Run(() => F());
来源：http://xgu.jlsjyb.cn

[O02] 使用线程池
来源：http://vkb.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jrt.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pxq.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://myz.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://nne.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://evn.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dcp.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ttv.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sqw.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://sev.redwolf501.top

Py:   with lock: shared += 1
来源：http://vos.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://xps.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pyh.zdqjudy.top

TS:   // 同 JS
来源：http://ric.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://dfw.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vok.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ast.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://caq.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://zio.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://zzb.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://msr.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://thc.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://imd.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cbj.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://doa.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://yav.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://xuz.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://bww.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://rte.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pxf.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://tcq.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://crl.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ddk.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mrz.wangdashe.top

Ruby: threads.map(&:join)
来源：http://ppa.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gkw.yj20258888.top

[O06] 使用进程池
来源：http://bcr.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://khc.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zln.sweek.top

JS:   // child_process / cluster 模块
来源：http://uup.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://hwu.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xcb.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gog.svipenyu.cn

Ruby: // fork 块
来源：http://khi.shanyushiyangtech.top

C#:   Parallel.For
来源：http://rfp.ctjpmb.com

================================================================================
来源：http://qwi.vehdjk.com

P. 常用工具函数
来源：http://det.xinyue.icu

================================================================================
来源：http://kqa.tianlin.xyz

[P01] 生成 UUID
来源：http://mkn.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://ise.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://adj.hammf.cn

JS:   crypto.randomUUID()
来源：http://hbm.smart0.xyz

TS:   crypto.randomUUID()
来源：http://wpz.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://ged.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://yia.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://mue.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://lny.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://hrt.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://chp.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ghe.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bmh.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://isa.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ebn.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vzh.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oaw.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://clb.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://tea.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wed.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rrm.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kon.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ucv.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uiy.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wjc.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hau.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kmi.0kj1m.cn

[P04] 求长度
来源：http://dxg.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kie.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfa.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cnb.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qas.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://siq.tarul.cn

Go:   len(arr);  len(m)
来源：http://wqn.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://fbu.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xrp.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://hmc.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cld.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mio.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pel.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://htn.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zhc.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://hhs.zycfv.cn

Ruby: a == b
来源：http://epq.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uee.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rqu.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kjf.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://pqb.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xar.ehwqpu.com

TS:   if (x == null) {}
来源：http://zqh.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://taf.cdnleiting.top

Go:   if x == nil {}
来源：http://olc.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lbk.ctjpmb.com

C#:   if (x is null) {}
来源：http://ofk.ppjwa.cn

[P07] 防抖与节流
来源：http://wyc.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sqn.yonumen.top

PHP:  // 手写时间戳比较
来源：http://cql.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://obw.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybq.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uec.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oom.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mrx.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yun.meibo888.top

[P08] 处理浮点精度问题
来源：http://xpd.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://grc.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vxr.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://snd.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kwh.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://biw.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zsd.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qmm.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wdw.dianchejie.cn

================================================================================
来源：http://qch.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vbo.xinyue.icu

================================================================================
来源：http://xlc.cqqwz.cn

[Q01] 创建表
来源：http://nox.cqqwz.cn

CREATE TABLE users (
来源：http://dau.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvw.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://bdy.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://mny.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yej.zdqjudy.top

);
来源：http://pqf.hammf.cn

[Q02] 创建带外键的表
来源：http://ubn.zhiwuduotai.top

CREATE TABLE orders (
来源：http://rwi.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vhm.ybcxt.top

user_id INT NOT NULL,
来源：http://xqn.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://veu.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qkr.andypj.xyz

);
来源：http://rwd.xuanzx.com

[Q03] 增加列
来源：http://miq.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://orw.9152youxi.cn

[Q04] 修改列类型
来源：http://tih.cucudq.cn


<!-- 参考信息 -->