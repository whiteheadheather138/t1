代发 wailian999

Ruby: ARGV
来源：http://icd.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://zmz.hnxiangtu.top

[M02] 读取环境变量
来源：http://ccz.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://svr.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kog.bjfxy.top

JS:   process.env.HOME
来源：http://wdn.cucudq.cn

TS:   process.env.HOME
来源：http://epe.aizwys.cn

Java: System.getenv("HOME")
来源：http://see.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://emp.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://hyg.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zhy.jqgfzy.top

[M03] 执行外部命令
来源：http://tcs.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bsy.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mjy.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dgn.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gbk.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://spg.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yly.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ggf.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://jbb.pycfn.com

[M04] 获取当前工作目录
来源：http://izz.yangfankeji.com

Py:   os.getcwd()
来源：http://yvc.zhiwuduotai.top

PHP:  getcwd();
来源：http://ykh.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://jjy.yj20258888.top

TS:   process.cwd()
来源：http://kpv.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://ptr.yfazqb.com

Go:   os.Getwd()
来源：http://pgw.jqgfzy.top

Ruby: Dir.pwd
来源：http://eyg.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://trb.sxryk.cn

[M05] 设置退出码
来源：http://sok.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://hfs.pengpengdd.cyou

PHP:  exit(1);
来源：http://yog.sysykeji.top

JS:   process.exit(1)
来源：http://ghn.havefunace.top

TS:   process.exit(1)
来源：http://dks.yvedp.cn

Java: System.exit(1)
来源：http://xwy.chenzaomai.com

Go:   os.Exit(1)
来源：http://vuu.feifeiyinyue.top

Ruby: exit 1
来源：http://azg.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ukv.52xcode.cn

[M06] 向标准错误输出
来源：http://sky.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://ppo.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nft.tianlin.xyz

JS:   console.error("err")
来源：http://feg.sxryk.cn

TS:   console.error("err")
来源：http://xtf.sweek.top

Java: System.err.println("err")
来源：http://jxq.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yab.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://mze.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://aak.ehwqpu.com

[M07] 判断是否为主入口
来源：http://zbt.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://svj.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fyu.hnqzz.top

JS:   require.main === module
来源：http://avs.9152youxi.cn

TS:   require.main === module
来源：http://cnm.snrcjt.cn

Java: public static void main(String[] args)
来源：http://alb.quarkkingdee.top

Go:   func main()
来源：http://qne.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dys.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://msr.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://elf.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://gtx.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://als.mhx1999.top

JS:   process.platform;  process.version
来源：http://jpe.jiagoushi.top

TS:   process.platform;  process.version
来源：http://ezh.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xkd.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://iax.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://seg.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://stx.zdqjudy.top

================================================================================
来源：http://gji.yj202588.top

N. 数据结构与算法
来源：http://zey.fehbvm.com

================================================================================
来源：http://eim.havefunace.top

[N01] 二分查找（有序数组）
来源：http://pao.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vbr.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nzg.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oev.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgh.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jou.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://jii.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://msu.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lyk.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://bvi.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://xib.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jnj.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jps.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rsf.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eld.ydzc1.top

Go:   slices.Sort(arr)
来源：http://jhz.hammf.cn

Ruby: arr.sort
来源：http://xyk.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zzs.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://zki.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://apb.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://iyt.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jex.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ioj.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://acs.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uzq.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rms.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://xmh.chenlongwang.top

[N04] 斐波那契数列
来源：http://xbn.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yir.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mcm.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ifi.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://alm.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jei.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nrp.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tvh.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yxm.vqdsnc.cn

[N05] 最大公约数
来源：http://bos.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://pik.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xnp.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbm.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sal.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eqy.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tgu.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://psb.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xrq.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://mmx.guannengcc.top

Py:   s == s[::-1]
来源：http://zeu.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://jio.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://oee.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://wss.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tkj.shuidangran.top

Go:   // 双指针从两端比较
来源：http://hgu.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://egv.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fju.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://wga.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vwh.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://inq.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mar.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://liq.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://dsz.fengsongda.top

Go:   // 手写 map[int]int
来源：http://yne.hysaishi.cn

Ruby: // 手写 Hash
来源：http://ghn.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jpp.yonumen.top

[N08] 生成全排列
来源：http://hhj.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://bax.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://xau.guowangkeji.top

JS:   // 手写回溯递归
来源：http://igz.cdnleiting.top

