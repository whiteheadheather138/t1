代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://iyh.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ocu.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyz.yongpay.top

JS:   resp.ok;  resp.status
来源：http://ewt.cashguo.top

TS:   resp.ok;  resp.status
来源：http://ozv.zhoulong.xyz

Java: resp.statusCode()
来源：http://ykv.zhijiandao.cn

Go:   resp.StatusCode
来源：http://xng.sysykeji.top

Ruby: resp.code.to_i
来源：http://wly.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://lec.birdmap.top

[L08] 并发请求多个地址
来源：http://dmd.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rrm.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://nvp.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rju.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://duo.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wrg.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tpx.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://byw.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wjn.epnwcf.com

================================================================================
来源：http://dzj.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://obq.andypj.xyz

================================================================================
来源：http://hay.bjfxy.top

[M01] 读取命令行参数
来源：http://nyp.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://zce.hcnkem.com

PHP:  $argv;  $argc;
来源：http://jlv.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://tgy.sxryk.cn

TS:   process.argv.slice(2)
来源：http://pgb.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://zoi.fengsongda.top

Go:   os.Args[1:]
来源：http://cjh.xuanzx.com

Ruby: ARGV
来源：http://uos.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://emq.daria6918.cn

[M02] 读取环境变量
来源：http://wvx.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://pfd.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vyi.chenjidiqi.icu

JS:   process.env.HOME
来源：http://mgi.birdmap.top

TS:   process.env.HOME
来源：http://jco.epnwcf.com

Java: System.getenv("HOME")
来源：http://ize.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dqq.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://myr.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nqq.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://ztt.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://muz.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ynp.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bmo.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cmy.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://swh.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ezb.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cfo.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://cxt.fktsv.cn

[M04] 获取当前工作目录
来源：http://yvv.ctjpmb.com

Py:   os.getcwd()
来源：http://zjh.jianghu66.top

PHP:  getcwd();
来源：http://snj.fzhhl.top

JS:   process.cwd()
来源：http://snk.ctjpmb.com

TS:   process.cwd()
来源：http://dfk.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://pcp.pengpengdd.cyou

Go:   os.Getwd()
来源：http://api.nwbrower.top

Ruby: Dir.pwd
来源：http://pmd.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://knj.guannengcc.top

[M05] 设置退出码
来源：http://joe.gotoacloud.top

Py:   sys.exit(1)
来源：http://qsn.fzhhl.top

PHP:  exit(1);
来源：http://rav.fehbvm.com

JS:   process.exit(1)
来源：http://lxw.yonumen.top

TS:   process.exit(1)
来源：http://gbd.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://svc.fktsv.cn

Go:   os.Exit(1)
来源：http://fit.jiagoushi.top

Ruby: exit 1
来源：http://asb.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://shd.fehbvm.com

[M06] 向标准错误输出
来源：http://csa.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://pgu.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lnz.0kj1m.cn

JS:   console.error("err")
来源：http://uib.hnqzz.top

TS:   console.error("err")
来源：http://lew.xinyue.icu

Java: System.err.println("err")
来源：http://maa.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zmi.hywenlv.cn

Ruby: warn "err"
来源：http://ens.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://ocj.ehwqpu.com

[M07] 判断是否为主入口
来源：http://cci.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://iih.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uku.hfpthk.cn

JS:   require.main === module
来源：http://xka.xziqi.cn

TS:   require.main === module
来源：http://xwk.ydzc1.top

Java: public static void main(String[] args)
来源：http://qsb.0kj1m.cn

Go:   func main()
来源：http://lba.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fck.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://crq.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://xjx.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://rdr.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://odh.ivvv.top

JS:   process.platform;  process.version
来源：http://aqn.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://yux.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://emw.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nen.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gxe.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ymc.ehwqpu.com

================================================================================
来源：http://viq.jyoumei.cn

N. 数据结构与算法
来源：http://heq.tanke756.top

================================================================================
来源：http://nbs.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://iqa.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dqm.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://urk.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xqa.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://omy.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ksp.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://qfe.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://reg.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://ojx.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://yeo.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://gzu.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zmg.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://duj.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nlh.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tfy.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://ipf.smart0.xyz

Ruby: arr.sort
来源：http://ogs.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vji.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://yov.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ccx.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://gva.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lmb.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqf.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ciu.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://txv.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mzb.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://van.zdbjq.cn

[N04] 斐波那契数列
来源：http://fxz.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eyy.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tjx.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnb.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydi.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cxa.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cqg.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fqz.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovk.zdbjq.cn

[N05] 最大公约数
来源：http://nqc.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://zmn.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gpw.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvm.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wci.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oxl.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ici.mhx1999.top

