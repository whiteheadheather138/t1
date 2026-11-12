代发 wailian999

Py:   resp.json()
来源：http://zyc.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://wnf.yvedp.cn

JS:   await resp.json()
来源：http://gjk.sufxvd.cn

TS:   await resp.json()
来源：http://zmj.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rwf.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://duz.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://bxm.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mtx.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://ozr.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eca.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbi.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://qdr.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://hng.tianlin.xyz

Java: resp.statusCode()
来源：http://wis.aizwys.cn

Go:   resp.StatusCode
来源：http://oem.316326.xyz

Ruby: resp.code.to_i
来源：http://icm.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://brr.cqqwz.cn

[L08] 并发请求多个地址
来源：http://slh.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://khx.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://ruz.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ino.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxs.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bab.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iuc.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fzt.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vhz.ehwqpu.com

================================================================================
来源：http://cra.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://fvu.jinghuilouyu.cn

================================================================================
来源：http://lzn.yanxiufei.cn

[M01] 读取命令行参数
来源：http://zik.cucudq.cn

Py:   sys.argv[1:]
来源：http://irx.jianghu66.top

PHP:  $argv;  $argc;
来源：http://rod.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://hqp.nwbrower.top

TS:   process.argv.slice(2)
来源：http://mof.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://ehi.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://brc.bbcook.cn

Ruby: ARGV
来源：http://bzj.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://rji.nanxinkj.top

[M02] 读取环境变量
来源：http://spq.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://tud.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pqu.havefunace.top

JS:   process.env.HOME
来源：http://ttz.yuxming.cn

TS:   process.env.HOME
来源：http://phi.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://rxy.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qxt.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://ssn.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lnu.hfpthk.cn

[M03] 执行外部命令
来源：http://rld.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hvk.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qrs.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vev.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://blp.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://txa.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://orf.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aha.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://uzd.316326.xyz

[M04] 获取当前工作目录
来源：http://vqz.ivvv.top

Py:   os.getcwd()
来源：http://tro.hysaishi.cn

PHP:  getcwd();
来源：http://mcd.ehwqpu.com

JS:   process.cwd()
来源：http://yzw.xuetiantiany.cn

TS:   process.cwd()
来源：http://dbi.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://unp.svipenyu.cn

Go:   os.Getwd()
来源：http://slb.zdqjudy.top

Ruby: Dir.pwd
来源：http://tpu.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xfq.gogol.net.cn

[M05] 设置退出码
来源：http://dir.jyoumei.cn

Py:   sys.exit(1)
来源：http://neq.zhiwuduotai.top

PHP:  exit(1);
来源：http://pjp.yanxiufei.cn

JS:   process.exit(1)
来源：http://ezp.52xcode.cn

TS:   process.exit(1)
来源：http://lfw.zhixingplan.top

Java: System.exit(1)
来源：http://kxo.xuanzx.com

Go:   os.Exit(1)
来源：http://yer.yanxiufei.cn

Ruby: exit 1
来源：http://evw.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zis.ehwqpu.com

[M06] 向标准错误输出
来源：http://mzx.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://uav.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cck.shangyingyoupin.top

JS:   console.error("err")
来源：http://yid.cucudq.cn

TS:   console.error("err")
来源：http://hdi.xziqi.cn

Java: System.err.println("err")
来源：http://aza.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nxw.jiagoushi.top

Ruby: warn "err"
来源：http://qfk.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://czs.hcnkem.com

[M07] 判断是否为主入口
来源：http://kit.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://zta.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://roi.dianchejie.cn

JS:   require.main === module
来源：http://xfk.hnqzz.top

TS:   require.main === module
来源：http://fzc.ybcxt.top

Java: public static void main(String[] args)
来源：http://ver.yuanzhike.top

Go:   func main()
来源：http://yll.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cmt.tanke756.top

C#:   static void Main(string[] args)
来源：http://lzp.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://xvm.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://zud.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://wyt.zhixingplan.top

JS:   process.platform;  process.version
来源：http://bpp.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://eeg.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oma.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ddk.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gbn.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hgr.fzhhl.top

================================================================================
来源：http://tsx.52xcode.cn

N. 数据结构与算法
来源：http://fmp.zdqjudy.top

================================================================================
来源：http://pfz.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://luw.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://ppr.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kfa.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wto.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kkm.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://egr.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://pqv.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://itb.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://kyo.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://jow.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://xzq.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fco.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jld.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://vvw.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://unu.hesvh.cn

Go:   slices.Sort(arr)
来源：http://odc.chenjidiqi.icu

Ruby: arr.sort
来源：http://qwr.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cka.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://rwt.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gov.tanke756.top

PHP:  // 递归实现，或用 usort
来源：http://lrr.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vql.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ezh.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://udv.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jmh.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ulh.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://pjw.zhongyouzk.top

