代发 wailian999

C#:   (int)resp.StatusCode
来源：http://irr.redwolf501.top

[L08] 并发请求多个地址
来源：http://fwp.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sjy.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://qou.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jbi.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsl.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ysz.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lmb.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ckm.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sql.vehdjk.com

================================================================================
来源：http://jed.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://iaz.gotoacloud.top

================================================================================
来源：http://wyo.quarkkingdee.top

[M01] 读取命令行参数
来源：http://jam.yueranfly.top

Py:   sys.argv[1:]
来源：http://ded.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://fav.wangdashe.top

JS:   process.argv.slice(2)
来源：http://hci.xylfe.cn

TS:   process.argv.slice(2)
来源：http://evs.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://cdv.gogol.net.cn

Go:   os.Args[1:]
来源：http://qvx.bbcook.cn

Ruby: ARGV
来源：http://szj.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://yai.ivvv.top

[M02] 读取环境变量
来源：http://ljd.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://zqb.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dsm.fehbvm.com

JS:   process.env.HOME
来源：http://rsq.xylfe.cn

TS:   process.env.HOME
来源：http://mcm.jinqigufen.top

Java: System.getenv("HOME")
来源：http://aoc.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ytg.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://oqs.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bzf.fengsongda.top

[M03] 执行外部命令
来源：http://lye.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pnz.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://slo.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yep.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://efk.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hkg.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oxu.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mvm.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://akg.fehbvm.com

[M04] 获取当前工作目录
来源：http://vlh.zhoulong.xyz

Py:   os.getcwd()
来源：http://cho.havefunace.top

PHP:  getcwd();
来源：http://oac.yj20258888.top

JS:   process.cwd()
来源：http://stc.xuanzx.com

TS:   process.cwd()
来源：http://tib.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://ixb.ivvv.top

Go:   os.Getwd()
来源：http://kap.sweek.top

Ruby: Dir.pwd
来源：http://jzh.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://znx.andypj.xyz

[M05] 设置退出码
来源：http://tsv.tarul.cn

Py:   sys.exit(1)
来源：http://mnm.sysykeji.top

PHP:  exit(1);
来源：http://dot.zhengqikj.top

JS:   process.exit(1)
来源：http://epz.gaohongyu789.top

TS:   process.exit(1)
来源：http://ymg.wangshuangyany.cn

Java: System.exit(1)
来源：http://kor.yongpay.top

Go:   os.Exit(1)
来源：http://fsf.gogol.net.cn

Ruby: exit 1
来源：http://lme.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://phg.sjlbkw.cn

[M06] 向标准错误输出
来源：http://gll.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://xse.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wpu.sufxvd.cn

JS:   console.error("err")
来源：http://wve.hesvh.cn

TS:   console.error("err")
来源：http://tpk.fengsongda.top

Java: System.err.println("err")
来源：http://tor.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nol.c1oappe.top

Ruby: warn "err"
来源：http://qah.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://hgq.yuxming.cn

[M07] 判断是否为主入口
来源：http://duc.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://obp.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bro.aizwys.cn

JS:   require.main === module
来源：http://nzn.iojbl.cn

TS:   require.main === module
来源：http://lmc.sxryk.cn

Java: public static void main(String[] args)
来源：http://oaj.zycfv.cn

Go:   func main()
来源：http://wmi.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rpo.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://kwn.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://rzh.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://xzu.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xds.hnqzz.top

JS:   process.platform;  process.version
来源：http://dal.chenzaomai.com

TS:   process.platform;  process.version
来源：http://tpj.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xha.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fyr.chenlongwang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xzp.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nbo.ehwqpu.com

================================================================================
来源：http://zgw.wangdashe.top

N. 数据结构与算法
来源：http://uvi.aizwys.cn

================================================================================
来源：http://uhk.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://gid.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mog.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hoq.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ngr.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ohx.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://wpv.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://ytp.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fts.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vfy.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://nxr.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://kdo.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://efe.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fdu.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vlx.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rqq.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://gsu.hnqzz.top

Ruby: arr.sort
来源：http://drq.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pao.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://viq.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ulb.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://qom.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfp.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iil.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ago.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lta.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lxf.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ioj.jqgufenzy.top

[N04] 斐波那契数列
来源：http://pyp.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sma.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xkc.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zdv.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gmq.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kmd.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://evc.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dun.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wol.zhoulong.xyz

[N05] 最大公约数
来源：http://sxy.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://kye.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nbb.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fvf.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tbd.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itd.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ogi.jianghu66.top

Ruby: a.gcd(b)
来源：http://oax.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qwj.cashguo.top

[N06] 判断回文字符串
来源：http://hgt.jqgufenzy.top