TS:   // 手写回溯递归
来源：http://xyi.mhx1999.top

Java: // 手写回溯递归
来源：http://qie.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://phb.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://yyx.yj20258888.top

C#:   // 手写回溯递归
来源：http://uuc.meibo888.top

[N09] 栈与队列
来源：http://evw.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mom.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ysf.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qzg.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ltz.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ufe.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nky.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nyl.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ybd.jqgfzy.top

[N10] 链表节点定义
来源：http://daj.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pll.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qex.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ibt.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pht.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://xfl.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://xcx.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oxu.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://brk.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://ujp.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lji.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://odw.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oqh.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://azq.yongpay.top

Java: // 手写递归
来源：http://ztp.quarkkingdee.top

Go:   // 手写递归
来源：http://ljl.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yin.yuanzhike.top

C#:   // 手写递归
来源：http://vqs.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eej.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pjr.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dyj.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjx.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttc.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eko.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ior.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ioi.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://caf.yj20258.top

================================================================================
来源：http://ggf.gzhubu.top

O. 并发与异步
来源：http://icq.zdqjudy.top

================================================================================
来源：http://ikw.feifeiyinyue.top

[O01] 启动一个线程
来源：http://ghd.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rkp.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rfu.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bui.yanxiufei.cn

TS:   // 同 JS
来源：http://bzn.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://mhs.smart0.xyz

Go:   go f()
来源：http://mhb.yuxming.cn

Ruby: Thread.new { f }
来源：http://rto.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://etb.chenlongwang.top

[O02] 使用线程池
来源：http://fmu.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zrk.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bwr.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://edw.yj20258.top

TS:   // worker_threads 线程池
来源：http://kap.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://ggl.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hjk.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fve.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zmb.bjfxy.top

[O03] 加锁保护共享数据
来源：http://zrc.yuxming.cn

Py:   with lock: shared += 1
来源：http://oey.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://suj.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://obt.zhiwuduotai.top

TS:   // 同 JS
来源：http://xpb.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://ibj.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pai.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://guw.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://vef.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://bvx.sweek.top

Py:   async def f():⏎    await g()
来源：http://sgn.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ipq.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://ujj.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xpb.fehbvm.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ohb.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nac.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://vkz.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://zel.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://xvw.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://vfu.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tbx.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://cht.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://vkd.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dio.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lba.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://cdq.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wqi.gzhubu.top

[O06] 使用进程池
来源：http://hyk.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bib.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vjx.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://aax.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://dno.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ewl.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jne.aibaodan.cn

Ruby: // fork 块
来源：http://cgi.cucudq.cn

C#:   Parallel.For
来源：http://sop.gogol.net.cn

================================================================================
来源：http://sgy.jianghu66.top

P. 常用工具函数
来源：http://dco.hammf.cn

================================================================================
来源：http://gzo.wangdashe.top

[P01] 生成 UUID
来源：http://spw.tanke756.top

Py:   str(uuid.uuid4())
来源：http://dyv.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kpr.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://oue.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://xzv.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://oun.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://itz.birdmap.top

Ruby: SecureRandom.uuid
来源：http://psw.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://vjx.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://nye.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ofo.dianchejie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ecb.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ogq.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://reu.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nip.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kjy.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zso.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://akb.uphjek.com

[P03] 生成短随机字符串
来源：http://xbm.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mzc.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nwc.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aca.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dzh.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dof.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rbg.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fxd.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cix.shuidangran.top

[P04] 求长度
来源：http://bng.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://txh.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hia.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dzs.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vrg.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://bfv.52xcode.cn

Go:   len(arr);  len(m)
来源：http://bhq.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://uej.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sdo.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://fsy.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fus.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://szm.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lwk.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ytm.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lye.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://ehq.fehbvm.com

Ruby: a == b
来源：http://seq.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lkw.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ebe.hammf.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://viv.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://veq.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zfw.zdqjudy.top

TS:   if (x == null) {}
来源：http://bhi.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://skt.daxiang520.top

Go:   if x == nil {}
来源：http://agl.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://llu.ydzc1.top

C#:   if (x is null) {}
来源：http://jmm.jqgfzy.top

[P07] 防抖与节流
来源：http://vno.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sgl.havefunace.top

PHP:  // 手写时间戳比较
来源：http://phi.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vur.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euv.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qdt.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aay.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vco.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://let.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://cao.yj202588.top


<!-- 参考信息 -->