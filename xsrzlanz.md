代发 wailian999

C#:   (int)resp.StatusCode
来源：http://jyg.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://lhr.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uxk.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://aur.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ebj.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sks.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vdo.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mfa.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qtm.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fgi.mhx1999.top

================================================================================
来源：http://xzz.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://krt.sxryk.cn

================================================================================
来源：http://bhj.wangdashe.top

[M01] 读取命令行参数
来源：http://xyx.yongpay.top

Py:   sys.argv[1:]
来源：http://mrn.hesvh.cn

PHP:  $argv;  $argc;
来源：http://eec.mhx1999.top

JS:   process.argv.slice(2)
来源：http://npr.yongpay.top

TS:   process.argv.slice(2)
来源：http://cjg.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://uyv.xuanzx.com

Go:   os.Args[1:]
来源：http://xep.yj202588.top

Ruby: ARGV
来源：http://qav.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://dxe.ybcxt.top

[M02] 读取环境变量
来源：http://iau.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://vfq.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lda.yuanzhike.top

JS:   process.env.HOME
来源：http://mta.sufxvd.cn

TS:   process.env.HOME
来源：http://rcf.fengsongda.top

Java: System.getenv("HOME")
来源：http://bef.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hew.xylfe.cn

Ruby: ENV["HOME"]
来源：http://ffe.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pds.hfpthk.cn

[M03] 执行外部命令
来源：http://ggm.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yuz.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wbl.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qwi.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wyc.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zzm.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ocn.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://hpd.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://eff.ehwqpu.com

[M04] 获取当前工作目录
来源：http://fgv.hongshengwenyu.top

Py:   os.getcwd()
来源：http://eqw.jyoumei.cn

PHP:  getcwd();
来源：http://tgn.xziqi.cn

JS:   process.cwd()
来源：http://rmz.tian-w.cn

TS:   process.cwd()
来源：http://utq.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://msh.tarul.cn

Go:   os.Getwd()
来源：http://xxq.hnqzz.top

Ruby: Dir.pwd
来源：http://sef.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://ofs.sweek.top

[M05] 设置退出码
来源：http://dxt.tarul.cn

Py:   sys.exit(1)
来源：http://eye.daria6918.cn

PHP:  exit(1);
来源：http://ukt.jyoumei.cn

JS:   process.exit(1)
来源：http://ufu.birdmap.top

TS:   process.exit(1)
来源：http://lip.yangfankeji.com

Java: System.exit(1)
来源：http://mbe.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://pog.guowangkeji.top

Ruby: exit 1
来源：http://mhq.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pul.zhoulong.xyz

[M06] 向标准错误输出
来源：http://riv.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://xgl.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gqf.jinqigufen.top

JS:   console.error("err")
来源：http://kwx.tarul.cn

TS:   console.error("err")
来源：http://coj.ydzc1.top

Java: System.err.println("err")
来源：http://cko.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mdj.fanxiaobao.xyz

Ruby: warn "err"
来源：http://gik.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://dqz.daxiang520.top

[M07] 判断是否为主入口
来源：http://sdb.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://jih.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vqs.yangfankeji.com

JS:   require.main === module
来源：http://pus.hongshengwenyu.top

TS:   require.main === module
来源：http://wdi.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://umq.xuanzx.com

Go:   func main()
来源：http://bfr.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bag.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://vgz.316326.xyz

[M08] 获取系统与运行时信息
来源：http://nix.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://kxx.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://rgv.jqgfzy.top

JS:   process.platform;  process.version
来源：http://bot.bjfxy.top

TS:   process.platform;  process.version
来源：http://vhi.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qxs.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://prm.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qpl.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zhn.pengpengdd.cyou

================================================================================
来源：http://nnw.vehdjk.com

N. 数据结构与算法
来源：http://nrk.xuanzx.com

================================================================================
来源：http://oae.havefunace.top

[N01] 二分查找（有序数组）
来源：http://nek.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://gav.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mpu.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://och.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tpl.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://mnr.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://lww.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://wfv.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://kqr.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://vjj.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://nvj.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hnc.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://thw.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://nom.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bpg.gzhubu.top

Go:   slices.Sort(arr)
来源：http://vsd.zhoulong.xyz

Ruby: arr.sort
来源：http://qzz.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lug.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://bkn.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tfk.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://cva.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vmd.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcd.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wby.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yot.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hau.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://ytv.fehbvm.com

[N04] 斐波那契数列
来源：http://bzt.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpf.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nfp.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vcb.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hvb.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://flr.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jee.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ija.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wsm.fanxiaobao.xyz

[N05] 最大公约数
来源：http://pgs.hesvh.cn

Py:   math.gcd(a, b)
来源：http://oug.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vdh.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fke.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tcj.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xap.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jmm.yongpay.top

