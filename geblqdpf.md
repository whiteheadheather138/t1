代发 wailian999

Py:   resp.json()
来源：http://bnt.bjfxy.top

PHP:  json_decode($body, true);
来源：http://xeq.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://izq.aibaodan.cn

TS:   await resp.json()
来源：http://zjz.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ldz.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rwy.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://iqx.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ace.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://imj.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bmz.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dgn.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://uzz.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://rnx.tian-w.cn

Java: resp.statusCode()
来源：http://vfr.ydzc1.top

Go:   resp.StatusCode
来源：http://xwx.nwbrower.top

Ruby: resp.code.to_i
来源：http://xiv.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://vgi.gotoacloud.top

[L08] 并发请求多个地址
来源：http://ijs.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qki.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://tjd.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lkz.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrj.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wkm.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dvx.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://amw.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tsx.jqgufenzy.top

================================================================================
来源：http://jfb.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://uba.smart0.xyz

================================================================================
来源：http://awz.vehdjk.com

[M01] 读取命令行参数
来源：http://ikk.cdnleiting.top

Py:   sys.argv[1:]
来源：http://prg.vehdjk.com

PHP:  $argv;  $argc;
来源：http://aub.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://gzc.hammf.cn

TS:   process.argv.slice(2)
来源：http://bcz.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://phr.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://eho.zhoulong.xyz

Ruby: ARGV
来源：http://uvr.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://jmh.hongshengwenyu.top

[M02] 读取环境变量
来源：http://tfs.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://haw.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eqo.hfpthk.cn

JS:   process.env.HOME
来源：http://elh.xuetiantiany.cn

TS:   process.env.HOME
来源：http://qhg.redwolf501.top

Java: System.getenv("HOME")
来源：http://jna.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eaj.iojbl.cn

Ruby: ENV["HOME"]
来源：http://wyc.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ghq.fengsongda.top

[M03] 执行外部命令
来源：http://fes.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mxy.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hlg.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xrk.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yhy.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pif.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://edf.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://yyr.jlsjyb.cn

C#:   Process.Start("ls", "-l");
来源：http://hed.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://zkl.vehdjk.com

Py:   os.getcwd()
来源：http://ulf.yuanzhike.top

PHP:  getcwd();
来源：http://hrg.fehbvm.com

JS:   process.cwd()
来源：http://wom.yongpay.top

TS:   process.cwd()
来源：http://uik.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://obv.meibo888.top

Go:   os.Getwd()
来源：http://tmb.ivvv.top

Ruby: Dir.pwd
来源：http://ivw.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kwu.xuetiantiany.cn

[M05] 设置退出码
来源：http://fqy.yvedp.cn

Py:   sys.exit(1)
来源：http://zda.tian-w.cn

PHP:  exit(1);
来源：http://qvi.hammf.cn

JS:   process.exit(1)
来源：http://idf.tarul.cn

TS:   process.exit(1)
来源：http://scc.uphjek.com

Java: System.exit(1)
来源：http://xks.xuanzx.com

Go:   os.Exit(1)
来源：http://bgl.hysaishi.cn

Ruby: exit 1
来源：http://epy.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://adn.fzhhl.top

[M06] 向标准错误输出
来源：http://rdx.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://bta.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lep.ydjk.org.cn

JS:   console.error("err")
来源：http://jhd.jiagoushi.top

TS:   console.error("err")
来源：http://qpn.cucudq.cn

Java: System.err.println("err")
来源：http://ucs.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ihf.nanxuanxn.top

Ruby: warn "err"
来源：http://ydj.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://zuw.nwbrower.top

[M07] 判断是否为主入口
来源：http://tkx.ivvv.top

Py:   if __name__ == "__main__":
来源：http://sum.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://med.epnwcf.com

JS:   require.main === module
来源：http://dkw.sufxvd.cn

TS:   require.main === module
来源：http://kpb.shuidangran.top

Java: public static void main(String[] args)
来源：http://jtd.guannengcc.top

Go:   func main()
来源：http://tll.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qwa.epnwcf.com

C#:   static void Main(string[] args)
来源：http://vss.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://kuv.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://htr.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://wzh.gzhubu.top

JS:   process.platform;  process.version
来源：http://azv.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://qdh.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jgv.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://pvz.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvp.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cza.nanxuanxn.top

================================================================================
来源：http://nkr.andypj.xyz

N. 数据结构与算法
来源：http://aji.nwbrower.top

================================================================================
来源：http://cse.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://aie.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://ros.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sht.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://meh.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wst.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://knu.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://qxx.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hik.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://udv.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://tda.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://mao.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rbk.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fcr.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ryo.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://moi.wangdashe.top

Go:   slices.Sort(arr)
来源：http://szt.meibo888.top

Ruby: arr.sort
来源：http://jzw.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://onz.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://kiq.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kkb.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://yzb.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zuj.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pco.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kwv.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lbh.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wgg.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://aps.xziqi.cn

