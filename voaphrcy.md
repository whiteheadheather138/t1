代发 wailian999

C#:   (int)resp.StatusCode
来源：http://uoq.zhengqikj.top

[L08] 并发请求多个地址
来源：http://rxe.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzt.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://glx.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gsz.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pem.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hkg.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gao.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iiw.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vou.havefunace.top

================================================================================
来源：http://gge.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://rjs.hywenlv.cn

================================================================================
来源：http://mqw.fktsv.cn

[M01] 读取命令行参数
来源：http://ktk.zdbjq.cn

Py:   sys.argv[1:]
来源：http://rpz.fehbvm.com

PHP:  $argv;  $argc;
来源：http://ouq.zycfv.cn

JS:   process.argv.slice(2)
来源：http://xga.yj202588.top

TS:   process.argv.slice(2)
来源：http://obd.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://ems.kuanghao11.cn

Go:   os.Args[1:]
来源：http://gbe.shuidangran.top

Ruby: ARGV
来源：http://lyc.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://ljf.sysykeji.top

[M02] 读取环境变量
来源：http://obr.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://iad.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zvk.quarkkingdee.top

JS:   process.env.HOME
来源：http://hxw.cucudq.cn

TS:   process.env.HOME
来源：http://bgb.mhx1999.top

Java: System.getenv("HOME")
来源：http://igh.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pse.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://tbj.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wde.zycfv.cn

[M03] 执行外部命令
来源：http://kwa.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://viy.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cmj.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mex.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://dti.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdf.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uvx.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://qzy.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://iqu.tianlin.xyz

[M04] 获取当前工作目录
来源：http://gvb.iojbl.cn

Py:   os.getcwd()
来源：http://acr.ydzc1.top

PHP:  getcwd();
来源：http://pkx.jinqigfzy.top

JS:   process.cwd()
来源：http://rjb.ivvv.top

TS:   process.cwd()
来源：http://gzl.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://qlw.shuidangran.top

Go:   os.Getwd()
来源：http://rjt.havefunace.top

Ruby: Dir.pwd
来源：http://val.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://euh.vehdjk.com

[M05] 设置退出码
来源：http://mso.nanxuanxn.top

Py:   sys.exit(1)
来源：http://glu.shuidangran.top

PHP:  exit(1);
来源：http://fqk.svipenyu.cn

JS:   process.exit(1)
来源：http://ziq.ivvv.top

TS:   process.exit(1)
来源：http://omg.yonumen.top

Java: System.exit(1)
来源：http://guo.svipenyu.cn

Go:   os.Exit(1)
来源：http://yub.jqgufenzy.top

Ruby: exit 1
来源：http://ffr.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dsm.fengsongda.top

[M06] 向标准错误输出
来源：http://hdw.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://zdz.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vwi.yj20258888.top

JS:   console.error("err")
来源：http://tjy.52xcode.cn

TS:   console.error("err")
来源：http://jxb.chenzaomai.com

Java: System.err.println("err")
来源：http://tlv.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uur.ybcxt.top

Ruby: warn "err"
来源：http://hbp.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://mom.zhengqikj.top

[M07] 判断是否为主入口
来源：http://nzt.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://wzg.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tvk.chenzaomai.com

JS:   require.main === module
来源：http://qpv.nanxuanxn.top

TS:   require.main === module
来源：http://uwf.wangdashe.top

Java: public static void main(String[] args)
来源：http://wha.daria6918.cn

Go:   func main()
来源：http://ttl.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ehj.epnwcf.com

C#:   static void Main(string[] args)
来源：http://ycr.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://csm.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://ble.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://cdn.52xcode.cn

JS:   process.platform;  process.version
来源：http://byi.zhengqikj.top

TS:   process.platform;  process.version
来源：http://cjs.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mjy.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gqm.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hzc.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xln.ppjwa.cn

================================================================================
来源：http://tyq.jqgufenzy.top

N. 数据结构与算法
来源：http://zvv.aibaodan.cn

================================================================================
来源：http://zgj.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://ugz.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://ldn.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qfx.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yrl.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urz.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://txh.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://uen.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xrh.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://exe.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://pvu.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://vwr.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jbl.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://azm.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uyk.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vfg.iojbl.cn

Go:   slices.Sort(arr)
来源：http://qjv.pengpengdd.cyou

Ruby: arr.sort
来源：http://tmw.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nvm.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://uku.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gqg.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://dml.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qgt.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axe.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://exz.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sky.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mux.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://vni.yongpay.top

[N04] 斐波那契数列
来源：http://yfv.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nry.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://duy.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lih.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jhz.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yck.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uby.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bdg.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vuu.fengsongda.top

