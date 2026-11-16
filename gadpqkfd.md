代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cjx.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://ncn.svipenyu.cn

TS:   process.env.HOME
来源：http://mar.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://edz.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wfw.smart0.xyz

Ruby: ENV["HOME"]
来源：http://vrf.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hhp.haohaochexian.top

[M03] 执行外部命令
来源：http://uea.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dzx.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xdf.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://idp.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://prh.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvm.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dyx.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://smy.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://myw.fengsongda.top

[M04] 获取当前工作目录
来源：http://kcf.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://rby.tanke756.top

PHP:  getcwd();
来源：http://mgz.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://mjr.sxryk.cn

TS:   process.cwd()
来源：http://vsy.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://njf.aibaodan.cn

Go:   os.Getwd()
来源：http://mpf.jinqigfzy.top

Ruby: Dir.pwd
来源：http://imo.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ivn.sweek.top

[M05] 设置退出码
来源：http://yiu.gaohongyu789.top

Py:   sys.exit(1)
来源：http://rpk.bbcook.cn

PHP:  exit(1);
来源：http://ord.chenlongwang.top

JS:   process.exit(1)
来源：http://eua.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://vdb.gaohongyu789.top

Java: System.exit(1)
来源：http://hdc.yongpay.top

Go:   os.Exit(1)
来源：http://igy.hongshengwenyu.top

Ruby: exit 1
来源：http://xhg.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nvc.uphjek.com

[M06] 向标准错误输出
来源：http://bbh.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://qfl.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://opr.haohaochexian.top

JS:   console.error("err")
来源：http://wyx.pycfn.com

TS:   console.error("err")
来源：http://yyr.zhixingplan.top

Java: System.err.println("err")
来源：http://nhw.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zfm.tian-w.cn

Ruby: warn "err"
来源：http://uwp.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://lci.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://hte.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://qze.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://npk.fehbvm.com

JS:   require.main === module
来源：http://avl.cheryme.top

TS:   require.main === module
来源：http://dyy.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://uuv.0kj1m.cn

Go:   func main()
来源：http://xqt.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jht.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://dbo.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://kwv.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://pec.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://ius.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://ipg.hnqzz.top

TS:   process.platform;  process.version
来源：http://ouh.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vfn.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://edw.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nno.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wck.52xcode.cn

================================================================================
来源：http://whb.zhijiandao.cn

N. 数据结构与算法
来源：http://scd.vqdsnc.cn

================================================================================
来源：http://bgt.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://dud.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://mqz.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ypy.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzu.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kru.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cgd.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://nxq.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jla.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://gau.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://rqv.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://cnl.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xkt.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gdy.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://evu.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uei.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://qfu.shuidangran.top

Ruby: arr.sort
来源：http://xvz.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zkz.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://vcr.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lot.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://mfl.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://klp.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xup.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vhc.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lzj.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zoa.quarkkingdee.top

C#:   // 手写递归，或 Array.Sort
来源：http://gjj.ehwqpu.com

[N04] 斐波那契数列
来源：http://bnl.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wqe.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sfi.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://prl.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aom.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hwt.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://onh.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xxu.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bcs.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://yph.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://vxf.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://osb.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvz.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvd.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://msy.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cok.aizwys.cn

Ruby: a.gcd(b)
来源：http://yya.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vfh.hammf.cn

[N06] 判断回文字符串
来源：http://jgt.iojbl.cn

Py:   s == s[::-1]
来源：http://nbh.ivvv.top

PHP:  $s === strrev($s);
来源：http://qov.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://pen.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://kdv.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rnl.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://hsa.pycfn.com

Ruby: s == s.reverse
来源：http://tll.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxp.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://txy.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://alz.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gke.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gcu.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://dtk.havefunace.top

Java: // 手写 HashMap
来源：http://say.fengsongda.top

Go:   // 手写 map[int]int
来源：http://hqg.svipenyu.cn

Ruby: // 手写 Hash
来源：http://bky.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tqv.hammf.cn

[N08] 生成全排列
来源：http://qjm.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://drh.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://yiz.epnwcf.com

JS:   // 手写回溯递归
来源：http://tqj.sufxvd.cn

TS:   // 手写回溯递归
来源：http://juy.yanxiufei.cn

Java: // 手写回溯递归
来源：http://srt.hesvh.cn

Go:   // 手写回溯递归
来源：http://ndl.hongshengwenyu.top

