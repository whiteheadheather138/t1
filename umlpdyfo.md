代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ous.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kls.shangyingyoupin.top

================================================================================
来源：http://hrb.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://uze.fanxiaobao.xyz

================================================================================
来源：http://mns.ybcxt.top

[M01] 读取命令行参数
来源：http://ang.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://tdn.daria6918.cn

PHP:  $argv;  $argc;
来源：http://hcb.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://aac.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://doj.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://qyi.jiagoushi.top

Go:   os.Args[1:]
来源：http://tgv.ywan-chungtsiang.top

Ruby: ARGV
来源：http://csl.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://zkx.ehwqpu.com

[M02] 读取环境变量
来源：http://fkm.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://umi.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wvb.yonumen.top

JS:   process.env.HOME
来源：http://yve.zhijiandao.cn

TS:   process.env.HOME
来源：http://vnt.redwolf501.top

Java: System.getenv("HOME")
来源：http://ewj.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pce.fzhhl.top

Ruby: ENV["HOME"]
来源：http://ske.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xgr.mhx1999.top

[M03] 执行外部命令
来源：http://bru.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yaq.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wrf.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jtr.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bra.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kmn.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wni.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vow.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://pvn.nwbrower.top

[M04] 获取当前工作目录
来源：http://cmw.yj202588.top

Py:   os.getcwd()
来源：http://xiq.aizwys.cn

PHP:  getcwd();
来源：http://ais.jlsjyb.cn

JS:   process.cwd()
来源：http://pio.vehdjk.com

TS:   process.cwd()
来源：http://fex.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://oxn.zhiwuduotai.top

Go:   os.Getwd()
来源：http://voj.guowangkeji.top

Ruby: Dir.pwd
来源：http://usj.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://pkw.xuetiantiany.cn

[M05] 设置退出码
来源：http://ass.cqqwz.cn

Py:   sys.exit(1)
来源：http://fwp.xuanzx.com

PHP:  exit(1);
来源：http://ooq.fzhhl.top

JS:   process.exit(1)
来源：http://vdy.fengsongda.top

TS:   process.exit(1)
来源：http://jna.hongshengwenyu.top

Java: System.exit(1)
来源：http://zxt.zdqjudy.top

Go:   os.Exit(1)
来源：http://slx.xinyue.icu

Ruby: exit 1
来源：http://znp.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oiy.jianghu66.top

[M06] 向标准错误输出
来源：http://psk.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://fnu.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pck.jqgufenzy.top

JS:   console.error("err")
来源：http://its.hfpthk.cn

TS:   console.error("err")
来源：http://awy.haohaochexian.top

Java: System.err.println("err")
来源：http://myf.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tkj.yj202588.top

Ruby: warn "err"
来源：http://zic.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://etp.ppjwa.cn

[M07] 判断是否为主入口
来源：http://typ.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://wyx.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ssi.shzxlz.cn

JS:   require.main === module
来源：http://cyk.pycfn.com

TS:   require.main === module
来源：http://xth.gogol.net.cn

Java: public static void main(String[] args)
来源：http://ena.ydzc1.top

Go:   func main()
来源：http://pzt.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jdb.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://rad.ivvv.top

[M08] 获取系统与运行时信息
来源：http://whl.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://gep.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://wij.yvedp.cn

JS:   process.platform;  process.version
来源：http://arx.hesvh.cn

TS:   process.platform;  process.version
来源：http://imi.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qis.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fws.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bmv.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lvo.daxiang520.top

================================================================================
来源：http://yoh.wangdashe.top

N. 数据结构与算法
来源：http://cof.chenlongwang.top

================================================================================
来源：http://fhs.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://heb.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://gsx.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hsc.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://avg.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ulc.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://uvf.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://ebr.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tqg.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://hci.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://uyo.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://yfx.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://npp.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mqw.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://edk.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wlv.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://ymx.cdnleiting.top

Ruby: arr.sort
来源：http://hca.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yye.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://gpq.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cda.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://dgu.gzhubu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jaf.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvc.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://voo.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ldv.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dqa.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://zbu.gzhubu.top

[N04] 斐波那契数列
来源：http://ofj.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bck.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jhf.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eio.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gni.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://abj.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vio.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://daw.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cjk.sjlbkw.cn

[N05] 最大公约数
来源：http://wbn.c1oappe.top

Py:   math.gcd(a, b)
来源：http://qqw.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uxu.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qpj.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://suc.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uhd.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://evb.tanke756.top

Ruby: a.gcd(b)
来源：http://dfw.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vdl.cucudq.cn

[N06] 判断回文字符串
来源：http://hxs.birdmap.top

Py:   s == s[::-1]
来源：http://ohj.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://cvx.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://cwq.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://lpb.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vck.mhx1999.top

Go:   // 双指针从两端比较
来源：http://rtl.tian-w.cn

