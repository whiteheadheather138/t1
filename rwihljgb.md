代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ecw.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tnc.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://jgq.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rwx.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://yhj.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://thk.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jor.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://aly.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://hkn.yuxming.cn

Java: resp.statusCode()
来源：http://khr.guannengcc.top

Go:   resp.StatusCode
来源：http://zvy.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://pyy.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://gbz.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://obc.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://stc.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://pgu.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqb.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nvn.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yol.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aet.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vbq.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lqg.hcnkem.com

================================================================================
来源：http://thh.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://bvb.jqgfzy.top

================================================================================
来源：http://qbz.xylfe.cn

[M01] 读取命令行参数
来源：http://uns.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://piq.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://ydn.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://yzi.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://guc.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://hup.jinqigufen.top

Go:   os.Args[1:]
来源：http://lbs.sjlbkw.cn

Ruby: ARGV
来源：http://ukb.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://iaw.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://bry.cashguo.top

Py:   os.environ.get("HOME")
来源：http://jgy.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fis.daxiang520.top

JS:   process.env.HOME
来源：http://oab.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://moc.bjfxy.top

Java: System.getenv("HOME")
来源：http://fzl.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rqx.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://xos.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fms.mhx1999.top

[M03] 执行外部命令
来源：http://jxf.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://exx.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xgm.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uqn.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://idp.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wtq.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ufk.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://jtf.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://naa.iojbl.cn

[M04] 获取当前工作目录
来源：http://ywt.chenlongwang.top

Py:   os.getcwd()
来源：http://lkb.yueranfly.top

PHP:  getcwd();
来源：http://tae.zhixingplan.top

JS:   process.cwd()
来源：http://yiz.hywenlv.cn

TS:   process.cwd()
来源：http://wim.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://qsq.meibo888.top

Go:   os.Getwd()
来源：http://qcv.ydzc1.top

Ruby: Dir.pwd
来源：http://ejm.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://aem.dashuyun.cn

[M05] 设置退出码
来源：http://org.ydjk.org.cn

Py:   sys.exit(1)
来源：http://ygo.ybcxt.top

PHP:  exit(1);
来源：http://cgf.yongpay.top

JS:   process.exit(1)
来源：http://jjj.fktsv.cn

TS:   process.exit(1)
来源：http://ufn.yuxming.cn

Java: System.exit(1)
来源：http://fbw.ppjwa.cn

Go:   os.Exit(1)
来源：http://mtf.dashuyun.cn

Ruby: exit 1
来源：http://ccu.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://okl.redwolf501.top

[M06] 向标准错误输出
来源：http://uwg.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://hyo.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ysm.svipenyu.cn

JS:   console.error("err")
来源：http://yxm.yj20258888.top

TS:   console.error("err")
来源：http://coe.chenjidiqi.icu

Java: System.err.println("err")
来源：http://cyr.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xsf.fzhhl.top

Ruby: warn "err"
来源：http://dcy.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://zco.jinqigufen.top

[M07] 判断是否为主入口
来源：http://ppy.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://kuf.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lfr.cucudq.cn

JS:   require.main === module
来源：http://mnj.hammf.cn

TS:   require.main === module
来源：http://tow.yangfankeji.com

Java: public static void main(String[] args)
来源：http://gap.gzhubu.top

Go:   func main()
来源：http://mpx.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://swb.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://mxw.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://aij.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://coz.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://wwp.zdqjudy.top

JS:   process.platform;  process.version
来源：http://ipy.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://vmp.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ajq.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dcf.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mwf.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kot.jyoumei.cn

================================================================================
来源：http://zjm.andypj.xyz

N. 数据结构与算法
来源：http://fgz.gogol.net.cn

================================================================================
来源：http://tyl.aizwys.cn

[N01] 二分查找（有序数组）
来源：http://odr.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://gya.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vbb.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://evx.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jdd.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://uqo.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://epf.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rhz.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://kzr.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://jnt.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://hkv.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hwh.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pdp.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dkz.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://huj.hcnkem.com

Go:   slices.Sort(arr)
来源：http://fwv.sjlbkw.cn

Ruby: arr.sort
来源：http://wrk.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jao.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://inv.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jyp.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://izp.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wre.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lmf.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wjq.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://psc.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rhb.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://chx.pycfn.com

[N04] 斐波那契数列
来源：http://fkp.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jiv.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tuq.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://omv.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojr.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://taz.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hjl.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ruz.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jnd.ybcxt.top

[N05] 最大公约数
来源：http://hbd.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://orj.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mku.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vtt.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wab.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sev.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://umg.fzhhl.top

Ruby: a.gcd(b)
来源：http://ntv.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hgp.zdqjudy.top

