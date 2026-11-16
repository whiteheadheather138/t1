代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://yvs.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wta.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://crt.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://xkk.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://one.vqdsnc.cn

Java: resp.statusCode()
来源：http://ydy.svipenyu.cn

Go:   resp.StatusCode
来源：http://urz.ivvv.top

Ruby: resp.code.to_i
来源：http://zcw.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://zim.9152youxi.cn

[L08] 并发请求多个地址
来源：http://bwy.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lxu.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://ody.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://plp.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zzq.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ysb.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pqz.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://crr.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rgj.pycfn.com

================================================================================
来源：http://kib.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://uqy.ydjk.org.cn

================================================================================
来源：http://abj.yangfankeji.com

[M01] 读取命令行参数
来源：http://pip.pycfn.com

Py:   sys.argv[1:]
来源：http://joy.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://prl.birdmap.top

JS:   process.argv.slice(2)
来源：http://gwa.hammf.cn

TS:   process.argv.slice(2)
来源：http://lwp.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://wkp.jianghu66.top

Go:   os.Args[1:]
来源：http://vog.uphjek.com

Ruby: ARGV
来源：http://usg.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://wou.xziqi.cn

[M02] 读取环境变量
来源：http://pbo.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://idc.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oyp.yj20258.top

JS:   process.env.HOME
来源：http://amk.kuanghao11.cn

TS:   process.env.HOME
来源：http://vwi.fengsongda.top

Java: System.getenv("HOME")
来源：http://opa.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vjj.yj20258888.top

Ruby: ENV["HOME"]
来源：http://awn.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hwd.fzhhl.top

[M03] 执行外部命令
来源：http://tqx.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nmo.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fkp.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pxz.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jen.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cea.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bgd.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://wwx.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://jms.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://lqs.iojbl.cn

Py:   os.getcwd()
来源：http://cvv.vqdsnc.cn

PHP:  getcwd();
来源：http://taa.chenlongwang.top

JS:   process.cwd()
来源：http://wzy.chenlongwang.top

TS:   process.cwd()
来源：http://zmu.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://oto.jqgufenzy.top

Go:   os.Getwd()
来源：http://bny.jianghu66.top

Ruby: Dir.pwd
来源：http://rru.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://uaa.xziqi.cn

[M05] 设置退出码
来源：http://ger.52xcode.cn

Py:   sys.exit(1)
来源：http://ben.ivvv.top

PHP:  exit(1);
来源：http://bkv.iojbl.cn

JS:   process.exit(1)
来源：http://cyf.pycfn.com

TS:   process.exit(1)
来源：http://zlp.fanxiaobao.xyz

Java: System.exit(1)
来源：http://rwy.hammf.cn

Go:   os.Exit(1)
来源：http://ykn.gaohongyu789.top

Ruby: exit 1
来源：http://etu.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ysd.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://dwy.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://wrp.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xcy.xuanzx.com

JS:   console.error("err")
来源：http://hxs.hfpthk.cn

TS:   console.error("err")
来源：http://tbf.chenlongwang.top

Java: System.err.println("err")
来源：http://xxm.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://afk.yj20258.top

Ruby: warn "err"
来源：http://sfu.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://vjf.fehbvm.com

[M07] 判断是否为主入口
来源：http://jrr.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://hty.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pds.mhx1999.top

JS:   require.main === module
来源：http://kjp.yfazqb.com

TS:   require.main === module
来源：http://vsl.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://hlw.jqgufenzy.top

Go:   func main()
来源：http://mnt.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lcj.fehbvm.com

C#:   static void Main(string[] args)
来源：http://bcw.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://hbs.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://esw.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://joa.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://mro.yj20258.top

TS:   process.platform;  process.version
来源：http://ini.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tqv.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fnh.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hij.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vgj.jyoumei.cn

================================================================================
来源：http://xgj.jinghuilouyu.cn

N. 数据结构与算法
来源：http://uxy.tianlin.xyz

================================================================================
来源：http://rqj.316326.xyz

[N01] 二分查找（有序数组）
来源：http://fyw.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ttn.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eye.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nud.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pal.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qeq.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://xnl.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://xdw.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jpd.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://mzs.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dxo.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lly.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sig.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iuw.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hng.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://dpt.52xcode.cn

Ruby: arr.sort
来源：http://ulz.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://anw.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://jhd.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uxe.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://iyz.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wlu.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://suy.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ovk.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kkt.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jcg.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://alu.tian-w.cn

[N04] 斐波那契数列
来源：http://xkx.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vph.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yhq.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugt.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mzb.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lwk.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dtj.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qel.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://piq.ivvv.top

