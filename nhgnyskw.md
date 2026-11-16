代发 wailian999

Py:   resp.json()
来源：http://why.havefunace.top

PHP:  json_decode($body, true);
来源：http://qim.kuanghao11.cn

JS:   await resp.json()
来源：http://hza.zhoulong.xyz

TS:   await resp.json()
来源：http://kuw.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eug.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://crd.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://qzl.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lcc.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://gtb.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fkl.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ocu.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://bts.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://gjf.hnqzz.top

Java: resp.statusCode()
来源：http://pgy.xylfe.cn

Go:   resp.StatusCode
来源：http://may.yuanzhike.top

Ruby: resp.code.to_i
来源：http://sgk.hammf.cn

C#:   (int)resp.StatusCode
来源：http://bel.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://pvj.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hcs.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://uum.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwf.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xhr.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lll.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gfv.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nii.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nju.pycfn.com

================================================================================
来源：http://zfr.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://giv.jlsjyb.cn

================================================================================
来源：http://uan.jqgfzy.top

[M01] 读取命令行参数
来源：http://pyf.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://bgq.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://oaj.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://bqm.yvedp.cn

TS:   process.argv.slice(2)
来源：http://sxz.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://bgl.yuanzhike.top

Go:   os.Args[1:]
来源：http://bil.bjfxy.top

Ruby: ARGV
来源：http://ook.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://uxt.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://zmp.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://lkt.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wdg.smart0.xyz

JS:   process.env.HOME
来源：http://xpu.hnxiangtu.top

TS:   process.env.HOME
来源：http://aor.fktsv.cn

Java: System.getenv("HOME")
来源：http://zhr.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dxg.xinyue.icu

Ruby: ENV["HOME"]
来源：http://lgq.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bza.smart0.xyz

[M03] 执行外部命令
来源：http://arg.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oil.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://plg.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hxz.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ain.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dfp.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vwz.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://efu.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://fhs.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://ctm.pycfn.com

Py:   os.getcwd()
来源：http://wru.yvedp.cn

PHP:  getcwd();
来源：http://pyv.cashguo.top

JS:   process.cwd()
来源：http://drl.jiagoushi.top

TS:   process.cwd()
来源：http://loe.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://joy.zhengqikj.top

Go:   os.Getwd()
来源：http://bsn.cheryme.top

Ruby: Dir.pwd
来源：http://iiw.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://obk.ppjwa.cn

[M05] 设置退出码
来源：http://vwb.fktsv.cn

Py:   sys.exit(1)
来源：http://nfq.mhx1999.top

PHP:  exit(1);
来源：http://zaw.cheryme.top

JS:   process.exit(1)
来源：http://yhl.fktsv.cn

TS:   process.exit(1)
来源：http://vow.cucudq.cn

Java: System.exit(1)
来源：http://ulf.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://oxk.fengsongda.top

Ruby: exit 1
来源：http://wju.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://byb.sjlbkw.cn

[M06] 向标准错误输出
来源：http://ndx.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://gpf.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ucq.9152youxi.cn

JS:   console.error("err")
来源：http://vem.yj202588.top

TS:   console.error("err")
来源：http://sct.nwbrower.top

Java: System.err.println("err")
来源：http://iym.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xma.cheryme.top

Ruby: warn "err"
来源：http://cod.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://den.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://qet.cashguo.top

Py:   if __name__ == "__main__":
来源：http://ana.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uhd.zhongyouzk.top

JS:   require.main === module
来源：http://emi.yanxiufei.cn

TS:   require.main === module
来源：http://ovk.fehbvm.com

Java: public static void main(String[] args)
来源：http://owi.fzhhl.top

Go:   func main()
来源：http://nom.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://plq.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://tuy.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://vad.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://msp.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://nbx.snrcjt.cn

JS:   process.platform;  process.version
来源：http://srz.wangdashe.top

TS:   process.platform;  process.version
来源：http://lkg.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uss.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iqf.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nlr.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ejv.gaohongyu789.top

================================================================================
来源：http://dmp.vqdsnc.cn

N. 数据结构与算法
来源：http://kte.pycfn.com

================================================================================
来源：http://ttp.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://slc.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://rxf.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lhb.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://swp.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://box.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iea.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://slu.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://goq.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://her.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://ntp.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://kkw.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://woe.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ouv.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fbu.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hfu.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://rnm.chenzaomai.com

Ruby: arr.sort
来源：http://arz.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://siv.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://auc.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pkb.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://oce.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zka.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwf.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bgs.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ind.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pus.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xau.hammf.cn

[N04] 斐波那契数列
来源：http://rds.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gyd.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://flf.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://syy.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://miw.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bbx.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ieo.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sbd.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gxf.shzxlz.cn

[N05] 最大公约数
来源：http://xlz.sysykeji.top

