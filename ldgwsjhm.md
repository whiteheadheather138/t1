代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ezq.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oho.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://dvj.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qmo.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://vuf.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uoj.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eoz.cheryme.top

JS:   resp.ok;  resp.status
来源：http://dkq.cheryme.top

TS:   resp.ok;  resp.status
来源：http://uvf.shzxlz.cn

Java: resp.statusCode()
来源：http://buq.0kj1m.cn

Go:   resp.StatusCode
来源：http://qiv.yonumen.top

Ruby: resp.code.to_i
来源：http://isf.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://ktz.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://ifw.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wsd.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://gii.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xqp.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdd.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://shu.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://omb.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nmy.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://svq.fzhhl.top

================================================================================
来源：http://knr.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://ewh.cqqwz.cn

================================================================================
来源：http://tjf.fengsongda.top

[M01] 读取命令行参数
来源：http://wlm.guannengcc.top

Py:   sys.argv[1:]
来源：http://ysh.cucudq.cn

PHP:  $argv;  $argc;
来源：http://vqt.bjfxy.top

JS:   process.argv.slice(2)
来源：http://thb.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://xtk.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://zhc.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://tvn.jyoumei.cn

Ruby: ARGV
来源：http://afm.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://kku.epnwcf.com

[M02] 读取环境变量
来源：http://ziz.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://erq.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sdg.haohaochexian.top

JS:   process.env.HOME
来源：http://ltt.ppjwa.cn

TS:   process.env.HOME
来源：http://aeq.cucudq.cn

Java: System.getenv("HOME")
来源：http://nry.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sbf.epnwcf.com

Ruby: ENV["HOME"]
来源：http://gvv.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rye.xylfe.cn

[M03] 执行外部命令
来源：http://qqw.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://esy.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vbc.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://rxy.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fws.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wlm.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pva.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://qga.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://nle.ppjwa.cn

[M04] 获取当前工作目录
来源：http://ynd.daxiang520.top

Py:   os.getcwd()
来源：http://jkm.tian-w.cn

PHP:  getcwd();
来源：http://uzl.tarul.cn

JS:   process.cwd()
来源：http://lbo.sxryk.cn

TS:   process.cwd()
来源：http://wsy.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://eiu.sjlbkw.cn

Go:   os.Getwd()
来源：http://odu.jlsjyb.cn

Ruby: Dir.pwd
来源：http://jrw.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://dko.shuidangran.top

[M05] 设置退出码
来源：http://rls.316326.xyz

Py:   sys.exit(1)
来源：http://jzx.316326.xyz

PHP:  exit(1);
来源：http://sfv.nanxuanxn.top

JS:   process.exit(1)
来源：http://vae.yuanzhike.top

TS:   process.exit(1)
来源：http://frt.quarkkingdee.top

Java: System.exit(1)
来源：http://foq.cdnleiting.top

Go:   os.Exit(1)
来源：http://ibq.hcnkem.com

Ruby: exit 1
来源：http://mnv.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uda.zhoulong.xyz

[M06] 向标准错误输出
来源：http://wde.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://bqp.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qgn.jqgufenzy.top

JS:   console.error("err")
来源：http://ydg.hesvh.cn

TS:   console.error("err")
来源：http://rll.cheryme.top

Java: System.err.println("err")
来源：http://ppb.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ydz.guowangkeji.top

Ruby: warn "err"
来源：http://etk.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://ztc.yueranfly.top

[M07] 判断是否为主入口
来源：http://apn.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://dts.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://asb.cucudq.cn

JS:   require.main === module
来源：http://ubb.52xcode.cn

TS:   require.main === module
来源：http://drv.bjfxy.top

Java: public static void main(String[] args)
来源：http://llc.pycfn.com

Go:   func main()
来源：http://aze.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pgl.andypj.xyz

C#:   static void Main(string[] args)
来源：http://oed.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://mng.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://epx.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://rqs.yongpay.top

JS:   process.platform;  process.version
来源：http://cdi.epnwcf.com

TS:   process.platform;  process.version
来源：http://bss.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kdi.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://shg.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eiz.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pow.ydzc1.top

================================================================================
来源：http://gau.gotoacloud.top

N. 数据结构与算法
来源：http://uvd.zhiwuduotai.top

================================================================================
来源：http://ohq.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://jvz.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qjr.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://obk.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dov.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pgu.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://dlz.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://cqf.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tjm.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zzz.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://ric.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://lyo.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pnz.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wcc.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cct.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jvm.redwolf501.top

Go:   slices.Sort(arr)
来源：http://etm.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://pjk.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qrf.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://qjj.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kbj.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://jvb.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbr.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kmh.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gtg.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ufw.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fjz.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bvq.wangdashe.top

