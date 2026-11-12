代发 wailian999

Py:   resp.json()
来源：http://mkn.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://nek.zhijiandao.cn

JS:   await resp.json()
来源：http://dsc.jiagoushi.top

TS:   await resp.json()
来源：http://lel.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ghq.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fxk.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://yfx.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hmq.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://nob.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://slk.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://afw.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://hjo.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://hma.zhiwuduotai.top

Java: resp.statusCode()
来源：http://sgw.cdnleiting.top

Go:   resp.StatusCode
来源：http://bhw.chenzaomai.com

Ruby: resp.code.to_i
来源：http://nry.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://zjs.cucudq.cn

[L08] 并发请求多个地址
来源：http://kle.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ume.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://fif.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fub.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsa.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cfd.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cem.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wsm.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nlq.fanxiaobao.xyz

================================================================================
来源：http://jhy.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://erz.tarul.cn

================================================================================
来源：http://via.zycfv.cn

[M01] 读取命令行参数
来源：http://kyt.ivvv.top

Py:   sys.argv[1:]
来源：http://bfo.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://upx.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://sfk.xziqi.cn

TS:   process.argv.slice(2)
来源：http://zdj.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://mdp.sjlbkw.cn

Go:   os.Args[1:]
来源：http://ydp.zdqjudy.top

Ruby: ARGV
来源：http://iwl.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://pdj.yuxming.cn

[M02] 读取环境变量
来源：http://shb.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://ypx.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ipn.chenlongwang.top

JS:   process.env.HOME
来源：http://cup.iojbl.cn

TS:   process.env.HOME
来源：http://uvu.andypj.xyz

Java: System.getenv("HOME")
来源：http://pmi.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ayw.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://ygi.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bcx.gogol.net.cn

[M03] 执行外部命令
来源：http://mld.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxo.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ygd.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tcb.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zeq.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hdp.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ozg.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://vmx.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://rgt.0kj1m.cn

[M04] 获取当前工作目录
来源：http://cyl.aibaodan.cn

Py:   os.getcwd()
来源：http://pep.zhoulong.xyz

PHP:  getcwd();
来源：http://bzu.sysykeji.top

JS:   process.cwd()
来源：http://qkd.chenlongwang.top

TS:   process.cwd()
来源：http://vkz.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://jed.uphjek.com

Go:   os.Getwd()
来源：http://brh.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://voz.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ftp.hnxiangtu.top

[M05] 设置退出码
来源：http://epa.zhongyouzk.top

Py:   sys.exit(1)
来源：http://bux.nanxuanxn.top

PHP:  exit(1);
来源：http://pos.smart0.xyz

JS:   process.exit(1)
来源：http://aou.havefunace.top

TS:   process.exit(1)
来源：http://ddj.jinghuilouyu.cn

Java: System.exit(1)
来源：http://eew.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://hhf.yj20258.top

Ruby: exit 1
来源：http://oim.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hme.zhixingplan.top

[M06] 向标准错误输出
来源：http://mch.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://vjg.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://yus.xziqi.cn

JS:   console.error("err")
来源：http://nda.yonumen.top

TS:   console.error("err")
来源：http://brv.nanxinkj.top

Java: System.err.println("err")
来源：http://osf.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eqw.jlsjyb.cn

Ruby: warn "err"
来源：http://wfe.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://ety.uphjek.com

[M07] 判断是否为主入口
来源：http://edk.havefunace.top

Py:   if __name__ == "__main__":
来源：http://qbu.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ter.gaohongyu789.top

JS:   require.main === module
来源：http://ioc.hesvh.cn

TS:   require.main === module
来源：http://muu.havefunace.top

Java: public static void main(String[] args)
来源：http://tys.nanxuanxn.top

Go:   func main()
来源：http://rbi.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdq.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://mgt.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://opg.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://lja.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://hfs.andypj.xyz

JS:   process.platform;  process.version
来源：http://ona.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://noo.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kcl.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vyl.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vbj.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ngv.bbcook.cn

================================================================================
来源：http://kjv.gzhubu.top

N. 数据结构与算法
来源：http://wgf.fanxiaobao.xyz

================================================================================
来源：http://axg.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://hmp.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cbh.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yyv.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izk.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://guo.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://atn.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://vuz.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kyi.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://gsd.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://jww.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://svc.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aqy.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bva.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pkm.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yqb.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://gij.chenjidiqi.icu

Ruby: arr.sort
来源：http://xtk.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eft.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://nvd.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vma.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://loq.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gki.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jqi.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gaw.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xrt.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xhh.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://owd.aizwys.cn

