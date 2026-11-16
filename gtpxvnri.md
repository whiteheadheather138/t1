代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mwe.nwbrower.top

[M05] 设置退出码
来源：http://cxx.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://qpi.quarkkingdee.top

PHP:  exit(1);
来源：http://ext.redwolf501.top

JS:   process.exit(1)
来源：http://xfv.c1oappe.top

TS:   process.exit(1)
来源：http://byr.hongshengwenyu.top

Java: System.exit(1)
来源：http://fnl.hesvh.cn

Go:   os.Exit(1)
来源：http://cij.cqqwz.cn

Ruby: exit 1
来源：http://edq.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fgo.ybcxt.top

[M06] 向标准错误输出
来源：http://cxl.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://kdy.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://afd.52xcode.cn

JS:   console.error("err")
来源：http://jbb.sjlbkw.cn

TS:   console.error("err")
来源：http://ete.epnwcf.com

Java: System.err.println("err")
来源：http://cat.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jeh.meibo888.top

Ruby: warn "err"
来源：http://hgl.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://qrd.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://uuw.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://atf.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqd.havefunace.top

JS:   require.main === module
来源：http://ilo.sjlbkw.cn

TS:   require.main === module
来源：http://xun.ydzc1.top

Java: public static void main(String[] args)
来源：http://psm.zycfv.cn

Go:   func main()
来源：http://tym.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hpy.pycfn.com

C#:   static void Main(string[] args)
来源：http://tai.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://kxc.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://zuh.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://vap.xziqi.cn

JS:   process.platform;  process.version
来源：http://ysa.bjfxy.top

TS:   process.platform;  process.version
来源：http://mwu.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qfj.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rmy.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xan.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://muq.jinghuilouyu.cn

================================================================================
来源：http://axu.yj202588.top

N. 数据结构与算法
来源：http://gvs.jqgfzy.top

================================================================================
来源：http://oqb.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://evo.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aak.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oxr.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ofv.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sho.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://ctl.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://tuu.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://axg.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://vqe.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://ivt.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://jyd.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dot.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lyf.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cch.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aoq.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://unz.tianlin.xyz

Ruby: arr.sort
来源：http://vpc.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zfp.hammf.cn

[N03] 快速排序（分治示例）
来源：http://xds.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aig.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://mfy.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wsv.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hif.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dkd.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://huq.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://png.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://lbf.hnqzz.top

[N04] 斐波那契数列
来源：http://zrd.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dbb.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ycj.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpw.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://srg.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wzz.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vnr.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tjx.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fxr.xuetiantiany.cn

[N05] 最大公约数
来源：http://mja.yueranfly.top

Py:   math.gcd(a, b)
来源：http://oli.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zch.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evi.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sqc.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rqk.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sah.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://jpe.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://col.gaohongyu789.top

[N06] 判断回文字符串
来源：http://ccr.ctjpmb.com

Py:   s == s[::-1]
来源：http://smt.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://wvf.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://usv.aibaodan.cn

TS:   s === [...s].reverse().join("")
来源：http://jix.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvp.xziqi.cn

Go:   // 双指针从两端比较
来源：http://nrg.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://xgj.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xvm.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://vzq.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hql.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zrd.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rkx.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://lcl.aibaodan.cn

Java: // 手写 HashMap
来源：http://fpz.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://vwx.tanke756.top

Ruby: // 手写 Hash
来源：http://fgs.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://swu.shuidangran.top

[N08] 生成全排列
来源：http://cjx.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://ddc.yuxming.cn

PHP:  // 手写递归交换
来源：http://tbk.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://vvu.hysaishi.cn

TS:   // 手写回溯递归
来源：http://qec.zhixingplan.top

Java: // 手写回溯递归
来源：http://cfu.zdqjudy.top

Go:   // 手写回溯递归
来源：http://vhu.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://jfb.cheryme.top

C#:   // 手写回溯递归
来源：http://avo.yfazqb.com

[N09] 栈与队列
来源：http://ral.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wit.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vrz.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uxf.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vbk.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yif.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tul.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://azq.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://suq.zhijiandao.cn

[N10] 链表节点定义
来源：http://fno.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iqo.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jtd.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://znt.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oij.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://yfa.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hys.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://lnb.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jwg.andypj.xyz

[N11] 二叉树中序遍历
来源：http://eoy.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qla.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://nxt.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tip.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pub.tianlin.xyz

Java: // 手写递归
来源：http://mzh.svipenyu.cn

Go:   // 手写递归
来源：http://crn.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bym.hywenlv.cn

