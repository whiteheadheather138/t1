代发 wailian999

Py:   resp.json()
来源：http://tiy.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://xku.dashuyun.cn

JS:   await resp.json()
来源：http://hrw.cashguo.top

TS:   await resp.json()
来源：http://ids.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ptk.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ttu.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://msx.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pri.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://mlh.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iog.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upz.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://mrr.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://ygm.smart0.xyz

Java: resp.statusCode()
来源：http://mqn.gotoacloud.top

Go:   resp.StatusCode
来源：http://kaw.tanke756.top

Ruby: resp.code.to_i
来源：http://wju.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://avn.smart0.xyz

[L08] 并发请求多个地址
来源：http://rrh.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jtd.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://hru.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzt.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rix.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eue.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jiz.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttq.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vuu.yangfankeji.com

================================================================================
来源：http://fmi.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://jbl.316326.xyz

================================================================================
来源：http://won.0kj1m.cn

[M01] 读取命令行参数
来源：http://awy.gzhubu.top

Py:   sys.argv[1:]
来源：http://bml.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://zur.redwolf501.top

JS:   process.argv.slice(2)
来源：http://jlg.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://faf.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://udi.bjfxy.top

Go:   os.Args[1:]
来源：http://don.snrcjt.cn

Ruby: ARGV
来源：http://vlf.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://gnb.hongshengwenyu.top

[M02] 读取环境变量
来源：http://zpq.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://fuk.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hxq.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://wmj.birdmap.top

TS:   process.env.HOME
来源：http://uvi.gzhubu.top

Java: System.getenv("HOME")
来源：http://zji.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ptf.zycfv.cn

Ruby: ENV["HOME"]
来源：http://mig.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jru.dianchejie.cn

[M03] 执行外部命令
来源：http://pxy.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ntr.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mqs.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://cpa.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eii.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zlc.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kkx.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://vwo.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://gao.aizwys.cn

[M04] 获取当前工作目录
来源：http://gxr.gzhubu.top

Py:   os.getcwd()
来源：http://ned.dianchejie.cn

PHP:  getcwd();
来源：http://enb.wangshuangyany.cn

JS:   process.cwd()
来源：http://hzi.chenzaomai.com

TS:   process.cwd()
来源：http://wbj.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://hdj.sweek.top

Go:   os.Getwd()
来源：http://tqt.zhongyouzk.top

Ruby: Dir.pwd
来源：http://gqq.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://tmc.yj202588.top

[M05] 设置退出码
来源：http://kvy.hesvh.cn

Py:   sys.exit(1)
来源：http://owx.chenlongwang.top

PHP:  exit(1);
来源：http://utm.xylfe.cn

JS:   process.exit(1)
来源：http://gsp.snrcjt.cn

TS:   process.exit(1)
来源：http://tdh.quarkkingdee.top

Java: System.exit(1)
来源：http://xhj.tian-w.cn

Go:   os.Exit(1)
来源：http://omy.jyoumei.cn

Ruby: exit 1
来源：http://zpz.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bbp.zdqjudy.top

[M06] 向标准错误输出
来源：http://epc.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://icq.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bkw.yvedp.cn

JS:   console.error("err")
来源：http://gpm.guannengcc.top

TS:   console.error("err")
来源：http://qld.zhongyouzk.top

Java: System.err.println("err")
来源：http://sbv.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lgv.zdbjq.cn

Ruby: warn "err"
来源：http://mpg.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://rmh.jiagoushi.top

[M07] 判断是否为主入口
来源：http://tor.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://jvh.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqx.daria6918.cn

JS:   require.main === module
来源：http://rok.fktsv.cn

TS:   require.main === module
来源：http://rsw.yangfankeji.com

Java: public static void main(String[] args)
来源：http://gkt.gogol.net.cn

Go:   func main()
来源：http://zne.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rjq.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://opg.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://hjw.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://jsm.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://sxa.cashguo.top

JS:   process.platform;  process.version
来源：http://nuy.jqgfzy.top

TS:   process.platform;  process.version
来源：http://pgp.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wbd.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://twq.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pwd.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ibf.mhx1999.top

================================================================================
来源：http://wop.9152youxi.cn

N. 数据结构与算法
来源：http://ndq.nwbrower.top

================================================================================
来源：http://crr.havefunace.top

[N01] 二分查找（有序数组）
来源：http://fzc.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vvn.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xuo.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ofb.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fyg.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://kti.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://nbe.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mke.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zyy.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://jop.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://goq.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tny.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aql.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oej.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nel.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://ncs.hnqzz.top

Ruby: arr.sort
来源：http://kdb.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uya.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://pci.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sgy.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://ccj.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tlb.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vvb.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bpy.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cps.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jjk.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://vir.pycfn.com

