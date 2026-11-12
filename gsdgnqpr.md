代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://enp.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ouq.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://try.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gnw.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://tda.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nlv.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ivz.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://dsk.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://jab.hesvh.cn

Java: resp.statusCode()
来源：http://sla.chenlongwang.top

Go:   resp.StatusCode
来源：http://oyf.hesvh.cn

Ruby: resp.code.to_i
来源：http://nll.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://kbg.daria6918.cn

[L08] 并发请求多个地址
来源：http://oqy.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hiw.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://zdi.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://erw.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uyf.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ueo.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ojz.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://myg.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://plm.ehwqpu.com

================================================================================
来源：http://lyj.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://owm.iojbl.cn

================================================================================
来源：http://hjz.ppjwa.cn

[M01] 读取命令行参数
来源：http://viq.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://eex.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://ouq.tanke756.top

JS:   process.argv.slice(2)
来源：http://bcb.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://baf.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://hwk.meibo888.top

Go:   os.Args[1:]
来源：http://kap.sxryk.cn

Ruby: ARGV
来源：http://tdy.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://hyd.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://mah.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://xzu.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbk.tian-w.cn

JS:   process.env.HOME
来源：http://ylr.epnwcf.com

TS:   process.env.HOME
来源：http://nxi.hfpthk.cn

Java: System.getenv("HOME")
来源：http://aai.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pjo.xylfe.cn

Ruby: ENV["HOME"]
来源：http://ptb.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xyi.hfpthk.cn

[M03] 执行外部命令
来源：http://bry.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://suq.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qmt.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ucj.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://byt.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lwy.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sxt.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://fmg.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://vef.andypj.xyz

[M04] 获取当前工作目录
来源：http://cwt.zdqjudy.top

Py:   os.getcwd()
来源：http://ive.yj202588.top

PHP:  getcwd();
来源：http://ggb.ydjk.org.cn

JS:   process.cwd()
来源：http://zvm.hammf.cn

TS:   process.cwd()
来源：http://aqm.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://wfy.yuxming.cn

Go:   os.Getwd()
来源：http://aul.smart0.xyz

Ruby: Dir.pwd
来源：http://ewo.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://ajy.zdbjq.cn

[M05] 设置退出码
来源：http://rtb.fktsv.cn

Py:   sys.exit(1)
来源：http://ixq.xylfe.cn

PHP:  exit(1);
来源：http://war.zhengqikj.top

JS:   process.exit(1)
来源：http://nvs.yvedp.cn

TS:   process.exit(1)
来源：http://evk.zhijiandao.cn

Java: System.exit(1)
来源：http://czq.sxryk.cn

Go:   os.Exit(1)
来源：http://rkp.ydjk.org.cn

Ruby: exit 1
来源：http://vhh.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://usi.jinqigufen.top

[M06] 向标准错误输出
来源：http://dph.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://efd.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kfk.jlsjyb.cn

JS:   console.error("err")
来源：http://cdh.sufxvd.cn

TS:   console.error("err")
来源：http://rsc.c1oappe.top

Java: System.err.println("err")
来源：http://uog.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://soe.birdmap.top

Ruby: warn "err"
来源：http://ygs.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://yjj.zhixingplan.top

[M07] 判断是否为主入口
来源：http://xqx.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://mca.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://knn.bjfxy.top

JS:   require.main === module
来源：http://sye.birdmap.top

TS:   require.main === module
来源：http://mha.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://ceu.yfazqb.com

Go:   func main()
来源：http://kkj.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dtp.tarul.cn

C#:   static void Main(string[] args)
来源：http://wuj.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://brf.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://tmc.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://xde.c1oappe.top

JS:   process.platform;  process.version
来源：http://wub.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://lvo.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qhm.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pvu.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nbf.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mno.yonumen.top

================================================================================
来源：http://bhi.zhoulong.xyz

N. 数据结构与算法
来源：http://oib.sjlbkw.cn

================================================================================
来源：http://rqe.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://xpm.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://jeu.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wms.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pfy.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qxf.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://eoa.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://ptm.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mxs.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://vwp.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://zto.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://bcp.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://syl.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sax.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ffj.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ipp.smart0.xyz

Go:   slices.Sort(arr)
来源：http://bou.havefunace.top

Ruby: arr.sort
来源：http://kpy.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mls.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://ilb.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cli.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://sbv.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tnr.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gri.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vrt.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://awn.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iiu.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lmm.nanxuanxn.top

[N04] 斐波那契数列
来源：http://zru.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lzx.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://poc.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://agc.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rbf.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gah.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://scd.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ycg.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cql.yuxming.cn

