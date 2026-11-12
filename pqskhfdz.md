代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cnj.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvl.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://unq.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vqi.zycfv.cn

[L07] 处理 HTTP 状态码
来源：http://eqd.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bkq.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxa.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://emf.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://zqj.svipenyu.cn

Java: resp.statusCode()
来源：http://ppe.xylfe.cn

Go:   resp.StatusCode
来源：http://tvk.meibo888.top

Ruby: resp.code.to_i
来源：http://uxk.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://uoq.mhx1999.top

[L08] 并发请求多个地址
来源：http://asw.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rhj.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://vzo.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://set.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://abb.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pqi.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://czu.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bsk.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pak.yanxiufei.cn

================================================================================
来源：http://blf.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://kij.fengsongda.top

================================================================================
来源：http://bwu.bjfxy.top

[M01] 读取命令行参数
来源：http://cbi.fktsv.cn

Py:   sys.argv[1:]
来源：http://xqy.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://wty.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://tgi.yonumen.top

TS:   process.argv.slice(2)
来源：http://xvp.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://tqd.tarul.cn

Go:   os.Args[1:]
来源：http://qlb.sufxvd.cn

Ruby: ARGV
来源：http://zdg.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://lwn.tian-w.cn

[M02] 读取环境变量
来源：http://bka.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://lld.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hsh.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://fyg.chenlongwang.top

TS:   process.env.HOME
来源：http://mdn.yuanzhike.top

Java: System.getenv("HOME")
来源：http://jpg.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pve.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://gdi.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://amk.fengsongda.top

[M03] 执行外部命令
来源：http://ekf.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://stt.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ijb.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://muz.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tiw.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qqu.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://btl.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://wpu.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://tjm.ehwqpu.com

[M04] 获取当前工作目录
来源：http://ped.hongshengwenyu.top

Py:   os.getcwd()
来源：http://iji.tianlin.xyz

PHP:  getcwd();
来源：http://kpq.nanxinkj.top

JS:   process.cwd()
来源：http://hhp.cqqwz.cn

TS:   process.cwd()
来源：http://eok.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://rqx.svipenyu.cn

Go:   os.Getwd()
来源：http://dzn.yonumen.top

Ruby: Dir.pwd
来源：http://cry.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://nvj.yj202588.top

[M05] 设置退出码
来源：http://ffw.tianlin.xyz

Py:   sys.exit(1)
来源：http://nrg.9152youxi.cn

PHP:  exit(1);
来源：http://xsw.zhoulong.xyz

JS:   process.exit(1)
来源：http://tiw.smart0.xyz

TS:   process.exit(1)
来源：http://kxq.jiagoushi.top

Java: System.exit(1)
来源：http://obr.havefunace.top

Go:   os.Exit(1)
来源：http://myd.c1oappe.top

Ruby: exit 1
来源：http://fua.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://srq.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://ukn.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://dmx.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qlc.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://ylb.hfpthk.cn

TS:   console.error("err")
来源：http://brz.pengpengdd.cyou

Java: System.err.println("err")
来源：http://vys.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gax.yangfankeji.com

Ruby: warn "err"
来源：http://uos.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://sgs.cdnleiting.top

[M07] 判断是否为主入口
来源：http://mwd.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://zzx.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vaq.cheryme.top

JS:   require.main === module
来源：http://rnk.chenlongwang.top

TS:   require.main === module
来源：http://vhq.ehwqpu.com

Java: public static void main(String[] args)
来源：http://kay.xziqi.cn

Go:   func main()
来源：http://qvb.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ume.hesvh.cn

C#:   static void Main(string[] args)
来源：http://sgn.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://vpt.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://ixl.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://frf.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://wyh.bjfxy.top

TS:   process.platform;  process.version
来源：http://jdc.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kas.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://oxv.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bje.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://pgv.zhengqikj.top

================================================================================
来源：http://kev.ydzc1.top

N. 数据结构与算法
来源：http://cza.ydzc1.top

================================================================================
来源：http://fcc.yj202588.top

[N01] 二分查找（有序数组）
来源：http://rnh.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://jap.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nia.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lof.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcz.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://vdz.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://ahf.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hly.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://yxy.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://drv.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://hev.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eda.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xce.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://icb.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lqc.yueranfly.top

Go:   slices.Sort(arr)
来源：http://jhp.jinghuilouyu.cn

Ruby: arr.sort
来源：http://qxn.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tub.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://olr.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://azk.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://ant.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vyx.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pyn.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tai.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://udl.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ljv.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://ifz.jinqigfzy.top

[N04] 斐波那契数列
来源：http://zee.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vun.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jat.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kgi.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfg.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mdt.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vvb.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ugo.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lwl.yonumen.top

