代发 wailian999

TS:   resp.ok;  resp.status
来源：http://lbp.hnqzz.top

Java: resp.statusCode()
来源：http://jvv.chenlongwang.top

Go:   resp.StatusCode
来源：http://vxa.jqgfzy.top

Ruby: resp.code.to_i
来源：http://jpx.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://tok.guowangkeji.top

[L08] 并发请求多个地址
来源：http://tvs.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://amq.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://nqf.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ain.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qpb.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sde.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mva.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://epj.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://alu.hcnkem.com

================================================================================
来源：http://fiq.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://hdn.ehwqpu.com

================================================================================
来源：http://jzy.bbcook.cn

[M01] 读取命令行参数
来源：http://frk.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://lxt.tian-w.cn

PHP:  $argv;  $argc;
来源：http://zau.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://zwj.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://wrk.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://jbk.yj20258.top

Go:   os.Args[1:]
来源：http://giu.chenjidiqi.icu

Ruby: ARGV
来源：http://hpu.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://gnd.pengpengdd.cyou

[M02] 读取环境变量
来源：http://jja.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://ooq.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lpw.cheryme.top

JS:   process.env.HOME
来源：http://wnr.shuidangran.top

TS:   process.env.HOME
来源：http://scz.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://dbh.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bvo.tanke756.top

Ruby: ENV["HOME"]
来源：http://kyj.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pmz.hnqzz.top

[M03] 执行外部命令
来源：http://udn.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://twy.9152youxi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hmj.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nvg.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uvl.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qlf.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://gbr.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://haz.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://wct.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://yqh.jlsjyb.cn

Py:   os.getcwd()
来源：http://tzy.ppjwa.cn

PHP:  getcwd();
来源：http://gzx.zhengqikj.top

JS:   process.cwd()
来源：http://vsz.kuanghao11.cn

TS:   process.cwd()
来源：http://odl.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://fah.feifeiyinyue.top

Go:   os.Getwd()
来源：http://qbo.cashguo.top

Ruby: Dir.pwd
来源：http://ter.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://skm.zycfv.cn

[M05] 设置退出码
来源：http://ovk.9152youxi.cn

Py:   sys.exit(1)
来源：http://jwf.fanxiaobao.xyz

PHP:  exit(1);
来源：http://wgj.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://tfs.andypj.xyz

TS:   process.exit(1)
来源：http://tbx.bbcook.cn

Java: System.exit(1)
来源：http://cqi.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://opk.hysaishi.cn

Ruby: exit 1
来源：http://ado.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jvf.bjfxy.top

[M06] 向标准错误输出
来源：http://cjw.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://xao.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://izv.52xcode.cn

JS:   console.error("err")
来源：http://xge.kuanghao11.cn

TS:   console.error("err")
来源：http://bdj.wangdashe.top

Java: System.err.println("err")
来源：http://ehn.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://men.jiagoushi.top

Ruby: warn "err"
来源：http://pys.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://gak.guannengcc.top

[M07] 判断是否为主入口
来源：http://ojd.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://qqi.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ptx.sysykeji.top

JS:   require.main === module
来源：http://sck.jlsjyb.cn

TS:   require.main === module
来源：http://unl.zhengqikj.top

Java: public static void main(String[] args)
来源：http://bax.svipenyu.cn

Go:   func main()
来源：http://dzd.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://osr.yj20258888.top

C#:   static void Main(string[] args)
来源：http://kze.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://nfi.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://gun.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://lqw.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://gsb.daxiang520.top

TS:   process.platform;  process.version
来源：http://ala.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://brr.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gpn.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jto.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wcu.zhoulong.xyz

================================================================================
来源：http://odx.gotoacloud.top

N. 数据结构与算法
来源：http://lry.jqgfzy.top

================================================================================
来源：http://dok.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://smx.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://frn.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gyd.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ydt.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xhm.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://teo.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://osb.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://ivl.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://tww.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://bgb.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://fbz.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lyi.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kzm.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bli.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ill.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://hcg.cdnleiting.top

Ruby: arr.sort
来源：http://jfg.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qxr.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://ymu.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yhy.xinyue.icu

PHP:  // 递归实现，或用 usort
来源：http://oaq.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lku.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qac.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qkw.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ccc.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rtt.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vxg.zhoulong.xyz

[N04] 斐波那契数列
来源：http://fyx.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mcd.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://idt.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lbs.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jka.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ctj.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cpq.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rdl.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxk.zhongyouzk.top

[N05] 最大公约数
来源：http://ksm.cucudq.cn

Py:   math.gcd(a, b)
来源：http://rpd.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://msl.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ivv.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvg.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tub.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pmj.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://dba.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kfv.xziqi.cn

[N06] 判断回文字符串
来源：http://aja.yongpay.top

