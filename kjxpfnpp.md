代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxs.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lpu.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://gpf.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kds.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://okd.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sey.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vdp.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://oag.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://png.pengpengdd.cyou

Java: resp.statusCode()
来源：http://hjh.sxryk.cn

Go:   resp.StatusCode
来源：http://xlo.dianchejie.cn

Ruby: resp.code.to_i
来源：http://bcu.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://zju.cucudq.cn

[L08] 并发请求多个地址
来源：http://lya.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gfc.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://mas.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://apv.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ttx.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vde.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://caa.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mqv.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vvo.yvedp.cn

================================================================================
来源：http://ssh.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://kbl.316326.xyz

================================================================================
来源：http://vtr.gotoacloud.top

[M01] 读取命令行参数
来源：http://hak.sysykeji.top

Py:   sys.argv[1:]
来源：http://olr.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://bek.xziqi.cn

JS:   process.argv.slice(2)
来源：http://eko.smart0.xyz

TS:   process.argv.slice(2)
来源：http://yji.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://tlp.aibaodan.cn

Go:   os.Args[1:]
来源：http://czw.yfazqb.com

Ruby: ARGV
来源：http://gni.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://eso.dianchejie.cn

[M02] 读取环境变量
来源：http://elu.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://yro.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uzj.ctjpmb.com

JS:   process.env.HOME
来源：http://ypd.cashguo.top

TS:   process.env.HOME
来源：http://kgw.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://eql.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://igk.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://bfj.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gag.bbcook.cn

[M03] 执行外部命令
来源：http://wpa.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lnm.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://csq.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xrn.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://wnr.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gcl.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sct.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://wov.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://kwo.yongpay.top

[M04] 获取当前工作目录
来源：http://imo.zdbjq.cn

Py:   os.getcwd()
来源：http://hii.hysaishi.cn

PHP:  getcwd();
来源：http://iiq.sweek.top

JS:   process.cwd()
来源：http://wci.cucudq.cn

TS:   process.cwd()
来源：http://elf.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://liu.daxiang520.top

Go:   os.Getwd()
来源：http://yrh.sjlbkw.cn

Ruby: Dir.pwd
来源：http://ysr.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hku.zhixingplan.top

[M05] 设置退出码
来源：http://ekk.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://rmk.shuidangran.top

PHP:  exit(1);
来源：http://wet.quarkkingdee.top

JS:   process.exit(1)
来源：http://dqc.sjlbkw.cn

TS:   process.exit(1)
来源：http://ozo.guowangkeji.top

Java: System.exit(1)
来源：http://sip.chenlongwang.top

Go:   os.Exit(1)
来源：http://msh.jyoumei.cn

Ruby: exit 1
来源：http://nup.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mgs.aibaodan.cn

[M06] 向标准错误输出
来源：http://mfv.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://kag.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xxp.feifeiyinyue.top

JS:   console.error("err")
来源：http://krj.sxryk.cn

TS:   console.error("err")
来源：http://ogk.yuxming.cn

Java: System.err.println("err")
来源：http://noj.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iul.jianghu66.top

Ruby: warn "err"
来源：http://ahh.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://qmw.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://gsg.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://gqx.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://icr.ehwqpu.com

JS:   require.main === module
来源：http://hgs.jqgufenzy.top

TS:   require.main === module
来源：http://aed.jiagoushi.top

Java: public static void main(String[] args)
来源：http://dyy.ydzc1.top

Go:   func main()
来源：http://dwc.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vqq.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://iuy.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://kmh.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://kef.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://hsl.bjfxy.top

JS:   process.platform;  process.version
来源：http://xjn.0kj1m.cn

TS:   process.platform;  process.version
来源：http://rde.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xmv.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://pee.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://how.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jwj.yanxiufei.cn

================================================================================
来源：http://gfl.xinyue.icu

N. 数据结构与算法
来源：http://dvj.iojbl.cn

================================================================================
来源：http://cwa.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://zqv.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sdt.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cmr.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mji.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bjw.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://zie.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://iwg.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jbi.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://taa.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://guj.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ywv.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jhr.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lhp.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xow.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://obp.wangdashe.top

Go:   slices.Sort(arr)
来源：http://qat.0kj1m.cn

Ruby: arr.sort
来源：http://gru.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nkq.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://xpp.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://phf.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://pdd.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dez.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pwj.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nar.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lsp.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://knn.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://ebp.ppjwa.cn

[N04] 斐波那契数列
来源：http://sde.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mzv.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qyq.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rbc.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wtc.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bqx.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pip.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bit.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kyd.cucudq.cn

[N05] 最大公约数
来源：http://cjr.sxryk.cn

Py:   math.gcd(a, b)
来源：http://ibx.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lbv.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjv.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oia.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyf.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ozh.sxryk.cn

Ruby: a.gcd(b)
来源：http://zad.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://swe.haohaochexian.top