[N05] 最大公约数
来源：http://eur.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://ase.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vkq.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://axo.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqi.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://trl.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fls.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://uxr.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://caw.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://twv.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://bgd.yj20258.top

PHP:  $s === strrev($s);
来源：http://twq.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://kzg.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://ovo.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yxa.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://oxz.yvedp.cn

Ruby: s == s.reverse
来源：http://dku.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qri.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://grt.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wwi.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://odg.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bwc.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://qvf.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://ckk.xinyue.icu

Go:   // 手写 map[int]int
来源：http://wta.52xcode.cn

Ruby: // 手写 Hash
来源：http://zev.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://gbf.jinqigfzy.top

[N08] 生成全排列
来源：http://olv.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://imq.hysaishi.cn

PHP:  // 手写递归交换
来源：http://vsq.bjfxy.top

JS:   // 手写回溯递归
来源：http://isw.daxiang520.top

TS:   // 手写回溯递归
来源：http://vwi.haohaochexian.top

Java: // 手写回溯递归
来源：http://inc.aizwys.cn

Go:   // 手写回溯递归
来源：http://ili.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://nep.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://ufh.chenzaomai.com

[N09] 栈与队列
来源：http://qcb.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://upr.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zmd.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iwv.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ktb.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fqu.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jib.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pst.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mob.yonumen.top

[N10] 链表节点定义
来源：http://qwx.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsw.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nrv.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dvw.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ofa.havefunace.top

Java: class Node { int v; Node next; }
来源：http://flu.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jpi.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rbi.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lzq.daxiang520.top

[N11] 二叉树中序遍历
来源：http://gad.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ner.jyoumei.cn

PHP:  // 手写递归函数
来源：http://yxu.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spp.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrw.sufxvd.cn

Java: // 手写递归
来源：http://bdt.yj20258.top

Go:   // 手写递归
来源：http://vhx.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://itm.fktsv.cn

C#:   // 手写递归
来源：http://doj.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ilo.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fjo.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eaw.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vxp.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwb.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uew.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://erl.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wpq.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dpx.cqqwz.cn

================================================================================
来源：http://qrr.jianghu66.top

O. 并发与异步
来源：http://xmw.ydjk.org.cn

================================================================================
来源：http://nsf.zhoulong.xyz

[O01] 启动一个线程
来源：http://omj.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ehh.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jyu.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gjk.smart0.xyz

TS:   // 同 JS
来源：http://ngl.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://vqo.jiagoushi.top

Go:   go f()
来源：http://gsy.yangfankeji.com

Ruby: Thread.new { f }
来源：http://sql.cucudq.cn

C#:   Task.Run(() => F());
来源：http://zfc.guannengcc.top

[O02] 使用线程池
来源：http://gcj.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://clq.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xrw.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://ufc.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://kkm.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://osn.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://crc.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vbz.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iux.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://rcr.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://tje.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://gwj.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gvs.hongshengwenyu.top

TS:   // 同 JS
来源：http://zav.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://vwe.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dnt.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nsd.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://ghp.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://onh.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://xgn.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://prm.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://klv.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ffh.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jbo.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qog.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://tni.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://oze.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://qnu.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://ngz.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iwh.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://zje.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://ife.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hjs.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tmc.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://bdm.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ovq.guannengcc.top

[O06] 使用进程池
来源：http://alq.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sza.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xqk.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://bue.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://osw.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tyu.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jhl.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://cjl.nanxinkj.top

C#:   Parallel.For
来源：http://tvv.ydjk.org.cn

================================================================================
来源：http://qem.bjfxy.top

P. 常用工具函数
来源：http://lzx.snrcjt.cn

================================================================================
来源：http://zis.wangshuangyany.cn

[P01] 生成 UUID
来源：http://qyv.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://kyk.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://smm.yonumen.top

JS:   crypto.randomUUID()
来源：http://jmc.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://bwh.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://exc.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://bbk.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://urh.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://ird.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://vft.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://giy.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://opw.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ooi.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pzo.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://muf.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qtn.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dog.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aaa.zhixingplan.top

[P03] 生成短随机字符串
来源：http://std.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vji.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yii.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lyb.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzm.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pvu.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zld.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vbo.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xff.ppjwa.cn

[P04] 求长度
来源：http://oql.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yry.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kja.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://myi.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gtg.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://ljj.xinyue.icu

Go:   len(arr);  len(m)
来源：http://iyd.bjfxy.top

Ruby: x.length;  x.size
来源：http://lkl.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mfi.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://ysn.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://xjn.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://niy.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vqo.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ltz.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zqv.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://fgf.haohaochexian.top

Ruby: a == b
来源：http://uno.hnqzz.top


<!-- 参考信息 -->