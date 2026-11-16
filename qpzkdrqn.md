代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ukl.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://skr.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://kml.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mek.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://gkw.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ple.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://omz.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://slo.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://gix.jqgfzy.top

Java: resp.statusCode()
来源：http://yab.316326.xyz

Go:   resp.StatusCode
来源：http://hki.birdmap.top

Ruby: resp.code.to_i
来源：http://jqq.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://zux.haohaochexian.top

[L08] 并发请求多个地址
来源：http://nkh.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yyf.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://wyq.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://skm.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://leo.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bpf.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yes.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pfh.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hcr.vehdjk.com

================================================================================
来源：http://ubk.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://ahg.xinyue.icu

================================================================================
来源：http://ppi.andypj.xyz

[M01] 读取命令行参数
来源：http://ass.iojbl.cn

Py:   sys.argv[1:]
来源：http://mac.fengsongda.top

PHP:  $argv;  $argc;
来源：http://hyh.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://trj.cashguo.top

TS:   process.argv.slice(2)
来源：http://ayx.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://eus.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://ikm.dashuyun.cn

Ruby: ARGV
来源：http://zxs.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://mzg.shzxlz.cn

[M02] 读取环境变量
来源：http://eps.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://ywj.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mya.yueranfly.top

JS:   process.env.HOME
来源：http://gyt.shuidangran.top

TS:   process.env.HOME
来源：http://uxg.zhengqikj.top

Java: System.getenv("HOME")
来源：http://irj.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hgs.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://vjc.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cuk.yanxiufei.cn

[M03] 执行外部命令
来源：http://cuk.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://edj.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yrf.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sny.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://hiz.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qnu.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hln.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://htv.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://ube.epnwcf.com

[M04] 获取当前工作目录
来源：http://rgt.cdnleiting.top

Py:   os.getcwd()
来源：http://jmb.sweek.top

PHP:  getcwd();
来源：http://urg.ybcxt.top

JS:   process.cwd()
来源：http://evw.cucudq.cn

TS:   process.cwd()
来源：http://lfp.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://tcz.yj202588.top

Go:   os.Getwd()
来源：http://ybm.aizwys.cn

Ruby: Dir.pwd
来源：http://sxv.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://tux.zhongyouzk.top

[M05] 设置退出码
来源：http://euw.sweek.top

Py:   sys.exit(1)
来源：http://ahp.sufxvd.cn

PHP:  exit(1);
来源：http://nee.kuanghao11.cn

JS:   process.exit(1)
来源：http://ith.wangshuangyany.cn

TS:   process.exit(1)
来源：http://oco.xuanzx.com

Java: System.exit(1)
来源：http://dkt.cashguo.top

Go:   os.Exit(1)
来源：http://iqg.pycfn.com

Ruby: exit 1
来源：http://qba.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ieq.dianchejie.cn

[M06] 向标准错误输出
来源：http://bjk.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://kmq.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xgt.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://qvx.daxiang520.top

TS:   console.error("err")
来源：http://giy.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://ufq.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bzt.hongshengwenyu.top

Ruby: warn "err"
来源：http://feo.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://sbt.redwolf501.top

[M07] 判断是否为主入口
来源：http://yoo.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://ycz.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wtz.nanxinkj.top

JS:   require.main === module
来源：http://iec.fzhhl.top

TS:   require.main === module
来源：http://lng.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://mxs.52xcode.cn

Go:   func main()
来源：http://wcm.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://anj.c1oappe.top

C#:   static void Main(string[] args)
来源：http://flv.meibo888.top

[M08] 获取系统与运行时信息
来源：http://urn.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://pbm.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://prr.yongpay.top

JS:   process.platform;  process.version
来源：http://hbm.sweek.top

TS:   process.platform;  process.version
来源：http://xgz.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://otf.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://twt.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dzq.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nlo.fehbvm.com

================================================================================
来源：http://pvq.hammf.cn

N. 数据结构与算法
来源：http://hac.hnqzz.top

================================================================================
来源：http://rah.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://rky.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lzh.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://stg.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cvi.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oey.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://chs.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://piv.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://txp.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://njm.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://ciy.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://jts.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://any.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qia.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://kcn.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fyi.aizwys.cn

Go:   slices.Sort(arr)
来源：http://ryi.zhengqikj.top

Ruby: arr.sort
来源：http://fpf.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gva.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://snd.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uqi.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://tcz.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tfz.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://onq.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://buk.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oav.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dep.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://dkw.yangfankeji.com

[N04] 斐波那契数列
来源：http://jfy.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blr.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cas.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vkl.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bkm.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iux.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hob.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mre.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://clk.cashguo.top

