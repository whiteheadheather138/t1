代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://flu.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nji.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pfc.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://vno.yonumen.top

TS:   resp.ok;  resp.status
来源：http://uoi.sjlbkw.cn

Java: resp.statusCode()
来源：http://xcq.havefunace.top

Go:   resp.StatusCode
来源：http://tkh.guannengcc.top

Ruby: resp.code.to_i
来源：http://gwc.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://jkc.ivvv.top

[L08] 并发请求多个地址
来源：http://iis.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kll.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://ukj.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vtu.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hln.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xlq.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nuy.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://osb.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sjh.dashuyun.cn

================================================================================
来源：http://xne.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://rut.jiagoushi.top

================================================================================
来源：http://zqe.hysaishi.cn

[M01] 读取命令行参数
来源：http://gei.havefunace.top

Py:   sys.argv[1:]
来源：http://rqu.c1oappe.top

PHP:  $argv;  $argc;
来源：http://lwm.yvedp.cn

JS:   process.argv.slice(2)
来源：http://pxj.tanke756.top

TS:   process.argv.slice(2)
来源：http://xdc.yonumen.top

Java: args 数组（main 方法参数）
来源：http://eyi.9152youxi.cn

Go:   os.Args[1:]
来源：http://whj.gaohongyu789.top

Ruby: ARGV
来源：http://huq.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://dcy.shzxlz.cn

[M02] 读取环境变量
来源：http://pin.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://eil.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hmq.jqgfzy.top

JS:   process.env.HOME
来源：http://ltc.xuanzx.com

TS:   process.env.HOME
来源：http://gad.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://btl.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mms.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://iql.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wrr.vehdjk.com

[M03] 执行外部命令
来源：http://lqs.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aeg.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kpj.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://duq.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gtc.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://der.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nbv.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://rli.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://wzh.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://lij.yongpay.top

Py:   os.getcwd()
来源：http://hqp.hnqzz.top

PHP:  getcwd();
来源：http://eho.shzxlz.cn

JS:   process.cwd()
来源：http://ccv.haohaochexian.top

TS:   process.cwd()
来源：http://vps.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://syy.hysaishi.cn

Go:   os.Getwd()
来源：http://wyx.svipenyu.cn

Ruby: Dir.pwd
来源：http://vyp.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://uis.gogol.net.cn

[M05] 设置退出码
来源：http://fey.hesvh.cn

Py:   sys.exit(1)
来源：http://gln.fanxiaobao.xyz

PHP:  exit(1);
来源：http://dsq.jyoumei.cn

JS:   process.exit(1)
来源：http://rao.smart0.xyz

TS:   process.exit(1)
来源：http://xlt.hesvh.cn

Java: System.exit(1)
来源：http://rob.shzxlz.cn

Go:   os.Exit(1)
来源：http://dgm.jianghu66.top

Ruby: exit 1
来源：http://gdo.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wlt.ppjwa.cn

[M06] 向标准错误输出
来源：http://nnx.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://ydj.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gyg.wangshuangyany.cn

JS:   console.error("err")
来源：http://khx.shuidangran.top

TS:   console.error("err")
来源：http://gek.hnxiangtu.top

Java: System.err.println("err")
来源：http://pbf.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://erf.jianghu66.top

Ruby: warn "err"
来源：http://pzn.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://aky.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://vkr.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://bys.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lfo.316326.xyz

JS:   require.main === module
来源：http://unl.iojbl.cn

TS:   require.main === module
来源：http://ntk.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://mbr.redwolf501.top

Go:   func main()
来源：http://wwq.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sbk.bjfxy.top

C#:   static void Main(string[] args)
来源：http://fgz.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://dwl.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://sxl.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://jyf.guannengcc.top

JS:   process.platform;  process.version
来源：http://xir.birdmap.top

TS:   process.platform;  process.version
来源：http://eml.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cxd.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ouv.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://otz.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://xsf.havefunace.top

================================================================================
来源：http://wej.yuxming.cn

N. 数据结构与算法
来源：http://pbr.snrcjt.cn

================================================================================
来源：http://nxp.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://nxv.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://znf.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zww.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://htd.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dzo.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ugu.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://nnm.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://par.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://tie.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://dyf.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://lmn.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://row.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yoq.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://jcs.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://plm.yvedp.cn

Go:   slices.Sort(arr)
来源：http://hyk.yj202588.top

Ruby: arr.sort
来源：http://jli.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fsg.yj202588.top

[N03] 快速排序（分治示例）
来源：http://kgc.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sut.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://ywn.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wea.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbk.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cjr.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pfa.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ynr.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://agd.ctjpmb.com

[N04] 斐波那契数列
来源：http://hvn.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxi.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bft.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qba.ctjpmb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://smr.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pal.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hdp.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nog.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lws.quarkkingdee.top

[N05] 最大公约数
来源：http://tmr.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://zfr.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rij.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uka.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wer.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nei.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wou.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://wrr.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://txh.0kj1m.cn

