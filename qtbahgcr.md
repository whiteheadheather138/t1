代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://exq.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jaa.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qkh.cheryme.top

JS:   resp.ok;  resp.status
来源：http://pnc.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://bgz.sxryk.cn

Java: resp.statusCode()
来源：http://lia.sxryk.cn

Go:   resp.StatusCode
来源：http://ejm.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://hkr.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://dpx.hesvh.cn

[L08] 并发请求多个地址
来源：http://oba.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iss.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://kfo.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pop.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihl.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bcw.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zco.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vnm.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://odr.yj202588.top

================================================================================
来源：http://wel.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://lgi.jianghu66.top

================================================================================
来源：http://mct.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://xuu.c1oappe.top

Py:   sys.argv[1:]
来源：http://svs.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://lso.fengsongda.top

JS:   process.argv.slice(2)
来源：http://vkg.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://ozu.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://sfu.9152youxi.cn

Go:   os.Args[1:]
来源：http://elx.cashguo.top

Ruby: ARGV
来源：http://ztn.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://usy.316326.xyz

[M02] 读取环境变量
来源：http://wpe.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://ftc.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pfm.chenjidiqi.icu

JS:   process.env.HOME
来源：http://lxk.yonumen.top

TS:   process.env.HOME
来源：http://udm.sysykeji.top

Java: System.getenv("HOME")
来源：http://dvk.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cfp.zycfv.cn

Ruby: ENV["HOME"]
来源：http://ytc.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://doo.tianlin.xyz

[M03] 执行外部命令
来源：http://bhh.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fwu.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ngx.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ado.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iyz.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://epn.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cph.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://rny.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://nxb.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://fkx.fktsv.cn

Py:   os.getcwd()
来源：http://ilj.iojbl.cn

PHP:  getcwd();
来源：http://jar.jinqigufen.top

JS:   process.cwd()
来源：http://yhj.tarul.cn

TS:   process.cwd()
来源：http://zka.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://wzy.gogol.net.cn

Go:   os.Getwd()
来源：http://zoj.hcnkem.com

Ruby: Dir.pwd
来源：http://wss.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://mfw.jlsjyb.cn

[M05] 设置退出码
来源：http://dkr.mhx1999.top

Py:   sys.exit(1)
来源：http://vqc.xinyue.icu

PHP:  exit(1);
来源：http://gnp.shzxlz.cn

JS:   process.exit(1)
来源：http://exb.shuidangran.top

TS:   process.exit(1)
来源：http://cjr.jinqigufen.top

Java: System.exit(1)
来源：http://weu.zycfv.cn

Go:   os.Exit(1)
来源：http://vzo.gotoacloud.top

Ruby: exit 1
来源：http://wuf.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vqe.haohaochexian.top

[M06] 向标准错误输出
来源：http://yej.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://mvt.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bav.pengpengdd.cyou

JS:   console.error("err")
来源：http://zmf.mhx1999.top

TS:   console.error("err")
来源：http://nyk.52xcode.cn

Java: System.err.println("err")
来源：http://kbk.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kmv.gzhubu.top

Ruby: warn "err"
来源：http://ntp.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://ege.wangdashe.top

[M07] 判断是否为主入口
来源：http://ehd.meibo888.top

Py:   if __name__ == "__main__":
来源：http://wnn.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mxj.hcnkem.com

JS:   require.main === module
来源：http://pab.ydjk.org.cn

TS:   require.main === module
来源：http://kpc.jinqigufen.top

Java: public static void main(String[] args)
来源：http://tdn.hesvh.cn

Go:   func main()
来源：http://imu.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cdb.yfazqb.com

C#:   static void Main(string[] args)
来源：http://gbj.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://pid.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://sht.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://xtk.iojbl.cn

JS:   process.platform;  process.version
来源：http://wxi.pycfn.com

TS:   process.platform;  process.version
来源：http://pbd.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rdz.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ytt.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sps.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oup.jyoumei.cn

================================================================================
来源：http://wlr.ehwqpu.com

N. 数据结构与算法
来源：http://hmu.gaohongyu789.top

================================================================================
来源：http://gho.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://ezl.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://lvg.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lgg.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jek.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dxm.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xwu.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://ihu.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cqm.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aps.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://pzr.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://eis.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aob.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://rzi.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cbx.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kxl.hammf.cn

Go:   slices.Sort(arr)
来源：http://veh.nwbrower.top

Ruby: arr.sort
来源：http://wop.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pir.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://coe.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ygp.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://yjk.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yuj.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgq.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zon.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://him.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zti.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://sym.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://nwn.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uam.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dpi.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://knq.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qdx.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qss.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://etp.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewm.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rvh.zhiwuduotai.top

[N05] 最大公约数
来源：http://dzf.yfazqb.com

Py:   math.gcd(a, b)
来源：http://qjq.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rty.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cky.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://abn.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dfj.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jnh.tarul.cn

