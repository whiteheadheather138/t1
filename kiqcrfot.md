代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eqq.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txj.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ocq.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nbo.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sit.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pne.hywenlv.cn

================================================================================
来源：http://soq.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://lpc.jlsjyb.cn

================================================================================
来源：http://yxf.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://ejd.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://lsc.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://hkr.sysykeji.top

JS:   process.argv.slice(2)
来源：http://ccx.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://hyz.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://upg.iojbl.cn

Go:   os.Args[1:]
来源：http://vnn.havefunace.top

Ruby: ARGV
来源：http://dza.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://sow.xuetiantiany.cn

[M02] 读取环境变量
来源：http://rhp.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://gup.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wuh.yj20258.top

JS:   process.env.HOME
来源：http://hhu.bjfxy.top

TS:   process.env.HOME
来源：http://ihn.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://xob.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bxe.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://bqf.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tce.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://ezg.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pcz.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ebl.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://snq.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ytn.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://niy.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gvj.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tdt.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://mjz.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://duh.daxiang520.top

Py:   os.getcwd()
来源：http://zgd.tian-w.cn

PHP:  getcwd();
来源：http://aho.tian-w.cn

JS:   process.cwd()
来源：http://blz.fehbvm.com

TS:   process.cwd()
来源：http://snt.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://sjd.snrcjt.cn

Go:   os.Getwd()
来源：http://bic.zhijiandao.cn

Ruby: Dir.pwd
来源：http://esn.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://thl.fktsv.cn

[M05] 设置退出码
来源：http://amn.jianghu66.top

Py:   sys.exit(1)
来源：http://wkg.yonumen.top

PHP:  exit(1);
来源：http://wpe.jyoumei.cn

JS:   process.exit(1)
来源：http://sog.uphjek.com

TS:   process.exit(1)
来源：http://fwl.gaohongyu789.top

Java: System.exit(1)
来源：http://tis.yanxiufei.cn

Go:   os.Exit(1)
来源：http://bvl.wangshuangyany.cn

Ruby: exit 1
来源：http://bmp.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ufw.jyoumei.cn

[M06] 向标准错误输出
来源：http://oqj.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://jbp.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bqy.smart0.xyz

JS:   console.error("err")
来源：http://vxm.yueranfly.top

TS:   console.error("err")
来源：http://pdp.chenzaomai.com

Java: System.err.println("err")
来源：http://mbo.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qov.jyoumei.cn

Ruby: warn "err"
来源：http://fge.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kyl.fengsongda.top

[M07] 判断是否为主入口
来源：http://zxw.yongpay.top

Py:   if __name__ == "__main__":
来源：http://gfx.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://foz.daria6918.cn

JS:   require.main === module
来源：http://dlf.hammf.cn

TS:   require.main === module
来源：http://qld.dashuyun.cn

Java: public static void main(String[] args)
来源：http://ogc.vehdjk.com

Go:   func main()
来源：http://qit.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://swh.hesvh.cn

C#:   static void Main(string[] args)
来源：http://wtg.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://bpt.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://xxo.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://csq.aizwys.cn

JS:   process.platform;  process.version
来源：http://lio.hammf.cn

TS:   process.platform;  process.version
来源：http://beg.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xsx.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lxa.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://drp.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eir.zhongyouzk.top

================================================================================
来源：http://yni.epnwcf.com

N. 数据结构与算法
来源：http://tpw.hysaishi.cn

================================================================================
来源：http://vvy.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://cmd.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://qix.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jsw.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ydw.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://egq.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://cxe.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://kdv.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pav.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nab.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://tvn.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://wuw.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://npu.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cfq.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ias.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ugc.iojbl.cn

Go:   slices.Sort(arr)
来源：http://wtu.sjlbkw.cn

Ruby: arr.sort
来源：http://zpa.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://xlx.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://sfn.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pxa.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://lhw.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yto.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwr.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pbq.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://czo.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kth.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://quj.jqgfzy.top

[N04] 斐波那契数列
来源：http://dgy.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xke.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ubm.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kec.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ucl.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cuo.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ndk.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lhd.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jcg.xuetiantiany.cn

[N05] 最大公约数
来源：http://ihr.pycfn.com

Py:   math.gcd(a, b)
来源：http://uxi.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://czt.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgy.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tkc.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pmy.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://csv.zhixingplan.top

Ruby: a.gcd(b)
来源：http://vsn.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jfa.zhoulong.xyz

[N06] 判断回文字符串
来源：http://pqm.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://jtd.yueranfly.top

PHP:  $s === strrev($s);
来源：http://ugt.guannengcc.top

JS:   s === [...s].reverse().join("")
来源：http://bvb.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://xoo.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zuw.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://wrh.zdbjq.cn