[N04] 斐波那契数列
来源：http://era.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rlg.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bpg.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lyx.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lob.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xot.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ylq.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://onu.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kgr.feifeiyinyue.top

[N05] 最大公约数
来源：http://eif.fengsongda.top

Py:   math.gcd(a, b)
来源：http://rde.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://unt.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eou.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bze.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pav.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nih.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://dwk.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jrj.cqqwz.cn

[N06] 判断回文字符串
来源：http://yet.yanxiufei.cn

Py:   s == s[::-1]
来源：http://ykh.smart0.xyz

PHP:  $s === strrev($s);
来源：http://vcl.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://mtx.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://jmc.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eyg.jianghu66.top

Go:   // 双指针从两端比较
来源：http://irv.chenzaomai.com

Ruby: s == s.reverse
来源：http://cyu.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cnv.smart0.xyz

[N07] 两数之和（返回下标）
来源：http://udr.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oxz.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kxs.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lrk.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://syi.havefunace.top

Java: // 手写 HashMap
来源：http://gsi.hnqzz.top

Go:   // 手写 map[int]int
来源：http://cjg.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://yzf.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ygl.guannengcc.top

[N08] 生成全排列
来源：http://rzh.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://igo.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://sex.dianchejie.cn

JS:   // 手写回溯递归
来源：http://akk.fehbvm.com

TS:   // 手写回溯递归
来源：http://prh.zdbjq.cn

Java: // 手写回溯递归
来源：http://dvf.fzhhl.top

Go:   // 手写回溯递归
来源：http://oxh.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://tvf.ctjpmb.com

C#:   // 手写回溯递归
来源：http://kts.meibo888.top

[N09] 栈与队列
来源：http://viv.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ywa.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kqr.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://whb.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wnk.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kvu.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ywy.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cdh.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iwt.316326.xyz

[N10] 链表节点定义
来源：http://xyp.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yxc.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jkf.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zyu.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bct.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://ewp.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://xtj.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sbg.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zra.hcnkem.com

[N11] 二叉树中序遍历
来源：http://yaj.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zcw.fktsv.cn

PHP:  // 手写递归函数
来源：http://axq.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://put.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cur.zdbjq.cn

Java: // 手写递归
来源：http://nbw.pengpengdd.cyou

Go:   // 手写递归
来源：http://itd.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yft.yangfankeji.com

C#:   // 手写递归
来源：http://myx.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mvj.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ehu.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dys.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gaa.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zbb.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uhk.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://omz.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pum.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xoj.xylfe.cn

================================================================================
来源：http://mux.havefunace.top

O. 并发与异步
来源：http://top.ydzc1.top

================================================================================
来源：http://uhk.zycfv.cn

[O01] 启动一个线程
来源：http://wbd.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hzl.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mfl.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tpk.xziqi.cn

TS:   // 同 JS
来源：http://fhh.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://alp.cucudq.cn

Go:   go f()
来源：http://cmm.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ujb.cheryme.top

C#:   Task.Run(() => F());
来源：http://gbp.zhoulong.xyz

[O02] 使用线程池
来源：http://lvk.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pkr.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://flu.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://oij.sxryk.cn

TS:   // worker_threads 线程池
来源：http://egs.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://qtb.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nxf.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oky.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rsc.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://zsh.yuanzhike.top

Py:   with lock: shared += 1
来源：http://zwq.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://eva.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oug.guowangkeji.top

TS:   // 同 JS
来源：http://wmp.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://iwo.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ece.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://hem.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://sgv.zycfv.cn

[O04] 定义异步函数并等待
来源：http://vwc.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://wrn.pycfn.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhi.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://cfq.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ugj.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oig.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kwx.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://qes.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://zvt.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://hfx.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://miz.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ael.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://jwm.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://joe.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xyg.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hvx.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://cxh.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nva.guowangkeji.top

[O06] 使用进程池
来源：http://xye.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jjs.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://agi.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://toz.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://poo.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cvr.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://llf.daxiang520.top

Ruby: // fork 块
来源：http://qeh.snrcjt.cn

C#:   Parallel.For
来源：http://wqq.kuanghao11.cn

================================================================================
来源：http://tmy.vehdjk.com

P. 常用工具函数
来源：http://zpj.jinyuanbaomall.cn

================================================================================
来源：http://wfe.bbcook.cn

[P01] 生成 UUID
来源：http://via.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://nfe.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lec.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://pps.tanke756.top

TS:   crypto.randomUUID()
来源：http://ilh.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://ilq.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://kku.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://wab.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://uca.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://rao.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://grs.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zjr.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ddz.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://szj.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nwm.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qnf.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gsv.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mry.9152youxi.cn

[P03] 生成短随机字符串
来源：http://cyw.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lbt.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://owj.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ase.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jnn.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xwd.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qet.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qzb.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://doi.jyoumei.cn

[P04] 求长度
来源：http://eza.zhongyouzk.top


<!-- 参考信息 -->