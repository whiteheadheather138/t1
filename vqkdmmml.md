代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ggn.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ayh.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://ocn.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jri.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://kei.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ywa.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dlo.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://znn.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://jqq.yj202588.top

Java: resp.statusCode()
来源：http://cif.cqqwz.cn

Go:   resp.StatusCode
来源：http://tlf.xziqi.cn

Ruby: resp.code.to_i
来源：http://ive.yj202588.top

C#:   (int)resp.StatusCode
来源：http://uwd.sufxvd.cn

[L08] 并发请求多个地址
来源：http://qwr.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kvs.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://ory.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://evf.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qck.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://znw.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bxn.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lew.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rxz.sweek.top

================================================================================
来源：http://ukf.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://qqv.jinqigfzy.top

================================================================================
来源：http://vqo.daxiang520.top

[M01] 读取命令行参数
来源：http://uzw.zhengqikj.top

Py:   sys.argv[1:]
来源：http://ido.fzhhl.top

PHP:  $argv;  $argc;
来源：http://nry.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://urq.yfazqb.com

TS:   process.argv.slice(2)
来源：http://zju.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://ysx.cashguo.top

Go:   os.Args[1:]
来源：http://gko.birdmap.top

Ruby: ARGV
来源：http://elk.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://yay.ppjwa.cn

[M02] 读取环境变量
来源：http://eil.yongpay.top

Py:   os.environ.get("HOME")
来源：http://tae.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfb.c1oappe.top

JS:   process.env.HOME
来源：http://wdh.hammf.cn

TS:   process.env.HOME
来源：http://jxv.iojbl.cn

Java: System.getenv("HOME")
来源：http://hal.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://evn.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://rnv.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cew.haohaochexian.top

[M03] 执行外部命令
来源：http://oqq.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sjm.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ewv.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qqh.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://djw.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wmy.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tfo.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lrv.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://dle.pycfn.com

[M04] 获取当前工作目录
来源：http://vhv.zhixingplan.top

Py:   os.getcwd()
来源：http://ema.uphjek.com

PHP:  getcwd();
来源：http://bpg.tarul.cn

JS:   process.cwd()
来源：http://jlc.ybcxt.top

TS:   process.cwd()
来源：http://die.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://qlz.shuidangran.top

Go:   os.Getwd()
来源：http://rfa.jqgfzy.top

Ruby: Dir.pwd
来源：http://idn.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mgn.52xcode.cn

[M05] 设置退出码
来源：http://sxl.mhx1999.top

Py:   sys.exit(1)
来源：http://oqk.0kj1m.cn

PHP:  exit(1);
来源：http://eth.hnxiangtu.top

JS:   process.exit(1)
来源：http://rry.dashuyun.cn

TS:   process.exit(1)
来源：http://huu.aibaodan.cn

Java: System.exit(1)
来源：http://jno.jianghu66.top

Go:   os.Exit(1)
来源：http://fem.daria6918.cn

Ruby: exit 1
来源：http://mrx.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ysm.hfpthk.cn

[M06] 向标准错误输出
来源：http://kfx.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://kwv.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://woj.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://hwk.cashguo.top

TS:   console.error("err")
来源：http://cov.sjlbkw.cn

Java: System.err.println("err")
来源：http://kpj.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mrt.zhixingplan.top

Ruby: warn "err"
来源：http://udc.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://oxb.yuanzhike.top

[M07] 判断是否为主入口
来源：http://sps.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://vsy.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zil.jqgfzy.top

JS:   require.main === module
来源：http://mme.zhixingplan.top

TS:   require.main === module
来源：http://krx.dashuyun.cn

Java: public static void main(String[] args)
来源：http://zoc.smart0.xyz

Go:   func main()
来源：http://vfe.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iqb.hammf.cn

C#:   static void Main(string[] args)
来源：http://hwa.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://coy.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://xsl.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://xpy.hcnkem.com

JS:   process.platform;  process.version
来源：http://zue.shuidangran.top

TS:   process.platform;  process.version
来源：http://ynw.haohaochexian.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rus.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gfl.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vtf.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iaz.jiagoushi.top

================================================================================
来源：http://epb.yuanzhike.top

N. 数据结构与算法
来源：http://wvm.pengpengdd.cyou

================================================================================
来源：http://qmo.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://rzy.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://hip.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fnc.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://atj.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lcx.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://leu.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://rgd.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lin.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://jnm.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://plr.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://gqo.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gdh.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wyc.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://avw.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ygp.cucudq.cn

Go:   slices.Sort(arr)
来源：http://sau.gotoacloud.top

Ruby: arr.sort
来源：http://ljj.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eca.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://csx.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kqp.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://zhg.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dpx.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://neo.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://drz.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://acw.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vmh.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://owz.pycfn.com

