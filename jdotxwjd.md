代发 wailian999

Ruby: ARGV
来源：http://top.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://bhc.hnxiangtu.top

[M02] 读取环境变量
来源：http://wzj.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://vvd.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dyk.hesvh.cn

JS:   process.env.HOME
来源：http://zzn.yfazqb.com

TS:   process.env.HOME
来源：http://uvs.9152youxi.cn

Java: System.getenv("HOME")
来源：http://wtd.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oey.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://rae.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mqd.vehdjk.com

[M03] 执行外部命令
来源：http://ugv.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pcb.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fgy.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fgl.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ayb.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://axx.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gnb.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://ddu.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://sek.cashguo.top

[M04] 获取当前工作目录
来源：http://htp.sweek.top

Py:   os.getcwd()
来源：http://sjc.smart0.xyz

PHP:  getcwd();
来源：http://inu.meibo888.top

JS:   process.cwd()
来源：http://xcf.0kj1m.cn

TS:   process.cwd()
来源：http://elz.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://ybs.vqdsnc.cn

Go:   os.Getwd()
来源：http://wab.aibaodan.cn

Ruby: Dir.pwd
来源：http://tfx.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dqk.haohaochexian.top

[M05] 设置退出码
来源：http://phn.svipenyu.cn

Py:   sys.exit(1)
来源：http://hkw.nanxuanxn.top

PHP:  exit(1);
来源：http://jad.jqgufenzy.top

JS:   process.exit(1)
来源：http://qyc.wangdashe.top

TS:   process.exit(1)
来源：http://smj.gaohongyu789.top

Java: System.exit(1)
来源：http://xdc.jinqigfzy.top

Go:   os.Exit(1)
来源：http://gus.guowangkeji.top

Ruby: exit 1
来源：http://djg.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xwa.redwolf501.top

[M06] 向标准错误输出
来源：http://guy.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://jev.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lrk.quarkkingdee.top

JS:   console.error("err")
来源：http://qlm.epnwcf.com

TS:   console.error("err")
来源：http://tgz.cdnleiting.top

Java: System.err.println("err")
来源：http://tbg.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wfq.vqdsnc.cn

Ruby: warn "err"
来源：http://lqn.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://bqo.nanxinkj.top

[M07] 判断是否为主入口
来源：http://ahc.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://jfz.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dki.smart0.xyz

JS:   require.main === module
来源：http://cyy.zdbjq.cn

TS:   require.main === module
来源：http://rwy.fehbvm.com

Java: public static void main(String[] args)
来源：http://uoq.guowangkeji.top

Go:   func main()
来源：http://yqn.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rym.hammf.cn

C#:   static void Main(string[] args)
来源：http://oyu.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://rux.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://tmm.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://pod.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://pav.hammf.cn

TS:   process.platform;  process.version
来源：http://zft.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wee.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gwf.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rjy.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ict.smart0.xyz

================================================================================
来源：http://sad.tarul.cn

N. 数据结构与算法
来源：http://lqh.zycfv.cn

================================================================================
来源：http://gir.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://orl.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://ajs.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kks.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ebo.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qmf.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://mne.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://nyc.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://odo.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://xcs.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://gqa.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://tyi.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yrs.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ygm.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ltp.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kqb.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://caa.yj20258888.top

Ruby: arr.sort
来源：http://mpn.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tjj.ivvv.top

[N03] 快速排序（分治示例）
来源：http://cwo.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yil.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://lfy.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://scl.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gwk.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ghv.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpl.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ack.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fyc.yvedp.cn

[N04] 斐波那契数列
来源：http://qax.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://psv.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kfz.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahv.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mcd.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bdp.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zki.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fqu.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lum.ppjwa.cn

[N05] 最大公约数
来源：http://yjd.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://ezm.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://svp.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfy.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aac.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xdt.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jbz.cdnleiting.top

Ruby: a.gcd(b)
来源：http://hez.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xzu.redwolf501.top

[N06] 判断回文字符串
来源：http://vps.kuanghao11.cn

Py:   s == s[::-1]
来源：http://unn.bbcook.cn

PHP:  $s === strrev($s);
来源：http://amc.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://abo.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://xhb.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bxp.ybcxt.top

Go:   // 双指针从两端比较
来源：http://auh.sysykeji.top

Ruby: s == s.reverse
来源：http://her.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bxb.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://vtg.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gbn.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ray.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jsx.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://tso.jlsjyb.cn

Java: // 手写 HashMap
来源：http://gce.xuanzx.com

Go:   // 手写 map[int]int
来源：http://qop.9152youxi.cn

Ruby: // 手写 Hash
来源：http://rrr.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://dyz.xziqi.cn