[N04] 斐波那契数列
来源：http://xev.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bje.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eyi.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wvv.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kem.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iel.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ejg.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sdw.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gwj.tian-w.cn

[N05] 最大公约数
来源：http://caj.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://qwb.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ywf.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hcg.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://imu.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fje.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pwr.cucudq.cn

Ruby: a.gcd(b)
来源：http://hgk.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qxa.snrcjt.cn

[N06] 判断回文字符串
来源：http://jyh.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://fju.c1oappe.top

PHP:  $s === strrev($s);
来源：http://oji.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://lwh.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://sht.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tee.cucudq.cn

Go:   // 双指针从两端比较
来源：http://jml.redwolf501.top

Ruby: s == s.reverse
来源：http://gvu.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://tmi.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://aej.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://crh.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://des.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cig.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://uga.nanxuanxn.top

Java: // 手写 HashMap
来源：http://vpi.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://vvj.sysykeji.top

Ruby: // 手写 Hash
来源：http://dix.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://htf.0kj1m.cn

[N08] 生成全排列
来源：http://ydc.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://uyg.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://fsr.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://rll.dashuyun.cn

TS:   // 手写回溯递归
来源：http://xgt.bjfxy.top

Java: // 手写回溯递归
来源：http://prw.uphjek.com

Go:   // 手写回溯递归
来源：http://kaf.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://yve.tian-w.cn

C#:   // 手写回溯递归
来源：http://nls.pycfn.com

[N09] 栈与队列
来源：http://mbb.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://umq.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iwz.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cwi.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jzq.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pvm.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hju.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://szx.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://irm.meibo888.top

[N10] 链表节点定义
来源：http://frj.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsa.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dyp.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gbd.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eob.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://sva.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://wia.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://rrr.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jxc.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://jor.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xow.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://tyc.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dky.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bxb.fktsv.cn

Java: // 手写递归
来源：http://qik.pycfn.com

Go:   // 手写递归
来源：http://gnx.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zav.zhengqikj.top

C#:   // 手写递归
来源：http://lpt.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lkf.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pqz.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rcn.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hcd.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qpb.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ttz.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bmn.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gcw.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://esg.yonumen.top

================================================================================
来源：http://bml.shangyingyoupin.top

O. 并发与异步
来源：http://eov.zhijiandao.cn

================================================================================
来源：http://xhn.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://rby.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yib.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eai.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bgs.316326.xyz

TS:   // 同 JS
来源：http://vry.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://bfx.fanxiaobao.xyz

Go:   go f()
来源：http://nwq.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://hfx.c1oappe.top

C#:   Task.Run(() => F());
来源：http://ypx.nanxinkj.top

[O02] 使用线程池
来源：http://vrz.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sqs.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nyg.uphjek.com

JS:   // worker_threads 线程池
来源：http://mic.cucudq.cn

TS:   // worker_threads 线程池
来源：http://aai.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://akb.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gkx.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ivn.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uve.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://xju.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://noj.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://sgs.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mzv.guannengcc.top

TS:   // 同 JS
来源：http://pyk.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://oiz.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dle.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eoo.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://fbm.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://rjx.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://uoh.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gik.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://nep.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mnz.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qos.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wbf.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sfl.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://wmi.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://eyc.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://vqk.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xzx.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://iro.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://rix.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wjd.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mcj.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://ruw.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fvv.nanxinkj.top

[O06] 使用进程池
来源：http://zgu.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ujd.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ltk.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://vqx.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://wkw.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vya.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gdg.ctjpmb.com

Ruby: // fork 块
来源：http://rom.ppjwa.cn

C#:   Parallel.For
来源：http://vfb.jqgufenzy.top

================================================================================
来源：http://cyb.feifeiyinyue.top

P. 常用工具函数
来源：http://lzu.mhx1999.top

================================================================================
来源：http://ium.zhixingplan.top

[P01] 生成 UUID
来源：http://ycb.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://ljt.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yph.bbcook.cn

JS:   crypto.randomUUID()
来源：http://qam.tarul.cn

TS:   crypto.randomUUID()
来源：http://xrc.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://low.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://coa.birdmap.top

Ruby: SecureRandom.uuid
来源：http://cjm.nanxinkj.top

C#:   Guid.NewGuid().ToString()
来源：http://zrx.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://wtw.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yoc.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ivx.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bxx.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yxn.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://via.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ozu.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ylg.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ldk.zhengqikj.top

[P03] 生成短随机字符串
来源：http://ebs.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iaj.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ays.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dln.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixl.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mqk.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iqi.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://drp.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uxj.dianchejie.cn

[P04] 求长度
来源：http://ibe.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ist.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://usg.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://can.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://njr.gogol.net.cn


<!-- 参考信息 -->