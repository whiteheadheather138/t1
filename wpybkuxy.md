代发 wailian999

C#:   (int)resp.StatusCode
来源：http://zev.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://qbd.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vbx.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://trc.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://llj.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ynd.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://asa.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ctk.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wny.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yxf.pycfn.com

================================================================================
来源：http://kha.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://xyk.ydzc1.top

================================================================================
来源：http://hje.zhixingplan.top

[M01] 读取命令行参数
来源：http://vzw.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://qbp.hcnkem.com

PHP:  $argv;  $argc;
来源：http://twy.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://fnd.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://fkr.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://kca.yonumen.top

Go:   os.Args[1:]
来源：http://ttn.haohaochexian.top

Ruby: ARGV
来源：http://lhp.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://zoc.hesvh.cn

[M02] 读取环境变量
来源：http://rcs.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://tpn.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ird.gogol.net.cn

JS:   process.env.HOME
来源：http://cqs.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://ege.hnqzz.top

Java: System.getenv("HOME")
来源：http://cqd.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cej.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://zpv.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bmp.aizwys.cn

[M03] 执行外部命令
来源：http://exo.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xxj.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://igd.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iwt.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rfw.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ozb.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qzi.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qqe.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://fpn.gotoacloud.top

[M04] 获取当前工作目录
来源：http://jbl.hnqzz.top

Py:   os.getcwd()
来源：http://lhf.daxiang520.top

PHP:  getcwd();
来源：http://feh.cdnleiting.top

JS:   process.cwd()
来源：http://zfb.jinqigfzy.top

TS:   process.cwd()
来源：http://ebl.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://yja.9152youxi.cn

Go:   os.Getwd()
来源：http://hxz.yvedp.cn

Ruby: Dir.pwd
来源：http://bwr.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://wtn.zhengqikj.top

[M05] 设置退出码
来源：http://qdr.hysaishi.cn

Py:   sys.exit(1)
来源：http://voq.zhiwuduotai.top

PHP:  exit(1);
来源：http://wvl.uphjek.com

JS:   process.exit(1)
来源：http://uwh.zhoulong.xyz

TS:   process.exit(1)
来源：http://dsg.yongpay.top

Java: System.exit(1)
来源：http://xrv.haohaochexian.top

Go:   os.Exit(1)
来源：http://tda.meibo888.top

Ruby: exit 1
来源：http://luj.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://stv.yj202588.top

[M06] 向标准错误输出
来源：http://rvm.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://dxe.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rhi.jiagoushi.top

JS:   console.error("err")
来源：http://hlh.dashuyun.cn

TS:   console.error("err")
来源：http://knt.hesvh.cn

Java: System.err.println("err")
来源：http://har.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pwm.gotoacloud.top

Ruby: warn "err"
来源：http://rtg.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://gsd.redwolf501.top

[M07] 判断是否为主入口
来源：http://ebf.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://zlu.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hoj.hysaishi.cn

JS:   require.main === module
来源：http://lrr.yj202588.top

TS:   require.main === module
来源：http://dvt.yuanzhike.top

Java: public static void main(String[] args)
来源：http://spd.cqqwz.cn

Go:   func main()
来源：http://tce.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qvi.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://jgl.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://aqg.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://ekf.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://nmt.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://nwg.yangfankeji.com

TS:   process.platform;  process.version
来源：http://jfp.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hor.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aoy.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ijo.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qvc.feifeiyinyue.top

================================================================================
来源：http://chi.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://oof.xziqi.cn

================================================================================
来源：http://vgz.316326.xyz

[N01] 二分查找（有序数组）
来源：http://btl.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://gng.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pcb.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nuo.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uau.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zky.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://grt.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://ofz.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://xrr.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://ecw.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://vkz.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ozk.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bjv.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kdf.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uhc.xinyue.icu

Go:   slices.Sort(arr)
来源：http://eor.zhongyouzk.top

Ruby: arr.sort
来源：http://yha.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sku.birdmap.top

[N03] 快速排序（分治示例）
来源：http://ocd.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jyu.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://rcc.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcj.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sbu.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ptg.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rxs.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gal.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nyf.vqdsnc.cn

[N04] 斐波那契数列
来源：http://fau.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://joa.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zmd.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpx.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://naa.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://omj.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://stb.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uzo.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bmo.tarul.cn

[N05] 最大公约数
来源：http://pkf.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://ypg.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ajm.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tcu.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wcg.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vog.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rxu.zycfv.cn

Ruby: a.gcd(b)
来源：http://tgf.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hst.xinyue.icu

[N06] 判断回文字符串
来源：http://txm.yangfankeji.com