[N05] 最大公约数
来源：http://juf.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://ztl.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rof.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rap.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fkb.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zgv.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cpa.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://wem.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lgv.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://zro.mhx1999.top

Py:   s == s[::-1]
来源：http://rlj.hnqzz.top

PHP:  $s === strrev($s);
来源：http://prm.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://ibr.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://hea.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jqz.gzhubu.top

Go:   // 双指针从两端比较
来源：http://juk.jqgfzy.top

Ruby: s == s.reverse
来源：http://gkm.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://off.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://spk.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zae.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xyo.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gnr.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://afc.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://jkk.daria6918.cn

Go:   // 手写 map[int]int
来源：http://sbk.yangfankeji.com

Ruby: // 手写 Hash
来源：http://ssm.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://pbn.aibaodan.cn

[N08] 生成全排列
来源：http://tlr.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://yox.gotoacloud.top

PHP:  // 手写递归交换
来源：http://rhm.cdnleiting.top

JS:   // 手写回溯递归
来源：http://jvv.yj20258888.top

TS:   // 手写回溯递归
来源：http://pny.yvedp.cn

Java: // 手写回溯递归
来源：http://dgn.hnqzz.top

Go:   // 手写回溯递归
来源：http://ros.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://mkl.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://kih.tanke756.top

[N09] 栈与队列
来源：http://whk.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zff.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rug.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://flr.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ttn.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://amu.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ael.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vef.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oft.gotoacloud.top

[N10] 链表节点定义
来源：http://yow.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uyn.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vbn.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://axo.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bio.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://irn.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zgz.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gsb.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rah.tanke756.top

[N11] 二叉树中序遍历
来源：http://gki.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://epm.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://hbv.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fwh.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffs.bbcook.cn

Java: // 手写递归
来源：http://ttm.nanxuanxn.top

Go:   // 手写递归
来源：http://vbs.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://slm.cdnleiting.top

C#:   // 手写递归
来源：http://zhv.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://djh.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpz.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rti.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://shh.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qha.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cnb.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fih.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zka.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hme.yj20258888.top

================================================================================
来源：http://zwd.haohaochexian.top

O. 并发与异步
来源：http://rdy.dianchejie.cn

================================================================================
来源：http://vri.dashuyun.cn

[O01] 启动一个线程
来源：http://ctk.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://inj.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eih.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bim.fanxiaobao.xyz

TS:   // 同 JS
来源：http://cmh.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://vku.hfpthk.cn

Go:   go f()
来源：http://dsm.aibaodan.cn

Ruby: Thread.new { f }
来源：http://lwp.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://kac.tian-w.cn

[O02] 使用线程池
来源：http://tbh.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xlu.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xzw.hesvh.cn

JS:   // worker_threads 线程池
来源：http://noc.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://kca.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://owk.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vhx.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yhm.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zjy.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://yoi.yj20258888.top

Py:   with lock: shared += 1
来源：http://kxq.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://ofz.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rab.gotoacloud.top

TS:   // 同 JS
来源：http://nzx.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://rsn.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bzo.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jgn.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://wcb.ivvv.top

[O04] 定义异步函数并等待
来源：http://uar.cashguo.top

Py:   async def f():⏎    await g()
来源：http://nvf.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bcl.52xcode.cn

JS:   async function f() { await g(); }
来源：http://lvl.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lkf.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aqz.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jhc.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jsm.ivvv.top

C#:   async Task F() { await G(); }
来源：http://gaz.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://vro.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://hud.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uus.ivvv.top

JS:   await Promise.all(tasks)
来源：http://rul.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://wte.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbc.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jyz.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://ars.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xgl.fengsongda.top

[O06] 使用进程池
来源：http://hxz.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dqx.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cfw.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://bql.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://cbb.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://krq.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tsg.aizwys.cn

Ruby: // fork 块
来源：http://cwa.snrcjt.cn

C#:   Parallel.For
来源：http://hly.jianghu66.top

================================================================================
来源：http://oho.yj20258.top

P. 常用工具函数
来源：http://mmy.svipenyu.cn

================================================================================
来源：http://ybn.wangshuangyany.cn

[P01] 生成 UUID
来源：http://nmb.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://vgw.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://abx.cheryme.top

JS:   crypto.randomUUID()
来源：http://oau.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://raz.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://yjr.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://phj.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://bvi.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://vyr.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://jpt.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://axd.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qfj.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qvr.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://osk.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ugc.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gcj.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dqt.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nvy.havefunace.top

[P03] 生成短随机字符串
来源：http://rky.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://azu.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mxv.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://omy.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wyl.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vlx.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jzf.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ptc.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gsf.dianchejie.cn

[P04] 求长度
来源：http://vqn.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xhj.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gro.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kkn.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rvb.aibaodan.cn


<!-- 参考信息 -->