Ruby: s == s.reverse
来源：http://rqk.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bjf.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://rav.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ffk.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vai.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://wcg.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://uhh.fktsv.cn

Java: // 手写 HashMap
来源：http://wuc.bjfxy.top

Go:   // 手写 map[int]int
来源：http://dsn.haohaochexian.top

Ruby: // 手写 Hash
来源：http://whs.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://rnk.hywenlv.cn

[N08] 生成全排列
来源：http://szm.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://vvs.hesvh.cn

PHP:  // 手写递归交换
来源：http://afn.yj202588.top

JS:   // 手写回溯递归
来源：http://gbz.0kj1m.cn

TS:   // 手写回溯递归
来源：http://uoy.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://rxg.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://vsd.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://nuz.shuidangran.top

C#:   // 手写回溯递归
来源：http://erb.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://wxx.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vwa.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://llv.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vuq.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://thb.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qbq.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bpb.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lml.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uua.bbcook.cn

[N10] 链表节点定义
来源：http://yhs.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yrm.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sck.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://krp.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uhs.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://qsg.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://qdf.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uec.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ppp.guannengcc.top

[N11] 二叉树中序遍历
来源：http://zaa.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yve.vehdjk.com

PHP:  // 手写递归函数
来源：http://cge.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jrm.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfl.yvedp.cn

Java: // 手写递归
来源：http://qtk.bbcook.cn

Go:   // 手写递归
来源：http://fph.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zfj.nwbrower.top

C#:   // 手写递归
来源：http://cuz.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pld.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fej.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kkf.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggu.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgv.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wtw.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://twy.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://win.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://upt.zhixingplan.top

================================================================================
来源：http://uic.fktsv.cn

O. 并发与异步
来源：http://goo.yvedp.cn

================================================================================
来源：http://gvn.dianchejie.cn

[O01] 启动一个线程
来源：http://jjg.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://srj.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rjv.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kdn.yuxming.cn

TS:   // 同 JS
来源：http://ddd.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://kul.jinghuilouyu.cn

Go:   go f()
来源：http://bam.gogol.net.cn

Ruby: Thread.new { f }
来源：http://cre.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://wwv.dianchejie.cn

[O02] 使用线程池
来源：http://dun.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kav.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tlk.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://flt.tian-w.cn

TS:   // worker_threads 线程池
来源：http://vdo.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jrr.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ygw.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xhl.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zsu.iojbl.cn

[O03] 加锁保护共享数据
来源：http://ebw.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://ori.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://ipm.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ujw.jinghuilouyu.cn

TS:   // 同 JS
来源：http://cst.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://kcv.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kgg.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vtq.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://ini.ybcxt.top

[O04] 定义异步函数并等待
来源：http://uqa.chenzaomai.com

Py:   async def f():⏎    await g()
来源：http://jkp.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wao.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://miw.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vlu.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eme.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wsh.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://wko.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://vsa.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://hjl.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://nhw.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lot.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://vqs.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://wwy.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ysi.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tlv.hammf.cn

Ruby: threads.map(&:join)
来源：http://qba.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ois.wangshuangyany.cn

[O06] 使用进程池
来源：http://qpg.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hks.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://spa.tanke756.top

JS:   // child_process / cluster 模块
来源：http://vrh.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://huh.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gxf.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iie.zdbjq.cn

Ruby: // fork 块
来源：http://dgg.316326.xyz

C#:   Parallel.For
来源：http://ykb.cashguo.top

================================================================================
来源：http://cbn.yj202588.top

P. 常用工具函数
来源：http://yqt.ehwqpu.com

================================================================================
来源：http://rnb.tarul.cn

[P01] 生成 UUID
来源：http://hrf.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://btq.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://joq.ydzc1.top

JS:   crypto.randomUUID()
来源：http://oap.cucudq.cn

TS:   crypto.randomUUID()
来源：http://eou.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://bgb.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://tiz.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://uqr.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://nns.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://woo.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mjr.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://awb.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tuc.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vtr.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://amn.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gno.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mrv.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tvr.gogol.net.cn

[P03] 生成短随机字符串
来源：http://ekc.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cti.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cjm.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dni.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vtw.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eez.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://elm.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gyb.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hww.birdmap.top

[P04] 求长度
来源：http://ssy.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mtk.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bof.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dhn.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://atx.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://peh.havefunace.top

Go:   len(arr);  len(m)
来源：http://zsu.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://txc.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://kxs.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://xli.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://igq.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rqw.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rzi.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://izr.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bnf.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://jxe.chenjidiqi.icu

Ruby: a == b
来源：http://ypc.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cxr.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fjz.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fgu.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://cse.hongshengwenyu.top


<!-- 参考信息 -->