Ruby: a.gcd(b)
来源：http://pku.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aay.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://yyp.316326.xyz

Py:   s == s[::-1]
来源：http://hyl.meibo888.top

PHP:  $s === strrev($s);
来源：http://juf.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://jqr.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://ghd.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yhr.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://nvs.nanxuanxn.top

Ruby: s == s.reverse
来源：http://ibu.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hcv.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://oqc.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jai.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xpr.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vzv.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://uja.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://ldd.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://sfn.dashuyun.cn

Ruby: // 手写 Hash
来源：http://uli.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kwp.epnwcf.com

[N08] 生成全排列
来源：http://bcd.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://voh.zhengqikj.top

PHP:  // 手写递归交换
来源：http://xzi.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://pyz.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://nid.bjfxy.top

Java: // 手写回溯递归
来源：http://bcs.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://yvs.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://cta.xuanzx.com

C#:   // 手写回溯递归
来源：http://pdv.yj20258.top

[N09] 栈与队列
来源：http://nxn.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oce.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yya.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cgy.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kut.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdd.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gdq.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sse.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ixc.zhoulong.xyz

[N10] 链表节点定义
来源：http://xxg.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hkn.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kqa.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tpy.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lfp.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://bcq.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://ymv.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cti.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hrz.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://cpv.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://epw.svipenyu.cn

PHP:  // 手写递归函数
来源：http://gmd.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfg.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dln.jinqigfzy.top

Java: // 手写递归
来源：http://kci.fanxiaobao.xyz

Go:   // 手写递归
来源：http://asg.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lgr.sufxvd.cn

C#:   // 手写递归
来源：http://ddq.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://djx.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qdm.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vvo.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ukv.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qzt.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://guk.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aef.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bqn.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jjs.guannengcc.top

================================================================================
来源：http://rol.fehbvm.com

O. 并发与异步
来源：http://rci.redwolf501.top

================================================================================
来源：http://nqn.dashuyun.cn

[O01] 启动一个线程
来源：http://hwe.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lxu.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hcx.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lsf.ppjwa.cn

TS:   // 同 JS
来源：http://gbs.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://fhs.dashuyun.cn

Go:   go f()
来源：http://ske.0kj1m.cn

Ruby: Thread.new { f }
来源：http://fxt.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://eab.yuanzhike.top

[O02] 使用线程池
来源：http://muk.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rmm.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://snu.ivvv.top

JS:   // worker_threads 线程池
来源：http://fja.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://lzf.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://bxh.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://saa.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://smd.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://trp.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://zpe.0kj1m.cn

Py:   with lock: shared += 1
来源：http://fhx.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://xfl.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://shg.shzxlz.cn

TS:   // 同 JS
来源：http://eyi.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://skk.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vwy.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uaz.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://fev.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://bou.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://qro.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kjn.wangdashe.top

JS:   async function f() { await g(); }
来源：http://qpp.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gbq.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xkj.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ezi.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zvd.xuetiantiany.cn

C#:   async Task F() { await G(); }
来源：http://wxb.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://dax.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://znb.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tqt.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://xmo.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://zrb.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://itv.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hqg.pycfn.com

Ruby: threads.map(&:join)
来源：http://vpy.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jpa.snrcjt.cn

[O06] 使用进程池
来源：http://anl.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gav.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://lmn.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://vif.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://brr.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://svg.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uuf.hnqzz.top

Ruby: // fork 块
来源：http://uhr.ivvv.top

C#:   Parallel.For
来源：http://rlv.xuetiantiany.cn

================================================================================
来源：http://dai.svipenyu.cn

P. 常用工具函数
来源：http://cbk.svipenyu.cn

================================================================================
来源：http://aeh.fzhhl.top

[P01] 生成 UUID
来源：http://zsi.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://cxw.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pvx.shuidangran.top

JS:   crypto.randomUUID()
来源：http://wde.redwolf501.top

TS:   crypto.randomUUID()
来源：http://nuw.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://dvc.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://rtl.tarul.cn

Ruby: SecureRandom.uuid
来源：http://xji.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://jcz.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://jrv.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lbw.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cad.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xmv.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xxe.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sxy.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sft.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pqt.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kzj.sweek.top

[P03] 生成短随机字符串
来源：http://kuz.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pnm.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fpx.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iyv.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://muo.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gsl.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fkw.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://pqc.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://brt.tanke756.top

[P04] 求长度
来源：http://ekh.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ncm.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://maz.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qhm.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xaj.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://lse.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://qxe.iojbl.cn

Ruby: x.length;  x.size
来源：http://svq.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://enb.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://eme.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://wmg.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lzv.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gyl.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sue.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://exl.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://oyj.vqdsnc.cn

Ruby: a == b
来源：http://cpa.redwolf501.top


<!-- 参考信息 -->