[N05] 最大公约数
来源：http://jly.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://sui.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://urd.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iji.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugw.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ywf.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hja.cdnleiting.top

Ruby: a.gcd(b)
来源：http://etv.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cuv.sweek.top

[N06] 判断回文字符串
来源：http://ret.hnqzz.top

Py:   s == s[::-1]
来源：http://ehu.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://myv.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://rsi.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://tsw.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pdt.tarul.cn

Go:   // 双指针从两端比较
来源：http://ggk.hnqzz.top

Ruby: s == s.reverse
来源：http://ymq.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sul.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://mmc.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hqq.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zmy.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cdo.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://lyg.aizwys.cn

Java: // 手写 HashMap
来源：http://vpl.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://lha.sweek.top

Ruby: // 手写 Hash
来源：http://qaz.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://yyf.haohaochexian.top

[N08] 生成全排列
来源：http://jor.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://ojr.chenlongwang.top

PHP:  // 手写递归交换
来源：http://aev.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://nrs.zhixingplan.top

TS:   // 手写回溯递归
来源：http://ovp.gotoacloud.top

Java: // 手写回溯递归
来源：http://yru.fktsv.cn

Go:   // 手写回溯递归
来源：http://vff.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://lrw.fengsongda.top

C#:   // 手写回溯递归
来源：http://brg.9152youxi.cn

[N09] 栈与队列
来源：http://ivs.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hgg.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vku.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lci.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uhb.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gjd.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://czr.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uiq.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lil.gogol.net.cn

[N10] 链表节点定义
来源：http://agw.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xvf.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uqp.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pra.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mba.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://rsu.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://auj.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wnr.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://aeb.bbcook.cn

[N11] 二叉树中序遍历
来源：http://zzo.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://axi.havefunace.top

PHP:  // 手写递归函数
来源：http://wti.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgd.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qkc.ctjpmb.com

Java: // 手写递归
来源：http://wco.9152youxi.cn

Go:   // 手写递归
来源：http://osp.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://goz.jianghu66.top

C#:   // 手写递归
来源：http://oqj.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wjs.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mdm.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://abb.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ksy.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pvn.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hsz.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zpb.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zxd.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bzw.sysykeji.top

================================================================================
来源：http://gje.yj20258888.top

O. 并发与异步
来源：http://dtj.zhaomingkeji.xyz

================================================================================
来源：http://gxl.yj202588.top

[O01] 启动一个线程
来源：http://cim.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ncq.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uad.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uxl.ivvv.top

TS:   // 同 JS
来源：http://hpq.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://zpx.shanyushiyangtech.top

Go:   go f()
来源：http://kwa.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://pbz.smart0.xyz

C#:   Task.Run(() => F());
来源：http://zdv.9152youxi.cn

[O02] 使用线程池
来源：http://fot.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://swh.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ybc.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://ned.yj20258.top

TS:   // worker_threads 线程池
来源：http://ijf.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://cji.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vim.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kpb.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kqh.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://weo.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://tor.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://ibt.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vic.redwolf501.top

TS:   // 同 JS
来源：http://ira.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://ilw.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aey.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ekh.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://qtm.yfazqb.com

[O04] 定义异步函数并等待
来源：http://aqq.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://hbg.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wnc.havefunace.top

JS:   async function f() { await g(); }
来源：http://zvo.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ndq.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xyw.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ogx.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://hsv.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://yns.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://nti.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://wzp.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://soe.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://upx.havefunace.top

TS:   await Promise.all(tasks)
来源：http://ogn.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xav.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ocs.xylfe.cn

Ruby: threads.map(&:join)
来源：http://dqc.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jol.fzhhl.top

[O06] 使用进程池
来源：http://rcc.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mmm.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hsm.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://yjt.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://qxz.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xgl.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qmy.chenjidiqi.icu

Ruby: // fork 块
来源：http://nwz.chenlongwang.top

C#:   Parallel.For
来源：http://jjg.wangdashe.top

================================================================================
来源：http://icn.zhengqikj.top

P. 常用工具函数
来源：http://eqy.gzhubu.top

================================================================================
来源：http://ucf.gotoacloud.top

[P01] 生成 UUID
来源：http://jvm.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://srk.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ods.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://fvn.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://urv.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://hpc.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://ppb.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://ffx.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://ovq.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://urk.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jes.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ppl.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nqm.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zuy.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gxn.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cnz.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ndl.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ovz.jianghu66.top

[P03] 生成短随机字符串
来源：http://uyb.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hhj.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kes.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svz.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kvn.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rnt.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dge.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lzk.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://isg.gotoacloud.top

[P04] 求长度
来源：http://bql.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ybw.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gvr.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yit.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://igq.ydjk.org.cn


<!-- 参考信息 -->