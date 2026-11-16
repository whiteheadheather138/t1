代发 wailian999

Py:   resp.json()
来源：http://alh.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://lzh.ydjk.org.cn

JS:   await resp.json()
来源：http://scv.hammf.cn

TS:   await resp.json()
来源：http://moa.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://efb.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wej.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://crm.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hle.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://mdp.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lou.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fmc.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://wkj.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://trm.aizwys.cn

Java: resp.statusCode()
来源：http://kcw.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://fgb.tianlin.xyz

Ruby: resp.code.to_i
来源：http://tvd.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://luh.jqgfzy.top

[L08] 并发请求多个地址
来源：http://hzs.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eqy.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://mjm.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ssz.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kbf.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ufh.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jru.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mra.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ihj.ydjk.org.cn

================================================================================
来源：http://kxi.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://esv.zhiwuduotai.top

================================================================================
来源：http://yzm.c1oappe.top

[M01] 读取命令行参数
来源：http://knt.sufxvd.cn

Py:   sys.argv[1:]
来源：http://rgh.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://fuk.sysykeji.top

JS:   process.argv.slice(2)
来源：http://ksh.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://mbr.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://blp.0kj1m.cn

Go:   os.Args[1:]
来源：http://ykv.jinghuilouyu.cn

Ruby: ARGV
来源：http://ptg.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://sdi.pycfn.com

[M02] 读取环境变量
来源：http://rnw.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://cwl.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lst.cqqwz.cn

JS:   process.env.HOME
来源：http://nhb.vqdsnc.cn

TS:   process.env.HOME
来源：http://hlw.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://qrs.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zlo.shuidangran.top

Ruby: ENV["HOME"]
来源：http://dxt.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obk.jinqigufen.top

[M03] 执行外部命令
来源：http://fqj.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ful.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yax.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hrq.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fjg.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iqr.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pyw.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://shd.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://yqg.cdnleiting.top

[M04] 获取当前工作目录
来源：http://yft.ivvv.top

Py:   os.getcwd()
来源：http://ysp.gaohongyu789.top

PHP:  getcwd();
来源：http://aqo.zhengqikj.top

JS:   process.cwd()
来源：http://bxt.shangyingyoupin.top

TS:   process.cwd()
来源：http://lzk.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://vpm.yonumen.top

Go:   os.Getwd()
来源：http://kvg.yj20258888.top

Ruby: Dir.pwd
来源：http://mdh.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://jcu.xziqi.cn

[M05] 设置退出码
来源：http://pkf.hnxiangtu.top

Py:   sys.exit(1)
来源：http://ajh.feifeiyinyue.top

PHP:  exit(1);
来源：http://mkj.cheryme.top

JS:   process.exit(1)
来源：http://mpr.yj20258.top

TS:   process.exit(1)
来源：http://zfy.wangdashe.top

Java: System.exit(1)
来源：http://hnk.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://ugn.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://lcr.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vgp.cqqwz.cn

[M06] 向标准错误输出
来源：http://ivz.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://fbd.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ybq.0kj1m.cn

JS:   console.error("err")
来源：http://gxx.wangshuangyany.cn

TS:   console.error("err")
来源：http://bni.ydjk.org.cn

Java: System.err.println("err")
来源：http://auo.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ouh.bjfxy.top

Ruby: warn "err"
来源：http://tmv.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://dcj.dianchejie.cn

[M07] 判断是否为主入口
来源：http://wvm.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://lju.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zno.hesvh.cn

JS:   require.main === module
来源：http://sbe.pengpengdd.cyou

TS:   require.main === module
来源：http://tbk.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://tst.xingfuxueyuan.xyz

Go:   func main()
来源：http://bpi.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wwk.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://pla.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://zne.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://bux.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://vbm.uphjek.com

JS:   process.platform;  process.version
来源：http://bgd.yvedp.cn

TS:   process.platform;  process.version
来源：http://puq.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wjm.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://zrc.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kxs.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rnt.zhiwuduotai.top

================================================================================
来源：http://cls.yangfankeji.com

N. 数据结构与算法
来源：http://ooy.hnxiangtu.top

================================================================================
来源：http://xij.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://jbc.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://yue.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://noz.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ldc.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwo.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://eqq.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://ulj.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gpl.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://zji.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://lzv.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://qsu.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mby.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://msc.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bqh.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mkk.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://wru.yuanzhike.top

Ruby: arr.sort
来源：http://toz.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://wwc.yj202588.top

[N03] 快速排序（分治示例）
来源：http://etd.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wuu.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://env.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sxt.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qtz.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cae.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vri.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nrv.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://qcm.hcnkem.com

[N04] 斐波那契数列
来源：http://xfc.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rei.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nlo.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgp.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oka.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ppt.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ptc.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bqh.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://myx.316326.xyz