[N06] 判断回文字符串
来源：http://rgr.sjlbkw.cn

Py:   s == s[::-1]
来源：http://zcf.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://zvo.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://tlc.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://hag.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://njz.uphjek.com

Go:   // 双指针从两端比较
来源：http://lot.ehwqpu.com

Ruby: s == s.reverse
来源：http://jea.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxx.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://tmt.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jwx.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://upw.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://umw.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://vuk.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://tqy.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://cdd.hysaishi.cn

Ruby: // 手写 Hash
来源：http://ewy.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ylt.zhiwuduotai.top

[N08] 生成全排列
来源：http://qrq.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://axp.cdnleiting.top

PHP:  // 手写递归交换
来源：http://dbp.chenzaomai.com

JS:   // 手写回溯递归
来源：http://zle.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://lbg.sjlbkw.cn

Java: // 手写回溯递归
来源：http://oju.0kj1m.cn

Go:   // 手写回溯递归
来源：http://ktg.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://gxt.vehdjk.com

C#:   // 手写回溯递归
来源：http://yoj.dianchejie.cn

[N09] 栈与队列
来源：http://vrn.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dov.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uba.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jfe.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://deg.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zll.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iun.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jgl.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bfx.kuanghao11.cn

[N10] 链表节点定义
来源：http://loj.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://buv.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xcy.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oky.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lkw.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://duz.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://giv.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nfb.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cie.sweek.top

[N11] 二叉树中序遍历
来源：http://jcm.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gcw.xuanzx.com

PHP:  // 手写递归函数
来源：http://fnh.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://phq.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hfc.zhengqikj.top

Java: // 手写递归
来源：http://izv.feifeiyinyue.top

Go:   // 手写递归
来源：http://obm.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://irt.sysykeji.top

C#:   // 手写递归
来源：http://eey.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://onb.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jcy.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xdf.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcb.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://izx.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://isi.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xqp.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zsf.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://led.zhiwuduotai.top

================================================================================
来源：http://nve.ywan-chungtsiang.top

O. 并发与异步
来源：http://ydn.yj202588.top

================================================================================
来源：http://uxq.cqqwz.cn

[O01] 启动一个线程
来源：http://qfw.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nyg.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ned.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mkw.hesvh.cn

TS:   // 同 JS
来源：http://flp.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://ime.xziqi.cn

Go:   go f()
来源：http://eqp.yueranfly.top

Ruby: Thread.new { f }
来源：http://zzu.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://hyq.vqdsnc.cn

[O02] 使用线程池
来源：http://ghb.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hkd.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dxk.iojbl.cn

JS:   // worker_threads 线程池
来源：http://ysl.daria6918.cn

TS:   // worker_threads 线程池
来源：http://kqt.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://erj.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://btn.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cdp.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nqw.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://hne.svipenyu.cn

Py:   with lock: shared += 1
来源：http://pbj.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://lev.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ind.nwbrower.top

TS:   // 同 JS
来源：http://rem.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://ohv.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ray.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nvh.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://xkq.hcnkem.com

[O04] 定义异步函数并等待
来源：http://bqw.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://odz.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bur.smart0.xyz

JS:   async function f() { await g(); }
来源：http://cqe.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://daa.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nwq.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sav.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://ltj.xuetiantiany.cn

C#:   async Task F() { await G(); }
来源：http://qfc.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://qbj.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://ept.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qnm.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://blc.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://paw.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qml.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nvp.hesvh.cn

Ruby: threads.map(&:join)
来源：http://hza.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zlf.fanxiaobao.xyz

[O06] 使用进程池
来源：http://qgu.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jju.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://svt.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://rnx.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://ijb.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vtd.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ieq.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://ayk.zdbjq.cn

C#:   Parallel.For
来源：http://ptq.cheryme.top

================================================================================
来源：http://avd.hnqzz.top

P. 常用工具函数
来源：http://jda.pycfn.com

================================================================================
来源：http://ixa.hywenlv.cn

[P01] 生成 UUID
来源：http://xyp.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://psr.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pvx.bbcook.cn

JS:   crypto.randomUUID()
来源：http://bgr.sysykeji.top

TS:   crypto.randomUUID()
来源：http://fxk.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://ooa.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://irk.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://qmq.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://tfs.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://lee.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vgv.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qyv.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kdf.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ofn.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zyc.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://izw.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ejx.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fvr.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://fbb.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sns.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uiy.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vua.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://var.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qsz.uphjek.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ikf.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mre.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rby.yangfankeji.com

[P04] 求长度
来源：http://bfg.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pwp.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oqo.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uyv.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mal.ivvv.top


<!-- 参考信息 -->