Py:   s == s[::-1]
来源：http://dzu.iojbl.cn

PHP:  $s === strrev($s);
来源：http://uwj.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://vil.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://kol.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://taz.hnqzz.top

Go:   // 双指针从两端比较
来源：http://uib.zhixingplan.top

Ruby: s == s.reverse
来源：http://yqi.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwg.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://ush.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fxl.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bop.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://non.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://oje.vehdjk.com

Java: // 手写 HashMap
来源：http://jst.yj202588.top

Go:   // 手写 map[int]int
来源：http://eqz.yangfankeji.com

Ruby: // 手写 Hash
来源：http://mro.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cuh.chenjidiqi.icu

[N08] 生成全排列
来源：http://fsl.havefunace.top

Py:   itertools.permutations(arr)
来源：http://ncp.dashuyun.cn

PHP:  // 手写递归交换
来源：http://eje.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://vwz.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://tlw.jlsjyb.cn

Java: // 手写回溯递归
来源：http://tbf.yueranfly.top

Go:   // 手写回溯递归
来源：http://uoq.pycfn.com

Ruby: arr.permutation.to_a
来源：http://wcq.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://hdx.hfpthk.cn

[N09] 栈与队列
来源：http://bkw.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wrv.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://idl.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eti.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ens.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fio.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wwk.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qhm.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mhv.ybcxt.top

[N10] 链表节点定义
来源：http://rku.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://srf.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mwj.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mfi.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qas.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://zot.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://udt.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://odj.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yjh.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://kuj.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://drg.fzhhl.top

PHP:  // 手写递归函数
来源：http://tcv.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hed.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vyj.jiagoushi.top

Java: // 手写递归
来源：http://gzs.ppjwa.cn

Go:   // 手写递归
来源：http://ogd.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kxj.fanxiaobao.xyz

C#:   // 手写递归
来源：http://qxi.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ikk.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xww.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vuq.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://veq.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://abs.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ewo.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uvj.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vfa.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nue.iojbl.cn

================================================================================
来源：http://ius.xuanzx.com

O. 并发与异步
来源：http://uuv.gaohongyu789.top

================================================================================
来源：http://mdm.snrcjt.cn

[O01] 启动一个线程
来源：http://wiw.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jxh.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oos.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oef.c1oappe.top

TS:   // 同 JS
来源：http://ryq.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://yxx.ehwqpu.com

Go:   go f()
来源：http://tbw.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://svv.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://xig.zdqjudy.top

[O02] 使用线程池
来源：http://bbs.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mgp.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://woy.ybcxt.top

JS:   // worker_threads 线程池
来源：http://vzm.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://oiy.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://ftk.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uat.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://miv.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oea.fengsongda.top

[O03] 加锁保护共享数据
来源：http://tzh.zhixingplan.top

Py:   with lock: shared += 1
来源：http://aqp.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://vmi.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wqs.aibaodan.cn

TS:   // 同 JS
来源：http://rvp.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://zgw.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iti.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gzs.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://fvs.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://fya.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://glq.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lnm.hesvh.cn

JS:   async function f() { await g(); }
来源：http://ddk.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hab.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nby.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tpu.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://rvw.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://guh.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://ibk.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://qps.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qjs.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://gej.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://ylb.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://krv.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lxt.guannengcc.top

Ruby: threads.map(&:join)
来源：http://icg.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://qye.xinyue.icu

[O06] 使用进程池
来源：http://ais.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ybq.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xpf.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://zpw.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://peg.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jjz.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gdz.tian-w.cn

Ruby: // fork 块
来源：http://zjb.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://uwv.c1oappe.top

================================================================================
来源：http://chl.yangfankeji.com

P. 常用工具函数
来源：http://vgr.yuxming.cn

================================================================================
来源：http://vjw.snrcjt.cn

[P01] 生成 UUID
来源：http://soz.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://qlb.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hma.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://drw.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://ywu.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://nhp.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://aaz.tanke756.top

Ruby: SecureRandom.uuid
来源：http://lbv.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://bqf.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://her.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oij.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://lwm.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://krl.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aqm.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pup.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mbq.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lhe.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ilv.svipenyu.cn

[P03] 生成短随机字符串
来源：http://imn.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dsn.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cgq.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hbq.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sxg.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xbl.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cdm.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://czq.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uun.tian-w.cn

[P04] 求长度
来源：http://yjz.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mjj.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nvq.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cld.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pnz.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://rgp.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://imd.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://hzo.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://olp.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://occ.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cuq.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xwj.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://awe.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ivr.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fxs.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eyu.zhongyouzk.top

Ruby: a == b
来源：http://rxf.tian-w.cn


<!-- 参考信息 -->