[N04] 斐波那契数列
来源：http://ruc.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://toj.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ylp.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eiy.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsv.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jib.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ayl.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ixp.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rsj.fehbvm.com

[N05] 最大公约数
来源：http://fkk.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://jvr.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qvn.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpv.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdv.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ddk.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dfg.tarul.cn

Ruby: a.gcd(b)
来源：http://acm.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eil.zhoulong.xyz

[N06] 判断回文字符串
来源：http://dqp.zhijiandao.cn

Py:   s == s[::-1]
来源：http://ezm.xziqi.cn

PHP:  $s === strrev($s);
来源：http://cgu.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://ljg.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://lgm.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fzp.yj202588.top

Go:   // 双指针从两端比较
来源：http://iul.52xcode.cn

Ruby: s == s.reverse
来源：http://ekq.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hqs.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://uac.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zzp.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bbu.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sjb.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://tbc.shzxlz.cn

Java: // 手写 HashMap
来源：http://hmy.epnwcf.com

Go:   // 手写 map[int]int
来源：http://tul.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://tay.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ipf.sufxvd.cn

[N08] 生成全排列
来源：http://wtw.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://pbu.meibo888.top

PHP:  // 手写递归交换
来源：http://lqv.fktsv.cn

JS:   // 手写回溯递归
来源：http://rgr.tianlin.xyz

TS:   // 手写回溯递归
来源：http://nmp.uphjek.com

Java: // 手写回溯递归
来源：http://vse.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://qud.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://mdz.tian-w.cn

C#:   // 手写回溯递归
来源：http://pdf.dianchejie.cn

[N09] 栈与队列
来源：http://zwv.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kuh.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zbv.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mzx.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lzv.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vxm.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bmw.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tau.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gqz.iojbl.cn

[N10] 链表节点定义
来源：http://sef.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cid.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lsm.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://owe.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jkv.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://vxd.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nhl.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://crd.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tcr.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://ogi.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lyu.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://zvw.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://svj.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vtb.guowangkeji.top

Java: // 手写递归
来源：http://vip.sjlbkw.cn

Go:   // 手写递归
来源：http://txs.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uhd.shuidangran.top

C#:   // 手写递归
来源：http://mzw.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fqo.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dnh.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zha.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imq.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qou.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fdg.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://imj.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mxr.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://onr.ybcxt.top

================================================================================
来源：http://sfb.dianchejie.cn

O. 并发与异步
来源：http://wyv.birdmap.top

================================================================================
来源：http://oif.zhijiandao.cn

[O01] 启动一个线程
来源：http://kwm.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dyo.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uug.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xjp.shangyingyoupin.top

TS:   // 同 JS
来源：http://nlh.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://six.xinyue.icu

Go:   go f()
来源：http://htb.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://yov.bbcook.cn

C#:   Task.Run(() => F());
来源：http://sju.yueranfly.top

[O02] 使用线程池
来源：http://bbt.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nby.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ldl.xylfe.cn

JS:   // worker_threads 线程池
来源：http://cyi.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://icb.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vjm.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vqn.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vsx.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jyi.gzhubu.top

[O03] 加锁保护共享数据
来源：http://fhz.daria6918.cn

Py:   with lock: shared += 1
来源：http://hck.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://bpf.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cgy.hfpthk.cn

TS:   // 同 JS
来源：http://smr.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://xqw.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bov.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://agj.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://ztf.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://owg.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://uqz.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hgy.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://sok.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rpa.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cts.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ded.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://vau.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://kea.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://pmj.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://deb.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://afi.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://hku.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://jsh.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vxg.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qrp.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://zza.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cfh.xziqi.cn

[O06] 使用进程池
来源：http://rau.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pzv.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://tvy.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://eva.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://ile.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ndg.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gwt.yangfankeji.com

Ruby: // fork 块
来源：http://vth.vehdjk.com

C#:   Parallel.For
来源：http://faq.jinqigfzy.top

================================================================================
来源：http://hdr.smart0.xyz

P. 常用工具函数
来源：http://nsy.hcnkem.com

================================================================================
来源：http://loo.ybcxt.top

[P01] 生成 UUID
来源：http://kai.birdmap.top

Py:   str(uuid.uuid4())
来源：http://lyr.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mfd.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://pml.wangdashe.top

TS:   crypto.randomUUID()
来源：http://qot.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://cyn.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://nrg.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://zzb.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://bej.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://gfr.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fjt.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://did.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dow.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://owj.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ftg.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mfy.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qyw.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ctl.yj20258888.top

[P03] 生成短随机字符串
来源：http://tbz.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yov.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://woi.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rvr.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lmp.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ino.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wpc.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bib.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://njg.zhijiandao.cn

[P04] 求长度
来源：http://jul.zdbjq.cn


<!-- 参考信息 -->