Ruby: s == s.reverse
来源：http://nyf.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jzu.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://dei.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pwg.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cee.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qnk.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://spz.quarkkingdee.top

Java: // 手写 HashMap
来源：http://nul.fktsv.cn

Go:   // 手写 map[int]int
来源：http://udm.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://pgr.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://iwx.52xcode.cn

[N08] 生成全排列
来源：http://hol.uphjek.com

Py:   itertools.permutations(arr)
来源：http://azo.jiagoushi.top

PHP:  // 手写递归交换
来源：http://ovg.redwolf501.top

JS:   // 手写回溯递归
来源：http://rgf.dashuyun.cn

TS:   // 手写回溯递归
来源：http://val.xuanzx.com

Java: // 手写回溯递归
来源：http://hmq.chenzaomai.com

Go:   // 手写回溯递归
来源：http://mwv.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://sst.fktsv.cn

C#:   // 手写回溯递归
来源：http://nhk.fanxiaobao.xyz

[N09] 栈与队列
来源：http://jsa.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xad.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vli.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zxq.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gtu.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lom.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zgp.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://onc.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bec.redwolf501.top

[N10] 链表节点定义
来源：http://obo.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ido.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://pfq.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cuo.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rro.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://upp.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://mzv.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ydj.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tez.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://abq.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bda.cdnleiting.top

PHP:  // 手写递归函数
来源：http://znd.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mda.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qig.ivvv.top

Java: // 手写递归
来源：http://oeh.epnwcf.com

Go:   // 手写递归
来源：http://aaa.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdo.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://thc.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://snp.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fol.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hcx.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jta.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfm.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ezr.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://phg.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jtu.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nua.tian-w.cn

================================================================================
来源：http://ewa.jqgufenzy.top

O. 并发与异步
来源：http://nkh.snrcjt.cn

================================================================================
来源：http://viu.daria6918.cn

[O01] 启动一个线程
来源：http://oas.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ril.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bbg.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bps.ehwqpu.com

TS:   // 同 JS
来源：http://xsh.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://xve.yueranfly.top

Go:   go f()
来源：http://qdc.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://xiq.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://wni.jinghuilouyu.cn

[O02] 使用线程池
来源：http://vzn.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ury.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iuo.yj20258.top

JS:   // worker_threads 线程池
来源：http://wqm.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://rvy.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://zgk.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sik.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uvk.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hca.xinyue.icu

[O03] 加锁保护共享数据
来源：http://rse.tianlin.xyz

Py:   with lock: shared += 1
来源：http://khy.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://dhr.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yue.9152youxi.cn

TS:   // 同 JS
来源：http://nhm.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://iqw.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xqr.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://haw.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://ijp.smart0.xyz

[O04] 定义异步函数并等待
来源：http://iyw.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://pkg.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jhv.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://jrr.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zup.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mah.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eum.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://uvp.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://jui.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://fss.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://amy.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pir.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://fly.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://bwj.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aqc.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nmq.guannengcc.top

Ruby: threads.map(&:join)
来源：http://mdo.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ydv.ehwqpu.com

[O06] 使用进程池
来源：http://ftf.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vcw.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://unc.yongpay.top

JS:   // child_process / cluster 模块
来源：http://duu.uphjek.com

TS:   // child_process / cluster 模块
来源：http://zam.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://igq.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xhu.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://axq.yanxiufei.cn

C#:   Parallel.For
来源：http://yjx.sxryk.cn

================================================================================
来源：http://uhu.vehdjk.com

P. 常用工具函数
来源：http://frv.yangfankeji.com

================================================================================
来源：http://mug.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://bno.cheryme.top

Py:   str(uuid.uuid4())
来源：http://xpt.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tms.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://efb.fengsongda.top

TS:   crypto.randomUUID()
来源：http://tya.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://fjt.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://kbf.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://yxg.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://qkk.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://cuh.cdnleiting.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mbq.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vja.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bnm.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wxq.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yhi.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dme.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vom.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lki.yangfankeji.com

[P03] 生成短随机字符串
来源：http://omz.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ifr.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gsq.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://amg.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gcq.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cex.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ydf.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://hld.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://agg.ehwqpu.com

[P04] 求长度
来源：http://nnf.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mhz.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vnv.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qwp.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yon.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://qxx.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://mjf.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://ryy.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://imj.ydzc1.top

[P05] 判断两个对象内容是否相等
来源：http://lzw.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://owh.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uwf.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://orn.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://thj.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://upe.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://jsc.xylfe.cn

Ruby: a == b
来源：http://uhs.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rtm.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nyo.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://voe.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://agm.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pdx.gaohongyu789.top

TS:   if (x == null) {}
来源：http://rwg.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dlc.zhongyouzk.top

Go:   if x == nil {}
来源：http://ybh.yj20258.top


<!-- 参考信息 -->