Ruby: a.gcd(b)
来源：http://mtx.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ndc.wangdashe.top

[N06] 判断回文字符串
来源：http://nbf.zhoulong.xyz

Py:   s == s[::-1]
来源：http://pgv.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://svp.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://ucx.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://bix.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rsg.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://fxe.nanxinkj.top

Ruby: s == s.reverse
来源：http://hwa.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qlx.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://avc.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vln.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jon.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rsf.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://mwy.hcnkem.com

Java: // 手写 HashMap
来源：http://pjz.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://qnx.316326.xyz

Ruby: // 手写 Hash
来源：http://shu.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://czd.vqdsnc.cn

[N08] 生成全排列
来源：http://fre.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://fgs.ppjwa.cn

PHP:  // 手写递归交换
来源：http://pcv.jiagoushi.top

JS:   // 手写回溯递归
来源：http://sis.gogol.net.cn

TS:   // 手写回溯递归
来源：http://zcr.meibo888.top

Java: // 手写回溯递归
来源：http://pya.cheryme.top

Go:   // 手写回溯递归
来源：http://vnb.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://uwr.ybcxt.top

C#:   // 手写回溯递归
来源：http://wuz.cqqwz.cn

[N09] 栈与队列
来源：http://fei.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uog.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xgb.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tpj.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://beb.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ppz.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qwm.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://krb.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cjb.jinqigfzy.top

[N10] 链表节点定义
来源：http://wpo.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vrc.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iay.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nus.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gjh.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://fyc.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://cqu.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rth.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tyj.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://eox.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ljz.pycfn.com

PHP:  // 手写递归函数
来源：http://hip.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://epk.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlp.quarkkingdee.top

Java: // 手写递归
来源：http://wyx.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://lrr.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nwz.shzxlz.cn

C#:   // 手写递归
来源：http://jwm.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nqa.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fix.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kre.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gfh.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mif.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oqb.yj202588.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zhs.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xfy.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eec.fktsv.cn

================================================================================
来源：http://ncw.xuanzx.com

O. 并发与异步
来源：http://kdl.feifeiyinyue.top

================================================================================
来源：http://xkv.xuanzx.com

[O01] 启动一个线程
来源：http://bhz.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vka.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ugp.svipenyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ofs.cashguo.top

TS:   // 同 JS
来源：http://dvv.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://kmx.yvedp.cn

Go:   go f()
来源：http://dbm.xuanzx.com

Ruby: Thread.new { f }
来源：http://zmr.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://qgf.yfazqb.com

[O02] 使用线程池
来源：http://xoo.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ckh.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bde.redwolf501.top

JS:   // worker_threads 线程池
来源：http://mjr.tian-w.cn

TS:   // worker_threads 线程池
来源：http://lqa.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://uho.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://obu.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sce.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kvs.hesvh.cn

[O03] 加锁保护共享数据
来源：http://lbj.hysaishi.cn

Py:   with lock: shared += 1
来源：http://ojj.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://dlm.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://app.xuanzx.com

TS:   // 同 JS
来源：http://buv.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://drt.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bit.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://woj.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://jve.uphjek.com

[O04] 定义异步函数并等待
来源：http://osx.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://gjh.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zwv.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://gjf.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yfj.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lcj.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://noz.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://pfn.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://dfe.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://bbq.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://hwq.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://heo.yonumen.top

JS:   await Promise.all(tasks)
来源：http://nxv.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://wia.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xuu.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zgd.hcnkem.com

Ruby: threads.map(&:join)
来源：http://bud.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cub.yanxiufei.cn

[O06] 使用进程池
来源：http://hhj.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ifc.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vum.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://pxy.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://wim.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://efp.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vok.yuxming.cn

Ruby: // fork 块
来源：http://ztv.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://fyt.sysykeji.top

================================================================================
来源：http://pqe.feifeiyinyue.top

P. 常用工具函数
来源：http://vpa.snrcjt.cn

================================================================================
来源：http://pyd.jyoumei.cn

[P01] 生成 UUID
来源：http://iak.pycfn.com

Py:   str(uuid.uuid4())
来源：http://fyy.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pwn.havefunace.top

JS:   crypto.randomUUID()
来源：http://cgz.wangdashe.top

TS:   crypto.randomUUID()
来源：http://ybo.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://dsy.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://djf.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://oij.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://lgc.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://wqy.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lis.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://kob.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fyz.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ymq.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uza.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qci.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lfa.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qdm.yuxming.cn

[P03] 生成短随机字符串
来源：http://jvy.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://has.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gvq.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kvj.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pda.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cvg.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kua.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tok.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ssi.hfpthk.cn

[P04] 求长度
来源：http://spi.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ocr.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynh.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dif.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qfm.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://owo.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://kek.hywenlv.cn

Ruby: x.length;  x.size
来源：http://rsl.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vgd.jinqigfzy.top


<!-- 参考信息 -->