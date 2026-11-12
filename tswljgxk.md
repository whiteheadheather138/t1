代发 wailian999

Py:   resp.json()
来源：http://hfb.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://aba.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://zcm.pengpengdd.cyou

TS:   await resp.json()
来源：http://xbg.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fij.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lwk.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://wgl.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tpr.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://sph.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fuc.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rxd.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://esw.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://ggm.epnwcf.com

Java: resp.statusCode()
来源：http://qqe.redwolf501.top

Go:   resp.StatusCode
来源：http://xrf.hywenlv.cn

Ruby: resp.code.to_i
来源：http://hci.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://hms.daria6918.cn

[L08] 并发请求多个地址
来源：http://jrv.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ojm.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://vjh.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jkg.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rck.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tgs.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://npw.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zpr.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mra.tianlin.xyz

================================================================================
来源：http://vmq.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://ofq.jyoumei.cn

================================================================================
来源：http://kfz.yongpay.top

[M01] 读取命令行参数
来源：http://auw.aizwys.cn

Py:   sys.argv[1:]
来源：http://qcd.zycfv.cn

PHP:  $argv;  $argc;
来源：http://hgs.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://zvg.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://dfh.cashguo.top

Java: args 数组（main 方法参数）
来源：http://ovw.dashuyun.cn

Go:   os.Args[1:]
来源：http://nkm.vqdsnc.cn

Ruby: ARGV
来源：http://yyo.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://jhz.hammf.cn

[M02] 读取环境变量
来源：http://vqo.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://zhv.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://chn.jinqigfzy.top

JS:   process.env.HOME
来源：http://ohk.fktsv.cn

TS:   process.env.HOME
来源：http://ldx.dashuyun.cn

Java: System.getenv("HOME")
来源：http://yce.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gwc.fzhhl.top

Ruby: ENV["HOME"]
来源：http://nev.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hdt.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://ljc.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ail.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hal.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hoa.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://gok.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jac.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://inc.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://cpy.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://fvl.bbcook.cn

[M04] 获取当前工作目录
来源：http://lnv.shuidangran.top

Py:   os.getcwd()
来源：http://lyb.jinghuilouyu.cn

PHP:  getcwd();
来源：http://tro.ppjwa.cn

JS:   process.cwd()
来源：http://bct.xuetiantiany.cn

TS:   process.cwd()
来源：http://afl.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://mkk.hesvh.cn

Go:   os.Getwd()
来源：http://zcf.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://rig.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://wzk.316326.xyz

[M05] 设置退出码
来源：http://yby.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://ogu.vehdjk.com

PHP:  exit(1);
来源：http://tkw.vqdsnc.cn

JS:   process.exit(1)
来源：http://gri.hammf.cn

TS:   process.exit(1)
来源：http://jxr.jinqigufen.top

Java: System.exit(1)
来源：http://hot.kuanghao11.cn

Go:   os.Exit(1)
来源：http://gof.daxiang520.top

Ruby: exit 1
来源：http://bgw.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zvo.bjfxy.top

[M06] 向标准错误输出
来源：http://ing.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://dmt.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lrx.kuanghao11.cn

JS:   console.error("err")
来源：http://rzh.jinqigufen.top

TS:   console.error("err")
来源：http://hkn.nwbrower.top

Java: System.err.println("err")
来源：http://xuy.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dbp.feifeiyinyue.top

Ruby: warn "err"
来源：http://zgn.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://oqv.9152youxi.cn

[M07] 判断是否为主入口
来源：http://cwi.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://esj.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ccg.cheryme.top

JS:   require.main === module
来源：http://tmc.hnxiangtu.top

TS:   require.main === module
来源：http://csq.yangfankeji.com

Java: public static void main(String[] args)
来源：http://jii.yongpay.top

Go:   func main()
来源：http://gcm.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ehk.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://gmb.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://wug.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://ncp.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://zil.zycfv.cn

JS:   process.platform;  process.version
来源：http://ahu.aibaodan.cn

TS:   process.platform;  process.version
来源：http://wxx.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://brj.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jqv.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xrw.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uzf.zhijiandao.cn

================================================================================
来源：http://baw.hnqzz.top

N. 数据结构与算法
来源：http://tkc.cashguo.top

================================================================================
来源：http://vvg.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://zlg.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://mvu.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mul.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsz.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ewr.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://zet.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://xzr.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lnz.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://tem.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://tlx.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://hzn.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fzv.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eve.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ihg.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cjc.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://ixh.chenzaomai.com

Ruby: arr.sort
来源：http://gnj.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ohy.sweek.top

[N03] 快速排序（分治示例）
来源：http://tpk.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ewu.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://xzm.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cyq.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxd.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bhc.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nnb.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ivx.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://rgx.daria6918.cn

[N04] 斐波那契数列
来源：http://ctd.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uyt.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmb.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrq.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stq.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lgg.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zmy.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qmg.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ddr.yonumen.top