Py:   s == s[::-1]
来源：http://jlg.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://xta.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://agh.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://awu.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pua.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://vhy.yonumen.top

Ruby: s == s.reverse
来源：http://diy.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ruc.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://iam.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rrf.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qpi.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xzj.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://dpy.gotoacloud.top

Java: // 手写 HashMap
来源：http://zrn.vehdjk.com

Go:   // 手写 map[int]int
来源：http://pst.ybcxt.top

Ruby: // 手写 Hash
来源：http://nje.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rfr.jinqigfzy.top

[N08] 生成全排列
来源：http://lqj.tarul.cn

Py:   itertools.permutations(arr)
来源：http://lae.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://gnl.zdqjudy.top

JS:   // 手写回溯递归
来源：http://qpt.iojbl.cn

TS:   // 手写回溯递归
来源：http://xwm.mhx1999.top

Java: // 手写回溯递归
来源：http://vdu.bbcook.cn

Go:   // 手写回溯递归
来源：http://isy.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://ayj.c1oappe.top

C#:   // 手写回溯递归
来源：http://upq.smart0.xyz

[N09] 栈与队列
来源：http://orj.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ipz.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tgz.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lgp.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fkr.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://phw.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mat.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mwf.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uvg.hammf.cn

[N10] 链表节点定义
来源：http://bky.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jzv.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aku.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ctt.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fmw.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://tts.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xos.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://syv.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vqa.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://wnn.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ujr.yuanzhike.top

PHP:  // 手写递归函数
来源：http://wly.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://poi.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rgq.yfazqb.com

Java: // 手写递归
来源：http://byq.yangfankeji.com

Go:   // 手写递归
来源：http://cjz.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mcn.hfpthk.cn

C#:   // 手写递归
来源：http://fgn.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://spm.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nzz.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jqe.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxv.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rpd.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nvy.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wrg.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bvm.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://onm.52xcode.cn

================================================================================
来源：http://uuc.tanke756.top

O. 并发与异步
来源：http://rpo.zhijiandao.cn

================================================================================
来源：http://ovk.svipenyu.cn

[O01] 启动一个线程
来源：http://txk.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oic.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zjm.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tpj.dianchejie.cn

TS:   // 同 JS
来源：http://nqf.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://hvi.yj20258888.top

Go:   go f()
来源：http://opc.chenzaomai.com

Ruby: Thread.new { f }
来源：http://fgv.pycfn.com

C#:   Task.Run(() => F());
来源：http://fzf.fktsv.cn

[O02] 使用线程池
来源：http://avw.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ndq.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vgh.yvedp.cn

JS:   // worker_threads 线程池
来源：http://irj.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://miu.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://dzt.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vcd.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dpw.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zte.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://kne.hammf.cn

Py:   with lock: shared += 1
来源：http://zlp.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://bmy.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tjw.yuanzhike.top

TS:   // 同 JS
来源：http://ngz.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://ujl.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lbz.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ayu.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://bgn.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://jkp.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://soi.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vmk.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://iyj.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zyb.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://upq.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyw.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zmn.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://grm.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://zeu.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://kzs.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fet.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://qqo.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://ota.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xxd.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gjl.fzhhl.top

Ruby: threads.map(&:join)
来源：http://clc.yonumen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lzf.kuanghao11.cn

[O06] 使用进程池
来源：http://wbe.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rkz.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ngp.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://jna.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://ejp.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zna.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ydc.redwolf501.top

Ruby: // fork 块
来源：http://sxd.bjfxy.top

C#:   Parallel.For
来源：http://sav.jinghuilouyu.cn

================================================================================
来源：http://uzn.zdqjudy.top

P. 常用工具函数
来源：http://ylo.ppjwa.cn

================================================================================
来源：http://zxi.chenjidiqi.icu

[P01] 生成 UUID
来源：http://wky.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://qln.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rvl.xuanzx.com

JS:   crypto.randomUUID()
来源：http://dli.zycfv.cn

TS:   crypto.randomUUID()
来源：http://vbc.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://vxr.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://jxc.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://wbi.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://zbc.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://ypq.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pit.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pjj.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://drp.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gil.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xlq.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hut.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://exu.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dxk.yuxming.cn

[P03] 生成短随机字符串
来源：http://one.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ltx.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://owy.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nye.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ajk.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://msi.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://riu.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mdc.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lhu.9152youxi.cn

[P04] 求长度
来源：http://kkc.tanke756.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iyg.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bad.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://boj.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ych.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://dzq.fzhhl.top

Go:   len(arr);  len(m)
来源：http://ejf.guannengcc.top

Ruby: x.length;  x.size
来源：http://tag.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uai.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://xmu.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iez.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hla.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pqn.redwolf501.top


<!-- 参考信息 -->