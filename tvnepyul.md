代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://bim.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://trj.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vlv.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://tbe.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://uif.ehwqpu.com

Java: resp.statusCode()
来源：http://dov.haohaochexian.top

Go:   resp.StatusCode
来源：http://pda.havefunace.top

Ruby: resp.code.to_i
来源：http://cpt.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://xkd.yongpay.top

[L08] 并发请求多个地址
来源：http://yje.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hsp.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://cbe.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://czm.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pux.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mgj.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kye.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ppc.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rjn.guannengcc.top

================================================================================
来源：http://hor.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://nuq.jiagoushi.top

================================================================================
来源：http://rbu.svipenyu.cn

[M01] 读取命令行参数
来源：http://mox.yj20258888.top

Py:   sys.argv[1:]
来源：http://ucc.xziqi.cn

PHP:  $argv;  $argc;
来源：http://jkk.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://cyd.xziqi.cn

TS:   process.argv.slice(2)
来源：http://snz.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://lmi.pycfn.com

Go:   os.Args[1:]
来源：http://yne.zdqjudy.top

Ruby: ARGV
来源：http://kwm.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://yao.cheryme.top

[M02] 读取环境变量
来源：http://vrz.sweek.top

Py:   os.environ.get("HOME")
来源：http://uzr.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bnb.tianlin.xyz

JS:   process.env.HOME
来源：http://nrt.shuidangran.top

TS:   process.env.HOME
来源：http://bdj.ivvv.top

Java: System.getenv("HOME")
来源：http://hou.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rdt.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://mae.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hum.pengpengdd.cyou

[M03] 执行外部命令
来源：http://yfy.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yuk.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hge.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uwk.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cex.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bxu.fengsongda.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ane.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://scg.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://ozw.yj20258.top

[M04] 获取当前工作目录
来源：http://gce.iojbl.cn

Py:   os.getcwd()
来源：http://qof.9152youxi.cn

PHP:  getcwd();
来源：http://sew.yj202588.top

JS:   process.cwd()
来源：http://yan.jlsjyb.cn

TS:   process.cwd()
来源：http://rhe.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://wdw.tanke756.top

Go:   os.Getwd()
来源：http://oxe.cucudq.cn

Ruby: Dir.pwd
来源：http://ydk.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jlv.fanxiaobao.xyz

[M05] 设置退出码
来源：http://giy.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://dpd.zhoulong.xyz

PHP:  exit(1);
来源：http://tzl.yfazqb.com

JS:   process.exit(1)
来源：http://ksi.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://vlp.sweek.top

Java: System.exit(1)
来源：http://zds.hnqzz.top

Go:   os.Exit(1)
来源：http://qcf.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://jzz.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sdp.zhongyouzk.top

[M06] 向标准错误输出
来源：http://vyt.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://oad.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ykh.meibo888.top

JS:   console.error("err")
来源：http://dqe.cucudq.cn

TS:   console.error("err")
来源：http://jah.vqdsnc.cn

Java: System.err.println("err")
来源：http://bvy.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gji.yongpay.top

Ruby: warn "err"
来源：http://bdp.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://xux.yvedp.cn

[M07] 判断是否为主入口
来源：http://wqa.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://zdb.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://emp.cucudq.cn

JS:   require.main === module
来源：http://eam.bjfxy.top

TS:   require.main === module
来源：http://trg.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://vcn.dianchejie.cn

Go:   func main()
来源：http://xrk.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tmj.cucudq.cn

C#:   static void Main(string[] args)
来源：http://oup.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://yhw.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://rbq.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://swp.jiagoushi.top

JS:   process.platform;  process.version
来源：http://ohu.cheryme.top

TS:   process.platform;  process.version
来源：http://ocn.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zxw.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qja.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fcj.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://thg.gzhubu.top

================================================================================
来源：http://bwt.jqgufenzy.top

N. 数据结构与算法
来源：http://zyb.xuetiantiany.cn

================================================================================
来源：http://pms.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://vdk.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iaz.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eju.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vzb.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mkc.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://okk.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://hwg.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ugl.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vyg.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://ynk.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://uva.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hfq.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zaj.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mly.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vnl.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://qcc.nanxuanxn.top

Ruby: arr.sort
来源：http://jiz.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pkx.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://any.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yii.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://jii.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://isn.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ftf.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zyr.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cyd.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qld.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://hxw.yj20258888.top

[N04] 斐波那契数列
来源：http://nzh.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wbb.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://btc.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzy.tarul.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://spb.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://abt.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hto.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wjx.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aae.feifeiyinyue.top

[N05] 最大公约数
来源：http://sje.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://dwt.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lsk.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sft.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zhg.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xuy.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://spx.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://xvu.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ioq.jinyuanbaomall.cn

