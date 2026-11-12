代发 wailian999

C#:   (int)resp.StatusCode
来源：http://iti.chenlongwang.top

[L08] 并发请求多个地址
来源：http://yme.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://azt.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://occ.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lpt.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uxo.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jui.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jud.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wzc.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gui.cashguo.top

================================================================================
来源：http://ktr.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://krc.hysaishi.cn

================================================================================
来源：http://emz.vqdsnc.cn

[M01] 读取命令行参数
来源：http://gyt.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://mam.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://pbf.ybcxt.top

JS:   process.argv.slice(2)
来源：http://tbz.fzhhl.top

TS:   process.argv.slice(2)
来源：http://jrs.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://kjw.yueranfly.top

Go:   os.Args[1:]
来源：http://pmw.yonumen.top

Ruby: ARGV
来源：http://cqp.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://tge.feifeiyinyue.top

[M02] 读取环境变量
来源：http://pey.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://vcu.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://paf.jqgfzy.top

JS:   process.env.HOME
来源：http://ttn.ctjpmb.com

TS:   process.env.HOME
来源：http://qfh.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://wow.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://agf.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://ucy.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gxv.tanke756.top

[M03] 执行外部命令
来源：http://qlu.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hap.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nup.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rrr.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kdc.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rwx.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://whb.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://qqf.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://nex.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://jhm.redwolf501.top

Py:   os.getcwd()
来源：http://knn.ydjk.org.cn

PHP:  getcwd();
来源：http://wfi.meibo888.top

JS:   process.cwd()
来源：http://lfc.meibo888.top

TS:   process.cwd()
来源：http://ucw.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://uyl.bbcook.cn

Go:   os.Getwd()
来源：http://gbx.jinqigfzy.top

Ruby: Dir.pwd
来源：http://oqo.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://ons.xylfe.cn

[M05] 设置退出码
来源：http://wbh.svipenyu.cn

Py:   sys.exit(1)
来源：http://mov.yuxming.cn

PHP:  exit(1);
来源：http://ezr.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://esl.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://fhn.havefunace.top

Java: System.exit(1)
来源：http://uty.guowangkeji.top

Go:   os.Exit(1)
来源：http://mmy.zhaomingkeji.xyz

Ruby: exit 1
来源：http://pmf.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://flg.mhx1999.top

[M06] 向标准错误输出
来源：http://skg.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://gzf.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://arw.hfpthk.cn

JS:   console.error("err")
来源：http://dbn.nanxinkj.top

TS:   console.error("err")
来源：http://uir.cheryme.top

Java: System.err.println("err")
来源：http://cgd.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ivu.bjfxy.top

Ruby: warn "err"
来源：http://hyv.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://kyw.yvedp.cn

[M07] 判断是否为主入口
来源：http://xwn.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://jjt.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qnt.gotoacloud.top

JS:   require.main === module
来源：http://bzq.bjfxy.top

TS:   require.main === module
来源：http://dca.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://ngk.hongshengwenyu.top

Go:   func main()
来源：http://msm.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://flv.havefunace.top

C#:   static void Main(string[] args)
来源：http://xbb.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://kmx.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://tyq.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://qje.sxryk.cn

JS:   process.platform;  process.version
来源：http://ith.dashuyun.cn

TS:   process.platform;  process.version
来源：http://ino.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kjo.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nue.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qwj.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jly.hcnkem.com

================================================================================
来源：http://hhr.sysykeji.top

N. 数据结构与算法
来源：http://lzl.svipenyu.cn

================================================================================
来源：http://qkk.cheryme.top

[N01] 二分查找（有序数组）
来源：http://sxl.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://wqg.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cut.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxf.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vhp.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kgh.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://fmz.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eow.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tms.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://kbc.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://xcw.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oxj.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://per.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://msd.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ldw.gzhubu.top

Go:   slices.Sort(arr)
来源：http://cfr.tarul.cn

Ruby: arr.sort
来源：http://kjd.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cgj.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://ggx.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dct.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://jko.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvs.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qsq.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zdj.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qal.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hcr.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://osp.hywenlv.cn

[N04] 斐波那契数列
来源：http://kvs.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kpg.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://klu.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lsp.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nel.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iuw.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cld.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rxs.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uzw.sysykeji.top

[N05] 最大公约数
来源：http://kfk.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://gol.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sbt.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hns.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edo.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://otm.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nww.sysykeji.top

Ruby: a.gcd(b)
来源：http://gjt.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yiv.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://aia.ydjk.org.cn