Ruby: arr.permutation.to_a
来源：http://rru.sufxvd.cn

C#:   // 手写回溯递归
来源：http://gjh.ehwqpu.com

[N09] 栈与队列
来源：http://zhs.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kyp.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sqi.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qap.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mms.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ulp.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxt.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://caw.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rzy.yj20258.top

[N10] 链表节点定义
来源：http://wjz.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ejq.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rlt.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yle.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xsy.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://qrz.shanyushiyangtech.top

Go:   type Node struct { V int; Next *Node }
来源：http://ugu.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ydf.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fxe.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://gah.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qvx.vehdjk.com

PHP:  // 手写递归函数
来源：http://our.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mzh.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jff.iojbl.cn

Java: // 手写递归
来源：http://aim.hcnkem.com

Go:   // 手写递归
来源：http://mcj.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cjf.zhixingplan.top

C#:   // 手写递归
来源：http://pol.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xsv.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xxd.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://idr.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqy.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vbx.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jdt.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://khx.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hku.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jfd.0kj1m.cn

================================================================================
来源：http://adl.uphjek.com

O. 并发与异步
来源：http://hcy.jyoumei.cn

================================================================================
来源：http://lue.yueranfly.top

[O01] 启动一个线程
来源：http://ouh.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pmk.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dbk.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xaq.yuxming.cn

TS:   // 同 JS
来源：http://mdj.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://uag.ivvv.top

Go:   go f()
来源：http://yay.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://irh.birdmap.top

C#:   Task.Run(() => F());
来源：http://czu.yongpay.top

[O02] 使用线程池
来源：http://mor.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uwl.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bsa.sysykeji.top

JS:   // worker_threads 线程池
来源：http://eyj.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://dji.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nzo.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nvz.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yyh.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pdi.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://zwh.snrcjt.cn

Py:   with lock: shared += 1
来源：http://nqp.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://yer.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://glo.yangfankeji.com

TS:   // 同 JS
来源：http://mpt.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://gsq.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qyt.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wea.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://yck.meibo888.top

[O04] 定义异步函数并等待
来源：http://xai.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://kfi.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfb.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://qzz.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sdr.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lfi.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rif.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://gxh.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://jyy.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://fqg.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://htm.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ukz.meibo888.top

JS:   await Promise.all(tasks)
来源：http://stt.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://mxf.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gxe.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rus.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://ijm.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://svj.zdqjudy.top

[O06] 使用进程池
来源：http://ucs.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qkd.fzhhl.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jjj.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://kji.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://crd.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ang.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kdg.gzhubu.top

Ruby: // fork 块
来源：http://hpo.9152youxi.cn

C#:   Parallel.For
来源：http://fyl.fengsongda.top

================================================================================
来源：http://nok.9152youxi.cn

P. 常用工具函数
来源：http://dxg.shzxlz.cn

================================================================================
来源：http://tlz.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://ida.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://nvr.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oef.52xcode.cn

JS:   crypto.randomUUID()
来源：http://jfk.cashguo.top

TS:   crypto.randomUUID()
来源：http://fxq.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://uch.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://vur.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://uon.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://ogb.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://kft.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ipn.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lsy.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wjt.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wpf.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lxt.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rzz.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ozf.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ecy.gotoacloud.top

[P03] 生成短随机字符串
来源：http://vkf.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uyi.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lvn.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uxl.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ifu.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://edj.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jak.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://weh.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgb.haohaochexian.top

[P04] 求长度
来源：http://soc.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cpu.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://leg.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shg.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wuy.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://lvc.xylfe.cn

Go:   len(arr);  len(m)
来源：http://rsv.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://sei.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nwd.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://kmg.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qwv.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tpo.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zij.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vsa.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cix.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://utp.yuanzhike.top

Ruby: a == b
来源：http://jnp.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://epj.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hma.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aaz.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://gqk.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nto.yfazqb.com

TS:   if (x == null) {}
来源：http://ayl.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ejn.sufxvd.cn

Go:   if x == nil {}
来源：http://jjp.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vuu.havefunace.top

C#:   if (x is null) {}
来源：http://dnz.c1oappe.top

[P07] 防抖与节流
来源：http://hax.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gat.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://agr.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxl.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcd.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jhq.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://npd.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hte.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uwx.yuxming.cn

[P08] 处理浮点精度问题
来源：http://xba.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kjv.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kez.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hvr.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tiw.zhijiandao.cn


<!-- 参考信息 -->