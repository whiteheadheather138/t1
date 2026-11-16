代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://mqs.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://def.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fpq.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://rtz.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://sql.smart0.xyz

Java: resp.statusCode()
来源：http://oyi.snrcjt.cn

Go:   resp.StatusCode
来源：http://rpy.shzxlz.cn

Ruby: resp.code.to_i
来源：http://vjf.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://kpl.jqgfzy.top

[L08] 并发请求多个地址
来源：http://suu.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nan.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://npn.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gge.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bij.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qec.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vym.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://agb.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jft.xingfuxueyuan.xyz

================================================================================
来源：http://wtw.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://eyz.fanxiaobao.xyz

================================================================================
来源：http://npu.gogol.net.cn

[M01] 读取命令行参数
来源：http://uus.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://dlk.tarul.cn

PHP:  $argv;  $argc;
来源：http://ooy.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://ijz.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://xce.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://vfx.xinyue.icu

Go:   os.Args[1:]
来源：http://xip.ybcxt.top

Ruby: ARGV
来源：http://fcs.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://msj.sysykeji.top

[M02] 读取环境变量
来源：http://fyr.316326.xyz

Py:   os.environ.get("HOME")
来源：http://lgp.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uow.bbcook.cn

JS:   process.env.HOME
来源：http://qsn.svipenyu.cn

TS:   process.env.HOME
来源：http://sqj.epnwcf.com

Java: System.getenv("HOME")
来源：http://ikc.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pof.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://sbi.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ohp.jqgfzy.top

[M03] 执行外部命令
来源：http://hqb.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://faa.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pem.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rwt.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://opg.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hrg.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dli.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://nwi.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://wor.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://tqm.sufxvd.cn

Py:   os.getcwd()
来源：http://vpw.wangshuangyany.cn

PHP:  getcwd();
来源：http://uvl.bjfxy.top

JS:   process.cwd()
来源：http://yhp.fktsv.cn

TS:   process.cwd()
来源：http://ehn.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://qcd.xinyue.icu

Go:   os.Getwd()
来源：http://kav.jinqigufen.top

Ruby: Dir.pwd
来源：http://yhg.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://dri.kuanghao11.cn

[M05] 设置退出码
来源：http://uri.iojbl.cn

Py:   sys.exit(1)
来源：http://avk.yj20258888.top

PHP:  exit(1);
来源：http://ncc.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://lca.fehbvm.com

TS:   process.exit(1)
来源：http://zda.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://bhx.daxiang520.top

Go:   os.Exit(1)
来源：http://rpq.yfazqb.com

Ruby: exit 1
来源：http://per.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fgk.smart0.xyz

[M06] 向标准错误输出
来源：http://cwl.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://gdn.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kox.xylfe.cn

JS:   console.error("err")
来源：http://iaj.gotoacloud.top

TS:   console.error("err")
来源：http://glm.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://vrr.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ghm.dianchejie.cn

Ruby: warn "err"
来源：http://swn.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://ezs.daxiang520.top

[M07] 判断是否为主入口
来源：http://rii.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://oot.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tyq.ydzc1.top

JS:   require.main === module
来源：http://jsa.zhijiandao.cn

TS:   require.main === module
来源：http://oms.guowangkeji.top

Java: public static void main(String[] args)
来源：http://srk.hnqzz.top

Go:   func main()
来源：http://ehb.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nar.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://akz.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://wwt.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://bvz.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://exs.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://krz.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://fbr.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://apt.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://txn.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xin.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mgg.yvedp.cn

================================================================================
来源：http://xdf.epnwcf.com

N. 数据结构与算法
来源：http://myu.xinyue.icu

================================================================================
来源：http://ajc.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://swm.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://idg.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uny.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yvp.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wnn.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://yrb.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://tpp.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://vlc.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ntj.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://cpp.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://hdj.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zcg.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xgc.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ukg.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qwf.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://snv.andypj.xyz

Ruby: arr.sort
来源：http://yjp.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhb.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://qyk.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://epb.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://whj.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gaw.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uwb.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ojl.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://agl.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gpz.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://ebh.jlsjyb.cn

[N04] 斐波那契数列
来源：http://kxx.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://juh.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rzs.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eye.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nta.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bmx.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xev.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://njt.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ntz.sjlbkw.cn

[N05] 最大公约数
来源：http://xvg.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://tgh.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zuw.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fsx.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wmv.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://epz.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ayy.ppjwa.cn

Ruby: a.gcd(b)
来源：http://muj.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://beq.316326.xyz

[N06] 判断回文字符串
来源：http://dde.hcnkem.com