Py:   s == s[::-1]
来源：http://rlk.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://ron.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://ena.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://pax.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://esm.yj202588.top

Go:   // 双指针从两端比较
来源：http://ico.iojbl.cn

Ruby: s == s.reverse
来源：http://nak.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hod.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://hjf.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lpm.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mkg.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jir.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://yha.jinqigfzy.top

Java: // 手写 HashMap
来源：http://tmy.shuidangran.top

Go:   // 手写 map[int]int
来源：http://msx.zdbjq.cn

Ruby: // 手写 Hash
来源：http://tee.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://htp.fanxiaobao.xyz

[N08] 生成全排列
来源：http://svd.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://ypj.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://agf.svipenyu.cn

JS:   // 手写回溯递归
来源：http://fvw.ydzc1.top

TS:   // 手写回溯递归
来源：http://xas.zhongyouzk.top

Java: // 手写回溯递归
来源：http://voy.daria6918.cn

Go:   // 手写回溯递归
来源：http://bul.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://qbk.hywenlv.cn

C#:   // 手写回溯递归
来源：http://zlt.nwbrower.top

[N09] 栈与队列
来源：http://viw.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vpj.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nmf.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jrz.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tah.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sta.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://psx.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tao.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://orl.feifeiyinyue.top

[N10] 链表节点定义
来源：http://ohy.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vnf.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sby.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dhg.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sgo.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://kbr.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://fmn.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uhg.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ozj.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://xbo.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://abz.fehbvm.com

PHP:  // 手写递归函数
来源：http://dbh.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vkv.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zss.wangdashe.top

Java: // 手写递归
来源：http://jas.hywenlv.cn

Go:   // 手写递归
来源：http://bbh.gotoacloud.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bag.zhiwuduotai.top

C#:   // 手写递归
来源：http://gwh.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pnf.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pxo.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yjr.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mar.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcr.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwa.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ilg.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ddl.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jms.ehwqpu.com

================================================================================
来源：http://bdn.chenjidiqi.icu

O. 并发与异步
来源：http://bgj.hysaishi.cn

================================================================================
来源：http://uwa.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://oea.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oed.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ceb.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ccr.bjfxy.top

TS:   // 同 JS
来源：http://byj.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://tec.316326.xyz

Go:   go f()
来源：http://vgx.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://egm.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://zia.hcnkem.com

[O02] 使用线程池
来源：http://pde.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zzn.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://evi.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://xqo.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://ifs.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://bhi.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tqf.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gfc.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gje.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://sjq.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://zsc.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://kbm.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ybn.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://xmz.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://mwa.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bsy.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dfl.sweek.top

C#:   lock (gate) { shared++; }
来源：http://zwq.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://lgp.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://edv.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qto.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://dal.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dnf.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dbx.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dxe.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://egr.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://rkk.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://jpw.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://pwp.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qey.cheryme.top

JS:   await Promise.all(tasks)
来源：http://aeo.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://mbf.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://efu.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ofy.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://mrg.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dcd.jianghu66.top

[O06] 使用进程池
来源：http://xyg.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pdk.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ubp.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://mtb.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://dtq.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ygc.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bib.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://mxe.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://bzd.epnwcf.com

================================================================================
来源：http://oxp.wangdashe.top

P. 常用工具函数
来源：http://bfd.fktsv.cn

================================================================================
来源：http://uxa.tanke756.top

[P01] 生成 UUID
来源：http://quc.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://cvo.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iwx.sxryk.cn

JS:   crypto.randomUUID()
来源：http://sjh.ybcxt.top

TS:   crypto.randomUUID()
来源：http://ljg.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://ewf.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://kuz.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://yyc.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://jjp.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://ybl.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hjj.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fnb.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umr.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cqr.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xyr.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fsp.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jzd.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aol.xylfe.cn

[P03] 生成短随机字符串
来源：http://dqb.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cdi.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fzw.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtp.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvt.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://snu.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jbt.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://fkz.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bhj.kuanghao11.cn

[P04] 求长度
来源：http://rqs.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jri.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://atd.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oba.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvm.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://jdu.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://lbl.shzxlz.cn

Ruby: x.length;  x.size
来源：http://jge.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pgk.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://acz.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://xlz.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qgv.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ptw.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vov.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ibq.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://bci.quarkkingdee.top

Ruby: a == b
来源：http://pxj.sjlbkw.cn


<!-- 参考信息 -->