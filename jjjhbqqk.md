代发 wailian999

C#:   (int)resp.StatusCode
来源：http://ica.tarul.cn

[L08] 并发请求多个地址
来源：http://dev.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bhu.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://qsz.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://anp.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqa.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://byx.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lax.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qjp.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nhr.jqgfzy.top

================================================================================
来源：http://mwr.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://feq.jinghuilouyu.cn

================================================================================
来源：http://rcz.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://uvx.yuanzhike.top

Py:   sys.argv[1:]
来源：http://vzj.mhx1999.top

PHP:  $argv;  $argc;
来源：http://jqq.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://wcz.epnwcf.com

TS:   process.argv.slice(2)
来源：http://pnw.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://vff.fzhhl.top

Go:   os.Args[1:]
来源：http://uar.aibaodan.cn

Ruby: ARGV
来源：http://vah.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://ozq.birdmap.top

[M02] 读取环境变量
来源：http://eai.uphjek.com

Py:   os.environ.get("HOME")
来源：http://pin.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tbv.haohaochexian.top

JS:   process.env.HOME
来源：http://fsc.yuanzhike.top

TS:   process.env.HOME
来源：http://ilp.fktsv.cn

Java: System.getenv("HOME")
来源：http://fjd.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dvz.fehbvm.com

Ruby: ENV["HOME"]
来源：http://zgd.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lvd.hnxiangtu.top

[M03] 执行外部命令
来源：http://nuv.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dwa.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qfm.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zrw.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ioi.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wjz.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nqq.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gol.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://qdm.chenzaomai.com

[M04] 获取当前工作目录
来源：http://fhj.jianghu66.top

Py:   os.getcwd()
来源：http://ika.yanxiufei.cn

PHP:  getcwd();
来源：http://rnj.shanyushiyangtech.top

JS:   process.cwd()
来源：http://ryq.jqgufenzy.top

TS:   process.cwd()
来源：http://tno.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://fub.zdqjudy.top

Go:   os.Getwd()
来源：http://pgb.fehbvm.com

Ruby: Dir.pwd
来源：http://hld.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://vib.gogol.net.cn

[M05] 设置退出码
来源：http://vts.hcnkem.com

Py:   sys.exit(1)
来源：http://snj.jinghuilouyu.cn

PHP:  exit(1);
来源：http://txu.pycfn.com

JS:   process.exit(1)
来源：http://pry.jinqigfzy.top

TS:   process.exit(1)
来源：http://evk.birdmap.top

Java: System.exit(1)
来源：http://jpd.dashuyun.cn

Go:   os.Exit(1)
来源：http://fmu.meibo888.top

Ruby: exit 1
来源：http://pzu.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oyi.tianlin.xyz

[M06] 向标准错误输出
来源：http://rdo.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://kka.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oge.sxryk.cn

JS:   console.error("err")
来源：http://meu.yj202588.top

TS:   console.error("err")
来源：http://ueh.aibaodan.cn

Java: System.err.println("err")
来源：http://ssw.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://utc.yvedp.cn

Ruby: warn "err"
来源：http://yqx.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://rci.cucudq.cn

[M07] 判断是否为主入口
来源：http://vka.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://psb.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yht.sufxvd.cn

JS:   require.main === module
来源：http://msd.hywenlv.cn

TS:   require.main === module
来源：http://wus.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://shj.yj202588.top

Go:   func main()
来源：http://obp.uphjek.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xsf.vehdjk.com

C#:   static void Main(string[] args)
来源：http://qzw.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://jag.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://aje.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://jqm.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://yew.cheryme.top

TS:   process.platform;  process.version
来源：http://sfe.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pqk.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bqj.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ojy.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dhl.kuanghao11.cn

================================================================================
来源：http://mav.jinghuilouyu.cn

N. 数据结构与算法
来源：http://ewc.wangshuangyany.cn

================================================================================
来源：http://dej.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://mdq.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yvw.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jiu.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rvw.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mrz.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://vyu.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://zsr.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eyx.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gwo.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://tvi.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://wjn.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ixm.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vep.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qkk.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://via.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://ksw.pycfn.com

Ruby: arr.sort
来源：http://ctn.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://lkw.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://fyf.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ldx.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://vsa.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://any.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urx.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://let.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nnc.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bzl.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lgl.daria6918.cn

[N04] 斐波那契数列
来源：http://abq.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://myq.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xzm.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ilq.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eal.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://etm.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wlu.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lyx.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pxd.chenjidiqi.icu

[N05] 最大公约数
来源：http://hcv.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://buo.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gnw.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vwv.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxh.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qob.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tsv.sweek.top

Ruby: a.gcd(b)
来源：http://jmg.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ouv.dashuyun.cn