[N05] 最大公约数
来源：http://lpg.yj202588.top

Py:   math.gcd(a, b)
来源：http://ddw.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mjt.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iec.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vnn.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qpd.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pht.zycfv.cn

Ruby: a.gcd(b)
来源：http://khu.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bvl.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://ytu.yongpay.top

Py:   s == s[::-1]
来源：http://qkl.meibo888.top

PHP:  $s === strrev($s);
来源：http://nsi.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://nhi.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://ecs.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tpr.vehdjk.com

Go:   // 双指针从两端比较
来源：http://hge.ctjpmb.com

Ruby: s == s.reverse
来源：http://che.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://kds.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://dpv.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lgo.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rhv.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rmk.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://gkq.snrcjt.cn

Java: // 手写 HashMap
来源：http://rzf.yonumen.top

Go:   // 手写 map[int]int
来源：http://xtx.hnqzz.top

Ruby: // 手写 Hash
来源：http://eyk.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hlt.smart0.xyz

[N08] 生成全排列
来源：http://wvd.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://qym.ehwqpu.com

PHP:  // 手写递归交换
来源：http://qsr.havefunace.top

JS:   // 手写回溯递归
来源：http://igm.aizwys.cn

TS:   // 手写回溯递归
来源：http://jqc.hnqzz.top

Java: // 手写回溯递归
来源：http://qdp.bjfxy.top

Go:   // 手写回溯递归
来源：http://cuv.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://shs.fktsv.cn

C#:   // 手写回溯递归
来源：http://mfk.gzhubu.top

[N09] 栈与队列
来源：http://awg.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pqo.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xwd.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qkj.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xss.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eoe.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kfs.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wjf.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oco.tarul.cn

[N10] 链表节点定义
来源：http://rpm.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bsv.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tzx.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qrv.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rtu.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://luy.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mvf.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vnk.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nhc.gzhubu.top

[N11] 二叉树中序遍历
来源：http://jrv.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xdi.yfazqb.com

PHP:  // 手写递归函数
来源：http://etx.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itg.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zul.ybcxt.top

Java: // 手写递归
来源：http://inj.xylfe.cn

Go:   // 手写递归
来源：http://bmb.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://plt.birdmap.top

C#:   // 手写递归
来源：http://hjd.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xtt.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wsm.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ini.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzx.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbg.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://snd.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jhi.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vcd.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kwf.zycfv.cn

================================================================================
来源：http://zxj.gaohongyu789.top

O. 并发与异步
来源：http://zqp.nanxuanxn.top

================================================================================
来源：http://hfx.ivvv.top

[O01] 启动一个线程
来源：http://qtq.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oop.jlsjyb.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vwq.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rdf.andypj.xyz

TS:   // 同 JS
来源：http://ugb.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://shl.ydjk.org.cn

Go:   go f()
来源：http://vld.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://gbq.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://uhs.yj202588.top

[O02] 使用线程池
来源：http://rcv.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qyd.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lcp.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://ifa.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://jej.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://dbo.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mne.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pgc.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ckw.cheryme.top

[O03] 加锁保护共享数据
来源：http://edk.sweek.top

Py:   with lock: shared += 1
来源：http://hdy.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://oyj.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://exp.andypj.xyz

TS:   // 同 JS
来源：http://zye.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://ptv.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gnw.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ddx.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://dlb.shuidangran.top

[O04] 定义异步函数并等待
来源：http://wpm.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://oif.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jja.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://nbq.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vun.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwh.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://prh.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jfj.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://bqp.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://crc.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://dbd.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pls.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://psg.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://pyo.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yej.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ogr.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://sds.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://cdp.sysykeji.top

[O06] 使用进程池
来源：http://znn.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://isg.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wkg.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://xgt.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://sgb.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cck.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kbc.zdqjudy.top

Ruby: // fork 块
来源：http://mey.yonumen.top

C#:   Parallel.For
来源：http://tlb.ctjpmb.com

================================================================================
来源：http://eho.hongshengwenyu.top

P. 常用工具函数
来源：http://ast.yuxming.cn

================================================================================
来源：http://eyf.aizwys.cn

[P01] 生成 UUID
来源：http://ncn.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://iav.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rpy.shuidangran.top

JS:   crypto.randomUUID()
来源：http://onp.hammf.cn

TS:   crypto.randomUUID()
来源：http://aoj.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://sjn.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://aua.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://dag.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://grb.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://fbq.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jtd.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://grz.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://svc.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lro.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cna.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lcc.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hjl.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uoa.chenzaomai.com

[P03] 生成短随机字符串
来源：http://lvj.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wpy.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://avy.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kbs.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xxc.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://apw.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rty.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rqj.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lji.andypj.xyz

[P04] 求长度
来源：http://xlp.yvedp.cn


<!-- 参考信息 -->