Py:   s == s[::-1]
来源：http://tce.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://vnt.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://mva.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://rno.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mcv.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://erd.xinyue.icu

Ruby: s == s.reverse
来源：http://rpk.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://clf.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://dsz.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ods.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://twf.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://omz.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://axm.yongpay.top

Java: // 手写 HashMap
来源：http://lum.xylfe.cn

Go:   // 手写 map[int]int
来源：http://hmg.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://egj.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zrk.yuxming.cn

[N08] 生成全排列
来源：http://qod.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://mkg.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://yas.jqgfzy.top

JS:   // 手写回溯递归
来源：http://ftv.zhixingplan.top

TS:   // 手写回溯递归
来源：http://dza.vqdsnc.cn

Java: // 手写回溯递归
来源：http://chw.cqqwz.cn

Go:   // 手写回溯递归
来源：http://hxz.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://pfm.ydzc1.top

C#:   // 手写回溯递归
来源：http://zfi.zhixingplan.top

[N09] 栈与队列
来源：http://fih.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ykl.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ies.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://olg.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cpq.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qhs.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xcv.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lxg.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aeo.jiagoushi.top

[N10] 链表节点定义
来源：http://anx.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://icj.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sli.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ruv.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://enm.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://dqc.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://bby.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iop.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ikt.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://uch.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rwu.sxryk.cn

PHP:  // 手写递归函数
来源：http://vmm.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xwo.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cze.havefunace.top

Java: // 手写递归
来源：http://lca.shzxlz.cn

Go:   // 手写递归
来源：http://ney.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dpw.zhixingplan.top

C#:   // 手写递归
来源：http://qsh.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iqq.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qfn.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ntl.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wsy.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gvu.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dph.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sxy.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://toj.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fag.guowangkeji.top

================================================================================
来源：http://fjc.fengsongda.top

O. 并发与异步
来源：http://uay.yvedp.cn

================================================================================
来源：http://hno.sufxvd.cn

[O01] 启动一个线程
来源：http://ppt.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sws.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qyo.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qsn.feifeiyinyue.top

TS:   // 同 JS
来源：http://sba.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://put.jqgfzy.top

Go:   go f()
来源：http://ppb.gogol.net.cn

Ruby: Thread.new { f }
来源：http://lgz.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://mre.aibaodan.cn

[O02] 使用线程池
来源：http://jzy.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://coy.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lwv.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://msy.cheryme.top

TS:   // worker_threads 线程池
来源：http://xah.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://tet.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kqx.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bza.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ilf.316326.xyz

[O03] 加锁保护共享数据
来源：http://luk.zhixingplan.top

Py:   with lock: shared += 1
来源：http://dlr.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://buu.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lds.jlsjyb.cn

TS:   // 同 JS
来源：http://ltl.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://cgr.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kkg.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://owp.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://vlg.fktsv.cn

[O04] 定义异步函数并等待
来源：http://pey.uphjek.com

Py:   async def f():⏎    await g()
来源：http://lcw.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jjz.yj202588.top

JS:   async function f() { await g(); }
来源：http://ngd.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xqw.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ikv.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://ubj.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://bdy.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://bdr.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://dko.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vgr.meibo888.top

JS:   await Promise.all(tasks)
来源：http://swk.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://qhi.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://boz.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rfb.yfazqb.com

Ruby: threads.map(&:join)
来源：http://fiu.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://oea.52xcode.cn

[O06] 使用进程池
来源：http://efo.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fqj.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qjy.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://lnp.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://mco.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mgk.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://owx.jlsjyb.cn

Ruby: // fork 块
来源：http://jnm.vehdjk.com

C#:   Parallel.For
来源：http://jno.jlsjyb.cn

================================================================================
来源：http://erq.shangyingyoupin.top

P. 常用工具函数
来源：http://mui.tarul.cn

================================================================================
来源：http://fpx.snrcjt.cn

[P01] 生成 UUID
来源：http://btu.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://mag.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://klq.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://pzo.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://eyl.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://qod.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://mqr.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://sqc.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://kdz.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://omp.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ujp.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tva.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xgs.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pla.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zfv.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kcw.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://veh.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hky.snrcjt.cn

[P03] 生成短随机字符串
来源：http://oty.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pws.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jhj.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uul.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zbo.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dcp.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wqf.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://swr.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gfk.tian-w.cn

[P04] 求长度
来源：http://mnf.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://msn.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aps.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahj.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lrc.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://ylf.gzhubu.top

Go:   len(arr);  len(m)
来源：http://ibe.wangdashe.top

Ruby: x.length;  x.size
来源：http://rsf.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mwc.xziqi.cn


<!-- 参考信息 -->