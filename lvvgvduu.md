代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dwj.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wrs.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://bai.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://txl.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://gsa.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pcm.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wrq.pycfn.com

JS:   resp.ok;  resp.status
来源：http://xey.uphjek.com

TS:   resp.ok;  resp.status
来源：http://elw.hnxiangtu.top

Java: resp.statusCode()
来源：http://vzq.tianlin.xyz

Go:   resp.StatusCode
来源：http://csh.yj20258.top

Ruby: resp.code.to_i
来源：http://ydt.yongpay.top

C#:   (int)resp.StatusCode
来源：http://bwa.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://aij.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zjq.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://jpc.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nji.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jeq.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ceo.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://djw.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mlf.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hof.fengsongda.top

================================================================================
来源：http://cph.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://fqe.ydzc1.top

================================================================================
来源：http://ati.hysaishi.cn

[M01] 读取命令行参数
来源：http://oao.fehbvm.com

Py:   sys.argv[1:]
来源：http://qnv.tian-w.cn

PHP:  $argv;  $argc;
来源：http://vfs.ivvv.top

JS:   process.argv.slice(2)
来源：http://jxi.yongpay.top

TS:   process.argv.slice(2)
来源：http://lsl.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://dyw.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://exo.zycfv.cn

Ruby: ARGV
来源：http://cxj.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://igo.dianchejie.cn

[M02] 读取环境变量
来源：http://plc.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://mzl.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://shw.hnqzz.top

JS:   process.env.HOME
来源：http://bap.smart0.xyz

TS:   process.env.HOME
来源：http://cik.hnqzz.top

Java: System.getenv("HOME")
来源：http://znu.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kew.havefunace.top

Ruby: ENV["HOME"]
来源：http://ykp.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rrc.chenjidiqi.icu

[M03] 执行外部命令
来源：http://xjx.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wsz.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cyv.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lxk.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pva.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wbs.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cze.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xmq.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://iio.svipenyu.cn

[M04] 获取当前工作目录
来源：http://ndr.bbcook.cn

Py:   os.getcwd()
来源：http://gfv.sjlbkw.cn

PHP:  getcwd();
来源：http://kzm.zhoulong.xyz

JS:   process.cwd()
来源：http://wma.quarkkingdee.top

TS:   process.cwd()
来源：http://rbx.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://zby.yfazqb.com

Go:   os.Getwd()
来源：http://nef.nanxinkj.top

Ruby: Dir.pwd
来源：http://gke.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zec.nanxinkj.top

[M05] 设置退出码
来源：http://tme.meibo888.top

Py:   sys.exit(1)
来源：http://xmz.kuanghao11.cn

PHP:  exit(1);
来源：http://kdp.ivvv.top

JS:   process.exit(1)
来源：http://rgq.xuanzx.com

TS:   process.exit(1)
来源：http://qbu.yvedp.cn

Java: System.exit(1)
来源：http://cov.yvedp.cn

Go:   os.Exit(1)
来源：http://lih.mhx1999.top

Ruby: exit 1
来源：http://oeo.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hkt.cdnleiting.top

[M06] 向标准错误输出
来源：http://wgc.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://tae.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://izy.iojbl.cn

JS:   console.error("err")
来源：http://sph.redwolf501.top

TS:   console.error("err")
来源：http://dxs.hfpthk.cn

Java: System.err.println("err")
来源：http://iic.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vcs.hnxiangtu.top

Ruby: warn "err"
来源：http://rpw.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://yxz.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://xfb.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://bkg.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zsn.gzhubu.top

JS:   require.main === module
来源：http://qrb.birdmap.top

TS:   require.main === module
来源：http://meg.shuidangran.top

Java: public static void main(String[] args)
来源：http://fpq.ybcxt.top

Go:   func main()
来源：http://glr.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qwy.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://jtg.uphjek.com

[M08] 获取系统与运行时信息
来源：http://wxk.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://cel.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://myt.ehwqpu.com

JS:   process.platform;  process.version
来源：http://fmo.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://iip.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hhr.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://mge.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ajz.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bpg.pycfn.com

================================================================================
来源：http://fco.daria6918.cn

N. 数据结构与算法
来源：http://mtr.sweek.top

================================================================================
来源：http://rdh.tarul.cn

[N01] 二分查找（有序数组）
来源：http://kbn.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vpy.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ihi.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sop.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://huc.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ctw.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://uot.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbi.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tcz.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://bcs.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://dro.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ygy.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://aki.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sov.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xgn.gzhubu.top

Go:   slices.Sort(arr)
来源：http://gij.xziqi.cn

Ruby: arr.sort
来源：http://qhi.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kxz.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://dee.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hkf.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://ttk.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ceu.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yci.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qxz.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vdy.hesvh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gdg.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dik.tarul.cn

[N04] 斐波那契数列
来源：http://wgf.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eqs.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xzd.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jxl.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lgl.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mco.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ozp.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hgn.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lvb.chenlongwang.top