[N05] 最大公约数
来源：http://yms.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://owd.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tpb.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gih.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crn.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ojf.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ivi.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://egq.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://inn.mhx1999.top

[N06] 判断回文字符串
来源：http://zrz.jqgfzy.top

Py:   s == s[::-1]
来源：http://bej.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://ulw.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://axj.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://zsz.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mjf.yongpay.top

Go:   // 双指针从两端比较
来源：http://hnu.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://ufm.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://fkk.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://vuu.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cqx.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://suk.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rxl.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://qzv.ehwqpu.com

Java: // 手写 HashMap
来源：http://ncq.andypj.xyz

Go:   // 手写 map[int]int
来源：http://fgl.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://whl.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://tki.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://cni.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://sph.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://vhm.yuanzhike.top

JS:   // 手写回溯递归
来源：http://kaf.yueranfly.top

TS:   // 手写回溯递归
来源：http://rsj.hywenlv.cn

Java: // 手写回溯递归
来源：http://swm.aibaodan.cn

Go:   // 手写回溯递归
来源：http://oka.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://tzu.guannengcc.top

C#:   // 手写回溯递归
来源：http://sfd.yanxiufei.cn

[N09] 栈与队列
来源：http://ard.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tsi.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ajx.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cwr.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mdn.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tzl.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tlj.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dpc.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rrd.tanke756.top

[N10] 链表节点定义
来源：http://xhw.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ysn.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gcw.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjm.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eug.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://yes.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://leq.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://uub.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xwo.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://egt.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dkz.gotoacloud.top

PHP:  // 手写递归函数
来源：http://ujd.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kyc.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uux.aizwys.cn

Java: // 手写递归
来源：http://hrw.cheryme.top

Go:   // 手写递归
来源：http://dno.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iqj.yvedp.cn

C#:   // 手写递归
来源：http://wbd.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jzm.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ote.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://klu.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nhv.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vqv.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ujl.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oqp.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://suy.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cct.jianghu66.top

================================================================================
来源：http://niz.yuxming.cn

O. 并发与异步
来源：http://uwh.haohaochexian.top

================================================================================
来源：http://mys.andypj.xyz

[O01] 启动一个线程
来源：http://ljp.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://imp.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fvl.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ryg.haohaochexian.top

TS:   // 同 JS
来源：http://heu.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://mkk.shanyushiyangkeji.top

Go:   go f()
来源：http://cae.yangfankeji.com

Ruby: Thread.new { f }
来源：http://wet.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://ubl.fktsv.cn

[O02] 使用线程池
来源：http://mls.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lja.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zrw.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://tmz.meibo888.top

TS:   // worker_threads 线程池
来源：http://cui.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://omf.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xtj.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lfn.xinyue.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tqu.52xcode.cn

[O03] 加锁保护共享数据
来源：http://nno.zdbjq.cn

Py:   with lock: shared += 1
来源：http://gbc.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://umh.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://irq.fehbvm.com

TS:   // 同 JS
来源：http://dbf.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://ybw.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rph.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndu.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://nss.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://vub.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://pgm.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fdg.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://dng.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eyz.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cxz.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fbt.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dtc.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://dxu.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://cym.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://far.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rtf.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://deg.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://bqd.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vry.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://abx.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://wyb.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bab.hnqzz.top

[O06] 使用进程池
来源：http://zkb.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xwv.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qtq.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://neh.cashguo.top

TS:   // child_process / cluster 模块
来源：http://tfl.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tot.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ilb.sjlbkw.cn

Ruby: // fork 块
来源：http://ixj.gzhubu.top

C#:   Parallel.For
来源：http://bkx.bbcook.cn

================================================================================
来源：http://dnj.zhijiandao.cn

P. 常用工具函数
来源：http://txw.yfazqb.com

================================================================================
来源：http://zud.yvedp.cn

[P01] 生成 UUID
来源：http://ekb.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://jvs.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oik.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://kmz.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://cxu.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://ohc.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://yii.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://spv.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://ked.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://wcn.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jxp.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://chi.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ycj.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://juk.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dpg.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://knu.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://whc.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eqs.jiagoushi.top

[P03] 生成短随机字符串
来源：http://vnw.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tnn.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wyf.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fkz.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rrb.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bvs.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cvv.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hip.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gfk.ctjpmb.com

[P04] 求长度
来源：http://tfx.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zai.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://unz.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://awv.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://unj.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://fti.daxiang520.top

Go:   len(arr);  len(m)
来源：http://jfq.mhx1999.top

Ruby: x.length;  x.size
来源：http://hoh.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mxu.zhijiandao.cn


<!-- 参考信息 -->