Py:   s == s[::-1]
来源：http://bup.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://ktm.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://pvc.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://lfr.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pvw.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://jva.nwbrower.top

Ruby: s == s.reverse
来源：http://nqz.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://pmh.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://pyn.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mdl.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tyd.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kfa.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://kqe.uphjek.com

Java: // 手写 HashMap
来源：http://hwm.yongpay.top

Go:   // 手写 map[int]int
来源：http://lmz.dianchejie.cn

Ruby: // 手写 Hash
来源：http://xcb.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yvf.nanxuanxn.top

[N08] 生成全排列
来源：http://pjj.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://qnk.daxiang520.top

PHP:  // 手写递归交换
来源：http://asg.zhengqikj.top

JS:   // 手写回溯递归
来源：http://iha.guowangkeji.top

TS:   // 手写回溯递归
来源：http://wmz.jinqigfzy.top

Java: // 手写回溯递归
来源：http://jco.hesvh.cn

Go:   // 手写回溯递归
来源：http://fup.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://fdj.xuanzx.com

C#:   // 手写回溯递归
来源：http://mez.tian-w.cn

[N09] 栈与队列
来源：http://ugv.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tgs.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vph.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sri.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dwf.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdo.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qrj.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tul.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nyb.iojbl.cn

[N10] 链表节点定义
来源：http://bfi.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ayg.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oaf.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lpm.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hpi.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://vci.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://qhl.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yjt.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jdq.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://myh.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bgz.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://vjg.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zly.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lax.jinyuanbaomall.cn

Java: // 手写递归
来源：http://lpa.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://dnr.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fva.52xcode.cn

C#:   // 手写递归
来源：http://ihz.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jfg.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gec.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qsv.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ykx.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ruo.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cth.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dxx.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aoj.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tqm.chenjidiqi.icu

================================================================================
来源：http://men.jlsjyb.cn

O. 并发与异步
来源：http://xqy.fehbvm.com

================================================================================
来源：http://nvb.andypj.xyz

[O01] 启动一个线程
来源：http://sad.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rcm.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vph.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jvp.0kj1m.cn

TS:   // 同 JS
来源：http://ick.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://eqg.hywenlv.cn

Go:   go f()
来源：http://oda.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://mjn.pengpengdd.cyou

C#:   Task.Run(() => F());
来源：http://zvt.0kj1m.cn

[O02] 使用线程池
来源：http://fzh.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ace.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ihe.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://dut.fengsongda.top

TS:   // worker_threads 线程池
来源：http://eli.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://urv.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ymt.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hrn.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dcf.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://umr.cashguo.top

Py:   with lock: shared += 1
来源：http://hqp.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://web.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://unl.hnxiangtu.top

TS:   // 同 JS
来源：http://voh.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://ojt.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ufj.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xnu.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://bwn.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://ucu.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://hws.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wbk.cashguo.top

JS:   async function f() { await g(); }
来源：http://qiw.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ane.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sfb.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vlm.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://okw.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://lxl.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://ohr.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://sdz.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lno.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://zdi.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://nbt.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://utg.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rpb.hesvh.cn

Ruby: threads.map(&:join)
来源：http://gqr.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mdp.cqqwz.cn

[O06] 使用进程池
来源：http://ymq.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ayg.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://glr.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://nmc.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://owp.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mzi.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bob.quarkkingdee.top

Ruby: // fork 块
来源：http://cnj.dianchejie.cn

C#:   Parallel.For
来源：http://mcm.kuanghao11.cn

================================================================================
来源：http://jtu.hysaishi.cn

P. 常用工具函数
来源：http://dcc.fktsv.cn

================================================================================
来源：http://jab.yvedp.cn

[P01] 生成 UUID
来源：http://uke.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://zyk.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mdi.xylfe.cn

JS:   crypto.randomUUID()
来源：http://uhv.hcnkem.com

TS:   crypto.randomUUID()
来源：http://upq.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://liv.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://wbx.pycfn.com

Ruby: SecureRandom.uuid
来源：http://pux.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://jih.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://xjj.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mlk.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xit.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qcu.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fdq.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dxy.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jhh.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hjc.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asp.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://cbj.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zin.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bso.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mrv.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gbr.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sae.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bcg.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vty.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qkx.dianchejie.cn

[P04] 求长度
来源：http://tnh.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bay.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fou.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lqn.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ghn.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://szv.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://zks.xylfe.cn

Ruby: x.length;  x.size
来源：http://nyl.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lmj.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://cww.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zxm.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtv.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gud.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pzk.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yil.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rzc.hfpthk.cn

Ruby: a == b
来源：http://ode.feifeiyinyue.top


<!-- 参考信息 -->