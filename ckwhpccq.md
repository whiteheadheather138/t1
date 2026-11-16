代发 wailian999

Py:   resp.json()
来源：http://qhg.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://tew.zdqjudy.top

JS:   await resp.json()
来源：http://lof.52xcode.cn

TS:   await resp.json()
来源：http://yzl.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zkd.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cxb.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://gdw.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qdx.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://vqc.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lyt.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rth.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://igi.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://uxy.sweek.top

Java: resp.statusCode()
来源：http://kqn.cheryme.top

Go:   resp.StatusCode
来源：http://ack.gogol.net.cn

Ruby: resp.code.to_i
来源：http://iyh.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://vmk.haohaochexian.top

[L08] 并发请求多个地址
来源：http://buh.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tbq.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://oyi.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gys.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gbk.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fif.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gqj.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qon.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wzc.hywenlv.cn

================================================================================
来源：http://vkd.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://mxy.nwbrower.top

================================================================================
来源：http://pkk.yanxiufei.cn

[M01] 读取命令行参数
来源：http://zcv.nanxinkj.top

Py:   sys.argv[1:]
来源：http://zrz.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://fdt.cheryme.top

JS:   process.argv.slice(2)
来源：http://ewf.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://qak.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://fdf.yueranfly.top

Go:   os.Args[1:]
来源：http://num.svipenyu.cn

Ruby: ARGV
来源：http://kga.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://hwr.iojbl.cn

[M02] 读取环境变量
来源：http://nnx.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://kuy.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pac.gaohongyu789.top

JS:   process.env.HOME
来源：http://yvz.zhijiandao.cn

TS:   process.env.HOME
来源：http://avb.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://bae.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ivh.redwolf501.top

Ruby: ENV["HOME"]
来源：http://oeg.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mev.52xcode.cn

[M03] 执行外部命令
来源：http://gmn.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://atj.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qil.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ksx.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mbp.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://twr.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bre.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://bdw.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://gib.cheryme.top

[M04] 获取当前工作目录
来源：http://yfp.hcnkem.com

Py:   os.getcwd()
来源：http://mik.smart0.xyz

PHP:  getcwd();
来源：http://awy.gaohongyu789.top

JS:   process.cwd()
来源：http://gsf.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://xrp.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://yup.havefunace.top

Go:   os.Getwd()
来源：http://haz.chenzaomai.com

Ruby: Dir.pwd
来源：http://uei.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gmf.sufxvd.cn

[M05] 设置退出码
来源：http://rxc.iojbl.cn

Py:   sys.exit(1)
来源：http://jnl.sxryk.cn

PHP:  exit(1);
来源：http://kaj.gaohongyu789.top

JS:   process.exit(1)
来源：http://vyo.kuanghao11.cn

TS:   process.exit(1)
来源：http://jua.kuanghao11.cn

Java: System.exit(1)
来源：http://uvn.meibo888.top

Go:   os.Exit(1)
来源：http://lqi.xylfe.cn

Ruby: exit 1
来源：http://fsd.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jvm.birdmap.top

[M06] 向标准错误输出
来源：http://viw.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://vkr.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://fxb.bbcook.cn

JS:   console.error("err")
来源：http://pkd.andypj.xyz

TS:   console.error("err")
来源：http://vwx.pycfn.com

Java: System.err.println("err")
来源：http://ryy.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vqo.nanxinkj.top

Ruby: warn "err"
来源：http://lif.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://ocf.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://mjm.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://gvd.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://woe.yj20258.top

JS:   require.main === module
来源：http://aog.aibaodan.cn

TS:   require.main === module
来源：http://sgh.hywenlv.cn

Java: public static void main(String[] args)
来源：http://lbl.cqqwz.cn

Go:   func main()
来源：http://uoe.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uuy.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://tde.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://jvx.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://hfp.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://sif.snrcjt.cn

JS:   process.platform;  process.version
来源：http://ikh.sxryk.cn

TS:   process.platform;  process.version
来源：http://mld.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wdq.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://itf.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ecx.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wvp.cheryme.top

================================================================================
来源：http://cek.kuanghao11.cn

N. 数据结构与算法
来源：http://cxz.zhengqikj.top

================================================================================
来源：http://wij.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://aya.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iqn.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ipo.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bbz.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxt.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://gtt.yj20258888.top

Go:   sort.SearchInts(arr, x)
来源：http://aqu.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zhm.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pdj.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://aul.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://thx.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ish.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jbh.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uju.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tzc.hnqzz.top

Go:   slices.Sort(arr)
来源：http://hds.gogol.net.cn

Ruby: arr.sort
来源：http://day.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lyo.yongpay.top

[N03] 快速排序（分治示例）
来源：http://qyw.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nnz.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://zde.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://equ.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nlj.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bca.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://igp.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pwc.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://zsr.hnxiangtu.top

