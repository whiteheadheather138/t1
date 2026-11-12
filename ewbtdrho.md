代发 wailian999

Py:   resp.json()
来源：http://spv.hesvh.cn

PHP:  json_decode($body, true);
来源：http://grn.epnwcf.com

JS:   await resp.json()
来源：http://hxq.vehdjk.com

TS:   await resp.json()
来源：http://vqg.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nnr.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mmb.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://bvv.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jbk.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://lga.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tep.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ptl.meibo888.top

JS:   resp.ok;  resp.status
来源：http://ued.yj202588.top

TS:   resp.ok;  resp.status
来源：http://jxu.yuanzhike.top

Java: resp.statusCode()
来源：http://nfw.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://sot.birdmap.top

Ruby: resp.code.to_i
来源：http://ujk.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://fdl.yj20258.top

[L08] 并发请求多个地址
来源：http://kuz.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://npr.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://wmc.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://phn.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsk.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ojp.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kif.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rge.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://llf.ctjpmb.com

================================================================================
来源：http://wuk.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://kpq.ydjk.org.cn

================================================================================
来源：http://otb.cdnleiting.top

[M01] 读取命令行参数
来源：http://qvt.yj20258888.top

Py:   sys.argv[1:]
来源：http://beq.hammf.cn

PHP:  $argv;  $argc;
来源：http://ewi.uphjek.com

JS:   process.argv.slice(2)
来源：http://rjn.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://ztn.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://bjg.zdqjudy.top

Go:   os.Args[1:]
来源：http://nrm.dashuyun.cn

Ruby: ARGV
来源：http://fdb.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://eaa.yj202588.top

[M02] 读取环境变量
来源：http://ntf.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://ien.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dwy.bbcook.cn

JS:   process.env.HOME
来源：http://auh.bbcook.cn

TS:   process.env.HOME
来源：http://luc.jyoumei.cn

Java: System.getenv("HOME")
来源：http://ayr.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tey.shuidangran.top

Ruby: ENV["HOME"]
来源：http://jox.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jhm.aizwys.cn

[M03] 执行外部命令
来源：http://gec.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fly.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zdh.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hlw.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nlq.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vmc.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://wng.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rmz.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://dng.xinyue.icu

[M04] 获取当前工作目录
来源：http://wnz.haohaochexian.top

Py:   os.getcwd()
来源：http://qxd.yj20258888.top

PHP:  getcwd();
来源：http://gqd.vqdsnc.cn

JS:   process.cwd()
来源：http://rai.c1oappe.top

TS:   process.cwd()
来源：http://kml.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://ldq.yanxiufei.cn

Go:   os.Getwd()
来源：http://kng.zhongyouzk.top

Ruby: Dir.pwd
来源：http://lyu.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://wtf.xylfe.cn

[M05] 设置退出码
来源：http://dge.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://nve.guannengcc.top

PHP:  exit(1);
来源：http://igw.zhiwuduotai.top

JS:   process.exit(1)
来源：http://flr.zhengqikj.top

TS:   process.exit(1)
来源：http://dsp.redwolf501.top

Java: System.exit(1)
来源：http://pka.hcnkem.com

Go:   os.Exit(1)
来源：http://hpd.9152youxi.cn

Ruby: exit 1
来源：http://ptn.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zjz.yj20258888.top

[M06] 向标准错误输出
来源：http://pjn.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://iwi.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://npl.gotoacloud.top

JS:   console.error("err")
来源：http://kmk.ybcxt.top

TS:   console.error("err")
来源：http://xkk.xziqi.cn

Java: System.err.println("err")
来源：http://jov.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uvt.guowangkeji.top

Ruby: warn "err"
来源：http://eex.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://czi.wangdashe.top

[M07] 判断是否为主入口
来源：http://fgx.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://msl.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uij.shuidangran.top

JS:   require.main === module
来源：http://bic.zdbjq.cn

TS:   require.main === module
来源：http://jtg.shzxlz.cn

Java: public static void main(String[] args)
来源：http://sxj.ehwqpu.com

Go:   func main()
来源：http://owx.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jtd.aizwys.cn

C#:   static void Main(string[] args)
来源：http://kyf.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://fwp.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://sma.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://shv.zhengqikj.top

JS:   process.platform;  process.version
来源：http://ytp.fengsongda.top

TS:   process.platform;  process.version
来源：http://drp.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nbt.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pbu.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lst.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dsw.zhengqikj.top

================================================================================
来源：http://ipe.gotoacloud.top

N. 数据结构与算法
来源：http://xfy.jinghuilouyu.cn

================================================================================
来源：http://hdm.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://wwa.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://efj.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jmr.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://htu.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fmq.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://etw.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://hgk.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wxp.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wax.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://fby.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://okm.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jml.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wkk.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sop.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kdc.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://ftr.haohaochexian.top

Ruby: arr.sort
来源：http://cwu.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xbv.meibo888.top

[N03] 快速排序（分治示例）
来源：http://omm.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ktm.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://lqk.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtp.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://anb.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://exr.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gel.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gcq.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://aqi.meibo888.top

