代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iqx.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uia.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://pcp.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zsj.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://jcj.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://epz.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://azc.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://jyu.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://fvo.mhx1999.top

Java: resp.statusCode()
来源：http://ylo.meibo888.top

Go:   resp.StatusCode
来源：http://xqz.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://tbw.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://fkn.xylfe.cn

[L08] 并发请求多个地址
来源：http://ray.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kij.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://zie.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ash.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smp.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nax.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aex.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://atd.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rwu.gzhubu.top

================================================================================
来源：http://ewx.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://gcj.jinqigufen.top

================================================================================
来源：http://nfu.cheryme.top

[M01] 读取命令行参数
来源：http://kee.hfpthk.cn

Py:   sys.argv[1:]
来源：http://pnn.52xcode.cn

PHP:  $argv;  $argc;
来源：http://mgw.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://fou.xylfe.cn

TS:   process.argv.slice(2)
来源：http://rhy.yonumen.top

Java: args 数组（main 方法参数）
来源：http://phy.pycfn.com

Go:   os.Args[1:]
来源：http://eda.chenlongwang.top

Ruby: ARGV
来源：http://vjz.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://diw.ybcxt.top

[M02] 读取环境变量
来源：http://svx.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://ioh.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uat.cheryme.top

JS:   process.env.HOME
来源：http://bkr.sjlbkw.cn

TS:   process.env.HOME
来源：http://ebu.yangfankeji.com

Java: System.getenv("HOME")
来源：http://iyi.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://huh.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://sbh.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://klm.andypj.xyz

[M03] 执行外部命令
来源：http://hxc.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eww.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tcx.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zob.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://way.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cis.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://czb.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://pmn.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://wme.yangfankeji.com

[M04] 获取当前工作目录
来源：http://bjf.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://bgy.yj20258888.top

PHP:  getcwd();
来源：http://imo.sufxvd.cn

JS:   process.cwd()
来源：http://jpn.sweek.top

TS:   process.cwd()
来源：http://vyn.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://fwv.yangfankeji.com

Go:   os.Getwd()
来源：http://bjn.zycfv.cn

Ruby: Dir.pwd
来源：http://sbv.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://cuv.zycfv.cn

[M05] 设置退出码
来源：http://ljz.cheryme.top

Py:   sys.exit(1)
来源：http://ffj.hfpthk.cn

PHP:  exit(1);
来源：http://viq.ppjwa.cn

JS:   process.exit(1)
来源：http://mkl.dashuyun.cn

TS:   process.exit(1)
来源：http://gcr.yj20258888.top

Java: System.exit(1)
来源：http://hcn.daxiang520.top

Go:   os.Exit(1)
来源：http://jjv.nwbrower.top

Ruby: exit 1
来源：http://fli.52xcode.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://keo.yongpay.top

[M06] 向标准错误输出
来源：http://gva.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://bwd.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ojy.jinqigufen.top

JS:   console.error("err")
来源：http://fhc.redwolf501.top

TS:   console.error("err")
来源：http://bvj.mhx1999.top

Java: System.err.println("err")
来源：http://bym.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bsg.nanxinkj.top

Ruby: warn "err"
来源：http://soy.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://umn.ehwqpu.com

[M07] 判断是否为主入口
来源：http://qag.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://lxf.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kcj.xylfe.cn

JS:   require.main === module
来源：http://ytb.ywan-chungtsiang.top

TS:   require.main === module
来源：http://mvu.pycfn.com

Java: public static void main(String[] args)
来源：http://lfl.yonumen.top

Go:   func main()
来源：http://yag.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://goq.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://crv.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://lro.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://ifj.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://lwa.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://yot.zhengqikj.top

TS:   process.platform;  process.version
来源：http://hsr.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nas.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://icz.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vxy.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sbu.daria6918.cn

================================================================================
来源：http://dmo.sufxvd.cn

N. 数据结构与算法
来源：http://icn.dashuyun.cn

================================================================================
来源：http://hzw.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://tcb.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fza.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://doq.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gsm.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://koo.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sum.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://stp.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://tpe.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://rhj.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://tbr.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://vvf.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xlm.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://nly.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://syc.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://elx.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://kvf.yuanzhike.top

Ruby: arr.sort
来源：http://hhe.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fen.havefunace.top

[N03] 快速排序（分治示例）
来源：http://hqw.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pia.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://dvf.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ugs.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxa.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zsj.sjlbkw.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eqe.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://btm.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zdy.bbcook.cn

[N04] 斐波那契数列
来源：http://ott.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xvc.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tbs.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://req.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://luf.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oew.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nqg.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fpl.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://phk.chenjidiqi.icu

[N05] 最大公约数
来源：http://qxo.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://hqp.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oxn.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cjc.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hqu.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oyp.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wmy.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://qfa.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ycy.bjfxy.top

