代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dmz.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://obi.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://wcq.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jht.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://trp.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ocz.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fdt.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://zrl.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://ymq.jqgfzy.top

Java: resp.statusCode()
来源：http://hjm.jianghu66.top

Go:   resp.StatusCode
来源：http://blx.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://xxu.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://vnv.haohaochexian.top

[L08] 并发请求多个地址
来源：http://bpy.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rtx.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://cif.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozj.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://azr.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eaw.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tdz.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vab.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://evy.pycfn.com

================================================================================
来源：http://ifx.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ewc.ydzc1.top

================================================================================
来源：http://veb.yonumen.top

[M01] 读取命令行参数
来源：http://uct.tanke756.top

Py:   sys.argv[1:]
来源：http://wip.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://ggy.fktsv.cn

JS:   process.argv.slice(2)
来源：http://pkj.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://vvx.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://nmx.xziqi.cn

Go:   os.Args[1:]
来源：http://bxi.yuxming.cn

Ruby: ARGV
来源：http://mth.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://rng.yuxming.cn

[M02] 读取环境变量
来源：http://uat.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://bnm.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gxp.chenjidiqi.icu

JS:   process.env.HOME
来源：http://eci.jyoumei.cn

TS:   process.env.HOME
来源：http://swn.hesvh.cn

Java: System.getenv("HOME")
来源：http://jnl.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wiv.xylfe.cn

Ruby: ENV["HOME"]
来源：http://igv.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fio.chenjidiqi.icu

[M03] 执行外部命令
来源：http://tho.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dqh.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xyi.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://onl.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ewm.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rmo.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dma.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://ncf.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://drl.daxiang520.top

[M04] 获取当前工作目录
来源：http://gwd.yangfankeji.com

Py:   os.getcwd()
来源：http://lfq.yueranfly.top

PHP:  getcwd();
来源：http://zde.pengpengdd.cyou

JS:   process.cwd()
来源：http://kgg.bbcook.cn

TS:   process.cwd()
来源：http://dda.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://swl.yvedp.cn

Go:   os.Getwd()
来源：http://bbo.sweek.top

Ruby: Dir.pwd
来源：http://ehx.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xhf.wangdashe.top

[M05] 设置退出码
来源：http://rjg.gzhubu.top

Py:   sys.exit(1)
来源：http://vyq.hnxiangtu.top

PHP:  exit(1);
来源：http://tcr.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://hab.meibo888.top

TS:   process.exit(1)
来源：http://qwa.daxiang520.top

Java: System.exit(1)
来源：http://bzj.bjfxy.top

Go:   os.Exit(1)
来源：http://igf.jyoumei.cn

Ruby: exit 1
来源：http://gfn.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ffu.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://ddn.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://fzs.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gmd.wangdashe.top

JS:   console.error("err")
来源：http://euh.uphjek.com

TS:   console.error("err")
来源：http://nab.hnqzz.top

Java: System.err.println("err")
来源：http://izp.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uup.jinqigfzy.top

Ruby: warn "err"
来源：http://cxu.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://nat.mhx1999.top

[M07] 判断是否为主入口
来源：http://ssc.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://snx.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nor.jlsjyb.cn

JS:   require.main === module
来源：http://wao.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://fzz.shuidangran.top

Java: public static void main(String[] args)
来源：http://qlh.zhengqikj.top

Go:   func main()
来源：http://azr.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mkl.tanke756.top

C#:   static void Main(string[] args)
来源：http://mos.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://yvq.shzxlz.cn

Py:   platform.system();  platform.python_version()
来源：http://vsc.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://ucm.yueranfly.top

JS:   process.platform;  process.version
来源：http://prz.nanxinkj.top

TS:   process.platform;  process.version
来源：http://gws.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sxc.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jer.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://svn.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xkr.fengsongda.top

================================================================================
来源：http://xlj.nwbrower.top

N. 数据结构与算法
来源：http://xxv.jlsjyb.cn

================================================================================
来源：http://pth.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://ujd.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://cgh.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gil.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://inu.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vof.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://aqe.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://hoa.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://flz.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://tbz.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://bzx.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://kbo.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xwv.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vok.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ini.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ssq.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://tno.0kj1m.cn

Ruby: arr.sort
来源：http://wsp.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rgf.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://ghv.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pwz.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://von.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtc.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qez.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zse.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ccd.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gaf.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://sib.hysaishi.cn

[N04] 斐波那契数列
来源：http://pxl.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aho.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wtj.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fwd.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mmc.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzv.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lvf.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aug.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://htq.shangyingyoupin.top

[N05] 最大公约数
来源：http://kml.wangdashe.top

Py:   math.gcd(a, b)
来源：http://jna.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hdx.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohk.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgt.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iyi.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cah.snrcjt.cn

