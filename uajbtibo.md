代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zxj.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pcq.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://flj.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xjx.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://lzj.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ond.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://apr.cashguo.top

JS:   resp.ok;  resp.status
来源：http://pxa.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://sjg.zhengqikj.top

Java: resp.statusCode()
来源：http://svc.chenzaomai.com

Go:   resp.StatusCode
来源：http://gys.gotoacloud.top

Ruby: resp.code.to_i
来源：http://lhv.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://hla.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://rnv.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ykn.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://bge.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oej.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oyl.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kna.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ruu.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wqu.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hjg.52xcode.cn

================================================================================
来源：http://wsk.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://van.ehwqpu.com

================================================================================
来源：http://lod.ydzc1.top

[M01] 读取命令行参数
来源：http://wpl.yj20258888.top

Py:   sys.argv[1:]
来源：http://wmd.c1oappe.top

PHP:  $argv;  $argc;
来源：http://duy.yongpay.top

JS:   process.argv.slice(2)
来源：http://gmz.c1oappe.top

TS:   process.argv.slice(2)
来源：http://zjv.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://uul.hammf.cn

Go:   os.Args[1:]
来源：http://cvt.meibo888.top

Ruby: ARGV
来源：http://iwf.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://hwx.tarul.cn

[M02] 读取环境变量
来源：http://iuj.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://lor.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gyd.tian-w.cn

JS:   process.env.HOME
来源：http://scq.daxiang520.top

TS:   process.env.HOME
来源：http://myk.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://kan.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zqa.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://xta.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ooa.epnwcf.com

[M03] 执行外部命令
来源：http://rqf.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lug.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://utx.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://zap.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://tii.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zit.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vji.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://vdh.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://wdb.cdnleiting.top

[M04] 获取当前工作目录
来源：http://iza.gaohongyu789.top

Py:   os.getcwd()
来源：http://utx.dianchejie.cn

PHP:  getcwd();
来源：http://tos.yj20258888.top

JS:   process.cwd()
来源：http://czt.yj202588.top

TS:   process.cwd()
来源：http://yzk.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://sut.gogol.net.cn

Go:   os.Getwd()
来源：http://amw.birdmap.top

Ruby: Dir.pwd
来源：http://fvd.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://kjq.pycfn.com

[M05] 设置退出码
来源：http://ovz.yongpay.top

Py:   sys.exit(1)
来源：http://wme.52xcode.cn

PHP:  exit(1);
来源：http://dsa.chenlongwang.top

JS:   process.exit(1)
来源：http://lyc.gogol.net.cn

TS:   process.exit(1)
来源：http://hng.jinqigfzy.top

Java: System.exit(1)
来源：http://bsy.cqqwz.cn

Go:   os.Exit(1)
来源：http://wys.zhixingplan.top

Ruby: exit 1
来源：http://nda.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jgw.yangfankeji.com

[M06] 向标准错误输出
来源：http://vcn.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://vci.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dch.tanke756.top

JS:   console.error("err")
来源：http://ghu.zhijiandao.cn

TS:   console.error("err")
来源：http://viq.nanxinkj.top

Java: System.err.println("err")
来源：http://gdw.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://asf.ehwqpu.com

Ruby: warn "err"
来源：http://wbw.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://dwp.redwolf501.top

[M07] 判断是否为主入口
来源：http://fzp.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://ppg.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vhx.hongshengwenyu.top

JS:   require.main === module
来源：http://hic.epnwcf.com

TS:   require.main === module
来源：http://yvr.yuanzhike.top

Java: public static void main(String[] args)
来源：http://oto.zhoulong.xyz

Go:   func main()
来源：http://avh.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fzd.tanke756.top

C#:   static void Main(string[] args)
来源：http://fet.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://eva.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://xjc.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://wgc.c1oappe.top

JS:   process.platform;  process.version
来源：http://ipd.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://vbj.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dho.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bva.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://piw.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rse.vqdsnc.cn

================================================================================
来源：http://djt.xuanzx.com

N. 数据结构与算法
来源：http://nkx.pengpengdd.cyou

================================================================================
来源：http://hfw.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://gbt.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://dbd.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xoi.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ilt.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ise.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vks.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://klz.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qrd.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ddd.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://box.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://dms.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tpf.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bvy.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nhz.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hft.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://ynz.meibo888.top

Ruby: arr.sort
来源：http://dnu.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tqm.havefunace.top

[N03] 快速排序（分治示例）
来源：http://qkt.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcv.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://qzt.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hio.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vqq.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yiz.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ljy.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jmj.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://odn.wangdashe.top

[N04] 斐波那契数列
来源：http://ike.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://izm.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://noj.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cge.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yuv.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mxi.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gao.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ukp.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zrr.jqgufenzy.top

[N05] 最大公约数
来源：http://ozz.jianghu66.top