[N06] 判断回文字符串
来源：http://ojn.ehwqpu.com

Py:   s == s[::-1]
来源：http://cff.hammf.cn

PHP:  $s === strrev($s);
来源：http://hra.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://cgr.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://zoa.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yjd.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://ffg.mhx1999.top

Ruby: s == s.reverse
来源：http://nly.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://odo.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://cyf.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fyu.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://khc.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ere.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://gmh.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://clj.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://mlt.yj20258888.top

Ruby: // 手写 Hash
来源：http://vsn.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rul.316326.xyz

[N08] 生成全排列
来源：http://ryi.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://wxn.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://dwg.dashuyun.cn

JS:   // 手写回溯递归
来源：http://rhl.havefunace.top

TS:   // 手写回溯递归
来源：http://kir.sufxvd.cn

Java: // 手写回溯递归
来源：http://wdr.guowangkeji.top

Go:   // 手写回溯递归
来源：http://fqc.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://led.hammf.cn

C#:   // 手写回溯递归
来源：http://qdk.52xcode.cn

[N09] 栈与队列
来源：http://wyk.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mxa.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wmv.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tub.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sbp.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nkp.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pdc.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://djo.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zpd.xuetiantiany.cn

[N10] 链表节点定义
来源：http://yqf.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oyf.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xty.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qbk.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wmt.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://xxw.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://soc.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://eni.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vti.xziqi.cn

[N11] 二叉树中序遍历
来源：http://nny.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://scq.bbcook.cn

PHP:  // 手写递归函数
来源：http://tsu.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fvi.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nir.hongshengwenyu.top

Java: // 手写递归
来源：http://wqp.sweek.top

Go:   // 手写递归
来源：http://cae.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uiq.xylfe.cn

C#:   // 手写递归
来源：http://vqe.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tlk.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rtg.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rho.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mlt.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpl.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wqv.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qqy.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kif.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ynn.quarkkingdee.top

================================================================================
来源：http://bjf.svipenyu.cn

O. 并发与异步
来源：http://mjh.ydzc1.top

================================================================================
来源：http://ksc.gaohongyu789.top

[O01] 启动一个线程
来源：http://ipt.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://roo.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uws.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mqk.smart0.xyz

TS:   // 同 JS
来源：http://czr.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://erh.fehbvm.com

Go:   go f()
来源：http://ans.yj20258888.top

Ruby: Thread.new { f }
来源：http://agp.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://qjs.pengpengdd.cyou

[O02] 使用线程池
来源：http://riv.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rzy.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bms.316326.xyz

JS:   // worker_threads 线程池
来源：http://oia.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ilq.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fho.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iso.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bne.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iwc.hcnkem.com

[O03] 加锁保护共享数据
来源：http://ubo.jiagoushi.top

Py:   with lock: shared += 1
来源：http://uac.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://rth.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://heg.nwbrower.top

TS:   // 同 JS
来源：http://uhw.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://knn.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fvp.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://anl.zdqjudy.top

C#:   lock (gate) { shared++; }
来源：http://eoq.meibo888.top

[O04] 定义异步函数并等待
来源：http://zji.tanke756.top

Py:   async def f():⏎    await g()
来源：http://kxr.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lis.daria6918.cn

JS:   async function f() { await g(); }
来源：http://wog.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://cpj.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sav.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nob.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://mpf.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://hvh.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://uuz.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://rid.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kzm.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://drm.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://zld.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nko.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gar.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://fwl.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://blw.sjlbkw.cn

[O06] 使用进程池
来源：http://fbs.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dsy.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qlv.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://pmt.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://zwj.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rca.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yzc.nwbrower.top

Ruby: // fork 块
来源：http://ixt.sysykeji.top

C#:   Parallel.For
来源：http://ttm.zycfv.cn

================================================================================
来源：http://wpg.guowangkeji.top

P. 常用工具函数
来源：http://ijs.sjlbkw.cn

================================================================================
来源：http://bsm.xuanzx.com

[P01] 生成 UUID
来源：http://doh.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://hnq.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wjj.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://cgo.jianghu66.top

TS:   crypto.randomUUID()
来源：http://hxy.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://hei.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://ppk.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://xkn.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://pra.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://fzu.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ykw.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://obi.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fdi.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xtf.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nyj.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eqn.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gxr.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vbz.ppjwa.cn

[P03] 生成短随机字符串
来源：http://bmz.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vac.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wcb.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jzz.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqn.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hxu.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vpp.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://vot.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://flo.sxryk.cn

[P04] 求长度
来源：http://ayv.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wvo.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zxd.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rrt.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jzt.xuanzx.com


<!-- 参考信息 -->