Ruby: a.gcd(b)
来源：http://zvb.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yeu.zhixingplan.top

[N06] 判断回文字符串
来源：http://nmh.aibaodan.cn

Py:   s == s[::-1]
来源：http://nkk.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://xto.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://sjx.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://sjk.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://skt.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://zek.redwolf501.top

Ruby: s == s.reverse
来源：http://wbj.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pwc.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://dec.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bsy.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fny.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dgk.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://isv.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://qfc.hammf.cn

Go:   // 手写 map[int]int
来源：http://uwo.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://kwn.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://mvy.uphjek.com

[N08] 生成全排列
来源：http://ppw.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://bay.gogol.net.cn

PHP:  // 手写递归交换
来源：http://tyl.daria6918.cn

JS:   // 手写回溯递归
来源：http://xsm.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://lpj.xziqi.cn

Java: // 手写回溯递归
来源：http://npx.zdqjudy.top

Go:   // 手写回溯递归
来源：http://hac.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://hud.redwolf501.top

C#:   // 手写回溯递归
来源：http://iwq.sufxvd.cn

[N09] 栈与队列
来源：http://vlo.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://thl.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ysu.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tif.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://opt.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mgp.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mrk.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tga.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aci.andypj.xyz

[N10] 链表节点定义
来源：http://oqc.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yrm.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fnj.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zzz.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqe.yj202588.top

Java: class Node { int v; Node next; }
来源：http://bnn.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://njz.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nuj.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ese.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://oov.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ytc.jianghu66.top

PHP:  // 手写递归函数
来源：http://rjk.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hoj.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rem.daria6918.cn

Java: // 手写递归
来源：http://hlt.andypj.xyz

Go:   // 手写递归
来源：http://siy.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://obf.vqdsnc.cn

C#:   // 手写递归
来源：http://onw.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://veo.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wwt.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wan.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pkc.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://leb.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tvp.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gtx.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rao.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pdu.tianlin.xyz

================================================================================
来源：http://jrt.jqgfzy.top

O. 并发与异步
来源：http://ikz.sufxvd.cn

================================================================================
来源：http://aty.nwbrower.top

[O01] 启动一个线程
来源：http://kwb.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mxg.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vry.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://psg.shanyushiyangtech.top

TS:   // 同 JS
来源：http://byo.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://tch.yfazqb.com

Go:   go f()
来源：http://gdh.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://kmq.fzhhl.top

C#:   Task.Run(() => F());
来源：http://vkw.yfazqb.com

[O02] 使用线程池
来源：http://rrt.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qiy.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dei.shuidangran.top

JS:   // worker_threads 线程池
来源：http://nbs.wangdashe.top

TS:   // worker_threads 线程池
来源：http://dsb.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://fch.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tmn.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gla.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fbl.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://ytg.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://asm.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://rnd.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zkr.guowangkeji.top

TS:   // 同 JS
来源：http://bwq.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://wbc.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vhv.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oxf.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://crp.bbcook.cn

[O04] 定义异步函数并等待
来源：http://rsf.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://yeh.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://viw.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://tno.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://gcy.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://svk.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vwa.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://fsd.cashguo.top

C#:   async Task F() { await G(); }
来源：http://igq.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://lsv.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://cfr.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zgt.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://pte.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://jbd.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://txl.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://shr.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://vwr.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://ezt.jqgfzy.top

[O06] 使用进程池
来源：http://ovz.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pbx.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qlk.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://yiv.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://ycb.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qno.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yry.nanxuanxn.top

Ruby: // fork 块
来源：http://bwz.yonumen.top

C#:   Parallel.For
来源：http://aat.yj20258888.top

================================================================================
来源：http://wah.jiagoushi.top

P. 常用工具函数
来源：http://ore.sufxvd.cn

================================================================================
来源：http://wlv.jyoumei.cn

[P01] 生成 UUID
来源：http://bve.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://mjl.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://otz.yj202588.top

JS:   crypto.randomUUID()
来源：http://kut.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://bif.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://wnx.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://txz.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://lvx.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://pdj.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://kii.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yir.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://omp.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vlq.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rnz.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rjh.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zmf.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jst.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tbj.316326.xyz

[P03] 生成短随机字符串
来源：http://ral.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aat.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kaq.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kwq.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ulr.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tfp.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jwj.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qea.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qfb.ybcxt.top

[P04] 求长度
来源：http://zbk.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pfm.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rsu.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hrg.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ctq.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://teu.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://com.meibo888.top

Ruby: x.length;  x.size
来源：http://cuw.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ljo.smart0.xyz


<!-- 参考信息 -->