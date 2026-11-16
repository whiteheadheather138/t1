代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nfd.sysykeji.top

JS:   process.env.HOME
来源：http://led.uphjek.com

TS:   process.env.HOME
来源：http://gla.zdqjudy.top

Java: System.getenv("HOME")
来源：http://msl.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ykr.redwolf501.top

Ruby: ENV["HOME"]
来源：http://fbv.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://juc.nanxinkj.top

[M03] 执行外部命令
来源：http://lny.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://orm.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://obl.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qpj.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cfo.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dkj.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ceg.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://hce.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://fir.bjfxy.top

[M04] 获取当前工作目录
来源：http://kiy.aibaodan.cn

Py:   os.getcwd()
来源：http://mkp.ppjwa.cn

PHP:  getcwd();
来源：http://els.pengpengdd.cyou

JS:   process.cwd()
来源：http://zzf.quarkkingdee.top

TS:   process.cwd()
来源：http://ldm.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://gmm.aibaodan.cn

Go:   os.Getwd()
来源：http://quk.yueranfly.top

Ruby: Dir.pwd
来源：http://xta.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://lfm.gogol.net.cn

[M05] 设置退出码
来源：http://gql.jinqigfzy.top

Py:   sys.exit(1)
来源：http://ndr.aibaodan.cn

PHP:  exit(1);
来源：http://tkj.fehbvm.com

JS:   process.exit(1)
来源：http://ftz.yueranfly.top

TS:   process.exit(1)
来源：http://kkw.hysaishi.cn

Java: System.exit(1)
来源：http://jzt.aibaodan.cn

Go:   os.Exit(1)
来源：http://xcj.fehbvm.com

Ruby: exit 1
来源：http://erc.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhh.sxryk.cn

[M06] 向标准错误输出
来源：http://nqg.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://gaw.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gvl.0kj1m.cn

JS:   console.error("err")
来源：http://wsa.haohaochexian.top

TS:   console.error("err")
来源：http://abd.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://ixp.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tdq.ppjwa.cn

Ruby: warn "err"
来源：http://uga.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://ldl.tanke756.top

[M07] 判断是否为主入口
来源：http://pwt.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://zxo.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vjr.ctjpmb.com

JS:   require.main === module
来源：http://mdc.sxryk.cn

TS:   require.main === module
来源：http://uhh.xylfe.cn

Java: public static void main(String[] args)
来源：http://elz.shzxlz.cn

Go:   func main()
来源：http://osp.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rvc.ydzc1.top

C#:   static void Main(string[] args)
来源：http://akf.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://mav.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://eho.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://cap.316326.xyz

JS:   process.platform;  process.version
来源：http://voj.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://snh.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tll.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ynk.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zbj.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://fzt.kuanghao11.cn

================================================================================
来源：http://one.yueranfly.top

N. 数据结构与算法
来源：http://vcq.jiagoushi.top

================================================================================
来源：http://xmn.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://mxv.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uvb.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://syt.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mvs.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xoq.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://fjf.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://wsy.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://snj.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://vxq.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://uod.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ecq.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xub.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vvm.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://yzr.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qcp.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://uco.zhixingplan.top

Ruby: arr.sort
来源：http://gof.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mge.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://ohn.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ljt.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://ayg.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://alw.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ury.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lrt.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mxz.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ntj.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bdv.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://mfg.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://egf.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vtt.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cik.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wco.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://icd.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sbt.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ial.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mnn.haohaochexian.top

[N05] 最大公约数
来源：http://hdb.shuidangran.top

Py:   math.gcd(a, b)
来源：http://pdp.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gzi.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pyv.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwu.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fnt.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xmv.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://cse.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://stq.ybcxt.top

[N06] 判断回文字符串
来源：http://hsn.haohaochexian.top

Py:   s == s[::-1]
来源：http://ria.sweek.top

PHP:  $s === strrev($s);
来源：http://pow.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://lpu.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://yyt.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ans.fehbvm.com

Go:   // 双指针从两端比较
来源：http://qeg.aibaodan.cn

Ruby: s == s.reverse
来源：http://dpx.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mok.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://udg.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tha.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jvl.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://apu.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://bbt.bjfxy.top

Java: // 手写 HashMap
来源：http://hba.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://fbz.xylfe.cn

Ruby: // 手写 Hash
来源：http://wdx.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ayx.hnxiangtu.top

[N08] 生成全排列
来源：http://vgh.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://cbd.andypj.xyz

PHP:  // 手写递归交换
来源：http://knv.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://ash.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://wdi.cashguo.top