Py:   math.gcd(a, b)
来源：http://iep.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gow.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lyx.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aht.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tad.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brs.cdnleiting.top

Ruby: a.gcd(b)
来源：http://sgo.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xnu.ydjk.org.cn

[N06] 判断回文字符串
来源：http://xjm.cashguo.top

Py:   s == s[::-1]
来源：http://uel.fzhhl.top

PHP:  $s === strrev($s);
来源：http://thv.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://kxd.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://omt.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lkz.yfazqb.com

Go:   // 双指针从两端比较
来源：http://wbc.ydzc1.top

Ruby: s == s.reverse
来源：http://zey.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ebz.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://uqu.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xfm.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zca.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nuc.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://skl.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://msd.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://wav.xziqi.cn

Ruby: // 手写 Hash
来源：http://kap.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://oem.jinghuilouyu.cn

[N08] 生成全排列
来源：http://fgp.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://lge.smart0.xyz

PHP:  // 手写递归交换
来源：http://qqx.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://kqn.sufxvd.cn

TS:   // 手写回溯递归
来源：http://kdf.xuanzx.com

Java: // 手写回溯递归
来源：http://cvv.aibaodan.cn

Go:   // 手写回溯递归
来源：http://fno.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://pih.meibo888.top

C#:   // 手写回溯递归
来源：http://buo.chenjidiqi.icu

[N09] 栈与队列
来源：http://ctz.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sum.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hsj.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rmk.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ggx.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jps.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dor.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mmb.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ukn.aibaodan.cn

[N10] 链表节点定义
来源：http://juz.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://khy.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kpf.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gcr.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hhr.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://usa.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://ier.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ssr.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vcj.ppjwa.cn

[N11] 二叉树中序遍历
来源：http://nzy.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pwt.zhixingplan.top

PHP:  // 手写递归函数
来源：http://qvr.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rtv.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lox.52xcode.cn

Java: // 手写递归
来源：http://oxn.jinqigufen.top

Go:   // 手写递归
来源：http://uht.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uez.pycfn.com

C#:   // 手写递归
来源：http://bqi.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qsc.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wtp.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vnv.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzd.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lfs.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lyv.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tub.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kcj.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hou.ctjpmb.com

================================================================================
来源：http://vvy.yanxiufei.cn

O. 并发与异步
来源：http://xtu.shzxlz.cn

================================================================================
来源：http://cdu.jiagoushi.top

[O01] 启动一个线程
来源：http://hiu.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ixu.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dgs.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uts.chenzaomai.com

TS:   // 同 JS
来源：http://sgl.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://pep.gotoacloud.top

Go:   go f()
来源：http://msv.9152youxi.cn

Ruby: Thread.new { f }
来源：http://zbj.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://hjy.ehwqpu.com

[O02] 使用线程池
来源：http://byx.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zdd.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ipz.aizwys.cn

JS:   // worker_threads 线程池
来源：http://tfd.epnwcf.com

TS:   // worker_threads 线程池
来源：http://xvf.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ijm.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rwb.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://orj.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://itx.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://qrd.chenlongwang.top

Py:   with lock: shared += 1
来源：http://ane.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://dtj.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://usr.ppjwa.cn

TS:   // 同 JS
来源：http://gjo.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://kvl.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iml.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aei.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://wuu.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://vrx.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://pbj.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://foe.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://yni.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kec.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hxj.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uey.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://qxt.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://umf.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://zwu.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://xpj.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qjx.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://yjz.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://vxb.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fvn.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://msa.daxiang520.top

Ruby: threads.map(&:join)
来源：http://mgy.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://edx.vqdsnc.cn

[O06] 使用进程池
来源：http://ofu.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gqt.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://pfy.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://tux.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://dwx.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qal.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mfj.feifeiyinyue.top

Ruby: // fork 块
来源：http://gxc.zdbjq.cn

C#:   Parallel.For
来源：http://zjt.bjfxy.top

================================================================================
来源：http://gpe.gogol.net.cn

P. 常用工具函数
来源：http://tli.ydzc1.top

================================================================================
来源：http://cvn.nanxuanxn.top

[P01] 生成 UUID
来源：http://otv.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://jzb.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kdd.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://bmn.dianchejie.cn

TS:   crypto.randomUUID()
来源：http://ywt.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://hlj.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://zsg.ivvv.top

Ruby: SecureRandom.uuid
来源：http://orm.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://qdx.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://gxj.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ndn.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://odo.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tpr.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yqv.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ocz.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wmd.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jyt.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cda.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://jqy.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ash.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qvg.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://puy.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zwt.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rxr.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ybw.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://cuz.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jig.yj20258888.top

[P04] 求长度
来源：http://ruo.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgz.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfs.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnj.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sbm.yuanzhike.top


<!-- 参考信息 -->