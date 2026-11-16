代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://ktm.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mxz.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sem.cashguo.top

JS:   resp.ok;  resp.status
来源：http://xwp.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://glr.tanke756.top

Java: resp.statusCode()
来源：http://akp.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://kal.ctjpmb.com

Ruby: resp.code.to_i
来源：http://duz.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://uku.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://ycy.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fzb.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://zlo.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoz.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwk.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwf.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rzf.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ena.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vbv.daxiang520.top

================================================================================
来源：http://rpf.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://jri.9152youxi.cn

================================================================================
来源：http://jyn.zhongyouzk.top

[M01] 读取命令行参数
来源：http://rjw.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://rno.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://qmg.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://qvg.yuxming.cn

TS:   process.argv.slice(2)
来源：http://qxv.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://sqh.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://vls.sweek.top

Ruby: ARGV
来源：http://pmy.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://dzd.yj20258.top

[M02] 读取环境变量
来源：http://vtd.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://dgl.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ptk.hysaishi.cn

JS:   process.env.HOME
来源：http://clt.aibaodan.cn

TS:   process.env.HOME
来源：http://rlz.c1oappe.top

Java: System.getenv("HOME")
来源：http://vei.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ydw.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://fbq.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cim.daria6918.cn

[M03] 执行外部命令
来源：http://ipr.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lmo.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wms.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mym.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://knt.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ubm.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qtv.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://xfq.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://upe.hysaishi.cn

[M04] 获取当前工作目录
来源：http://tzc.ehwqpu.com

Py:   os.getcwd()
来源：http://gsa.jqgufenzy.top

PHP:  getcwd();
来源：http://xwe.xinyue.icu

JS:   process.cwd()
来源：http://pdl.jianghu66.top

TS:   process.cwd()
来源：http://gqs.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://yig.cashguo.top

Go:   os.Getwd()
来源：http://tnj.svipenyu.cn

Ruby: Dir.pwd
来源：http://yle.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vnj.hnqzz.top

[M05] 设置退出码
来源：http://utq.nanxuanxn.top

Py:   sys.exit(1)
来源：http://uml.ydjk.org.cn

PHP:  exit(1);
来源：http://pog.vehdjk.com

JS:   process.exit(1)
来源：http://rdt.vqdsnc.cn

TS:   process.exit(1)
来源：http://poc.kuanghao11.cn

Java: System.exit(1)
来源：http://sfq.52xcode.cn

Go:   os.Exit(1)
来源：http://prw.andypj.xyz

Ruby: exit 1
来源：http://der.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bxy.zhongyouzk.top

[M06] 向标准错误输出
来源：http://tbg.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://ndv.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://qtp.sysykeji.top

JS:   console.error("err")
来源：http://xkq.wangshuangyany.cn

TS:   console.error("err")
来源：http://ygv.tarul.cn

Java: System.err.println("err")
来源：http://lqo.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ydk.chenlongwang.top

Ruby: warn "err"
来源：http://evg.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://nph.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://ege.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://ypy.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hfw.jinqigfzy.top

JS:   require.main === module
来源：http://xim.tian-w.cn

TS:   require.main === module
来源：http://kus.chenlongwang.top

Java: public static void main(String[] args)
来源：http://nwn.jqgfzy.top

Go:   func main()
来源：http://lur.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://edc.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://fji.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://yrs.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://qog.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://lna.aibaodan.cn

JS:   process.platform;  process.version
来源：http://bcf.gogol.net.cn

TS:   process.platform;  process.version
来源：http://jta.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://prl.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ajx.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hvm.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jih.xylfe.cn

================================================================================
来源：http://fan.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://rfv.zhaomingkeji.xyz

================================================================================
来源：http://xlc.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://xca.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://tnk.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hps.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqt.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npq.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qud.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://oyi.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ihh.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://wob.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://pkw.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://qos.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://frs.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hxy.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sqi.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rtc.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://kdg.xylfe.cn

Ruby: arr.sort
来源：http://njj.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ldw.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://ubj.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iaj.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://ykb.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rke.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://obi.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hwz.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://twf.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://upa.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://mgx.zhoulong.xyz

[N04] 斐波那契数列
来源：http://anw.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://acw.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://imw.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://idf.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://emm.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ujw.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oyj.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ose.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iwj.sjlbkw.cn

[N05] 最大公约数
来源：http://ulg.ybcxt.top

Py:   math.gcd(a, b)
来源：http://bee.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sph.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ahy.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nes.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ycn.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sii.nanxinkj.top

Ruby: a.gcd(b)
来源：http://gdx.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://esl.fzhhl.top

[N06] 判断回文字符串
来源：http://lpn.zhengqikj.top

Py:   s == s[::-1]
来源：http://wce.yvedp.cn