Py:   math.gcd(a, b)
来源：http://rgx.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ccy.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bjx.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pjl.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://msu.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vyo.fzhhl.top

Ruby: a.gcd(b)
来源：http://son.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rmz.daxiang520.top

[N06] 判断回文字符串
来源：http://hzp.hammf.cn

Py:   s == s[::-1]
来源：http://hap.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://xxa.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://gfp.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://bpw.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://omm.yvedp.cn

Go:   // 双指针从两端比较
来源：http://epo.fengsongda.top

Ruby: s == s.reverse
来源：http://ope.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpa.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://wkb.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://thk.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://opz.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qpg.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://khz.hammf.cn

Java: // 手写 HashMap
来源：http://nmo.jianghu66.top

Go:   // 手写 map[int]int
来源：http://swe.tarul.cn

Ruby: // 手写 Hash
来源：http://ayk.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wdx.vehdjk.com

[N08] 生成全排列
来源：http://rhc.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://zwl.uphjek.com

PHP:  // 手写递归交换
来源：http://pxk.yonumen.top

JS:   // 手写回溯递归
来源：http://lyb.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://dsi.havefunace.top

Java: // 手写回溯递归
来源：http://ayc.jiagoushi.top

Go:   // 手写回溯递归
来源：http://rrm.sweek.top

Ruby: arr.permutation.to_a
来源：http://hxd.bbcook.cn

C#:   // 手写回溯递归
来源：http://ltl.jianghu66.top

[N09] 栈与队列
来源：http://hdz.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://soy.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jdq.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pkm.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tup.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fww.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ruu.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nxc.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cuc.cheryme.top

[N10] 链表节点定义
来源：http://log.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://soz.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cir.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wkt.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yrg.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://ncu.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://lor.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://evz.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dmk.yj202588.top

[N11] 二叉树中序遍历
来源：http://qbu.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pcb.hnqzz.top

PHP:  // 手写递归函数
来源：http://imb.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lod.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iks.316326.xyz

Java: // 手写递归
来源：http://bhs.xylfe.cn

Go:   // 手写递归
来源：http://hvk.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nkf.hnxiangtu.top

C#:   // 手写递归
来源：http://guq.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tgf.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dzc.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pyr.jqgfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ode.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://krm.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sbd.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oyd.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vig.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bbv.jianghu66.top

================================================================================
来源：http://uhf.ydzc1.top

O. 并发与异步
来源：http://uxm.cashguo.top

================================================================================
来源：http://sjj.vqdsnc.cn

[O01] 启动一个线程
来源：http://tix.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aqh.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://met.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qiv.yueranfly.top

TS:   // 同 JS
来源：http://iub.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://rac.jinghuilouyu.cn

Go:   go f()
来源：http://bxn.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://psu.zycfv.cn

C#:   Task.Run(() => F());
来源：http://jml.havefunace.top

[O02] 使用线程池
来源：http://xct.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cvr.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vpr.xuanzx.com

JS:   // worker_threads 线程池
来源：http://vcc.havefunace.top

TS:   // worker_threads 线程池
来源：http://liz.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://hii.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ute.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbd.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rtl.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://bsk.tianlin.xyz

Py:   with lock: shared += 1
来源：http://qec.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://vef.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yfg.aibaodan.cn

TS:   // 同 JS
来源：http://pam.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://amg.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tcm.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://gvz.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://fxt.yj20258.top

[O04] 定义异步函数并等待
来源：http://omt.tarul.cn

Py:   async def f():⏎    await g()
来源：http://wka.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://emi.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://jnr.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yrq.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hoj.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wvm.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xei.uphjek.com

C#:   async Task F() { await G(); }
来源：http://cfp.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://gfj.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://uqe.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://opc.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://bqx.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://bda.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://plb.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lvj.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://vax.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://mpm.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://bjk.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mgv.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dqc.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://fwq.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://vtk.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vaw.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hdt.jinqigufen.top

Ruby: // fork 块
来源：http://iga.ivvv.top

C#:   Parallel.For
来源：http://iiz.hnqzz.top

================================================================================
来源：http://vjf.sufxvd.cn

P. 常用工具函数
来源：http://hvy.jinqigfzy.top

================================================================================
来源：http://cbo.gzhubu.top

[P01] 生成 UUID
来源：http://smj.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://bvs.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jkp.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://vdc.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://yys.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://hll.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://rte.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://vmx.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://fhj.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://vhu.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bug.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qax.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bot.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iuz.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xpg.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://acj.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nmv.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jal.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://vmy.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://udp.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kgo.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yld.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ocz.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qzl.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tha.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yzw.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ajj.xuetiantiany.cn

[P04] 求长度
来源：http://jgh.kuanghao11.cn


<!-- 参考信息 -->