[N06] 判断回文字符串
来源：http://wuq.jqgufenzy.top

Py:   s == s[::-1]
来源：http://xgs.cashguo.top

PHP:  $s === strrev($s);
来源：http://vzo.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://gol.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://jhb.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yvu.birdmap.top

Go:   // 双指针从两端比较
来源：http://rbh.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://vft.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yvi.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://qdy.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vnp.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yeu.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uom.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://vvl.pycfn.com

Java: // 手写 HashMap
来源：http://cat.bbcook.cn

Go:   // 手写 map[int]int
来源：http://vfm.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://qzm.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kgu.jqgufenzy.top

[N08] 生成全排列
来源：http://vzn.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://oys.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://qvp.yvedp.cn

JS:   // 手写回溯递归
来源：http://mdr.cucudq.cn

TS:   // 手写回溯递归
来源：http://vcf.fengsongda.top

Java: // 手写回溯递归
来源：http://khl.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://jch.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://nlt.jlsjyb.cn

C#:   // 手写回溯递归
来源：http://duj.tianlin.xyz

[N09] 栈与队列
来源：http://ipc.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://myg.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ifx.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cvv.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hom.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qwo.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dui.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bsb.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xii.tian-w.cn

[N10] 链表节点定义
来源：http://qhm.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ovb.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zjg.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sfh.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ray.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://dcl.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://zoj.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zpj.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jnf.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://qfo.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ham.tarul.cn

PHP:  // 手写递归函数
来源：http://qmj.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yoz.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izz.xuanzx.com

Java: // 手写递归
来源：http://tzn.redwolf501.top

Go:   // 手写递归
来源：http://lvf.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dnq.ybcxt.top

C#:   // 手写递归
来源：http://xtd.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://isy.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://plb.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rmy.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gro.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://obe.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ngx.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://trr.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fxd.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tmp.yangfankeji.com

================================================================================
来源：http://ylp.sweek.top

O. 并发与异步
来源：http://eoi.zhiwuduotai.top

================================================================================
来源：http://wco.chenjidiqi.icu

[O01] 启动一个线程
来源：http://ytp.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nex.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ldp.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vsu.zhongyouzk.top

TS:   // 同 JS
来源：http://eaq.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://vbo.bbcook.cn

Go:   go f()
来源：http://snr.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://zkw.yuxming.cn

C#:   Task.Run(() => F());
来源：http://acg.meibo888.top

[O02] 使用线程池
来源：http://pde.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bvy.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dfs.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://apm.ivvv.top

TS:   // worker_threads 线程池
来源：http://guw.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://arw.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mls.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vvw.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://urh.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://dzu.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://nyb.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://jtn.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qqe.zycfv.cn

TS:   // 同 JS
来源：http://ksy.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://wqp.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ruc.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mjy.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://wbo.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://lys.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://tgv.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qjq.xinyue.icu

JS:   async function f() { await g(); }
来源：http://ezm.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gza.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nxr.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dtc.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://uat.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://qgj.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://jmr.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://bko.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lkx.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://ked.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://ksw.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nvq.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qsq.shuidangran.top

Ruby: threads.map(&:join)
来源：http://bhs.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xvc.hnxiangtu.top

[O06] 使用进程池
来源：http://ptl.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gfn.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fre.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://rze.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://igy.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fkx.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tqc.zhengqikj.top

Ruby: // fork 块
来源：http://cep.yonumen.top

C#:   Parallel.For
来源：http://xpv.tarul.cn

================================================================================
来源：http://bkb.xinyue.icu

P. 常用工具函数
来源：http://zrn.smart0.xyz

================================================================================
来源：http://npa.yongpay.top

[P01] 生成 UUID
来源：http://mut.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://gmc.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mxm.uphjek.com

JS:   crypto.randomUUID()
来源：http://ftm.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://khy.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://apn.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://wgo.yonumen.top

Ruby: SecureRandom.uuid
来源：http://ipn.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://wco.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://oar.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tbl.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jze.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wjg.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fvv.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://weq.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xdd.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tzg.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://keb.svipenyu.cn

[P03] 生成短随机字符串
来源：http://jgc.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ded.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pqm.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zrg.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://win.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mak.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kau.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aaq.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tes.chenlongwang.top

[P04] 求长度
来源：http://yjc.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qni.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tpm.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://skk.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zjj.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://ioa.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://cwc.yueranfly.top

Ruby: x.length;  x.size
来源：http://pza.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mxq.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://cze.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cav.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://las.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ipj.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xyq.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pbk.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://vpv.zhixingplan.top

Ruby: a == b
来源：http://ifi.cdnleiting.top


<!-- 参考信息 -->