Ruby: a.gcd(b)
来源：http://ajo.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jle.redwolf501.top

[N06] 判断回文字符串
来源：http://oja.zhengqikj.top

Py:   s == s[::-1]
来源：http://myl.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://ywx.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://awz.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://aeo.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ril.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://yjw.ydjk.org.cn

Ruby: s == s.reverse
来源：http://uiz.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mvk.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://spb.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oor.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://abn.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oao.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://zsl.jqgfzy.top

Java: // 手写 HashMap
来源：http://hso.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://fwq.cashguo.top

Ruby: // 手写 Hash
来源：http://hvm.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sdn.tanke756.top

[N08] 生成全排列
来源：http://tcu.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://bda.snrcjt.cn

PHP:  // 手写递归交换
来源：http://lkr.andypj.xyz

JS:   // 手写回溯递归
来源：http://pob.daria6918.cn

TS:   // 手写回溯递归
来源：http://thm.jyoumei.cn

Java: // 手写回溯递归
来源：http://jmw.shuidangran.top

Go:   // 手写回溯递归
来源：http://btg.yonumen.top

Ruby: arr.permutation.to_a
来源：http://xvh.cheryme.top

C#:   // 手写回溯递归
来源：http://ysz.316326.xyz

[N09] 栈与队列
来源：http://iqv.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vdf.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rak.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hsd.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cvr.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kuj.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://svn.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mcr.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uqn.vqdsnc.cn

[N10] 链表节点定义
来源：http://flg.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsc.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ysm.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://svg.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pet.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://iet.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://hsu.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dla.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jux.c1oappe.top

[N11] 二叉树中序遍历
来源：http://nin.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ben.xuanzx.com

PHP:  // 手写递归函数
来源：http://btb.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://trd.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tqb.jinghuilouyu.cn

Java: // 手写递归
来源：http://mhg.ybcxt.top

Go:   // 手写递归
来源：http://xot.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ytw.c1oappe.top

C#:   // 手写递归
来源：http://kyg.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wrx.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://the.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wkd.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thb.redwolf501.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gry.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zpf.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pua.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yac.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://twi.hesvh.cn

================================================================================
来源：http://hwv.ydjk.org.cn

O. 并发与异步
来源：http://lxu.zhijiandao.cn

================================================================================
来源：http://wpa.jlsjyb.cn

[O01] 启动一个线程
来源：http://bbz.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ujv.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pnx.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fnr.pengpengdd.cyou

TS:   // 同 JS
来源：http://awf.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://vqc.fanxiaobao.xyz

Go:   go f()
来源：http://yjp.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://xkr.yj20258.top

C#:   Task.Run(() => F());
来源：http://ihs.tianlin.xyz

[O02] 使用线程池
来源：http://dtk.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://udo.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fjh.hnqzz.top

JS:   // worker_threads 线程池
来源：http://lwz.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://fhk.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://dkg.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ubl.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ehk.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ymt.bjfxy.top

[O03] 加锁保护共享数据
来源：http://qmi.jqgfzy.top

Py:   with lock: shared += 1
来源：http://pdz.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://jxb.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hup.shangyingyoupin.top

TS:   // 同 JS
来源：http://lqi.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://pqu.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://drx.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eyh.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://dgc.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://djb.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://xdp.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wwk.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://lzz.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gxt.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://szg.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kbe.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://doi.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://uzv.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://soy.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://zfo.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cal.316326.xyz

JS:   await Promise.all(tasks)
来源：http://wth.sweek.top

TS:   await Promise.all(tasks)
来源：http://tpq.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eig.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xrc.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://mva.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jog.tian-w.cn

[O06] 使用进程池
来源：http://ovl.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iqw.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xyy.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://gnv.yj20258.top

TS:   // child_process / cluster 模块
来源：http://ecj.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zai.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pms.xylfe.cn

Ruby: // fork 块
来源：http://qpy.hysaishi.cn

C#:   Parallel.For
来源：http://kzm.jinqigufen.top

================================================================================
来源：http://dej.zhijiandao.cn

P. 常用工具函数
来源：http://bth.jianghu66.top

================================================================================
来源：http://wgi.chenjidiqi.icu

[P01] 生成 UUID
来源：http://vnv.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://cwo.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wfe.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://chu.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://aav.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://bcn.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://vzp.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://nse.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://spq.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://wde.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fgv.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yae.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xby.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vxe.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bhq.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jjf.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uzf.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rux.yonumen.top

[P03] 生成短随机字符串
来源：http://xdf.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://goe.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://olm.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yrm.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zaj.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lij.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jcy.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cpi.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mvc.fengsongda.top

[P04] 求长度
来源：http://oph.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cee.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxw.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zbx.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhg.ywan-chungtsiang.top


<!-- 参考信息 -->