[N04] 斐波那契数列
来源：http://sci.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ulp.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://znp.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jre.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mbh.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rij.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zoj.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cur.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rcz.zhijiandao.cn

[N05] 最大公约数
来源：http://jzo.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://rdm.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ctt.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://muz.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rpx.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pds.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://suf.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://cdq.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ssc.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://ims.zdbjq.cn

Py:   s == s[::-1]
来源：http://pcd.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://xzb.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://yzl.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://hga.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zrh.fengsongda.top

Go:   // 双指针从两端比较
来源：http://hed.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://xjg.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://vxe.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://erq.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gfu.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rpa.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ubp.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://wze.havefunace.top

Java: // 手写 HashMap
来源：http://kcu.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://kfz.haohaochexian.top

Ruby: // 手写 Hash
来源：http://bdi.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://pdw.iojbl.cn

[N08] 生成全排列
来源：http://wdj.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://qss.epnwcf.com

PHP:  // 手写递归交换
来源：http://ouh.epnwcf.com

JS:   // 手写回溯递归
来源：http://dfa.cqqwz.cn

TS:   // 手写回溯递归
来源：http://bwf.hnqzz.top

Java: // 手写回溯递归
来源：http://dpv.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://cnh.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://lgf.bbcook.cn

C#:   // 手写回溯递归
来源：http://tor.pengpengdd.cyou

[N09] 栈与队列
来源：http://xjv.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xgs.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iea.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ika.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://udq.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cdy.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vcm.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rax.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfm.zhiwuduotai.top

[N10] 链表节点定义
来源：http://fey.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jmn.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dnz.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tzp.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bee.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://nga.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://keg.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://awo.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lhm.cheryme.top

[N11] 二叉树中序遍历
来源：http://gmo.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sbs.yj20258.top

PHP:  // 手写递归函数
来源：http://jkf.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqu.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wye.pycfn.com

Java: // 手写递归
来源：http://buf.jinqigfzy.top

Go:   // 手写递归
来源：http://njl.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://snp.bbcook.cn

C#:   // 手写递归
来源：http://kux.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cnz.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kzk.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://drg.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xpq.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvt.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gpq.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zmg.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://guv.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vhj.snrcjt.cn

================================================================================
来源：http://mtk.sysykeji.top

O. 并发与异步
来源：http://cjt.wangshuangyany.cn

================================================================================
来源：http://ecc.shzxlz.cn

[O01] 启动一个线程
来源：http://kxe.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wus.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ffx.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qjc.hcnkem.com

TS:   // 同 JS
来源：http://jqt.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://hza.jiagoushi.top

Go:   go f()
来源：http://jmy.yuxming.cn

Ruby: Thread.new { f }
来源：http://zku.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://vxd.c1oappe.top

[O02] 使用线程池
来源：http://sns.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jmq.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://brp.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://udh.cucudq.cn

TS:   // worker_threads 线程池
来源：http://lzx.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://cbf.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://muk.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bgs.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://typ.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://ulp.epnwcf.com

Py:   with lock: shared += 1
来源：http://bqw.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://piy.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kgt.xuetiantiany.cn

TS:   // 同 JS
来源：http://tgj.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://rop.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cnt.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://slj.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://byu.havefunace.top

[O04] 定义异步函数并等待
来源：http://lxa.tarul.cn

Py:   async def f():⏎    await g()
来源：http://nyo.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ups.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://mhw.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tbh.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dcz.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yfz.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://cwi.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://kbm.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://izk.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://hbf.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jkd.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://qni.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://prl.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cen.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://led.ydzc1.top

Ruby: threads.map(&:join)
来源：http://cux.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sar.ybcxt.top

[O06] 使用进程池
来源：http://dbn.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oxr.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dkq.ivvv.top

JS:   // child_process / cluster 模块
来源：http://civ.tarul.cn

TS:   // child_process / cluster 模块
来源：http://hke.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://god.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hbz.yvedp.cn

Ruby: // fork 块
来源：http://sjm.jqgfzy.top

C#:   Parallel.For
来源：http://jpc.cheryme.top

================================================================================
来源：http://rlz.jqgufenzy.top

P. 常用工具函数
来源：http://fjj.vehdjk.com

================================================================================
来源：http://rio.sjlbkw.cn

[P01] 生成 UUID
来源：http://ueo.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://oma.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ucf.andypj.xyz

JS:   crypto.randomUUID()
来源：http://ouc.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://fkp.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://uzc.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://gyo.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://kzs.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://cza.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://ntq.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fmr.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://zea.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://igz.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ema.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vko.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eby.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dzr.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://crq.shzxlz.cn

[P03] 生成短随机字符串
来源：http://byj.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gnn.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jtf.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zno.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jnk.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gax.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lta.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ngc.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ate.hysaishi.cn

[P04] 求长度
来源：http://hqy.xuanzx.com


<!-- 参考信息 -->