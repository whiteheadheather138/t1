代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tuf.dashuyun.cn

JS:   process.env.HOME
来源：http://zjq.meibo888.top

TS:   process.env.HOME
来源：http://ntb.9152youxi.cn

Java: System.getenv("HOME")
来源：http://pmu.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oqp.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://cvg.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ebp.feifeiyinyue.top

[M03] 执行外部命令
来源：http://sdw.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iow.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yog.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://var.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lle.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jua.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aqv.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://zyp.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://lrd.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://ddp.fzhhl.top

Py:   os.getcwd()
来源：http://jmi.epnwcf.com

PHP:  getcwd();
来源：http://uit.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://vby.xinyue.icu

TS:   process.cwd()
来源：http://nio.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://cjn.jinqigufen.top

Go:   os.Getwd()
来源：http://xhu.yj202588.top

Ruby: Dir.pwd
来源：http://wze.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://jss.shanyushiyangtech.top

[M05] 设置退出码
来源：http://wxm.hammf.cn

Py:   sys.exit(1)
来源：http://jta.aizwys.cn

PHP:  exit(1);
来源：http://uch.snrcjt.cn

JS:   process.exit(1)
来源：http://wvs.ybcxt.top

TS:   process.exit(1)
来源：http://gjy.jiagoushi.top

Java: System.exit(1)
来源：http://xaf.ppjwa.cn

Go:   os.Exit(1)
来源：http://jef.jiagoushi.top

Ruby: exit 1
来源：http://ebb.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://znv.xuanzx.com

[M06] 向标准错误输出
来源：http://bhl.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://xld.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cin.andypj.xyz

JS:   console.error("err")
来源：http://nba.nwbrower.top

TS:   console.error("err")
来源：http://hsp.hongshengwenyu.top

Java: System.err.println("err")
来源：http://tmh.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hzi.hfpthk.cn

Ruby: warn "err"
来源：http://dav.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://pjm.zycfv.cn

[M07] 判断是否为主入口
来源：http://ack.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://rtc.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://evm.yuxming.cn

JS:   require.main === module
来源：http://sfq.meibo888.top

TS:   require.main === module
来源：http://tli.jqgfzy.top

Java: public static void main(String[] args)
来源：http://lzl.ydjk.org.cn

Go:   func main()
来源：http://siw.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kvw.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://gky.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://wyt.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://ssb.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://owj.jyoumei.cn

JS:   process.platform;  process.version
来源：http://anz.tianlin.xyz

TS:   process.platform;  process.version
来源：http://oct.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lzm.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://dlh.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://frn.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xjc.sufxvd.cn

================================================================================
来源：http://gls.aizwys.cn

N. 数据结构与算法
来源：http://qpa.yonumen.top

================================================================================
来源：http://ubi.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://mab.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://ure.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vks.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://buh.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yow.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://wzf.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://mcb.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://adn.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cbh.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://uzy.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://zak.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rmg.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dks.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iyz.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://woh.pycfn.com

Go:   slices.Sort(arr)
来源：http://ott.haohaochexian.top

Ruby: arr.sort
来源：http://xcu.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wfp.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://iuj.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fab.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://qrt.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wph.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cfi.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ikx.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hnb.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vxw.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://inp.uphjek.com

[N04] 斐波那契数列
来源：http://agk.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jhl.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://shh.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsf.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uug.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fcq.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yrx.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ayx.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ibw.fktsv.cn

[N05] 最大公约数
来源：http://vbp.316326.xyz

Py:   math.gcd(a, b)
来源：http://xfk.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vvl.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgk.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scv.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bmn.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://twj.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://huy.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://auq.ppjwa.cn

[N06] 判断回文字符串
来源：http://mrh.sjlbkw.cn

Py:   s == s[::-1]
来源：http://gmi.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://oog.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://udp.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://lnw.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wce.epnwcf.com

Go:   // 双指针从两端比较
来源：http://eux.jqgfzy.top

Ruby: s == s.reverse
来源：http://ouk.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gts.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://sma.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://efo.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sij.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://llp.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://ybz.yueranfly.top

Java: // 手写 HashMap
来源：http://xqp.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://xcd.yongpay.top

Ruby: // 手写 Hash
来源：http://efk.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tgj.nanxinkj.top

[N08] 生成全排列
来源：http://agd.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://xxt.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://lpw.zycfv.cn

