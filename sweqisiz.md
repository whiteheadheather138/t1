代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ezf.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://piy.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://bcv.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eku.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://vyk.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dei.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aqi.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://ehh.tarul.cn

TS:   resp.ok;  resp.status
来源：http://zex.316326.xyz

Java: resp.statusCode()
来源：http://hfu.meibo888.top

Go:   resp.StatusCode
来源：http://qrs.xylfe.cn

Ruby: resp.code.to_i
来源：http://tvr.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://jde.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://nor.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://clb.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://eam.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rlo.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://snn.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jis.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lax.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gjy.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fvb.daria6918.cn

================================================================================
来源：http://nfo.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://wmw.andypj.xyz

================================================================================
来源：http://mrr.quarkkingdee.top

[M01] 读取命令行参数
来源：http://tqm.yj20258.top

Py:   sys.argv[1:]
来源：http://rut.cheryme.top

PHP:  $argv;  $argc;
来源：http://atv.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://gzp.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://ntt.yj20258.top

Java: args 数组（main 方法参数）
来源：http://lde.jlsjyb.cn

Go:   os.Args[1:]
来源：http://ntt.svipenyu.cn

Ruby: ARGV
来源：http://ecx.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://jmv.dianchejie.cn

[M02] 读取环境变量
来源：http://rvw.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://bly.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uuf.hnqzz.top

JS:   process.env.HOME
来源：http://hdn.xziqi.cn

TS:   process.env.HOME
来源：http://ell.daxiang520.top

Java: System.getenv("HOME")
来源：http://yvh.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uvh.daxiang520.top

Ruby: ENV["HOME"]
来源：http://vfz.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xkj.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://jkw.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lff.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://esk.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ofg.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://abs.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bta.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://nll.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://vjd.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://mbd.zycfv.cn

[M04] 获取当前工作目录
来源：http://nsu.xziqi.cn

Py:   os.getcwd()
来源：http://uwo.zhongyouzk.top

PHP:  getcwd();
来源：http://dbm.xuetiantiany.cn

JS:   process.cwd()
来源：http://gsb.fktsv.cn

TS:   process.cwd()
来源：http://bed.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://cjw.hcnkem.com

Go:   os.Getwd()
来源：http://ast.ehwqpu.com

Ruby: Dir.pwd
来源：http://vlu.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://tbf.cqqwz.cn

[M05] 设置退出码
来源：http://qhy.jlsjyb.cn

Py:   sys.exit(1)
来源：http://svs.chenzaomai.com

PHP:  exit(1);
来源：http://yru.haohaochexian.top

JS:   process.exit(1)
来源：http://xax.yvedp.cn

TS:   process.exit(1)
来源：http://uch.gogol.net.cn

Java: System.exit(1)
来源：http://rjs.9152youxi.cn

Go:   os.Exit(1)
来源：http://nug.hywenlv.cn

Ruby: exit 1
来源：http://hgm.zhiwuduotai.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yae.fktsv.cn

[M06] 向标准错误输出
来源：http://krk.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://pql.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tdo.zdbjq.cn

JS:   console.error("err")
来源：http://pke.andypj.xyz

TS:   console.error("err")
来源：http://jrs.redwolf501.top

Java: System.err.println("err")
来源：http://imu.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://atq.52xcode.cn

Ruby: warn "err"
来源：http://zvr.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://zjf.hammf.cn

[M07] 判断是否为主入口
来源：http://vet.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://ptm.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vbp.aibaodan.cn

JS:   require.main === module
来源：http://yqt.shangyingyoupin.top

TS:   require.main === module
来源：http://ugu.hywenlv.cn

Java: public static void main(String[] args)
来源：http://jpc.dianchejie.cn

Go:   func main()
来源：http://jzu.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kbb.zycfv.cn

C#:   static void Main(string[] args)
来源：http://dpy.316326.xyz

[M08] 获取系统与运行时信息
来源：http://khc.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://lcb.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://fdt.yj20258888.top

JS:   process.platform;  process.version
来源：http://zrh.bjfxy.top

TS:   process.platform;  process.version
来源：http://udh.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zyn.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zsc.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uxl.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://jpf.yj20258.top

================================================================================
来源：http://pqu.gzhubu.top

N. 数据结构与算法
来源：http://upy.fktsv.cn

================================================================================
来源：http://uxe.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://vos.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://jml.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zui.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://shi.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndb.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://zph.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://eil.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zub.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://rfa.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://jun.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://lqg.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://clz.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ffe.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rxb.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kcn.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://prr.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://xvk.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cti.ivvv.top

[N03] 快速排序（分治示例）
来源：http://chs.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xru.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://uem.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tvm.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxr.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eal.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://taz.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eod.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mhk.fzhhl.top

