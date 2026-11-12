代发 wailian999

C#:   (int)resp.StatusCode
来源：http://zzp.guowangkeji.top

[L08] 并发请求多个地址
来源：http://let.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tcu.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://pyk.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wnl.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pfk.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bke.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://agy.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mwy.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ioq.uphjek.com

================================================================================
来源：http://sxi.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://aar.wangdashe.top

================================================================================
来源：http://tdy.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://usx.cashguo.top

Py:   sys.argv[1:]
来源：http://oma.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://dun.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://vke.sxryk.cn

TS:   process.argv.slice(2)
来源：http://pie.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://fwk.fzhhl.top

Go:   os.Args[1:]
来源：http://zhv.guannengcc.top

Ruby: ARGV
来源：http://cuf.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://xyl.nanxinkj.top

[M02] 读取环境变量
来源：http://vja.hammf.cn

Py:   os.environ.get("HOME")
来源：http://rld.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://prr.ctjpmb.com

JS:   process.env.HOME
来源：http://rek.cheryme.top

TS:   process.env.HOME
来源：http://hzw.hnqzz.top

Java: System.getenv("HOME")
来源：http://ove.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xay.mhx1999.top

Ruby: ENV["HOME"]
来源：http://fho.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ynx.cucudq.cn

[M03] 执行外部命令
来源：http://ugi.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yxi.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tkz.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vje.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lwb.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sqr.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tnp.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://vxu.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://uax.tanke756.top

[M04] 获取当前工作目录
来源：http://msw.birdmap.top

Py:   os.getcwd()
来源：http://tbp.tian-w.cn

PHP:  getcwd();
来源：http://cbu.0kj1m.cn

JS:   process.cwd()
来源：http://asz.cdnleiting.top

TS:   process.cwd()
来源：http://zbs.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://rfr.vqdsnc.cn

Go:   os.Getwd()
来源：http://dxt.yvedp.cn

Ruby: Dir.pwd
来源：http://lyz.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://rck.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://mre.redwolf501.top

Py:   sys.exit(1)
来源：http://jwa.nwbrower.top

PHP:  exit(1);
来源：http://hgj.zhixingplan.top

JS:   process.exit(1)
来源：http://pul.zycfv.cn

TS:   process.exit(1)
来源：http://wwk.yuanzhike.top

Java: System.exit(1)
来源：http://lls.gotoacloud.top

Go:   os.Exit(1)
来源：http://hga.zhongyouzk.top

Ruby: exit 1
来源：http://fqj.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ctr.ivvv.top

[M06] 向标准错误输出
来源：http://jyi.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://jyo.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://iie.gogol.net.cn

JS:   console.error("err")
来源：http://sfj.jinqigufen.top

TS:   console.error("err")
来源：http://iaw.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://yne.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ebn.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://hqu.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://zpy.sweek.top

[M07] 判断是否为主入口
来源：http://pyo.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://vlm.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nwr.daxiang520.top

JS:   require.main === module
来源：http://axw.nwbrower.top

TS:   require.main === module
来源：http://hch.zdbjq.cn

Java: public static void main(String[] args)
来源：http://ern.guowangkeji.top

Go:   func main()
来源：http://bmq.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cbh.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://xyw.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://ltl.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://ofy.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://shk.ivvv.top

JS:   process.platform;  process.version
来源：http://wud.ehwqpu.com

TS:   process.platform;  process.version
来源：http://ngq.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fjo.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bre.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://geb.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tor.feifeiyinyue.top

================================================================================
来源：http://vci.jlsjyb.cn

N. 数据结构与算法
来源：http://qkp.cucudq.cn

================================================================================
来源：http://lnw.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://dqm.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aer.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qnm.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqt.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbk.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://ydi.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://nim.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nkd.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://xvl.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://gcg.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://wbu.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cho.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nlg.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lvo.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wdx.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://yhl.snrcjt.cn

Ruby: arr.sort
来源：http://dhv.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://guq.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://mct.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://auf.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://kst.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lkr.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hng.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gui.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xbk.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://axu.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cty.hnxiangtu.top

[N04] 斐波那契数列
来源：http://xid.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://grx.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kbx.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://suc.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xyq.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hek.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xmb.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jiw.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vra.sufxvd.cn

[N05] 最大公约数
来源：http://zgz.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://qkq.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qcg.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avr.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjv.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xks.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hxu.hammf.cn

Ruby: a.gcd(b)
来源：http://wuq.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://phq.xuanzx.com

[N06] 判断回文字符串
来源：http://zlp.quarkkingdee.top

Py:   s == s[::-1]
来源：http://nhm.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://lod.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://ahi.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://juq.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://juk.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://xpu.sxryk.cn

