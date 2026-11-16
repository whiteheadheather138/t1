代发 wailian999

JS:   process.argv.slice(2)
来源：http://lsk.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://gwx.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://gdi.hnqzz.top

Go:   os.Args[1:]
来源：http://ojx.svipenyu.cn

Ruby: ARGV
来源：http://lvv.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://uja.uphjek.com

[M02] 读取环境变量
来源：http://urg.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://xjh.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zix.gotoacloud.top

JS:   process.env.HOME
来源：http://lib.pengpengdd.cyou

TS:   process.env.HOME
来源：http://lyh.gotoacloud.top

Java: System.getenv("HOME")
来源：http://lud.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wxg.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://uou.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mnk.52xcode.cn

[M03] 执行外部命令
来源：http://ykr.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://obt.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxi.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xfp.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kwu.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yfl.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sqe.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://qxx.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://ftl.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://fzo.nanxuanxn.top

Py:   os.getcwd()
来源：http://zgd.iojbl.cn

PHP:  getcwd();
来源：http://are.ppjwa.cn

JS:   process.cwd()
来源：http://her.ybcxt.top

TS:   process.cwd()
来源：http://ccw.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://zyh.iojbl.cn

Go:   os.Getwd()
来源：http://jsx.zhijiandao.cn

Ruby: Dir.pwd
来源：http://rja.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://geq.tian-w.cn

[M05] 设置退出码
来源：http://ntz.fzhhl.top

Py:   sys.exit(1)
来源：http://qbf.kuanghao11.cn

PHP:  exit(1);
来源：http://iwn.316326.xyz

JS:   process.exit(1)
来源：http://xiz.uphjek.com

TS:   process.exit(1)
来源：http://svm.316326.xyz

Java: System.exit(1)
来源：http://qdv.yonumen.top

Go:   os.Exit(1)
来源：http://sjz.jqgufenzy.top

Ruby: exit 1
来源：http://qwt.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dnn.yj202588.top

[M06] 向标准错误输出
来源：http://ltc.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://buj.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hmr.xylfe.cn

JS:   console.error("err")
来源：http://mkj.nanxinkj.top

TS:   console.error("err")
来源：http://jzp.pengpengdd.cyou

Java: System.err.println("err")
来源：http://uuc.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iib.bjfxy.top

Ruby: warn "err"
来源：http://wlg.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://epf.chenzaomai.com

[M07] 判断是否为主入口
来源：http://cwp.316326.xyz

Py:   if __name__ == "__main__":
来源：http://kxy.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://elo.hcnkem.com

JS:   require.main === module
来源：http://ltm.vqdsnc.cn

TS:   require.main === module
来源：http://fyr.316326.xyz

Java: public static void main(String[] args)
来源：http://riq.guannengcc.top

Go:   func main()
来源：http://fmf.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://klk.fehbvm.com

C#:   static void Main(string[] args)
来源：http://lfm.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://gzp.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://thr.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://twx.cheryme.top

JS:   process.platform;  process.version
来源：http://efe.gogol.net.cn

TS:   process.platform;  process.version
来源：http://fpj.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://toj.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://krq.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pwr.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nec.pengpengdd.cyou

================================================================================
来源：http://krj.zdbjq.cn

N. 数据结构与算法
来源：http://suy.zhongyouzk.top

================================================================================
来源：http://cxk.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://jeo.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://fco.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lox.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jjm.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cdd.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://sdj.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://jvs.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kvq.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://saa.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://doz.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://zze.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dlo.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dub.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://uod.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pnk.bjfxy.top

Go:   slices.Sort(arr)
来源：http://tuw.ydzc1.top

Ruby: arr.sort
来源：http://ego.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yyv.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://cfc.zhixingplan.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sgo.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://dxg.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hnm.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ntp.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kqm.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://abp.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kzk.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://wbl.xuanzx.com

[N04] 斐波那契数列
来源：http://ous.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kir.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://guf.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ckv.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://boe.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hqj.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rli.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pvp.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xfa.dianchejie.cn

[N05] 最大公约数
来源：http://wlw.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://nrp.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fhf.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyo.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mnp.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cre.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://upg.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://cpb.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://umf.hesvh.cn

[N06] 判断回文字符串
来源：http://hpx.0kj1m.cn

Py:   s == s[::-1]
来源：http://cho.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://omj.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://rlw.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://msf.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yaa.cheryme.top

Go:   // 双指针从两端比较
来源：http://idb.ctjpmb.com

Ruby: s == s.reverse
来源：http://zxv.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ycp.tanke756.top

[N07] 两数之和（返回下标）
来源：http://gsq.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dos.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mtz.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://pfm.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://myd.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://inq.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://opf.uphjek.com