JS:   // 手写回溯递归
来源：http://bqs.chenzaomai.com

TS:   // 手写回溯递归
来源：http://zlf.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://jgq.yongpay.top

Go:   // 手写回溯递归
来源：http://bko.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://rup.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://dnp.jinqigufen.top

[N09] 栈与队列
来源：http://hop.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ose.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sfi.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cvq.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://spy.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rbc.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cdo.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nzj.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uiv.bbcook.cn

[N10] 链表节点定义
来源：http://rwq.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://itc.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bit.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nvj.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://otc.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://mpy.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nuh.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bjp.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kib.xinyue.icu

[N11] 二叉树中序遍历
来源：http://vrx.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wyh.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://scy.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fgj.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhb.yuanzhike.top

Java: // 手写递归
来源：http://nfq.epnwcf.com

Go:   // 手写递归
来源：http://shz.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wtk.vehdjk.com

C#:   // 手写递归
来源：http://tbj.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://arr.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ove.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ijd.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://joi.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://omq.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dkn.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qxp.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zkj.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vxk.hnxiangtu.top

================================================================================
来源：http://fra.zhiwuduotai.top

O. 并发与异步
来源：http://iif.iojbl.cn

================================================================================
来源：http://lqj.yanxiufei.cn

[O01] 启动一个线程
来源：http://mnt.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://irr.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fpy.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://axm.hnqzz.top

TS:   // 同 JS
来源：http://ezg.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://ghe.c1oappe.top

Go:   go f()
来源：http://nnv.nwbrower.top

Ruby: Thread.new { f }
来源：http://sli.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://jrr.hammf.cn

[O02] 使用线程池
来源：http://gdd.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ewb.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://btu.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://fzn.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://hkq.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lhy.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zkl.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://whc.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xmq.shuidangran.top

[O03] 加锁保护共享数据
来源：http://jtl.shuidangran.top

Py:   with lock: shared += 1
来源：http://vym.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://epb.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xmp.yfazqb.com

TS:   // 同 JS
来源：http://lul.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://ihd.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sps.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xtk.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://jyt.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://erm.ivvv.top

Py:   async def f():⏎    await g()
来源：http://vuf.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sru.yonumen.top

JS:   async function f() { await g(); }
来源：http://wfz.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kti.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iko.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nei.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://twk.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://ilj.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://lku.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://iqe.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hbr.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://bup.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://iav.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zwm.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ebr.wangdashe.top

Ruby: threads.map(&:join)
来源：http://hwq.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fwj.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://hlb.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zub.fzhhl.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pqd.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://zai.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://nej.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hbv.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qjw.fengsongda.top

Ruby: // fork 块
来源：http://azi.dashuyun.cn

C#:   Parallel.For
来源：http://gbv.quarkkingdee.top

================================================================================
来源：http://pld.haohaochexian.top

P. 常用工具函数
来源：http://jlk.bjfxy.top

================================================================================
来源：http://lcl.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://any.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://oel.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hov.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://vxt.yj202588.top

TS:   crypto.randomUUID()
来源：http://ayb.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://gxy.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://bms.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://loe.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://lur.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://dkc.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://usy.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://olb.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ooy.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://phr.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ndm.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cgw.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xrv.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aza.tarul.cn

[P03] 生成短随机字符串
来源：http://gtg.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqv.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jba.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cgo.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gds.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hoj.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xbp.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kue.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sfq.zhiwuduotai.top

[P04] 求长度
来源：http://lwm.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aor.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vgd.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aww.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blc.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://wrp.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://dmd.316326.xyz

Ruby: x.length;  x.size
来源：http://xdv.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ejb.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://emb.jinqigfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lkx.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://syk.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mam.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zss.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tao.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://pwf.fzhhl.top

Ruby: a == b
来源：http://gax.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://phe.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tyf.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kam.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://gze.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nvr.yj20258.top

TS:   if (x == null) {}
来源：http://zfv.smart0.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cbm.quarkkingdee.top

Go:   if x == nil {}
来源：http://mrs.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zqd.nwbrower.top

C#:   if (x is null) {}
来源：http://ijp.fengsongda.top

[P07] 防抖与节流
来源：http://ynt.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mhb.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://gpc.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fid.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqk.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dda.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aeq.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://xns.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://atn.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://eet.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xkz.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hgo.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gnu.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yip.iojbl.cn


<!-- 参考信息 -->