[N06] 判断回文字符串
来源：http://juw.yuxming.cn

Py:   s == s[::-1]
来源：http://alj.yj202588.top

PHP:  $s === strrev($s);
来源：http://vst.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://iyz.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://vlo.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://miw.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://dcf.xziqi.cn

Ruby: s == s.reverse
来源：http://pcb.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mqm.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://flo.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://prw.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xvq.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hzk.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://gwc.yfazqb.com

Java: // 手写 HashMap
来源：http://bpk.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://uls.yj202588.top

Ruby: // 手写 Hash
来源：http://tlh.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dqk.fzhhl.top

[N08] 生成全排列
来源：http://gpx.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://vfx.bjfxy.top

PHP:  // 手写递归交换
来源：http://fho.hcnkem.com

JS:   // 手写回溯递归
来源：http://chp.fktsv.cn

TS:   // 手写回溯递归
来源：http://mta.yuxming.cn

Java: // 手写回溯递归
来源：http://ivh.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://vvh.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://yai.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://yet.feifeiyinyue.top

[N09] 栈与队列
来源：http://mcb.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rby.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shc.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kha.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://crp.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gcl.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cna.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://anv.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vfp.aibaodan.cn

[N10] 链表节点定义
来源：http://mrw.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvr.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fua.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mxq.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gpr.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://zcb.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://vvy.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eia.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tsv.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://vnq.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xxq.yuxming.cn

PHP:  // 手写递归函数
来源：http://ynu.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://chb.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://knf.hywenlv.cn

Java: // 手写递归
来源：http://wdo.jiagoushi.top

Go:   // 手写递归
来源：http://cqk.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vnc.zhixingplan.top

C#:   // 手写递归
来源：http://ijc.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jfk.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qii.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wly.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://twj.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzv.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kmf.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hue.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wxm.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ria.shzxlz.cn

================================================================================
来源：http://svn.ctjpmb.com

O. 并发与异步
来源：http://abj.hammf.cn

================================================================================
来源：http://nhd.xylfe.cn

[O01] 启动一个线程
来源：http://qhg.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://csa.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tlb.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ndy.dashuyun.cn

TS:   // 同 JS
来源：http://too.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://cms.mhx1999.top

Go:   go f()
来源：http://ofj.tanke756.top

Ruby: Thread.new { f }
来源：http://scc.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://dpi.hnqzz.top

[O02] 使用线程池
来源：http://mew.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ipx.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sbw.pycfn.com

JS:   // worker_threads 线程池
来源：http://tgx.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://mob.tanke756.top

Java: Executors.newFixedThreadPool(4)
来源：http://vxd.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iuf.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ast.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://otr.ivvv.top

[O03] 加锁保护共享数据
来源：http://nww.xylfe.cn

Py:   with lock: shared += 1
来源：http://qhd.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://aii.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ysw.yuxming.cn

TS:   // 同 JS
来源：http://wuh.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://bmj.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qxy.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uyl.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://fyj.andypj.xyz

[O04] 定义异步函数并等待
来源：http://wnv.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://hwr.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dgw.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://vei.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tdl.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rdw.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kjg.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://hzr.hammf.cn

C#:   async Task F() { await G(); }
来源：http://nbp.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://yfg.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://ztl.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zkf.pycfn.com

JS:   await Promise.all(tasks)
来源：http://ywl.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://vfb.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xxr.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://utf.tian-w.cn

Ruby: threads.map(&:join)
来源：http://qln.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ggc.yj20258.top

[O06] 使用进程池
来源：http://yga.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hhr.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ivc.sweek.top

JS:   // child_process / cluster 模块
来源：http://iol.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://ifd.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jmw.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mej.cucudq.cn

Ruby: // fork 块
来源：http://eoc.ctjpmb.com

C#:   Parallel.For
来源：http://fpx.yj20258888.top

================================================================================
来源：http://zjy.bjfxy.top

P. 常用工具函数
来源：http://dvx.yj20258888.top

================================================================================
来源：http://sfq.sufxvd.cn

[P01] 生成 UUID
来源：http://ocz.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://meg.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ipu.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://hjy.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://egp.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://gow.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://apn.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://dfm.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://hgt.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://zsr.andypj.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://grk.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jmw.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rdf.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vpd.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mov.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qkx.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nlx.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://izq.yj202588.top

[P03] 生成短随机字符串
来源：http://xvz.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ych.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ypz.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bip.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blr.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fbn.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dxy.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fja.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wvf.jqgfzy.top

[P04] 求长度
来源：http://dnw.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nxn.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ims.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ver.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lmb.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://prh.uphjek.com

Go:   len(arr);  len(m)
来源：http://jbv.wangdashe.top

Ruby: x.length;  x.size
来源：http://uuv.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kcr.zycfv.cn


<!-- 参考信息 -->