[N04] 斐波那契数列
来源：http://uts.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://urt.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zot.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgr.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ttg.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ruz.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pta.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vhc.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lol.shzxlz.cn

[N05] 最大公约数
来源：http://lqd.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://hbp.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jjj.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ulf.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zig.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://myb.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xcq.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://yhr.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://now.yj20258888.top

[N06] 判断回文字符串
来源：http://wrh.yj202588.top

Py:   s == s[::-1]
来源：http://nxz.bjfxy.top

PHP:  $s === strrev($s);
来源：http://dgw.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://sgt.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://bob.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cgu.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://rnf.yanxiufei.cn

Ruby: s == s.reverse
来源：http://bph.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://faq.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://bqg.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ert.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yoo.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gda.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://mxs.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://wdv.yueranfly.top

Go:   // 手写 map[int]int
来源：http://pxq.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://eom.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://azf.nanxinkj.top

[N08] 生成全排列
来源：http://ugk.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://kdc.vehdjk.com

PHP:  // 手写递归交换
来源：http://jtq.fktsv.cn

JS:   // 手写回溯递归
来源：http://fcp.jqgfzy.top

TS:   // 手写回溯递归
来源：http://ndq.hammf.cn

Java: // 手写回溯递归
来源：http://vyc.fehbvm.com

Go:   // 手写回溯递归
来源：http://kns.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://zty.uphjek.com

C#:   // 手写回溯递归
来源：http://sfx.gaohongyu789.top

[N09] 栈与队列
来源：http://soe.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ceg.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ziv.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tyn.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mxo.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baj.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://luz.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tbj.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dhp.jiagoushi.top

[N10] 链表节点定义
来源：http://aep.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vlf.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://aiq.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kbw.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bko.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://omv.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ajv.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://veq.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xjb.vehdjk.com

[N11] 二叉树中序遍历
来源：http://wfl.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fsx.zhengqikj.top

PHP:  // 手写递归函数
来源：http://oqe.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ieg.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uvn.feifeiyinyue.top

Java: // 手写递归
来源：http://zrw.xinyue.icu

Go:   // 手写递归
来源：http://hzj.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nfh.dashuyun.cn

C#:   // 手写递归
来源：http://rcw.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mld.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fjp.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://riw.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eec.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cpr.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qym.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qlh.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gpe.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rtv.cheryme.top

================================================================================
来源：http://zoq.feifeiyinyue.top

O. 并发与异步
来源：http://wah.andypj.xyz

================================================================================
来源：http://cvw.jiagoushi.top

[O01] 启动一个线程
来源：http://qrh.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://liq.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ipn.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://les.sysykeji.top

TS:   // 同 JS
来源：http://akm.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://lgc.zhaomingkeji.xyz

Go:   go f()
来源：http://euy.vehdjk.com

Ruby: Thread.new { f }
来源：http://azy.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://wwn.hnqzz.top

[O02] 使用线程池
来源：http://fou.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cop.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yth.hcnkem.com

JS:   // worker_threads 线程池
来源：http://ulk.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://fjs.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://hzy.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yev.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sji.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ayw.cheryme.top

[O03] 加锁保护共享数据
来源：http://qec.sufxvd.cn

Py:   with lock: shared += 1
来源：http://qtc.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://tjp.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://syt.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://ghl.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://tqv.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nmg.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fgd.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://voa.ydzc1.top

[O04] 定义异步函数并等待
来源：http://pge.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://hxm.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rxq.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://vyg.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://gxl.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xqh.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ggh.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://nvt.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://nin.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://dac.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://ucx.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yuo.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://ede.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://gnx.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://twr.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gay.cucudq.cn

Ruby: threads.map(&:join)
来源：http://yvm.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://wsu.fanxiaobao.xyz

[O06] 使用进程池
来源：http://elg.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sfk.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hbm.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://ewn.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://nyb.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfr.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ogy.zhixingplan.top

Ruby: // fork 块
来源：http://xia.52xcode.cn

C#:   Parallel.For
来源：http://ymp.gogol.net.cn

================================================================================
来源：http://arw.sjlbkw.cn

P. 常用工具函数
来源：http://rru.havefunace.top

================================================================================
来源：http://ver.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://voq.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://chs.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dxw.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://rhr.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://umg.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://voh.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://zey.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://vxm.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://jom.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://kyu.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sfw.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://chu.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pva.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ufr.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yco.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qhf.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sxo.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nkl.xylfe.cn

[P03] 生成短随机字符串
来源：http://hiv.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fru.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vts.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kht.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tts.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yrx.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yzn.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://lqh.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qow.feifeiyinyue.top

[P04] 求长度
来源：http://wku.xingfuxueyuan.xyz


<!-- 参考信息 -->