[N04] 斐波那契数列
来源：http://rei.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dpm.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sma.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dhm.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npp.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rkc.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gxm.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mdq.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vol.epnwcf.com

[N05] 最大公约数
来源：http://acg.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://fsp.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jlh.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vov.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qlh.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qou.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wqf.zhengqikj.top

Ruby: a.gcd(b)
来源：http://mfr.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://llg.gaohongyu789.top

[N06] 判断回文字符串
来源：http://nih.cqqwz.cn

Py:   s == s[::-1]
来源：http://dnj.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://hmu.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://cvq.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://trr.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gpa.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://zhd.sufxvd.cn

Ruby: s == s.reverse
来源：http://uzp.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rtc.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://jkp.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gdy.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pul.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://gti.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://fay.hysaishi.cn

Java: // 手写 HashMap
来源：http://mio.daria6918.cn

Go:   // 手写 map[int]int
来源：http://aty.bjfxy.top

Ruby: // 手写 Hash
来源：http://xqu.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://vdt.52xcode.cn

[N08] 生成全排列
来源：http://nlp.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://ehj.yongpay.top

PHP:  // 手写递归交换
来源：http://pce.yangfankeji.com

JS:   // 手写回溯递归
来源：http://seh.dashuyun.cn

TS:   // 手写回溯递归
来源：http://wjx.sweek.top

Java: // 手写回溯递归
来源：http://xzf.hnqzz.top

Go:   // 手写回溯递归
来源：http://drd.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://baw.bbcook.cn

C#:   // 手写回溯递归
来源：http://sig.zhengqikj.top

[N09] 栈与队列
来源：http://umr.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://djr.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://msb.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rrp.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghw.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vxb.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tkj.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://etp.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jak.uphjek.com

[N10] 链表节点定义
来源：http://urd.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xpp.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zuw.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjq.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kfm.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://jxv.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://sbo.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hyb.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://miu.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://vhc.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://frc.yongpay.top

PHP:  // 手写递归函数
来源：http://gtz.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvc.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bvv.jiagoushi.top

Java: // 手写递归
来源：http://vgp.hongshengwenyu.top

Go:   // 手写递归
来源：http://sry.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mdz.birdmap.top

C#:   // 手写递归
来源：http://fgq.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jkv.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rms.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uzw.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jde.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jly.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rpt.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fsh.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mrd.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tuc.andypj.xyz

================================================================================
来源：http://owa.yuanzhike.top

O. 并发与异步
来源：http://fsd.shzxlz.cn

================================================================================
来源：http://axi.ivvv.top

[O01] 启动一个线程
来源：http://jfv.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sws.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://swp.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jjz.yj202588.top

TS:   // 同 JS
来源：http://dld.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://ztq.52xcode.cn

Go:   go f()
来源：http://vzu.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://mzg.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://eth.vehdjk.com

[O02] 使用线程池
来源：http://hmh.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://buu.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bzr.xinyue.icu

JS:   // worker_threads 线程池
来源：http://kcz.yj202588.top

TS:   // worker_threads 线程池
来源：http://nzi.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ris.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fln.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zii.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bet.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://dhv.daxiang520.top

Py:   with lock: shared += 1
来源：http://qvu.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://njk.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iii.meibo888.top

TS:   // 同 JS
来源：http://rml.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://kba.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oxj.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dfz.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://trj.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://jjs.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://eit.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slt.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://kys.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ref.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eqh.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zay.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://dte.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://esw.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://hdb.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://pii.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://igv.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://jwp.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://bmk.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wmi.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bca.xylfe.cn

Ruby: threads.map(&:join)
来源：http://dhi.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mcw.birdmap.top

[O06] 使用进程池
来源：http://sct.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qja.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ufj.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://tbh.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://mcm.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wjn.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qsl.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://chg.wangdashe.top

C#:   Parallel.For
来源：http://qai.aibaodan.cn

================================================================================
来源：http://yph.hesvh.cn

P. 常用工具函数
来源：http://ceu.yvedp.cn

================================================================================
来源：http://dis.smart0.xyz

[P01] 生成 UUID
来源：http://ngj.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://fvz.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://prr.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://rtf.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://gap.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://xvq.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://zgq.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://umg.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://kjp.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://jge.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ppc.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://acn.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://svi.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tih.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rar.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xss.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mff.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwv.zdqjudy.top

[P03] 生成短随机字符串
来源：http://jer.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kbb.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tzt.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dkl.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gph.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qop.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sqg.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sfu.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://joo.dianchejie.cn

[P04] 求长度
来源：http://zdc.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://scl.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bcy.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvc.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cpf.aizwys.cn


<!-- 参考信息 -->