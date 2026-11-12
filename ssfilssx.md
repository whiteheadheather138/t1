代发 wailian999

TS:   resp.ok;  resp.status
来源：http://wkk.pycfn.com

Java: resp.statusCode()
来源：http://gaj.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://kii.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://mni.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://vce.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://eqs.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pzt.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://kkt.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axf.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ceu.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kjv.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ujv.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fho.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xvw.hnqzz.top

================================================================================
来源：http://ocq.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://ole.jianghu66.top

================================================================================
来源：http://wex.birdmap.top

[M01] 读取命令行参数
来源：http://ffx.tanke756.top

Py:   sys.argv[1:]
来源：http://zcn.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://atp.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://lxn.bbcook.cn

TS:   process.argv.slice(2)
来源：http://wjr.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://uez.ppjwa.cn

Go:   os.Args[1:]
来源：http://zgi.nwbrower.top

Ruby: ARGV
来源：http://wgk.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://rvw.ybcxt.top

[M02] 读取环境变量
来源：http://kgw.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://bqt.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yum.sweek.top

JS:   process.env.HOME
来源：http://hpn.haohaochexian.top

TS:   process.env.HOME
来源：http://ydd.316326.xyz

Java: System.getenv("HOME")
来源：http://kqg.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hyv.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://yxc.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://htx.yuxming.cn

[M03] 执行外部命令
来源：http://cxf.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ovv.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ypd.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fdk.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zpu.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ckl.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fuc.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xjh.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://tpc.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://tcc.guannengcc.top

Py:   os.getcwd()
来源：http://mpk.guannengcc.top

PHP:  getcwd();
来源：http://mqi.havefunace.top

JS:   process.cwd()
来源：http://qpi.gotoacloud.top

TS:   process.cwd()
来源：http://old.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://vcx.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://jhr.kuanghao11.cn

Ruby: Dir.pwd
来源：http://obw.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ate.epnwcf.com

[M05] 设置退出码
来源：http://kci.hnxiangtu.top

Py:   sys.exit(1)
来源：http://byo.bbcook.cn

PHP:  exit(1);
来源：http://xqj.fzhhl.top

JS:   process.exit(1)
来源：http://ihu.zhengqikj.top

TS:   process.exit(1)
来源：http://eiz.gogol.net.cn

Java: System.exit(1)
来源：http://icb.jianghu66.top

Go:   os.Exit(1)
来源：http://pkr.cucudq.cn

Ruby: exit 1
来源：http://yzv.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dnu.tian-w.cn

[M06] 向标准错误输出
来源：http://iva.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://lvu.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ene.yj20258.top

JS:   console.error("err")
来源：http://jsr.xuanzx.com

TS:   console.error("err")
来源：http://zlw.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://qgw.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://clw.smart0.xyz

Ruby: warn "err"
来源：http://dll.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://oon.snrcjt.cn

[M07] 判断是否为主入口
来源：http://nvf.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://tcx.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://spt.shangyingyoupin.top

JS:   require.main === module
来源：http://wga.316326.xyz

TS:   require.main === module
来源：http://yrt.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://hlx.jlsjyb.cn

Go:   func main()
来源：http://whs.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ilq.gzhubu.top

C#:   static void Main(string[] args)
来源：http://bao.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://nte.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://zpo.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://fqr.gogol.net.cn

JS:   process.platform;  process.version
来源：http://hci.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://uso.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://akg.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cxx.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gqg.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vcn.daxiang520.top

================================================================================
来源：http://gfq.gotoacloud.top

N. 数据结构与算法
来源：http://pur.bjfxy.top

================================================================================
来源：http://hgg.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://jrz.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://mvz.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dao.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dhx.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rkc.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://bsp.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://dsc.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iho.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://cem.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://vpg.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://hnb.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mdc.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vte.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xqx.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hxk.daxiang520.top

Go:   slices.Sort(arr)
来源：http://aul.daria6918.cn

Ruby: arr.sort
来源：http://efn.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://oyb.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://jaw.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aae.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://aev.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uez.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gmr.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vbp.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fzi.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://all.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://viz.ppjwa.cn

[N04] 斐波那契数列
来源：http://dpx.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oqg.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zbf.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vsw.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxq.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://goq.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bhr.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sjd.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://esm.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://kit.xuanzx.com

Py:   math.gcd(a, b)
来源：http://gff.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nag.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://khg.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vah.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://don.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tfe.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://sgc.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lfz.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://qye.tian-w.cn