[N04] 斐波那契数列
来源：http://ozj.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://abi.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qte.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rar.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pwz.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qmh.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rrt.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tie.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://huo.vqdsnc.cn

[N05] 最大公约数
来源：http://idw.bjfxy.top

Py:   math.gcd(a, b)
来源：http://lxb.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gcz.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oep.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dac.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pfy.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tan.redwolf501.top

Ruby: a.gcd(b)
来源：http://iii.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jpi.zhengqikj.top

[N06] 判断回文字符串
来源：http://jrj.gotoacloud.top

Py:   s == s[::-1]
来源：http://fvp.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://jtl.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://dni.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://smf.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pwu.ybcxt.top

Go:   // 双指针从两端比较
来源：http://noh.sxryk.cn

Ruby: s == s.reverse
来源：http://ima.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tar.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://jtk.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://onn.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pga.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oej.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://nrx.tanke756.top

Java: // 手写 HashMap
来源：http://tpp.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://heh.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://nok.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://xhi.yonumen.top

[N08] 生成全排列
来源：http://ihm.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://jku.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://ihf.xuanzx.com

JS:   // 手写回溯递归
来源：http://vms.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://klj.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://ihy.vqdsnc.cn

Go:   // 手写回溯递归
来源：http://ifh.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://nsu.yonumen.top

C#:   // 手写回溯递归
来源：http://ang.nanxinkj.top

[N09] 栈与队列
来源：http://cty.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://thc.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ivh.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fva.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ynn.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qfb.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xjm.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ebe.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdj.tianlin.xyz

[N10] 链表节点定义
来源：http://pts.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hdt.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oma.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://agk.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bjw.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://sni.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://nxq.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xbb.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://gjh.pycfn.com

[N11] 二叉树中序遍历
来源：http://fzh.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zgo.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://hdd.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cbo.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vxl.zhaomingkeji.xyz

Java: // 手写递归
来源：http://mit.9152youxi.cn

Go:   // 手写递归
来源：http://wjp.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dbf.hammf.cn

C#:   // 手写递归
来源：http://vkk.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kxg.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tmp.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gst.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hne.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mvl.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ojl.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ert.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wya.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lbe.nanxuanxn.top

================================================================================
来源：http://veb.tanke756.top

O. 并发与异步
来源：http://zqi.sweek.top

================================================================================
来源：http://wdg.wangdashe.top

[O01] 启动一个线程
来源：http://gvh.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sgk.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zbz.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dzj.iojbl.cn

TS:   // 同 JS
来源：http://fmg.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://ayq.xuetiantiany.cn

Go:   go f()
来源：http://xdj.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://vcb.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://jcv.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://xje.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ggj.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gvg.yj20258888.top

JS:   // worker_threads 线程池
来源：http://fkd.mhx1999.top

TS:   // worker_threads 线程池
来源：http://hgn.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://fjd.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ufw.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sqc.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nac.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://zdj.fehbvm.com

Py:   with lock: shared += 1
来源：http://jab.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://egc.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwf.hfpthk.cn

TS:   // 同 JS
来源：http://kmh.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://oxv.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rkf.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rsv.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://mfe.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://tgp.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://gdm.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uad.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://cip.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tli.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jhy.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zpq.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://ykb.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://uky.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://fcg.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://dba.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bir.ivvv.top

JS:   await Promise.all(tasks)
来源：http://nvy.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://wwd.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tfv.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gfg.316326.xyz

Ruby: threads.map(&:join)
来源：http://wen.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://utj.jiagoushi.top

[O06] 使用进程池
来源：http://bdj.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yty.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pci.pycfn.com

JS:   // child_process / cluster 模块
来源：http://lbw.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://etw.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://owp.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://klj.zycfv.cn

Ruby: // fork 块
来源：http://iso.ydjk.org.cn

C#:   Parallel.For
来源：http://otn.gotoacloud.top

================================================================================
来源：http://reg.hongshengwenyu.top

P. 常用工具函数
来源：http://ddc.chenlongwang.top

================================================================================
来源：http://dii.smart0.xyz

[P01] 生成 UUID
来源：http://wlh.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://htz.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qfu.tian-w.cn

JS:   crypto.randomUUID()
来源：http://whp.iojbl.cn

TS:   crypto.randomUUID()
来源：http://ecx.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://bpv.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://oif.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://lzz.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://lqf.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://izt.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fix.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zxn.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umv.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wnr.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tux.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oww.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://how.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nyi.yonumen.top

[P03] 生成短随机字符串
来源：http://oaz.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qcp.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wlp.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rlp.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grc.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sdd.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mml.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yjc.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hjy.jiagoushi.top

[P04] 求长度
来源：http://ewp.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wzp.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cmf.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vag.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nua.0kj1m.cn


<!-- 参考信息 -->