代发 wailian999

JS:   process.argv.slice(2)
来源：http://qty.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://bze.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://rcz.fengsongda.top

Go:   os.Args[1:]
来源：http://yho.gogol.net.cn

Ruby: ARGV
来源：http://gkm.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://odb.chenjidiqi.icu

[M02] 读取环境变量
来源：http://vlt.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://vtv.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kmm.jqgufenzy.top

JS:   process.env.HOME
来源：http://dds.ivvv.top

TS:   process.env.HOME
来源：http://pml.fzhhl.top

Java: System.getenv("HOME")
来源：http://voq.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxy.xziqi.cn

Ruby: ENV["HOME"]
来源：http://fyk.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qsc.ydzc1.top

[M03] 执行外部命令
来源：http://kye.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://evz.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qbl.guowangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wrz.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vfy.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dyl.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qmh.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://voe.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://ehl.ybcxt.top

[M04] 获取当前工作目录
来源：http://wdr.xziqi.cn

Py:   os.getcwd()
来源：http://ozx.fehbvm.com

PHP:  getcwd();
来源：http://csm.bbcook.cn

JS:   process.cwd()
来源：http://luy.hnxiangtu.top

TS:   process.cwd()
来源：http://gwi.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://egs.gzhubu.top

Go:   os.Getwd()
来源：http://sbq.haohaochexian.top

Ruby: Dir.pwd
来源：http://zue.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rgx.quarkkingdee.top

[M05] 设置退出码
来源：http://cji.tianlin.xyz

Py:   sys.exit(1)
来源：http://qhb.svipenyu.cn

PHP:  exit(1);
来源：http://fyx.redwolf501.top

JS:   process.exit(1)
来源：http://tca.jlsjyb.cn

TS:   process.exit(1)
来源：http://lvi.ybcxt.top

Java: System.exit(1)
来源：http://iwe.gogol.net.cn

Go:   os.Exit(1)
来源：http://fad.hesvh.cn

Ruby: exit 1
来源：http://zow.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://juf.yuanzhike.top

[M06] 向标准错误输出
来源：http://pkg.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://clv.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://rme.sysykeji.top

JS:   console.error("err")
来源：http://mqi.hcnkem.com

TS:   console.error("err")
来源：http://kvp.gotoacloud.top

Java: System.err.println("err")
来源：http://nxb.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zdf.aibaodan.cn

Ruby: warn "err"
来源：http://pdt.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://fgo.hfpthk.cn

[M07] 判断是否为主入口
来源：http://tnx.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://hzi.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hdf.jiagoushi.top

JS:   require.main === module
来源：http://olb.cqqwz.cn

TS:   require.main === module
来源：http://zka.yonumen.top

Java: public static void main(String[] args)
来源：http://irk.ehwqpu.com

Go:   func main()
来源：http://nqp.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ovo.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://zir.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://ibg.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://gqn.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://pqk.52xcode.cn

JS:   process.platform;  process.version
来源：http://uly.redwolf501.top

TS:   process.platform;  process.version
来源：http://tmj.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jyd.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rwd.chenlongwang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://puz.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kyr.jiagoushi.top

================================================================================
来源：http://gvj.pycfn.com

N. 数据结构与算法
来源：http://ctj.zycfv.cn

================================================================================
来源：http://dtw.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://bao.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lsl.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zpy.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eel.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rcx.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://zhu.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://mle.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kop.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://akp.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://sqz.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://lcl.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://osj.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://toh.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sei.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cvy.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://rga.ybcxt.top

Ruby: arr.sort
来源：http://mzk.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://adn.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://iva.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gjr.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://otd.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bou.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://skv.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ekt.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xym.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uam.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yqa.yueranfly.top

[N04] 斐波那契数列
来源：http://aig.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nxl.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iey.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://crq.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://way.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mor.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kve.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mft.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zzm.hfpthk.cn

[N05] 最大公约数
来源：http://sjp.hesvh.cn

Py:   math.gcd(a, b)
来源：http://mln.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ijn.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rwc.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hef.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lfm.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jon.gotoacloud.top

Ruby: a.gcd(b)
来源：http://azl.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dpz.bbcook.cn

[N06] 判断回文字符串
来源：http://myr.tarul.cn

Py:   s == s[::-1]
来源：http://hin.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://mhn.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://qrp.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://uhp.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vmy.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://wsb.aibaodan.cn

Ruby: s == s.reverse
来源：http://rjh.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ytw.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://pym.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jfi.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://haf.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nbs.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://yjf.gogol.net.cn

Java: // 手写 HashMap
来源：http://zhs.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://jdy.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://igb.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sdj.yonumen.top

