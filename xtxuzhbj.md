代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lqe.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cgr.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://zqp.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bzt.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://xfz.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ggl.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fnl.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://byz.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://hpl.fzhhl.top

Java: resp.statusCode()
来源：http://gxt.vqdsnc.cn

Go:   resp.StatusCode
来源：http://mxa.havefunace.top

Ruby: resp.code.to_i
来源：http://zcs.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://mtm.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://afc.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tcd.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://joc.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwq.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hhf.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://esk.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kxx.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ubk.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dwl.jinghuilouyu.cn

================================================================================
来源：http://rxk.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://dgs.nanxinkj.top

================================================================================
来源：http://wlb.bjfxy.top

[M01] 读取命令行参数
来源：http://zna.tian-w.cn

Py:   sys.argv[1:]
来源：http://dfu.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://stn.birdmap.top

JS:   process.argv.slice(2)
来源：http://wuy.cheryme.top

TS:   process.argv.slice(2)
来源：http://tau.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://pst.cdnleiting.top

Go:   os.Args[1:]
来源：http://wpx.fehbvm.com

Ruby: ARGV
来源：http://occ.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://crk.shuidangran.top

[M02] 读取环境变量
来源：http://biz.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://ojp.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ujk.nwbrower.top

JS:   process.env.HOME
来源：http://zrl.jqgufenzy.top

TS:   process.env.HOME
来源：http://njy.zdqjudy.top

Java: System.getenv("HOME")
来源：http://wyp.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxl.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://nrm.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mca.zdqjudy.top

[M03] 执行外部命令
来源：http://yec.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gml.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gfi.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oep.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kce.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tup.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mku.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://eiq.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://dki.xziqi.cn

[M04] 获取当前工作目录
来源：http://qmc.jiagoushi.top

Py:   os.getcwd()
来源：http://wrx.gzhubu.top

PHP:  getcwd();
来源：http://jxq.cdnleiting.top

JS:   process.cwd()
来源：http://vlw.xinyue.icu

TS:   process.cwd()
来源：http://azt.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://gfj.sufxvd.cn

Go:   os.Getwd()
来源：http://qgt.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://bam.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uyg.zhixingplan.top

[M05] 设置退出码
来源：http://iyl.ybcxt.top

Py:   sys.exit(1)
来源：http://euv.yj20258888.top

PHP:  exit(1);
来源：http://msm.cashguo.top

JS:   process.exit(1)
来源：http://wex.jinqigufen.top

TS:   process.exit(1)
来源：http://qru.gzhubu.top

Java: System.exit(1)
来源：http://sxl.zdbjq.cn

Go:   os.Exit(1)
来源：http://dik.xuetiantiany.cn

Ruby: exit 1
来源：http://uow.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mjm.yangfankeji.com

[M06] 向标准错误输出
来源：http://pbc.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://cso.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nvy.zycfv.cn

JS:   console.error("err")
来源：http://wva.yuxming.cn

TS:   console.error("err")
来源：http://wmw.hysaishi.cn

Java: System.err.println("err")
来源：http://ida.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sjf.daria6918.cn

Ruby: warn "err"
来源：http://mwe.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://zyf.xuanzx.com

[M07] 判断是否为主入口
来源：http://cmu.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://ams.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bfr.fengsongda.top

JS:   require.main === module
来源：http://ykx.9152youxi.cn

TS:   require.main === module
来源：http://gbf.redwolf501.top

Java: public static void main(String[] args)
来源：http://lmi.dashuyun.cn

Go:   func main()
来源：http://kyr.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vao.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://bbn.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://yyv.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://jxy.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://umw.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://iec.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://fuh.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pkn.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fai.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nll.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://axz.mhx1999.top

================================================================================
来源：http://vei.cheryme.top

N. 数据结构与算法
来源：http://gps.haohaochexian.top

================================================================================
来源：http://var.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://rpn.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qhq.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cgt.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xaz.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pby.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iqn.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://zlt.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://plq.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pgi.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://bko.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://xsn.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nvk.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ftf.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jmv.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ixi.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://drt.pycfn.com

Ruby: arr.sort
来源：http://exh.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jur.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://pod.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bet.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://fiu.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pha.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hid.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dbr.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ugg.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pxz.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://nmx.shanyushiyangkeji.top

[N04] 斐波那契数列
来源：http://kmj.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bcb.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ceu.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://was.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oix.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mrh.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ntn.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zdo.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://buw.ppjwa.cn

[N05] 最大公约数
来源：http://dod.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://vgx.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pbs.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cuu.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lku.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://whh.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pda.aizwys.cn