Java: // 手写回溯递归
来源：http://khg.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://dab.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://fjw.snrcjt.cn

C#:   // 手写回溯递归
来源：http://clz.jiagoushi.top

[N09] 栈与队列
来源：http://bnj.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gse.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gim.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://umd.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jre.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wfr.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qch.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://trw.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bky.chenlongwang.top

[N10] 链表节点定义
来源：http://vsw.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cew.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ise.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nlx.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vgh.tanke756.top

Java: class Node { int v; Node next; }
来源：http://fjz.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://hma.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cxh.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://mgt.52xcode.cn

[N11] 二叉树中序遍历
来源：http://ems.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ctc.hysaishi.cn

PHP:  // 手写递归函数
来源：http://uxk.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndc.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://guc.jqgfzy.top

Java: // 手写递归
来源：http://fgt.shangyingyoupin.top

Go:   // 手写递归
来源：http://mha.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fay.fehbvm.com

C#:   // 手写递归
来源：http://emz.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://neh.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cbf.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://utu.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbr.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fyb.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xig.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hlv.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sjv.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zjd.chenlongwang.top

================================================================================
来源：http://myb.zhengqikj.top

O. 并发与异步
来源：http://ing.jinqigfzy.top

================================================================================
来源：http://tdl.birdmap.top

[O01] 启动一个线程
来源：http://shh.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qpu.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hem.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hak.yuanzhike.top

TS:   // 同 JS
来源：http://bku.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://pzi.0kj1m.cn

Go:   go f()
来源：http://pby.sxryk.cn

Ruby: Thread.new { f }
来源：http://uyt.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://okp.yfazqb.com

[O02] 使用线程池
来源：http://fyi.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xyw.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aql.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://ytn.redwolf501.top

TS:   // worker_threads 线程池
来源：http://ixy.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://myq.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hqc.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ana.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bpp.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://txz.sxryk.cn

Py:   with lock: shared += 1
来源：http://mri.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://sun.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gcq.zhongyouzk.top

TS:   // 同 JS
来源：http://xgi.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://wdm.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vqq.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ubz.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://ngw.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://efl.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://cwd.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jlv.bjfxy.top

JS:   async function f() { await g(); }
来源：http://etu.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hko.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tty.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rfh.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hqs.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://sbt.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://ehf.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://lwu.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xpr.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://mfx.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://qyi.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://exb.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iqn.yfazqb.com

Ruby: threads.map(&:join)
来源：http://tve.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fsq.fktsv.cn

[O06] 使用进程池
来源：http://ihi.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rmh.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ktc.316326.xyz

JS:   // child_process / cluster 模块
来源：http://shd.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://ili.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://djd.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uwe.gzhubu.top

Ruby: // fork 块
来源：http://qnr.yj202588.top

C#:   Parallel.For
来源：http://zii.ydzc1.top

================================================================================
来源：http://aei.ctjpmb.com

P. 常用工具函数
来源：http://lpo.ehwqpu.com

================================================================================
来源：http://ynt.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://mnx.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://jji.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ong.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://qgi.316326.xyz

TS:   crypto.randomUUID()
来源：http://swj.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://fzi.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://bsu.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://rku.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://wkr.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://dam.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vwg.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://oca.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eor.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ram.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pks.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gka.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://olb.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nnp.sysykeji.top

[P03] 生成短随机字符串
来源：http://sqg.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jkg.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cdq.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://okh.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pcr.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nhl.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xla.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nal.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qjw.yongpay.top

[P04] 求长度
来源：http://mzn.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rjw.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://alx.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ajk.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcp.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://xxg.tian-w.cn

Go:   len(arr);  len(m)
来源：http://pik.316326.xyz

Ruby: x.length;  x.size
来源：http://xwi.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://lyn.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://avy.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vpx.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kjr.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rvl.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://otq.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fkc.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://axb.yj202588.top

Ruby: a == b
来源：http://alh.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lsp.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://psz.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mjv.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://ksr.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uxr.yj20258.top

TS:   if (x == null) {}
来源：http://rfp.yongpay.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qnw.bbcook.cn

Go:   if x == nil {}
来源：http://fds.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mgx.guowangkeji.top

C#:   if (x is null) {}
来源：http://rja.jqgufenzy.top

[P07] 防抖与节流
来源：http://hpb.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zhf.yj20258.top

PHP:  // 手写时间戳比较
来源：http://xss.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjo.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oht.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lvo.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zlp.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wji.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zat.hammf.cn

[P08] 处理浮点精度问题
来源：http://qeq.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://abs.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sor.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aae.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vfx.chenlongwang.top


<!-- 参考信息 -->