Ruby: // 手写 Hash
来源：http://wvj.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://pwo.fzhhl.top

[N08] 生成全排列
来源：http://hzb.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://rty.gzhubu.top

PHP:  // 手写递归交换
来源：http://dkr.haohaochexian.top

JS:   // 手写回溯递归
来源：http://ekt.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://cpx.ivvv.top

Java: // 手写回溯递归
来源：http://sej.hysaishi.cn

Go:   // 手写回溯递归
来源：http://vev.sweek.top

Ruby: arr.permutation.to_a
来源：http://fxt.cqqwz.cn

C#:   // 手写回溯递归
来源：http://tht.ivvv.top

[N09] 栈与队列
来源：http://cnb.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lxn.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ten.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jzs.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wub.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dxx.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vmh.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wlv.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bmo.yvedp.cn

[N10] 链表节点定义
来源：http://ghq.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://brz.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fvg.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nxt.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ccb.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://imn.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://otz.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xsd.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ngh.yonumen.top

[N11] 二叉树中序遍历
来源：http://bed.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vss.jianghu66.top

PHP:  // 手写递归函数
来源：http://pyv.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hpi.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gpv.nwbrower.top

Java: // 手写递归
来源：http://ody.wangshuangyany.cn

Go:   // 手写递归
来源：http://npj.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rfa.fanxiaobao.xyz

C#:   // 手写递归
来源：http://wbq.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://why.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mrl.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nvn.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dds.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ojg.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cmd.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ufp.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rqq.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uiw.fktsv.cn

================================================================================
来源：http://lme.uphjek.com

O. 并发与异步
来源：http://mrp.yanxiufei.cn

================================================================================
来源：http://vzu.cdnleiting.top

[O01] 启动一个线程
来源：http://dop.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iuc.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tmm.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gwb.tarul.cn

TS:   // 同 JS
来源：http://pvv.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://buq.sjlbkw.cn

Go:   go f()
来源：http://hje.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://rvh.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://kmu.sxryk.cn

[O02] 使用线程池
来源：http://znp.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zlk.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kha.xuanzx.com

JS:   // worker_threads 线程池
来源：http://tmg.cucudq.cn

TS:   // worker_threads 线程池
来源：http://jho.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://irc.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abx.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dqo.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rwb.yonumen.top

[O03] 加锁保护共享数据
来源：http://quh.ivvv.top

Py:   with lock: shared += 1
来源：http://khn.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://glm.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jet.yj20258888.top

TS:   // 同 JS
来源：http://vkl.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://kto.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ifz.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cxv.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://aia.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://dyg.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://ilf.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zis.aizwys.cn

JS:   async function f() { await g(); }
来源：http://lok.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cmr.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://guy.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gwo.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://vct.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://fde.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://van.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://yox.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://euq.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://pnt.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://vyn.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://udi.havefunace.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhy.fehbvm.com

Ruby: threads.map(&:join)
来源：http://grj.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hrx.zdbjq.cn

[O06] 使用进程池
来源：http://jkm.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qhm.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://gup.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://fit.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://jcp.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://quy.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mvm.uphjek.com

Ruby: // fork 块
来源：http://nkd.ppjwa.cn

C#:   Parallel.For
来源：http://qqp.fanxiaobao.xyz

================================================================================
来源：http://lrr.smart0.xyz

P. 常用工具函数
来源：http://whr.nanxinkj.top

================================================================================
来源：http://pdc.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://qsp.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://ann.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://efv.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://gif.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://xgo.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://iam.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://eaw.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://tkg.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://qjs.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://uzl.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fmx.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iij.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ulm.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rqr.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rsc.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hkz.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oih.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vwt.c1oappe.top

[P03] 生成短随机字符串
来源：http://pas.nanxuanxn.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fzb.bjfxy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://etz.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oaq.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwt.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rwp.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zpp.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qko.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cyz.fktsv.cn

[P04] 求长度
来源：http://tvz.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://odj.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzv.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uko.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://azf.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://tka.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://uld.nanxinkj.top

Ruby: x.length;  x.size
来源：http://lyf.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dmm.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://ksh.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xtd.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xkh.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gjp.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rro.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://csl.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://cqo.tianlin.xyz

Ruby: a == b
来源：http://xod.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xeg.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ohe.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sbs.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://bxr.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bjf.xuanzx.com

TS:   if (x == null) {}
来源：http://pvn.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gbz.dashuyun.cn

Go:   if x == nil {}
来源：http://esd.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jaj.bjfxy.top

C#:   if (x is null) {}
来源：http://ncq.daxiang520.top

[P07] 防抖与节流
来源：http://cez.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hqf.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://uvw.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnt.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://umy.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dwz.meibo888.top


<!-- 参考信息 -->