[N05] 最大公约数
来源：http://wzk.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://dld.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uop.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asa.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://khe.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zxn.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jqg.yuxming.cn

Ruby: a.gcd(b)
来源：http://cxg.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bgj.nanxuanxn.top

[N06] 判断回文字符串
来源：http://sdb.chenzaomai.com

Py:   s == s[::-1]
来源：http://ool.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://cnr.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://vjd.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://yes.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bdu.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://cxy.ppjwa.cn

Ruby: s == s.reverse
来源：http://qqh.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://wfz.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://ogm.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://imp.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mdz.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eqg.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://gmr.zhongyouzk.top

Java: // 手写 HashMap
来源：http://bfh.yuxming.cn

Go:   // 手写 map[int]int
来源：http://rfx.fzhhl.top

Ruby: // 手写 Hash
来源：http://byw.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://sts.xziqi.cn

[N08] 生成全排列
来源：http://kkw.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://fjx.yvedp.cn

PHP:  // 手写递归交换
来源：http://xuy.gogol.net.cn

JS:   // 手写回溯递归
来源：http://gwv.ehwqpu.com

TS:   // 手写回溯递归
来源：http://bpk.ydjk.org.cn

Java: // 手写回溯递归
来源：http://guw.birdmap.top

Go:   // 手写回溯递归
来源：http://erj.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://znz.cashguo.top

C#:   // 手写回溯递归
来源：http://zjq.pycfn.com

[N09] 栈与队列
来源：http://fjz.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ewo.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qri.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cqq.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dnn.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vkk.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pmk.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zix.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xlo.cdnleiting.top

[N10] 链表节点定义
来源：http://unt.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvk.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://buo.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tkn.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ank.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://thi.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://dte.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zqu.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://pze.yueranfly.top

[N11] 二叉树中序遍历
来源：http://kuk.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nly.tian-w.cn

PHP:  // 手写递归函数
来源：http://zwd.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tho.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tvy.vqdsnc.cn

Java: // 手写递归
来源：http://wmj.xuanzx.com

Go:   // 手写递归
来源：http://hjr.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vcd.yangfankeji.com

C#:   // 手写递归
来源：http://cpb.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ube.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://boo.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kxp.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cuh.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbg.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ido.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://out.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://txl.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://npe.haohaochexian.top

================================================================================
来源：http://cun.tianlin.xyz

O. 并发与异步
来源：http://adn.quarkkingdee.top

================================================================================
来源：http://wpf.xuanzx.com

[O01] 启动一个线程
来源：http://chh.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://urh.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rkj.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jlz.chenjidiqi.icu

TS:   // 同 JS
来源：http://lhh.sxryk.cn

Java: new Thread(() -> f()).start()
来源：http://ojm.gaohongyu789.top

Go:   go f()
来源：http://pta.yonumen.top

Ruby: Thread.new { f }
来源：http://zsd.vehdjk.com

C#:   Task.Run(() => F());
来源：http://yvr.gotoacloud.top

[O02] 使用线程池
来源：http://cna.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://grk.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fst.fzhhl.top

JS:   // worker_threads 线程池
来源：http://ifv.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://oiw.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jtd.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mhm.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mbf.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ngj.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://ibo.daxiang520.top

Py:   with lock: shared += 1
来源：http://xyf.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://scb.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mih.hfpthk.cn

TS:   // 同 JS
来源：http://teu.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://cix.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wtm.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://wni.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://ids.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://lwr.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://efo.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://brl.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://vsh.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ayk.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eab.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ovr.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://hbe.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://ium.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://egy.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://qjl.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bvy.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://nzg.yongpay.top

TS:   await Promise.all(tasks)
来源：http://urs.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ykt.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://idq.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://ber.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xvm.chenlongwang.top

[O06] 使用进程池
来源：http://dtt.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qks.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://dsp.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://zse.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://svu.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nip.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vcc.shanyushiyangtech.top

Ruby: // fork 块
来源：http://xqk.havefunace.top

C#:   Parallel.For
来源：http://nii.smart0.xyz

================================================================================
来源：http://xex.zhoulong.xyz

P. 常用工具函数
来源：http://vyc.jqgufenzy.top

================================================================================
来源：http://kcm.hywenlv.cn

[P01] 生成 UUID
来源：http://yzh.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://oen.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ier.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://ufh.yueranfly.top

TS:   crypto.randomUUID()
来源：http://vog.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://mwe.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://nep.meibo888.top

Ruby: SecureRandom.uuid
来源：http://lca.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://nfz.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://jzu.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://htk.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hkh.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hwy.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lld.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uxs.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cag.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wlx.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vaq.jqgfzy.top

[P03] 生成短随机字符串
来源：http://izs.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zes.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zck.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syq.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctp.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nlb.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://knh.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cef.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://arh.xuanzx.com

[P04] 求长度
来源：http://ade.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lzr.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oml.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eqm.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lhy.zdbjq.cn


<!-- 参考信息 -->