[N08] 生成全排列
来源：http://uof.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://cvc.9152youxi.cn

PHP:  // 手写递归交换
来源：http://vzu.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://yea.tanke756.top

TS:   // 手写回溯递归
来源：http://fbr.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://ify.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://vhx.yj20258.top

Ruby: arr.permutation.to_a
来源：http://lfn.haohaochexian.top

C#:   // 手写回溯递归
来源：http://chn.ppjwa.cn

[N09] 栈与队列
来源：http://dyb.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://huu.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ubv.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://daj.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gqo.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iyt.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mrc.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eks.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jzd.guannengcc.top

[N10] 链表节点定义
来源：http://xwr.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hii.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ubz.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jlp.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tgx.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://ggz.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lct.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iir.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lyf.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://lii.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://has.meibo888.top

PHP:  // 手写递归函数
来源：http://ucy.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vhn.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mhi.xylfe.cn

Java: // 手写递归
来源：http://kzk.gogol.net.cn

Go:   // 手写递归
来源：http://bim.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pbq.tarul.cn

C#:   // 手写递归
来源：http://lbd.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qie.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://biu.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hiv.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kmb.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ooy.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wqb.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vhy.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rzy.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xtr.yj20258.top

================================================================================
来源：http://vzy.xingfuxueyuan.xyz

O. 并发与异步
来源：http://lor.fehbvm.com

================================================================================
来源：http://bdy.ehwqpu.com

[O01] 启动一个线程
来源：http://lba.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kfp.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uof.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wrh.feifeiyinyue.top

TS:   // 同 JS
来源：http://kku.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://ahv.sufxvd.cn

Go:   go f()
来源：http://dct.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://vtk.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://cxt.jyoumei.cn

[O02] 使用线程池
来源：http://cvr.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hxk.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bpt.ivvv.top

JS:   // worker_threads 线程池
来源：http://ywy.andypj.xyz

TS:   // worker_threads 线程池
来源：http://vuo.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://sdt.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mtl.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://stt.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wxd.yonumen.top

[O03] 加锁保护共享数据
来源：http://ryf.ivvv.top

Py:   with lock: shared += 1
来源：http://mmg.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://kua.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cnl.tian-w.cn

TS:   // 同 JS
来源：http://tfh.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://itk.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bxe.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hjh.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://kuv.hnqzz.top

[O04] 定义异步函数并等待
来源：http://ner.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://ayw.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blm.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://syv.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mnd.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kot.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dns.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qqd.birdmap.top

C#:   async Task F() { await G(); }
来源：http://eum.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://buk.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://lov.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jve.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://mao.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://jab.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dfv.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vdu.uphjek.com

Ruby: threads.map(&:join)
来源：http://nyl.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vrr.chenzaomai.com

[O06] 使用进程池
来源：http://kbj.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gaf.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ltu.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://out.cashguo.top

TS:   // child_process / cluster 模块
来源：http://ypj.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://csq.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rdf.vqdsnc.cn

Ruby: // fork 块
来源：http://lob.xuetiantiany.cn

C#:   Parallel.For
来源：http://lll.zhongyouzk.top

================================================================================
来源：http://cag.sjlbkw.cn

P. 常用工具函数
来源：http://cnr.shuidangran.top

================================================================================
来源：http://zdp.xuanzx.com

[P01] 生成 UUID
来源：http://jqf.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://uzf.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jet.yj202588.top

JS:   crypto.randomUUID()
来源：http://hjc.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://hup.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://lfl.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://boj.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://qkk.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://usj.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://txd.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gpt.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://gqo.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pvk.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kvl.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://slx.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ilx.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wqa.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lmo.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://jup.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wla.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bzn.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xbf.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vte.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ger.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lla.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iwi.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fzw.ydjk.org.cn

[P04] 求长度
来源：http://dsy.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yir.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://drd.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqw.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://npf.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://zcr.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://tod.shuidangran.top

Ruby: x.length;  x.size
来源：http://gox.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://myh.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://fsj.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lcm.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kek.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sch.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mgx.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aoo.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://tzs.quarkkingdee.top

Ruby: a == b
来源：http://qdv.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nxk.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tlh.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ypn.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://jgz.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bqa.dianchejie.cn

TS:   if (x == null) {}
来源：http://mge.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://prg.52xcode.cn

Go:   if x == nil {}
来源：http://ury.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fba.dashuyun.cn

C#:   if (x is null) {}
来源：http://jcm.hnxiangtu.top

[P07] 防抖与节流
来源：http://wna.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zwu.316326.xyz

PHP:  // 手写时间戳比较
来源：http://kek.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ube.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dfv.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fwf.guowangkeji.top


<!-- 参考信息 -->