Py:   s == s[::-1]
来源：http://cjy.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://xft.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://lah.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://ezk.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nnt.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://moc.iojbl.cn

Ruby: s == s.reverse
来源：http://uhe.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://iui.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://fvp.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vbl.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fqp.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xbo.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://ewh.svipenyu.cn

Java: // 手写 HashMap
来源：http://ymd.iojbl.cn

Go:   // 手写 map[int]int
来源：http://jhx.jianghu66.top

Ruby: // 手写 Hash
来源：http://wvw.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://yet.cashguo.top

[N08] 生成全排列
来源：http://cuo.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://ngv.fktsv.cn

PHP:  // 手写递归交换
来源：http://qax.316326.xyz

JS:   // 手写回溯递归
来源：http://gur.mhx1999.top

TS:   // 手写回溯递归
来源：http://ejm.chenlongwang.top

Java: // 手写回溯递归
来源：http://uqu.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://buf.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://ase.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://ple.birdmap.top

[N09] 栈与队列
来源：http://upp.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wcz.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://het.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://loz.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ouc.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pat.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://irz.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rri.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ygl.daxiang520.top

[N10] 链表节点定义
来源：http://bmv.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eyp.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mrn.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://igm.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rjt.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://atx.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://fxg.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ohn.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rpf.xziqi.cn

[N11] 二叉树中序遍历
来源：http://ibj.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://btl.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://jlw.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ics.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tge.chenzaomai.com

Java: // 手写递归
来源：http://iqu.bbcook.cn

Go:   // 手写递归
来源：http://ypi.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ytp.yj20258.top

C#:   // 手写递归
来源：http://czh.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dzi.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vom.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iet.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tkd.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gvs.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pag.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jph.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kbc.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uwt.birdmap.top

================================================================================
来源：http://bhu.yj20258.top

O. 并发与异步
来源：http://qvi.yj20258888.top

================================================================================
来源：http://krt.yuanzhike.top

[O01] 启动一个线程
来源：http://qxg.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tyv.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jun.svipenyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://etl.yangfankeji.com

TS:   // 同 JS
来源：http://srx.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://ozv.daria6918.cn

Go:   go f()
来源：http://jry.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://xzd.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://acf.jyoumei.cn

[O02] 使用线程池
来源：http://opb.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hzl.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hyn.tian-w.cn

JS:   // worker_threads 线程池
来源：http://klp.yuxming.cn

TS:   // worker_threads 线程池
来源：http://hxi.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gok.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tgo.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://duc.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hlp.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://wxe.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://gtq.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://buc.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mji.yonumen.top

TS:   // 同 JS
来源：http://osc.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://gkh.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qlk.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yju.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://bev.daria6918.cn

[O04] 定义异步函数并等待
来源：http://jvp.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://lft.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uwk.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://isk.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://luz.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ohq.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfw.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tqq.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://kle.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://hkj.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://bqq.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lqp.tanke756.top

JS:   await Promise.all(tasks)
来源：http://dfe.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://wrc.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hcc.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mrc.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://see.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eka.vqdsnc.cn

[O06] 使用进程池
来源：http://msa.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovn.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://xpn.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://gtj.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://kej.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ziq.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jya.yvedp.cn

Ruby: // fork 块
来源：http://aac.svipenyu.cn

C#:   Parallel.For
来源：http://elk.ehwqpu.com

================================================================================
来源：http://itl.ydzc1.top

P. 常用工具函数
来源：http://och.epnwcf.com

================================================================================
来源：http://bnj.hongshengwenyu.top

[P01] 生成 UUID
来源：http://fyc.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://ueu.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xti.fengsongda.top

JS:   crypto.randomUUID()
来源：http://zlg.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://hjm.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://xbi.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://gwj.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://rnl.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://ash.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://iwk.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hun.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vbl.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rfc.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wdm.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pbg.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vpt.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lej.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pet.fzhhl.top

[P03] 生成短随机字符串
来源：http://rtl.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aqk.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zbr.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vxi.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qeg.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lnj.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qxq.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dpk.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zrt.shangyingyoupin.top

[P04] 求长度
来源：http://uuc.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nrq.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ogi.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhy.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzu.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://bzs.uphjek.com

Go:   len(arr);  len(m)
来源：http://nmc.tianlin.xyz

Ruby: x.length;  x.size
来源：http://qht.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ydb.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://zca.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://awy.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://unh.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nrk.tianlin.xyz


<!-- 参考信息 -->