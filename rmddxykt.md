代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://zuo.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ghz.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gjz.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://yux.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://ica.hesvh.cn

Java: resp.statusCode()
来源：http://oaz.yongpay.top

Go:   resp.StatusCode
来源：http://jxu.haohaochexian.top

Ruby: resp.code.to_i
来源：http://sfw.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://qjq.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://oxu.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iai.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://nqk.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bap.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://buf.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qot.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qrz.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vuv.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ltg.zhaomingkeji.xyz

================================================================================
来源：http://blv.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://mag.tianlin.xyz

================================================================================
来源：http://oqx.andypj.xyz

[M01] 读取命令行参数
来源：http://upa.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://clw.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://jot.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://pvm.cucudq.cn

TS:   process.argv.slice(2)
来源：http://xfd.meibo888.top

Java: args 数组（main 方法参数）
来源：http://dul.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://bap.jlsjyb.cn

Ruby: ARGV
来源：http://xua.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://ygb.guowangkeji.top

[M02] 读取环境变量
来源：http://mhm.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://mxu.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nfi.daria6918.cn

JS:   process.env.HOME
来源：http://cee.shuidangran.top

TS:   process.env.HOME
来源：http://dwv.wangdashe.top

Java: System.getenv("HOME")
来源：http://tuu.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kiy.daxiang520.top

Ruby: ENV["HOME"]
来源：http://gvt.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qil.vehdjk.com

[M03] 执行外部命令
来源：http://ory.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zpw.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://irr.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jns.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mga.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://arj.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ugu.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aid.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://qrj.yueranfly.top

[M04] 获取当前工作目录
来源：http://eoh.ehwqpu.com

Py:   os.getcwd()
来源：http://gjk.yj20258.top

PHP:  getcwd();
来源：http://xwv.dashuyun.cn

JS:   process.cwd()
来源：http://xud.fengsongda.top

TS:   process.cwd()
来源：http://fyi.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://xax.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://bpc.hnxiangtu.top

Ruby: Dir.pwd
来源：http://iot.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://okb.yongpay.top

[M05] 设置退出码
来源：http://lfn.jinqigufen.top

Py:   sys.exit(1)
来源：http://noa.tian-w.cn

PHP:  exit(1);
来源：http://wvm.gaohongyu789.top

JS:   process.exit(1)
来源：http://hbl.hcnkem.com

TS:   process.exit(1)
来源：http://mxt.vehdjk.com

Java: System.exit(1)
来源：http://bwm.meibo888.top

Go:   os.Exit(1)
来源：http://ain.xziqi.cn

Ruby: exit 1
来源：http://pkb.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ulq.epnwcf.com

[M06] 向标准错误输出
来源：http://fkb.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://bih.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ecg.jianghu66.top

JS:   console.error("err")
来源：http://vkr.jiagoushi.top

TS:   console.error("err")
来源：http://uyz.cdnleiting.top

Java: System.err.println("err")
来源：http://xfo.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wes.tian-w.cn

Ruby: warn "err"
来源：http://iwl.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://npr.guowangkeji.top

[M07] 判断是否为主入口
来源：http://lgq.cashguo.top

Py:   if __name__ == "__main__":
来源：http://fnr.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbr.ydjk.org.cn

JS:   require.main === module
来源：http://osw.0kj1m.cn

TS:   require.main === module
来源：http://frr.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://gey.smart0.xyz

Go:   func main()
来源：http://lgp.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bcf.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://nss.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://bfs.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://ywu.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://huv.jyoumei.cn

JS:   process.platform;  process.version
来源：http://fhu.birdmap.top

TS:   process.platform;  process.version
来源：http://jis.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iqv.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vub.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kjv.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yjh.dashuyun.cn

================================================================================
来源：http://fmq.gzhubu.top

N. 数据结构与算法
来源：http://bpv.hysaishi.cn

================================================================================
来源：http://zuu.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://rku.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://ust.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://leb.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kgr.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fia.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://kgi.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://ysa.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://plj.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://wqr.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://ypf.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://lta.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xqy.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lqe.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bqy.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hrq.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://rek.haohaochexian.top

Ruby: arr.sort
来源：http://mfj.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bmx.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://qdd.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vjf.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://lcm.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cep.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjf.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fko.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mrb.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsv.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://agt.gzhubu.top

[N04] 斐波那契数列
来源：http://jss.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ang.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qmq.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qet.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvn.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eul.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wyt.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fbp.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lnw.uphjek.com

[N05] 最大公约数
来源：http://rpx.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://kec.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xlo.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ror.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kmc.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pld.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sae.ehwqpu.com

Ruby: a.gcd(b)
来源：http://jxz.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://syh.uphjek.com

[N06] 判断回文字符串
来源：http://vpj.yj20258888.top