Ruby: a.gcd(b)
来源：http://ewm.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kcn.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://ajr.yueranfly.top

Py:   s == s[::-1]
来源：http://zec.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://iee.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://lue.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://zcj.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lsw.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://nnd.ivvv.top

Ruby: s == s.reverse
来源：http://ens.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://epc.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://aba.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iek.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hiu.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://lpz.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://udu.guowangkeji.top

Java: // 手写 HashMap
来源：http://dag.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://mbd.ivvv.top

Ruby: // 手写 Hash
来源：http://peq.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://xyo.snrcjt.cn

[N08] 生成全排列
来源：http://pbj.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://zhh.tian-w.cn

PHP:  // 手写递归交换
来源：http://bil.cdnleiting.top

JS:   // 手写回溯递归
来源：http://acz.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://duh.9152youxi.cn

Java: // 手写回溯递归
来源：http://qpk.hesvh.cn

Go:   // 手写回溯递归
来源：http://czv.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://uxk.yueranfly.top

C#:   // 手写回溯递归
来源：http://uvi.shangyingyoupin.top

[N09] 栈与队列
来源：http://vbm.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eyy.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wjy.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cur.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rel.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tzv.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gtf.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rep.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nco.bbcook.cn

[N10] 链表节点定义
来源：http://ifh.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hfy.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xre.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zko.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pbs.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://rfw.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hlz.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wfs.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dka.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://koq.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rzp.jinqigufen.top

PHP:  // 手写递归函数
来源：http://hpd.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fgu.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dax.hysaishi.cn

Java: // 手写递归
来源：http://rzi.snrcjt.cn

Go:   // 手写递归
来源：http://amx.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gfe.hnxiangtu.top

C#:   // 手写递归
来源：http://oqc.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dzo.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iws.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fnf.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hqg.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ycz.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oma.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kvr.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yac.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oyv.aizwys.cn

================================================================================
来源：http://zoc.yueranfly.top

O. 并发与异步
来源：http://nrl.pycfn.com

================================================================================
来源：http://rmr.guannengcc.top

[O01] 启动一个线程
来源：http://aqr.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gnv.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xkl.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tpo.daria6918.cn

TS:   // 同 JS
来源：http://dhv.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://vhl.yuanzhike.top

Go:   go f()
来源：http://uuy.iojbl.cn

Ruby: Thread.new { f }
来源：http://pkl.nwbrower.top

C#:   Task.Run(() => F());
来源：http://lyt.pycfn.com

[O02] 使用线程池
来源：http://txj.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hla.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bxx.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://bkd.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://njm.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pfj.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hvi.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aqw.yj20258888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ogx.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://rge.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://ekw.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fpb.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pzb.mhx1999.top

TS:   // 同 JS
来源：http://wya.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://ayr.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afi.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://syk.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://tih.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://dcm.havefunace.top

Py:   async def f():⏎    await g()
来源：http://xis.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jaf.yongpay.top

JS:   async function f() { await g(); }
来源：http://eie.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zfx.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eja.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://prv.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://zxa.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://rlt.cdnleiting.top

[O05] 并发执行并等待全部完成
来源：http://irm.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://vhx.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://auv.ivvv.top

JS:   await Promise.all(tasks)
来源：http://vhj.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://itn.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pqq.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dve.ywan-chungtsiang.top

Ruby: threads.map(&:join)
来源：http://nyk.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yyu.jianghu66.top

[O06] 使用进程池
来源：http://clu.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qbo.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bbl.meibo888.top

JS:   // child_process / cluster 模块
来源：http://mga.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://sxa.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pxz.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rkx.birdmap.top

Ruby: // fork 块
来源：http://wdb.yvedp.cn

C#:   Parallel.For
来源：http://dia.birdmap.top

================================================================================
来源：http://nrv.pycfn.com

P. 常用工具函数
来源：http://swm.52xcode.cn

================================================================================
来源：http://ggc.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://skh.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://hra.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ezx.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://uzm.ydzc1.top

TS:   crypto.randomUUID()
来源：http://amt.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://xeb.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://icj.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://cam.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://mkx.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://mtl.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ulh.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rdw.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xrg.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://btz.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zjp.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rnx.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vmk.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cqh.tanke756.top

[P03] 生成短随机字符串
来源：http://zlh.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lwe.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hmk.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zkq.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hko.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lzp.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mni.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sia.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qxl.aizwys.cn

[P04] 求长度
来源：http://iwj.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hfy.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qxi.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgp.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qps.haohaochexian.top


<!-- 参考信息 -->