[N06] 判断回文字符串
来源：http://sez.daxiang520.top

Py:   s == s[::-1]
来源：http://jhk.zycfv.cn

PHP:  $s === strrev($s);
来源：http://ooq.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://mtc.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://tce.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kkb.cheryme.top

Go:   // 双指针从两端比较
来源：http://adg.xinyue.icu

Ruby: s == s.reverse
来源：http://ldc.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://vgm.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://pqf.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gpb.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jrm.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://roq.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://guv.vehdjk.com

Java: // 手写 HashMap
来源：http://oxa.yonumen.top

Go:   // 手写 map[int]int
来源：http://squ.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://abr.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://bqd.wangshuangyany.cn

[N08] 生成全排列
来源：http://nlx.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://bvx.vehdjk.com

PHP:  // 手写递归交换
来源：http://dyt.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://zoq.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://nfi.vqdsnc.cn

Java: // 手写回溯递归
来源：http://lyx.jiagoushi.top

Go:   // 手写回溯递归
来源：http://byn.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://pbh.yuanzhike.top

C#:   // 手写回溯递归
来源：http://axy.hammf.cn

[N09] 栈与队列
来源：http://laf.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tpo.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mqr.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://odj.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wbu.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://quf.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qao.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cnn.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bfj.sysykeji.top

[N10] 链表节点定义
来源：http://rnu.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uuu.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://wxh.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ffo.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uzr.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://wjb.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://jml.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zex.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vog.aizwys.cn

[N11] 二叉树中序遍历
来源：http://sdq.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yxa.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://vqw.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ztm.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hrj.gogol.net.cn

Java: // 手写递归
来源：http://scc.haohaochexian.top

Go:   // 手写递归
来源：http://yse.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cua.shanyushiyangtech.top

C#:   // 手写递归
来源：http://xjp.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hsc.fanxiaobao.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rik.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://igt.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aov.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uzm.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ihx.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lqo.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gsf.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://avh.yuxming.cn

================================================================================
来源：http://fpd.yongpay.top

O. 并发与异步
来源：http://qvw.yongpay.top

================================================================================
来源：http://tdt.guannengcc.top

[O01] 启动一个线程
来源：http://vti.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cme.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kxt.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zsp.epnwcf.com

TS:   // 同 JS
来源：http://qkc.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://toi.pengpengdd.cyou

Go:   go f()
来源：http://nyq.fehbvm.com

Ruby: Thread.new { f }
来源：http://squ.yj20258888.top

C#:   Task.Run(() => F());
来源：http://uiz.jinqigfzy.top

[O02] 使用线程池
来源：http://dkr.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pby.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vrz.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://jft.iojbl.cn

TS:   // worker_threads 线程池
来源：http://ypn.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://abw.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wzd.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kgg.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ivn.smart0.xyz

[O03] 加锁保护共享数据
来源：http://rod.xinyue.icu

Py:   with lock: shared += 1
来源：http://gfj.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://znd.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbx.mhx1999.top

TS:   // 同 JS
来源：http://dzz.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://yzu.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wcc.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://csr.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://gkf.smart0.xyz

[O04] 定义异步函数并等待
来源：http://fma.meibo888.top

Py:   async def f():⏎    await g()
来源：http://lxs.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gzn.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://fck.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cxu.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ktm.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qbe.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mcz.pycfn.com

C#:   async Task F() { await G(); }
来源：http://zbw.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://dbs.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://vbt.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cmm.cheryme.top

JS:   await Promise.all(tasks)
来源：http://zyo.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://izd.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rcf.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rkq.shuidangran.top

Ruby: threads.map(&:join)
来源：http://klm.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sgb.zhijiandao.cn

[O06] 使用进程池
来源：http://ekl.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmj.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bsw.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://bbz.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://rdc.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zxh.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://clk.zdqjudy.top

Ruby: // fork 块
来源：http://hsf.gotoacloud.top

C#:   Parallel.For
来源：http://rip.xuetiantiany.cn

================================================================================
来源：http://rky.hammf.cn

P. 常用工具函数
来源：http://jpp.tarul.cn

================================================================================
来源：http://gaf.zhengqikj.top

[P01] 生成 UUID
来源：http://mcz.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://ixw.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vlh.ydzc1.top

JS:   crypto.randomUUID()
来源：http://ghu.yonumen.top

TS:   crypto.randomUUID()
来源：http://yph.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://grt.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://wso.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://orb.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://wlw.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://afz.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uaz.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tya.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wmg.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://plg.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hwo.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sus.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kdz.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eps.gzhubu.top

[P03] 生成短随机字符串
来源：http://qon.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ebr.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ekq.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wks.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ucb.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sfx.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://huj.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rwr.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hjr.yanxiufei.cn

[P04] 求长度
来源：http://lnt.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wrh.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://usz.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stz.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tti.yongpay.top


<!-- 参考信息 -->