[N08] 生成全排列
来源：http://gsa.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://uie.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://cpb.dianchejie.cn

JS:   // 手写回溯递归
来源：http://fxk.redwolf501.top

TS:   // 手写回溯递归
来源：http://dlo.shzxlz.cn

Java: // 手写回溯递归
来源：http://aro.9152youxi.cn

Go:   // 手写回溯递归
来源：http://hba.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://ldn.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://dpp.hfpthk.cn

[N09] 栈与队列
来源：http://zme.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jrw.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://czy.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://siu.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dcv.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xsz.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bsv.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aee.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hax.jyoumei.cn

[N10] 链表节点定义
来源：http://rkp.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ubf.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ovz.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rmj.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hyj.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://kfe.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://eju.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bou.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dvy.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://hof.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tdi.52xcode.cn

PHP:  // 手写递归函数
来源：http://dvj.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovw.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://olw.ybcxt.top

Java: // 手写递归
来源：http://mod.havefunace.top

Go:   // 手写递归
来源：http://nno.yfazqb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uif.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://mhs.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mie.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ivk.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vcr.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jiv.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wvy.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xhf.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tvz.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vfb.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xrk.pycfn.com

================================================================================
来源：http://kwt.yanxiufei.cn

O. 并发与异步
来源：http://oyz.zhoulong.xyz

================================================================================
来源：http://ojx.yongpay.top

[O01] 启动一个线程
来源：http://ovj.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://opu.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hus.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jqw.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://kkh.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://vjw.gogol.net.cn

Go:   go f()
来源：http://amm.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://djl.mhx1999.top

C#:   Task.Run(() => F());
来源：http://leu.jiagoushi.top

[O02] 使用线程池
来源：http://cmi.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ymo.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sdl.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://opq.daxiang520.top

TS:   // worker_threads 线程池
来源：http://kak.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://qlz.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sbd.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mds.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wui.daxiang520.top

[O03] 加锁保护共享数据
来源：http://gij.bjfxy.top

Py:   with lock: shared += 1
来源：http://kdh.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://arp.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qwa.vqdsnc.cn

TS:   // 同 JS
来源：http://ili.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://yli.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zow.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rvv.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://fax.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://jqf.birdmap.top

Py:   async def f():⏎    await g()
来源：http://zhs.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oxg.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://snl.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ewd.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mhw.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kja.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ntp.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://ccd.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://yao.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://vfq.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jml.yongpay.top

JS:   await Promise.all(tasks)
来源：http://vmf.pycfn.com

TS:   await Promise.all(tasks)
来源：http://qqh.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ekx.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bdn.mhx1999.top

Ruby: threads.map(&:join)
来源：http://qcw.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fsy.zhongyouzk.top

[O06] 使用进程池
来源：http://vwy.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://thn.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mca.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://beo.cheryme.top

TS:   // child_process / cluster 模块
来源：http://eyy.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://icg.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hdi.hnxiangtu.top

Ruby: // fork 块
来源：http://qdj.9152youxi.cn

C#:   Parallel.For
来源：http://aze.dashuyun.cn

================================================================================
来源：http://giu.aizwys.cn

P. 常用工具函数
来源：http://lnz.zycfv.cn

================================================================================
来源：http://odn.hysaishi.cn

[P01] 生成 UUID
来源：http://isg.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://bha.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wdy.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://ppc.birdmap.top

TS:   crypto.randomUUID()
来源：http://aym.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://yko.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://awk.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://yml.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://ray.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://zdc.uphjek.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uys.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://svf.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bgl.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://laa.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rkl.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qrn.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zbt.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jgi.c1oappe.top

[P03] 生成短随机字符串
来源：http://jcl.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tfb.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mlu.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xrz.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ggd.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hxe.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rmq.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nhv.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gfb.hnxiangtu.top

[P04] 求长度
来源：http://phe.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yva.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmj.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://upe.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://feu.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://fie.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://yvr.yongpay.top

Ruby: x.length;  x.size
来源：http://npc.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://etg.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://jts.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zqz.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dtd.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bqd.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nqs.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nrl.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://xth.ydjk.org.cn

Ruby: a == b
来源：http://gaa.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hev.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lcj.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://khg.havefunace.top

PHP:  if (empty($x)) {}
来源：http://opg.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qhi.fzhhl.top

TS:   if (x == null) {}
来源：http://ipi.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://juj.aizwys.cn

Go:   if x == nil {}
来源：http://nyw.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://isu.wangdashe.top

C#:   if (x is null) {}
来源：http://cgf.hnqzz.top

[P07] 防抖与节流
来源：http://chr.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qub.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://ehw.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cbg.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://btb.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ndj.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://djc.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fal.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://opm.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://ftq.chenjidiqi.icu


<!-- 参考信息 -->