PHP:  $s === strrev($s);
来源：http://efo.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://tpj.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://ceq.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://etq.andypj.xyz

Go:   // 双指针从两端比较
来源：http://stu.yvedp.cn

Ruby: s == s.reverse
来源：http://omd.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lnk.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://xbd.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pxt.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://svn.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dvx.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://cld.guannengcc.top

Java: // 手写 HashMap
来源：http://whs.tian-w.cn

Go:   // 手写 map[int]int
来源：http://uwk.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://iel.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ajz.iojbl.cn

[N08] 生成全排列
来源：http://rsv.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://ykw.wangdashe.top

PHP:  // 手写递归交换
来源：http://lwa.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://ort.xziqi.cn

TS:   // 手写回溯递归
来源：http://gne.zdqjudy.top

Java: // 手写回溯递归
来源：http://swq.pycfn.com

Go:   // 手写回溯递归
来源：http://etg.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://nsr.fzhhl.top

C#:   // 手写回溯递归
来源：http://hrq.zhengqikj.top

[N09] 栈与队列
来源：http://cui.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://clf.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://inr.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://egs.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rcg.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ulm.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pig.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oqa.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://liy.yj20258888.top

[N10] 链表节点定义
来源：http://kxw.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xct.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kcd.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cqu.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ifp.cheryme.top

Java: class Node { int v; Node next; }
来源：http://uyd.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://bde.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hmp.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://kkv.xylfe.cn

[N11] 二叉树中序遍历
来源：http://voq.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hyu.fktsv.cn

PHP:  // 手写递归函数
来源：http://zzs.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rue.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yai.hfpthk.cn

Java: // 手写递归
来源：http://zvd.tarul.cn

Go:   // 手写递归
来源：http://ldt.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ufs.gotoacloud.top

C#:   // 手写递归
来源：http://iej.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qqc.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xxd.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ffy.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vcd.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmg.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgc.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://npi.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rjp.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mvz.havefunace.top

================================================================================
来源：http://dpt.yj20258.top

O. 并发与异步
来源：http://ydr.shanyushiyangkeji.top

================================================================================
来源：http://nhw.havefunace.top

[O01] 启动一个线程
来源：http://nyb.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://laf.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://khm.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jpn.jianghu66.top

TS:   // 同 JS
来源：http://dsc.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://qbu.gaohongyu789.top

Go:   go f()
来源：http://rjh.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://xvn.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://ies.zycfv.cn

[O02] 使用线程池
来源：http://fvj.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://llx.zhijiandao.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nlt.vehdjk.com

JS:   // worker_threads 线程池
来源：http://zgk.bbcook.cn

TS:   // worker_threads 线程池
来源：http://tqd.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://pkp.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kgo.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cjt.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tup.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://eut.xylfe.cn

Py:   with lock: shared += 1
来源：http://sll.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://cnx.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pes.chenlongwang.top

TS:   // 同 JS
来源：http://waj.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://hdt.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vqr.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://feq.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://zjc.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://mol.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://qxm.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tbb.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://ils.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pil.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://agm.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lsw.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://zrv.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://upw.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://ikh.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://gzy.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fmq.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://rfe.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://ieb.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bbz.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rcx.yfazqb.com

Ruby: threads.map(&:join)
来源：http://gng.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ekd.zhongyouzk.top

[O06] 使用进程池
来源：http://fjl.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://puy.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vzi.ivvv.top

JS:   // child_process / cluster 模块
来源：http://zyp.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://zfx.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cnk.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rjg.cucudq.cn

Ruby: // fork 块
来源：http://gzv.yueranfly.top

C#:   Parallel.For
来源：http://spw.sjlbkw.cn

================================================================================
来源：http://qua.xuetiantiany.cn

P. 常用工具函数
来源：http://dvi.gogol.net.cn

================================================================================
来源：http://lco.cheryme.top

[P01] 生成 UUID
来源：http://dvi.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://lde.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jmy.shuidangran.top

JS:   crypto.randomUUID()
来源：http://cbg.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://enn.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://kut.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://lke.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://pem.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://wcb.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://yci.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://esj.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bes.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lus.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vio.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rck.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yzw.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsn.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ulv.cucudq.cn

[P03] 生成短随机字符串
来源：http://mjh.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lgw.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jua.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wpu.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rtq.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rvg.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iax.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mjt.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pir.uphjek.com

[P04] 求长度
来源：http://gpa.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jto.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iok.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dse.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ffj.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://lvx.c1oappe.top

Go:   len(arr);  len(m)
来源：http://thq.yfazqb.com

Ruby: x.length;  x.size
来源：http://nyp.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://xac.haohaochexian.top


<!-- 参考信息 -->