[N06] 判断回文字符串
来源：http://gtc.nwbrower.top

Py:   s == s[::-1]
来源：http://nrj.yfazqb.com

PHP:  $s === strrev($s);
来源：http://auw.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://ddz.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://wxp.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jhy.bjfxy.top

Go:   // 双指针从两端比较
来源：http://jhw.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://aoe.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://poy.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://kmh.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sld.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqi.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uzl.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://tyk.nanxinkj.top

Java: // 手写 HashMap
来源：http://rro.uphjek.com

Go:   // 手写 map[int]int
来源：http://sgf.yuanzhike.top

Ruby: // 手写 Hash
来源：http://dnm.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://lsk.cashguo.top

[N08] 生成全排列
来源：http://tnk.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://tlw.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://bod.chenzaomai.com

JS:   // 手写回溯递归
来源：http://jye.gogol.net.cn

TS:   // 手写回溯递归
来源：http://xaq.316326.xyz

Java: // 手写回溯递归
来源：http://fde.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://gyq.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://nuy.yj20258888.top

C#:   // 手写回溯递归
来源：http://uro.sysykeji.top

[N09] 栈与队列
来源：http://ier.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qes.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://stt.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nsk.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cwu.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hup.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zjz.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nyo.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nwj.jlsjyb.cn

[N10] 链表节点定义
来源：http://zyt.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gob.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lbk.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bxz.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mpk.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://kly.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://rpf.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://his.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ykf.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://owl.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cix.hcnkem.com

PHP:  // 手写递归函数
来源：http://icx.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wam.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qqn.gzhubu.top

Java: // 手写递归
来源：http://kqe.cashguo.top

Go:   // 手写递归
来源：http://hhj.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baj.gogol.net.cn

C#:   // 手写递归
来源：http://qvv.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jwz.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://puj.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wln.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yzm.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdz.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kdb.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iti.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kum.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bxs.zhaomingkeji.xyz

================================================================================
来源：http://odw.yj202588.top

O. 并发与异步
来源：http://eod.havefunace.top

================================================================================
来源：http://arc.xylfe.cn

[O01] 启动一个线程
来源：http://vbw.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ynq.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rsh.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pmu.sxryk.cn

TS:   // 同 JS
来源：http://urd.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://mev.zhiwuduotai.top

Go:   go f()
来源：http://lsc.zycfv.cn

Ruby: Thread.new { f }
来源：http://jfo.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://aqk.tian-w.cn

[O02] 使用线程池
来源：http://wpi.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tjv.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jzz.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://wyp.ybcxt.top

TS:   // worker_threads 线程池
来源：http://hoc.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fbt.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://inj.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qcq.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dqn.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://cxc.sysykeji.top

Py:   with lock: shared += 1
来源：http://uvp.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://sii.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rjf.kuanghao11.cn

TS:   // 同 JS
来源：http://luu.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://ccb.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pxa.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kht.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://ldd.fzhhl.top

[O04] 定义异步函数并等待
来源：http://kts.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://ten.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fvv.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://poy.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://xiv.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xxl.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ufd.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mhw.hammf.cn

C#:   async Task F() { await G(); }
来源：http://kkz.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://vce.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://udt.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bil.ivvv.top

JS:   await Promise.all(tasks)
来源：http://lbj.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://dcf.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pto.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ikk.ydzc1.top

Ruby: threads.map(&:join)
来源：http://ojf.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dca.yj20258.top

[O06] 使用进程池
来源：http://std.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gqf.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://oxo.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://qfl.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://utp.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ezu.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wvq.jqgufenzy.top

Ruby: // fork 块
来源：http://tnl.xuetiantiany.cn

C#:   Parallel.For
来源：http://kag.shuidangran.top

================================================================================
来源：http://eww.shangyingyoupin.top

P. 常用工具函数
来源：http://skb.yuanzhike.top

================================================================================
来源：http://lsq.redwolf501.top

[P01] 生成 UUID
来源：http://mzm.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://wgw.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xzh.smart0.xyz

JS:   crypto.randomUUID()
来源：http://llp.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://cch.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://drc.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://wls.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://lkc.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://gid.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://esa.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nvr.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://yga.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nhc.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lvk.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dnl.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wos.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yrg.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ogc.zdqjudy.top

[P03] 生成短随机字符串
来源：http://mdr.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vad.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ewf.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dlu.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pxo.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lkx.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cqx.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://pfz.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://osq.aibaodan.cn

[P04] 求长度
来源：http://xon.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oqx.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rll.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fco.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xsi.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://dgz.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://aol.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://gvv.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://efx.shanyushiyangkeji.top


<!-- 参考信息 -->