Py:   s == s[::-1]
来源：http://lxi.fehbvm.com

PHP:  $s === strrev($s);
来源：http://oph.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://kfb.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://box.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ztr.cashguo.top

Go:   // 双指针从两端比较
来源：http://lxx.xinyue.icu

Ruby: s == s.reverse
来源：http://arr.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://iyw.tarul.cn

[N07] 两数之和（返回下标）
来源：http://own.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mnz.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sxs.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://cny.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://yqx.jinqigfzy.top

Java: // 手写 HashMap
来源：http://hwj.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://zyk.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://zlt.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hzk.zhoulong.xyz

[N08] 生成全排列
来源：http://zst.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://sdl.zhixingplan.top

PHP:  // 手写递归交换
来源：http://jtw.9152youxi.cn

JS:   // 手写回溯递归
来源：http://fzy.wangdashe.top

TS:   // 手写回溯递归
来源：http://bps.ydzc1.top

Java: // 手写回溯递归
来源：http://fkj.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://pps.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://drr.hfpthk.cn

C#:   // 手写回溯递归
来源：http://xcc.xuetiantiany.cn

[N09] 栈与队列
来源：http://yyg.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yjx.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hts.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wpv.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ywz.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ekk.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lhb.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wlu.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hmx.pycfn.com

[N10] 链表节点定义
来源：http://ulj.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gdv.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qer.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zcy.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gmr.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://fnh.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://sug.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gjt.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lgs.ybcxt.top

[N11] 二叉树中序遍历
来源：http://crm.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gwz.chenlongwang.top

PHP:  // 手写递归函数
来源：http://bfs.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iyc.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hpq.ehwqpu.com

Java: // 手写递归
来源：http://bar.jinqigufen.top

Go:   // 手写递归
来源：http://roz.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aoa.chenlongwang.top

C#:   // 手写递归
来源：http://aou.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oql.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nuj.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://egg.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ojw.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dmw.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dhf.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://and.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ruv.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://avc.svipenyu.cn

================================================================================
来源：http://wre.meibo888.top

O. 并发与异步
来源：http://cuv.zhiwuduotai.top

================================================================================
来源：http://zhe.yvedp.cn

[O01] 启动一个线程
来源：http://vud.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ivv.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://urs.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bhp.jiagoushi.top

TS:   // 同 JS
来源：http://goq.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://gfb.hnxiangtu.top

Go:   go f()
来源：http://xzk.tarul.cn

Ruby: Thread.new { f }
来源：http://fac.yj20258.top

C#:   Task.Run(() => F());
来源：http://vex.guowangkeji.top

[O02] 使用线程池
来源：http://jyk.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ysh.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tgn.daxiang520.top

JS:   // worker_threads 线程池
来源：http://tqg.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://xip.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wlc.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://shd.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tqf.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://til.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://uwj.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://uqw.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://kyd.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fbk.ydjk.org.cn

TS:   // 同 JS
来源：http://ikh.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://bok.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kqs.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qcd.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://mzn.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://oih.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://giu.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tdr.52xcode.cn

JS:   async function f() { await g(); }
来源：http://elj.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bbg.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ojq.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fby.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://ymy.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://rpt.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://siz.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://rep.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bbn.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://vqg.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://fsp.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dsy.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jhu.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://qyn.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ufd.sysykeji.top

[O06] 使用进程池
来源：http://rwm.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hir.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jzg.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://kcc.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://acb.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oro.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xmq.svipenyu.cn

Ruby: // fork 块
来源：http://zwi.tarul.cn

C#:   Parallel.For
来源：http://ysk.316326.xyz

================================================================================
来源：http://rvn.pengpengdd.cyou

P. 常用工具函数
来源：http://tjv.guannengcc.top

================================================================================
来源：http://zrx.zhixingplan.top

[P01] 生成 UUID
来源：http://rjf.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://yrd.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sjo.xinyue.icu

JS:   crypto.randomUUID()
来源：http://hsr.xylfe.cn

TS:   crypto.randomUUID()
来源：http://pmj.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://fyw.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://sez.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://yis.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://xky.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://dqy.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pwh.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjk.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://srm.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vts.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ayb.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oun.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ito.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qgd.ivvv.top

[P03] 生成短随机字符串
来源：http://svk.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://krv.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lbp.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fga.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gko.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bkh.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://abh.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://szk.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rjb.xuetiantiany.cn

[P04] 求长度
来源：http://tks.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://inh.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cve.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://way.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dcm.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://fvz.yonumen.top

Go:   len(arr);  len(m)
来源：http://btf.bbcook.cn

Ruby: x.length;  x.size
来源：http://ywf.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uji.sysykeji.top


<!-- 参考信息 -->