[N04] 斐波那契数列
来源：http://knr.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hwy.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zdd.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uum.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnd.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dju.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gbf.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zaf.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://euu.meibo888.top

[N05] 最大公约数
来源：http://nmh.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://mto.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://obc.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbm.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vgh.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rxc.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qvv.yvedp.cn

Ruby: a.gcd(b)
来源：http://aht.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vpa.havefunace.top

[N06] 判断回文字符串
来源：http://qwv.vehdjk.com

Py:   s == s[::-1]
来源：http://uvg.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://bam.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://gly.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://lkb.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hrj.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://bst.9152youxi.cn

Ruby: s == s.reverse
来源：http://izy.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://veh.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://yen.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oij.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gvy.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vye.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://zpv.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://ksm.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://qke.smart0.xyz

Ruby: // 手写 Hash
来源：http://fmp.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zbe.birdmap.top

[N08] 生成全排列
来源：http://icd.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://xde.tarul.cn

PHP:  // 手写递归交换
来源：http://fbc.yongpay.top

JS:   // 手写回溯递归
来源：http://rmf.ppjwa.cn

TS:   // 手写回溯递归
来源：http://vxo.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://boa.cashguo.top

Go:   // 手写回溯递归
来源：http://wld.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://fha.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://oja.birdmap.top

[N09] 栈与队列
来源：http://dpj.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jsu.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://one.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gun.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fnf.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://adt.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ipy.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yuz.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hpw.ydjk.org.cn

[N10] 链表节点定义
来源：http://naj.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lyf.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://htx.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aya.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oyy.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://suw.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://iyd.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gxg.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qho.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://dxl.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fzo.chenlongwang.top

PHP:  // 手写递归函数
来源：http://xmi.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://leg.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdu.gaohongyu789.top

Java: // 手写递归
来源：http://mqk.ctjpmb.com

Go:   // 手写递归
来源：http://ptp.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fli.sjlbkw.cn

C#:   // 手写递归
来源：http://ddn.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bfy.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ttt.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cny.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://meh.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yrt.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fpl.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lna.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://krr.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dpb.zhaomingkeji.xyz

================================================================================
来源：http://vkv.c1oappe.top

O. 并发与异步
来源：http://wdo.aibaodan.cn

================================================================================
来源：http://ppq.hcnkem.com

[O01] 启动一个线程
来源：http://izm.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gbm.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iay.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vsp.hywenlv.cn

TS:   // 同 JS
来源：http://xlm.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://ldt.cucudq.cn

Go:   go f()
来源：http://fzt.aizwys.cn

Ruby: Thread.new { f }
来源：http://gio.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://ird.vqdsnc.cn

[O02] 使用线程池
来源：http://byc.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tqj.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iky.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://hyi.ydzc1.top

TS:   // worker_threads 线程池
来源：http://qxp.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://hle.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://utt.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yuv.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://snj.c1oappe.top

[O03] 加锁保护共享数据
来源：http://uyd.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://ujt.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://jxs.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uwi.fktsv.cn

TS:   // 同 JS
来源：http://xnb.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://wje.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vwk.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jeu.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://pcx.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://jvt.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://qxw.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfn.mhx1999.top

JS:   async function f() { await g(); }
来源：http://rnr.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://das.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zxp.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cll.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://xrh.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://ylg.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://loj.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://nlv.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zey.yj202588.top

JS:   await Promise.all(tasks)
来源：http://fik.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://gho.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ucb.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wcx.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://jfi.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://vhf.daria6918.cn

[O06] 使用进程池
来源：http://nik.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jya.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://skl.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://ale.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://tob.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sle.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ros.zdbjq.cn

Ruby: // fork 块
来源：http://fvx.xuetiantiany.cn

C#:   Parallel.For
来源：http://ink.gogol.net.cn

================================================================================
来源：http://dzs.ybcxt.top

P. 常用工具函数
来源：http://ohy.jianghu66.top

================================================================================
来源：http://gyw.xuetiantiany.cn

[P01] 生成 UUID
来源：http://qxm.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://gdy.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zpr.tian-w.cn

JS:   crypto.randomUUID()
来源：http://edw.ybcxt.top

TS:   crypto.randomUUID()
来源：http://zpp.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://aox.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://arc.yj202588.top

Ruby: SecureRandom.uuid
来源：http://ild.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://ycq.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://lsn.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cjh.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mdq.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jqk.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ctn.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zet.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://awc.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qiq.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xpr.andypj.xyz

[P03] 生成短随机字符串
来源：http://yjn.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jwc.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://opz.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vfc.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iyr.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://apt.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://osk.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://crn.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eof.ctjpmb.com

[P04] 求长度
来源：http://nxr.vqdsnc.cn


<!-- 参考信息 -->