[N05] 最大公约数
来源：http://fta.uphjek.com

Py:   math.gcd(a, b)
来源：http://bhk.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lkc.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://acg.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pfc.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sbq.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mab.daria6918.cn

Ruby: a.gcd(b)
来源：http://zdi.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cyq.wangdashe.top

[N06] 判断回文字符串
来源：http://kgv.jianghu66.top

Py:   s == s[::-1]
来源：http://qux.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://hyw.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://cep.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://eao.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uet.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://dgz.tianlin.xyz

Ruby: s == s.reverse
来源：http://vul.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fof.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://awe.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wyv.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dzn.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eig.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://fve.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://nlm.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://mcg.ivvv.top

Ruby: // 手写 Hash
来源：http://dlh.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://szf.sjlbkw.cn

[N08] 生成全排列
来源：http://aut.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://ehq.0kj1m.cn

PHP:  // 手写递归交换
来源：http://gcu.gotoacloud.top

JS:   // 手写回溯递归
来源：http://jbs.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://bvt.bjfxy.top

Java: // 手写回溯递归
来源：http://nao.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://jej.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://aab.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://eau.meibo888.top

[N09] 栈与队列
来源：http://ddw.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dac.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ccj.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wsk.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tmk.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pic.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cuc.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mgd.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eqf.vehdjk.com

[N10] 链表节点定义
来源：http://cpd.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ler.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://neo.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jog.yj202588.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hon.tanke756.top

Java: class Node { int v; Node next; }
来源：http://iim.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://bxk.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://nxt.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fqr.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://vaq.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rlh.cqqwz.cn

PHP:  // 手写递归函数
来源：http://amx.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jry.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqx.yj20258888.top

Java: // 手写递归
来源：http://emz.xinyue.icu

Go:   // 手写递归
来源：http://gyh.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gwv.yuanzhike.top

C#:   // 手写递归
来源：http://fky.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ley.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qzw.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://thc.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rpo.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://juv.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ssj.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hyx.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://haw.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pne.jinqigufen.top

================================================================================
来源：http://ksr.quarkkingdee.top

O. 并发与异步
来源：http://ukb.chenjidiqi.icu

================================================================================
来源：http://ncl.pycfn.com

[O01] 启动一个线程
来源：http://bup.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dae.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vwl.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://adw.zhengqikj.top

TS:   // 同 JS
来源：http://vav.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://oxc.gotoacloud.top

Go:   go f()
来源：http://oav.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://iix.yfazqb.com

C#:   Task.Run(() => F());
来源：http://baj.guowangkeji.top

[O02] 使用线程池
来源：http://mox.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ygs.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rex.gzhubu.top

JS:   // worker_threads 线程池
来源：http://kec.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://cos.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://dxa.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xce.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bpj.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kpi.yj20258888.top

[O03] 加锁保护共享数据
来源：http://lwp.fengsongda.top

Py:   with lock: shared += 1
来源：http://rwe.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://yzw.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pgp.tianlin.xyz

TS:   // 同 JS
来源：http://zdy.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://cyu.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cib.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fbv.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://ize.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://cgm.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://nwd.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nqh.316326.xyz

JS:   async function f() { await g(); }
来源：http://wuc.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://sfy.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ozc.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://brh.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://plf.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://jcn.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://xbp.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://anx.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hho.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://nli.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://xpy.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dxu.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cdt.hnqzz.top

Ruby: threads.map(&:join)
来源：http://ffe.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://esn.uphjek.com

[O06] 使用进程池
来源：http://gwp.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://umv.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dan.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://xzc.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://uze.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lbz.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wft.sweek.top

Ruby: // fork 块
来源：http://uxv.snrcjt.cn

C#:   Parallel.For
来源：http://epm.guowangkeji.top

================================================================================
来源：http://vrh.sysykeji.top

P. 常用工具函数
来源：http://qzl.hnxiangtu.top

================================================================================
来源：http://jbr.yangfankeji.com

[P01] 生成 UUID
来源：http://prq.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://vue.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ssf.mhx1999.top

JS:   crypto.randomUUID()
来源：http://xax.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://sgj.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://bad.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://aio.birdmap.top

Ruby: SecureRandom.uuid
来源：http://pgt.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://nki.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://rni.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://phh.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zcr.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ick.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xnt.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lte.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hyt.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fru.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vce.zhixingplan.top

[P03] 生成短随机字符串
来源：http://oje.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wzp.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fwv.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ocz.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mkz.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://njs.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fmo.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qqs.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hya.cucudq.cn

[P04] 求长度
来源：http://cyz.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wee.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zet.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gzp.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://suv.tianlin.xyz


<!-- 参考信息 -->