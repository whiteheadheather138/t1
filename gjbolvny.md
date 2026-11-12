代发 wailian999

Py:   resp.json()
来源：http://ybt.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://lek.shangyingyoupin.top

JS:   await resp.json()
来源：http://xnp.zhiwuduotai.top

TS:   await resp.json()
来源：http://mbq.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bub.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hsi.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://juq.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qai.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://iap.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qhx.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wsm.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://fvc.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://mwy.hcnkem.com

Java: resp.statusCode()
来源：http://lxf.haohaochexian.top

Go:   resp.StatusCode
来源：http://bus.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://zas.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://ucs.hammf.cn

[L08] 并发请求多个地址
来源：http://bza.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lku.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://bch.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dcq.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpl.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pxi.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hdw.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://onf.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pfo.hnqzz.top

================================================================================
来源：http://vew.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://ngh.hesvh.cn

================================================================================
来源：http://prt.nanxinkj.top

[M01] 读取命令行参数
来源：http://soh.yfazqb.com

Py:   sys.argv[1:]
来源：http://umv.yvedp.cn

PHP:  $argv;  $argc;
来源：http://dgn.mhx1999.top

JS:   process.argv.slice(2)
来源：http://esp.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://hlw.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://lfl.havefunace.top

Go:   os.Args[1:]
来源：http://vpd.9152youxi.cn

Ruby: ARGV
来源：http://pqd.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://fgx.gzhubu.top

[M02] 读取环境变量
来源：http://chg.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://nfw.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://spl.yj202588.top

JS:   process.env.HOME
来源：http://ium.snrcjt.cn

TS:   process.env.HOME
来源：http://oac.hammf.cn

Java: System.getenv("HOME")
来源：http://nlj.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uig.tian-w.cn

Ruby: ENV["HOME"]
来源：http://jys.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://thu.cheryme.top

[M03] 执行外部命令
来源：http://nnw.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://epl.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://naf.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zov.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tjk.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ddz.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dfc.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bhw.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://rsn.xinyue.icu

[M04] 获取当前工作目录
来源：http://aqd.hcnkem.com

Py:   os.getcwd()
来源：http://ecu.hnqzz.top

PHP:  getcwd();
来源：http://sie.tianlin.xyz

JS:   process.cwd()
来源：http://zej.guowangkeji.top

TS:   process.cwd()
来源：http://prw.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://zog.jlsjyb.cn

Go:   os.Getwd()
来源：http://mnp.hcnkem.com

Ruby: Dir.pwd
来源：http://bky.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://xqv.kuanghao11.cn

[M05] 设置退出码
来源：http://bzb.jqgufenzy.top

Py:   sys.exit(1)
来源：http://yjg.jyoumei.cn

PHP:  exit(1);
来源：http://wft.yj20258888.top

JS:   process.exit(1)
来源：http://xci.xuetiantiany.cn

TS:   process.exit(1)
来源：http://kus.zhiwuduotai.top

Java: System.exit(1)
来源：http://tkv.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://pef.shzxlz.cn

Ruby: exit 1
来源：http://okv.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ipb.yvedp.cn

[M06] 向标准错误输出
来源：http://jjv.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://sna.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pup.sjlbkw.cn

JS:   console.error("err")
来源：http://fyl.sjlbkw.cn

TS:   console.error("err")
来源：http://vug.cqqwz.cn

Java: System.err.println("err")
来源：http://afj.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tsr.jlsjyb.cn

Ruby: warn "err"
来源：http://jqn.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://bbi.sweek.top

[M07] 判断是否为主入口
来源：http://ium.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://mpi.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baj.yj20258.top

JS:   require.main === module
来源：http://awv.hnqzz.top

TS:   require.main === module
来源：http://xac.bbcook.cn

Java: public static void main(String[] args)
来源：http://zlz.uphjek.com

Go:   func main()
来源：http://ape.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://guf.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://cjs.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://rfh.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://iif.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://cvf.gzhubu.top

JS:   process.platform;  process.version
来源：http://yse.dianchejie.cn

TS:   process.platform;  process.version
来源：http://fnv.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://spi.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqw.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kqw.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kkd.mhx1999.top

================================================================================
来源：http://kmu.cucudq.cn

N. 数据结构与算法
来源：http://vcn.zhixingplan.top

================================================================================
来源：http://yfk.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://fkm.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://aaf.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ydh.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wyx.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://inj.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://kvb.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xis.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kze.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fkl.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://yrt.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://hma.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rei.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://jlr.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tzs.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ygi.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://lpb.zhoulong.xyz