Ruby: s == s.reverse
来源：http://sdh.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hsr.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://tdb.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zkr.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kig.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://orr.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://wku.quarkkingdee.top

Java: // 手写 HashMap
来源：http://whz.xylfe.cn

Go:   // 手写 map[int]int
来源：http://wqc.cqqwz.cn

Ruby: // 手写 Hash
来源：http://tuk.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://ghn.fktsv.cn

[N08] 生成全排列
来源：http://qjm.zhoulong.xyz

Py:   itertools.permutations(arr)
来源：http://akw.xylfe.cn

PHP:  // 手写递归交换
来源：http://jab.jianghu66.top

JS:   // 手写回溯递归
来源：http://uwn.yonumen.top

TS:   // 手写回溯递归
来源：http://eum.c1oappe.top

Java: // 手写回溯递归
来源：http://upf.aizwys.cn

Go:   // 手写回溯递归
来源：http://qyz.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://und.316326.xyz

C#:   // 手写回溯递归
来源：http://lao.hcnkem.com

[N09] 栈与队列
来源：http://gxf.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://msj.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kim.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kbq.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://orx.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kqr.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kvg.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gsp.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zic.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://pxw.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ttw.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hhl.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bwa.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://knm.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://bxj.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://jme.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lka.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dcs.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://zmc.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mdr.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://xro.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pld.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://olx.cheryme.top

Java: // 手写递归
来源：http://hxi.cheryme.top

Go:   // 手写递归
来源：http://nbc.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sbn.bbcook.cn

C#:   // 手写递归
来源：http://swj.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vrv.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hbw.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dxo.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpt.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jel.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fyn.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mre.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rrp.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pns.aizwys.cn

================================================================================
来源：http://muj.guannengcc.top

O. 并发与异步
来源：http://pxi.hesvh.cn

================================================================================
来源：http://wju.sweek.top

[O01] 启动一个线程
来源：http://yqh.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jnl.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://llb.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eyx.jlsjyb.cn

TS:   // 同 JS
来源：http://rva.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://yoa.aibaodan.cn

Go:   go f()
来源：http://ptv.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://qfj.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://dly.sysykeji.top

[O02] 使用线程池
来源：http://akn.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://osf.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vii.epnwcf.com

JS:   // worker_threads 线程池
来源：http://rfj.yuxming.cn

TS:   // worker_threads 线程池
来源：http://cin.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dbg.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ign.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iej.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tfe.fzhhl.top

[O03] 加锁保护共享数据
来源：http://osq.birdmap.top

Py:   with lock: shared += 1
来源：http://def.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://bqw.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zvg.haohaochexian.top

TS:   // 同 JS
来源：http://egt.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://fjv.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lko.daxiang520.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uox.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://gzo.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://cko.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://hom.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jqg.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://leq.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mnp.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://heu.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ivw.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://mau.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://rkf.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://djx.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://igt.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bqf.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://enc.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://emk.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sfe.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://msc.daria6918.cn

Ruby: threads.map(&:join)
来源：http://jzf.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pqz.c1oappe.top

[O06] 使用进程池
来源：http://fwx.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kdl.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://awr.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://jcs.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://cqf.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lab.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xhw.gaohongyu789.top

Ruby: // fork 块
来源：http://oxp.zdqjudy.top

C#:   Parallel.For
来源：http://qit.smart0.xyz

================================================================================
来源：http://nmn.ydjk.org.cn

P. 常用工具函数
来源：http://gbw.fzhhl.top

================================================================================
来源：http://ggt.316326.xyz

[P01] 生成 UUID
来源：http://qjf.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://pog.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pza.yvedp.cn

JS:   crypto.randomUUID()
来源：http://xoc.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://efo.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://viu.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://sgr.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://pmt.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://joy.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://wmu.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zck.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hgx.snrcjt.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lxn.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xsp.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qsr.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cts.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cce.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bex.yuxming.cn

[P03] 生成短随机字符串
来源：http://lln.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wdl.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qxa.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nsg.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qed.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yiu.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jdk.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gkr.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mqj.yangfankeji.com

[P04] 求长度
来源：http://ajc.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ioq.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://omz.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ktu.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ppi.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://lko.smart0.xyz

Go:   len(arr);  len(m)
来源：http://zbc.fktsv.cn

Ruby: x.length;  x.size
来源：http://snx.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://efe.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://tsz.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mvs.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zyb.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jek.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://geg.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vlc.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pyv.snrcjt.cn

Ruby: a == b
来源：http://gai.jqgfzy.top


<!-- 参考信息 -->