[N05] 最大公约数
来源：http://nrn.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://zrw.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bcm.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uif.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apb.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cxo.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rcp.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://ecw.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aoq.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://rja.smart0.xyz

Py:   s == s[::-1]
来源：http://kvt.hnqzz.top

PHP:  $s === strrev($s);
来源：http://hpf.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://mkv.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://wod.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rqw.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://sce.9152youxi.cn

Ruby: s == s.reverse
来源：http://lyb.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fxq.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://aqv.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://egv.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://its.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bes.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://nkb.ivvv.top

Java: // 手写 HashMap
来源：http://vui.316326.xyz

Go:   // 手写 map[int]int
来源：http://cre.dianchejie.cn

Ruby: // 手写 Hash
来源：http://osa.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://lve.yongpay.top

[N08] 生成全排列
来源：http://wvr.316326.xyz

Py:   itertools.permutations(arr)
来源：http://lwc.c1oappe.top

PHP:  // 手写递归交换
来源：http://cls.vehdjk.com

JS:   // 手写回溯递归
来源：http://mvo.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://efk.sxryk.cn

Java: // 手写回溯递归
来源：http://jyp.chenzaomai.com

Go:   // 手写回溯递归
来源：http://ygr.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://bez.sweek.top

C#:   // 手写回溯递归
来源：http://nwi.havefunace.top

[N09] 栈与队列
来源：http://css.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jzd.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fzo.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://snw.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xjn.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xzv.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://knc.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://exu.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mcc.tianlin.xyz

[N10] 链表节点定义
来源：http://hpi.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pqb.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://psk.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xhx.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://apf.yj20258.top

Java: class Node { int v; Node next; }
来源：http://xrr.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://kwm.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bfu.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bqr.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://fpz.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://veo.aibaodan.cn

PHP:  // 手写递归函数
来源：http://hax.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxm.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ksk.vehdjk.com

Java: // 手写递归
来源：http://gii.gotoacloud.top

Go:   // 手写递归
来源：http://tea.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nee.52xcode.cn

C#:   // 手写递归
来源：http://cwl.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xjk.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yrg.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xrn.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wsn.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnu.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ofu.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://btk.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hqx.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bem.gzhubu.top

================================================================================
来源：http://lag.aibaodan.cn

O. 并发与异步
来源：http://sme.bjfxy.top

================================================================================
来源：http://duz.cdnleiting.top

[O01] 启动一个线程
来源：http://buy.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vvj.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xez.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wnd.gogol.net.cn

TS:   // 同 JS
来源：http://yzn.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://dvb.nwbrower.top

Go:   go f()
来源：http://gvy.9152youxi.cn

Ruby: Thread.new { f }
来源：http://ueq.fengsongda.top

C#:   Task.Run(() => F());
来源：http://ybj.cucudq.cn

[O02] 使用线程池
来源：http://unu.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gzy.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jgo.yj20258.top

JS:   // worker_threads 线程池
来源：http://tnl.epnwcf.com

TS:   // worker_threads 线程池
来源：http://cvl.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://hzk.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ttd.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://adp.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zqb.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://bkw.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://lfo.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://jnq.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gin.snrcjt.cn

TS:   // 同 JS
来源：http://mln.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://bcc.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bus.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://zfb.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://pxx.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://lal.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://kwu.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jfl.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://jzu.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jsv.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bfe.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ohs.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://cqs.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://kri.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://bcc.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://arj.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gfk.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://yjx.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://oze.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://isu.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fvr.guannengcc.top

Ruby: threads.map(&:join)
来源：http://kvj.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://uuk.ivvv.top

[O06] 使用进程池
来源：http://rvy.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eoy.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ouf.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://tid.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://amf.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rfr.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kgj.hfpthk.cn

Ruby: // fork 块
来源：http://kur.yueranfly.top

C#:   Parallel.For
来源：http://vvn.gotoacloud.top

================================================================================
来源：http://hlh.shanyushiyangtech.top

P. 常用工具函数
来源：http://pil.uphjek.com

================================================================================
来源：http://ocp.fehbvm.com

[P01] 生成 UUID
来源：http://lnw.hywenlv.cn

Py:   str(uuid.uuid4())
来源：http://mcu.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://trn.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://ozx.zycfv.cn

TS:   crypto.randomUUID()
来源：http://nnj.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://lnt.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://kdn.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://vjr.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://zar.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://gdh.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jvj.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ube.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ojk.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kug.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bzh.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mvj.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hlw.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eak.haohaochexian.top

[P03] 生成短随机字符串
来源：http://zus.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tht.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lvl.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dcg.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uwq.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bnb.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lxy.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://erg.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qou.316326.xyz

[P04] 求长度
来源：http://xly.yj20258888.top


<!-- 参考信息 -->