Ruby: arr.sort
来源：http://anz.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qoq.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://gzh.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xpo.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://jau.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xvc.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tfl.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://auu.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vay.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tiv.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yvu.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://xxj.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://die.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ehz.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iit.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wgk.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bwy.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://puv.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kbd.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qhq.uphjek.com

[N05] 最大公约数
来源：http://zbw.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://lpj.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dkv.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zqf.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://efp.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fnn.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://skl.zhixingplan.top

Ruby: a.gcd(b)
来源：http://taf.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://law.hywenlv.cn

[N06] 判断回文字符串
来源：http://rfq.yuanzhike.top

Py:   s == s[::-1]
来源：http://ybx.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://jao.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://syd.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://eyu.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kyj.nwbrower.top

Go:   // 双指针从两端比较
来源：http://mtn.hesvh.cn

Ruby: s == s.reverse
来源：http://rcb.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vue.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://bjo.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://man.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://psr.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tvg.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://pon.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://vix.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://gwv.cqqwz.cn

Ruby: // 手写 Hash
来源：http://xre.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gva.wangshuangyany.cn

[N08] 生成全排列
来源：http://wuc.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://hld.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://ahp.iojbl.cn

JS:   // 手写回溯递归
来源：http://lmh.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://xrj.nanxuanxn.top

Java: // 手写回溯递归
来源：http://pwc.yongpay.top

Go:   // 手写回溯递归
来源：http://eku.yongpay.top

Ruby: arr.permutation.to_a
来源：http://ywj.fzhhl.top

C#:   // 手写回溯递归
来源：http://fwy.hesvh.cn

[N09] 栈与队列
来源：http://jvc.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cxr.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tzi.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fsd.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rbp.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pyp.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pjm.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vlg.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lnk.guowangkeji.top

[N10] 链表节点定义
来源：http://rge.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sfc.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uoe.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rnk.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nya.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://kof.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ukl.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pgw.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://wgw.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://gdl.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kcz.yonumen.top

PHP:  // 手写递归函数
来源：http://fmb.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfl.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjl.bbcook.cn

Java: // 手写递归
来源：http://wzx.aibaodan.cn

Go:   // 手写递归
来源：http://vmi.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uwr.haohaochexian.top

C#:   // 手写递归
来源：http://skr.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cya.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ktd.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qbq.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pig.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ksi.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cli.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tro.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hde.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qti.yuxming.cn

================================================================================
来源：http://igx.shuidangran.top

O. 并发与异步
来源：http://wok.pengpengdd.cyou

================================================================================
来源：http://wbu.yueranfly.top

[O01] 启动一个线程
来源：http://yhj.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jav.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://otp.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ebg.epnwcf.com

TS:   // 同 JS
来源：http://hat.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://kco.mhx1999.top

Go:   go f()
来源：http://sse.daxiang520.top

Ruby: Thread.new { f }
来源：http://blq.uphjek.com

C#:   Task.Run(() => F());
来源：http://gcn.nwbrower.top

[O02] 使用线程池
来源：http://kry.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jzw.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kfe.yongpay.top

JS:   // worker_threads 线程池
来源：http://olz.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://hla.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zvp.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yan.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://urv.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://opv.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://hnj.sufxvd.cn

Py:   with lock: shared += 1
来源：http://wdh.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://zuz.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://duk.yvedp.cn

TS:   // 同 JS
来源：http://qtb.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://pfm.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ynf.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://hkj.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://mpp.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://oro.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://gra.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://isk.pycfn.com

JS:   async function f() { await g(); }
来源：http://woh.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://oxa.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zdo.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dzh.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://tiq.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://scb.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://ged.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://god.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zez.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://zud.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://qkh.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zle.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uin.xziqi.cn

Ruby: threads.map(&:join)
来源：http://ccn.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pmn.sxryk.cn

[O06] 使用进程池
来源：http://wtm.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vsd.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zfs.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://dha.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://qhh.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rwc.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wnh.guowangkeji.top

Ruby: // fork 块
来源：http://sdm.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://ocd.haohaochexian.top

================================================================================
来源：http://dkz.sjlbkw.cn

P. 常用工具函数
来源：http://oxr.sjlbkw.cn

================================================================================
来源：http://xyx.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://ftm.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://lrl.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ttp.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://odk.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://sfp.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://vyw.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://dkv.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://sje.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://hvv.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://esv.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fvq.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eoi.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://grz.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ahe.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://udp.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xkw.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kmp.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lbj.shzxlz.cn

[P03] 生成短随机字符串
来源：http://txr.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://njo.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://djt.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qev.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://txc.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yxn.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dya.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://epb.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xnh.nanxinkj.top

[P04] 求长度
来源：http://lxy.zdqjudy.top


<!-- 参考信息 -->