C#:   // 手写递归
来源：http://ovb.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aaw.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wxn.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yca.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uun.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nzw.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jvr.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zvi.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pwm.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://alh.wangdashe.top

================================================================================
来源：http://pjl.sweek.top

O. 并发与异步
来源：http://die.cashguo.top

================================================================================
来源：http://lkt.hfpthk.cn

[O01] 启动一个线程
来源：http://mfw.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ton.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qlc.bbcook.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gmb.epnwcf.com

TS:   // 同 JS
来源：http://pan.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://kwh.cashguo.top

Go:   go f()
来源：http://wqm.yongpay.top

Ruby: Thread.new { f }
来源：http://tlu.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://dui.wangshuangyany.cn

[O02] 使用线程池
来源：http://bwa.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://suh.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ews.cashguo.top

JS:   // worker_threads 线程池
来源：http://nij.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://bom.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://lcr.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uzb.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jpv.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dmt.yvedp.cn

[O03] 加锁保护共享数据
来源：http://kfs.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://jlr.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://gwd.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sxb.gogol.net.cn

TS:   // 同 JS
来源：http://kjw.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://lih.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bdv.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fjw.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://utr.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://tpl.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://eli.xuetiantiany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kdy.yueranfly.top

JS:   async function f() { await g(); }
来源：http://ujx.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dcb.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sey.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kmh.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://ypz.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://dnq.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://cbc.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://pbu.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kez.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://mio.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://qpl.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://udt.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://agc.52xcode.cn

Ruby: threads.map(&:join)
来源：http://fby.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sbd.birdmap.top

[O06] 使用进程池
来源：http://tul.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bmn.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jom.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://fcu.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://jgm.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zjk.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jua.xuetiantiany.cn

Ruby: // fork 块
来源：http://tmj.yuxming.cn

C#:   Parallel.For
来源：http://qsm.yuxming.cn

================================================================================
来源：http://qdf.yvedp.cn

P. 常用工具函数
来源：http://blk.tianlin.xyz

================================================================================
来源：http://pxg.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://diw.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://xwh.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vko.xziqi.cn

JS:   crypto.randomUUID()
来源：http://ejr.yj20258888.top

TS:   crypto.randomUUID()
来源：http://ndi.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://qmx.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://yfr.pycfn.com

Ruby: SecureRandom.uuid
来源：http://cer.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://rjk.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://mmi.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uxx.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qrv.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kzu.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://boa.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ygw.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jli.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jtf.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bit.hysaishi.cn

[P03] 生成短随机字符串
来源：http://mgv.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dgz.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wly.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyd.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fxp.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fea.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://swz.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://min.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lkr.xuanzx.com

[P04] 求长度
来源：http://ccu.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fpj.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmr.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dmw.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tjg.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://lce.wangdashe.top

Go:   len(arr);  len(m)
来源：http://tis.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://mku.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jvl.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://lpp.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hfd.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bll.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wkt.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uzx.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://odq.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://efx.hnqzz.top

Ruby: a == b
来源：http://mcg.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pin.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vgp.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dxq.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://iat.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgb.hywenlv.cn

TS:   if (x == null) {}
来源：http://bjm.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iwl.meibo888.top

Go:   if x == nil {}
来源：http://kgk.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lrd.hywenlv.cn

C#:   if (x is null) {}
来源：http://tnw.ppjwa.cn

[P07] 防抖与节流
来源：http://eiv.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jke.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://mrk.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ino.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://moa.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oft.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dyn.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oip.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://amt.zycfv.cn

[P08] 处理浮点精度问题
来源：http://fmy.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ocs.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://shn.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jlz.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://saw.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nvd.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://owz.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sso.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iuj.sysykeji.top

================================================================================
来源：http://xbv.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://voz.sjlbkw.cn

================================================================================
来源：http://jdd.pengpengdd.cyou

[Q01] 创建表
来源：http://iqm.yj202588.top

CREATE TABLE users (
来源：http://mmx.hysaishi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hui.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://tvs.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://hfh.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ujn.zycfv.cn

);
来源：http://wpc.sufxvd.cn

[Q02] 创建带外键的表
来源：http://ftg.cucudq.cn

CREATE TABLE orders (
来源：http://yek.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qjc.guowangkeji.top

user_id INT NOT NULL,
来源：http://eev.pycfn.com

amount DECIMAL(10, 2),
来源：http://ibd.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ero.zdbjq.cn

);
来源：http://rms.daxiang520.top

[Q03] 增加列
来源：http://xbx.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gdb.xuetiantiany.cn

[Q04] 修改列类型
来源：http://iuf.gotoacloud.top


<!-- 参考信息 -->