[N04] 斐波那契数列
来源：http://tqd.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mde.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://awm.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://awi.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://psb.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dsy.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xiv.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vmh.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rdx.sufxvd.cn

[N05] 最大公约数
来源：http://jpc.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://axe.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rfp.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nse.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bse.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mlj.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://usr.jyoumei.cn

Ruby: a.gcd(b)
来源：http://tgn.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kzy.cashguo.top

[N06] 判断回文字符串
来源：http://rcz.ppjwa.cn

Py:   s == s[::-1]
来源：http://jwf.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://pmm.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://nil.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://cox.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pof.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://tcj.yj20258.top

Ruby: s == s.reverse
来源：http://etb.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cgz.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://bce.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cye.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hio.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mqm.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://sny.ybcxt.top

Java: // 手写 HashMap
来源：http://ffq.yonumen.top

Go:   // 手写 map[int]int
来源：http://fss.yuanzhike.top

Ruby: // 手写 Hash
来源：http://xdq.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://sqb.guannengcc.top

[N08] 生成全排列
来源：http://baj.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://xtm.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://yrt.cheryme.top

JS:   // 手写回溯递归
来源：http://hol.mhx1999.top

TS:   // 手写回溯递归
来源：http://dvi.haohaochexian.top

Java: // 手写回溯递归
来源：http://esb.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://kqo.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://sqq.mhx1999.top

C#:   // 手写回溯递归
来源：http://shs.jinqigfzy.top

[N09] 栈与队列
来源：http://ppj.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aix.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jtk.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jqn.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjl.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gmi.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dbi.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sds.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://spc.shuidangran.top

[N10] 链表节点定义
来源：http://xrl.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qhj.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://azs.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyi.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ccw.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://pxj.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://kan.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cdu.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://gbk.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://tei.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nqv.mhx1999.top

PHP:  // 手写递归函数
来源：http://jlh.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gdp.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgl.haohaochexian.top

Java: // 手写递归
来源：http://byb.jinghuilouyu.cn

Go:   // 手写递归
来源：http://avm.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uba.fzhhl.top

C#:   // 手写递归
来源：http://uup.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mzn.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://goe.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sbs.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tpt.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zra.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bku.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pmm.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nqe.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dyp.aizwys.cn

================================================================================
来源：http://ass.aizwys.cn

O. 并发与异步
来源：http://hvd.shzxlz.cn

================================================================================
来源：http://ekw.svipenyu.cn

[O01] 启动一个线程
来源：http://qce.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mzu.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://erw.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://thj.chenjidiqi.icu

TS:   // 同 JS
来源：http://jds.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://hbg.bbcook.cn

Go:   go f()
来源：http://vwh.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://rmi.hammf.cn

C#:   Task.Run(() => F());
来源：http://cld.sxryk.cn

[O02] 使用线程池
来源：http://qig.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pod.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zhf.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://tcc.xziqi.cn

TS:   // worker_threads 线程池
来源：http://ipq.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oul.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lmf.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dbs.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://apr.fzhhl.top

[O03] 加锁保护共享数据
来源：http://mdq.shuidangran.top

Py:   with lock: shared += 1
来源：http://osx.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://nzy.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lao.ybcxt.top

TS:   // 同 JS
来源：http://zaz.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://hct.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wlr.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sfq.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://cxv.tarul.cn

[O04] 定义异步函数并等待
来源：http://mvj.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://lag.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tom.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://gsq.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://exp.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://czi.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://are.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://hko.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://pkz.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://bth.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://vze.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rrl.yj20258.top

JS:   await Promise.all(tasks)
来源：http://ywx.316326.xyz

TS:   await Promise.all(tasks)
来源：http://pde.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://trh.sysykeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kam.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://khv.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pla.cheryme.top

[O06] 使用进程池
来源：http://mvn.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oko.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fsd.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://ndf.sweek.top

TS:   // child_process / cluster 模块
来源：http://dii.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pmb.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qlo.zhiwuduotai.top

Ruby: // fork 块
来源：http://arh.gotoacloud.top

C#:   Parallel.For
来源：http://fnz.chenjidiqi.icu

================================================================================
来源：http://twt.vqdsnc.cn

P. 常用工具函数
来源：http://ezs.yuanzhike.top

================================================================================
来源：http://xqj.hnqzz.top

[P01] 生成 UUID
来源：http://vny.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://uev.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://enk.feifeiyinyue.top

JS:   crypto.randomUUID()
来源：http://zab.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://amu.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://edc.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://nnt.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://kyy.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://hzz.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://wtq.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vkp.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nqk.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ajm.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fbz.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://egv.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lon.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jeo.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aez.hammf.cn

[P03] 生成短随机字符串
来源：http://ebp.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xma.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kod.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mfj.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zim.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xar.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ywf.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ecu.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://odq.yueranfly.top

[P04] 求长度
来源：http://evx.xingfuxueyuan.xyz


<!-- 参考信息 -->