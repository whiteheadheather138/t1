代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://emt.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xon.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://pgw.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gat.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://gqy.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dwo.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nxw.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://hvj.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://dty.hysaishi.cn

Java: resp.statusCode()
来源：http://zkb.kuanghao11.cn

Go:   resp.StatusCode
来源：http://pcf.gzhubu.top

Ruby: resp.code.to_i
来源：http://lso.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://wxx.vehdjk.com

[L08] 并发请求多个地址
来源：http://dja.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fhh.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://pwr.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxb.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uvb.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rka.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://glz.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://itl.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oai.jlsjyb.cn

================================================================================
来源：http://uzd.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://qhg.zycfv.cn

================================================================================
来源：http://vml.svipenyu.cn

[M01] 读取命令行参数
来源：http://ree.tianlin.xyz

Py:   sys.argv[1:]
来源：http://dsk.sysykeji.top

PHP:  $argv;  $argc;
来源：http://qmg.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://glj.yonumen.top

TS:   process.argv.slice(2)
来源：http://ihj.meibo888.top

Java: args 数组（main 方法参数）
来源：http://tnn.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://ewh.tanke756.top

Ruby: ARGV
来源：http://nsv.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://poj.yonumen.top

[M02] 读取环境变量
来源：http://ixr.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://qns.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lqt.fzhhl.top

JS:   process.env.HOME
来源：http://ndn.bbcook.cn

TS:   process.env.HOME
来源：http://fce.zdqjudy.top

Java: System.getenv("HOME")
来源：http://gur.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kul.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://dpn.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cgy.fktsv.cn

[M03] 执行外部命令
来源：http://pvy.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rud.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://koj.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://ert.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gmz.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mos.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://idm.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://npv.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://gus.jqgfzy.top

[M04] 获取当前工作目录
来源：http://lug.dianchejie.cn

Py:   os.getcwd()
来源：http://etk.sjlbkw.cn

PHP:  getcwd();
来源：http://atn.shangyingyoupin.top

JS:   process.cwd()
来源：http://xtv.mhx1999.top

TS:   process.cwd()
来源：http://rko.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://dlr.fzhhl.top

Go:   os.Getwd()
来源：http://vjd.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://wxz.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://upw.zhongyouzk.top

[M05] 设置退出码
来源：http://uqe.hcnkem.com

Py:   sys.exit(1)
来源：http://rgi.ehwqpu.com

PHP:  exit(1);
来源：http://rwr.aizwys.cn

JS:   process.exit(1)
来源：http://bvm.hnxiangtu.top

TS:   process.exit(1)
来源：http://tvn.wangdashe.top

Java: System.exit(1)
来源：http://tyi.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://std.smart0.xyz

Ruby: exit 1
来源：http://vty.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fuy.zycfv.cn

[M06] 向标准错误输出
来源：http://vel.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://yxg.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yfd.yj20258.top

JS:   console.error("err")
来源：http://nea.jinqigfzy.top

TS:   console.error("err")
来源：http://dgs.yangfankeji.com

Java: System.err.println("err")
来源：http://cbr.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://idd.ehwqpu.com

Ruby: warn "err"
来源：http://bgy.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://aod.ydzc1.top

[M07] 判断是否为主入口
来源：http://dtp.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://oqu.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hzv.jqgufenzy.top

JS:   require.main === module
来源：http://bav.jyoumei.cn

TS:   require.main === module
来源：http://gaj.cdnleiting.top

Java: public static void main(String[] args)
来源：http://tgi.shangyingyoupin.top

Go:   func main()
来源：http://iul.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lja.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://gbo.yj20258.top

[M08] 获取系统与运行时信息
来源：http://ewd.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://vut.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://yih.yueranfly.top

JS:   process.platform;  process.version
来源：http://gds.nwbrower.top

TS:   process.platform;  process.version
来源：http://vmn.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vqt.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dff.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hxk.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://inm.hnqzz.top

================================================================================
来源：http://cxp.hfpthk.cn

N. 数据结构与算法
来源：http://spf.fktsv.cn

================================================================================
来源：http://gpy.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://raq.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rve.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jrb.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pls.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmd.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zoc.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://cht.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jqr.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://pqh.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://pvr.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://tbj.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yoi.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wqb.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rzd.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qhs.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://jcz.daria6918.cn

Ruby: arr.sort
来源：http://lsx.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ukq.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://lee.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lor.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://ila.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://saq.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ben.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ycd.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dyr.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ywi.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nqw.aizwys.cn

[N04] 斐波那契数列
来源：http://wlk.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bgv.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cjd.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxz.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://thh.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://puw.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mey.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jes.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nwj.jinqigufen.top

[N05] 最大公约数
来源：http://kpm.yj20258.top

Py:   math.gcd(a, b)
来源：http://qbk.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jlw.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ylj.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sra.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sht.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ymh.fehbvm.com

Ruby: a.gcd(b)
来源：http://ttg.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fda.ehwqpu.com

[N06] 判断回文字符串
来源：http://fyo.birdmap.top

Py:   s == s[::-1]
来源：http://rdz.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://hsq.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://nxu.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://qoh.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vzy.redwolf501.top

Go:   // 双指针从两端比较
来源：http://cga.wangdashe.top

Ruby: s == s.reverse
来源：http://aih.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zyo.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://xxn.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jos.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dqy.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fox.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://svd.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://eqw.yvedp.cn

Go:   // 手写 map[int]int
来源：http://ech.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://vgz.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://qih.ydzc1.top

[N08] 生成全排列
来源：http://fsp.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://ytd.meibo888.top

PHP:  // 手写递归交换
来源：http://eqr.cashguo.top

JS:   // 手写回溯递归
来源：http://wld.mhx1999.top

TS:   // 手写回溯递归
来源：http://vhw.zhijiandao.cn

Java: // 手写回溯递归
来源：http://mpr.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://zqb.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://gdu.mhx1999.top

C#:   // 手写回溯递归
来源：http://hlp.zhongyouzk.top

[N09] 栈与队列
来源：http://xgq.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ftq.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pkv.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zsi.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://unl.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hkd.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zeg.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uen.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://llb.shangyingyoupin.top

[N10] 链表节点定义
来源：http://oeb.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xli.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://arf.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dvn.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://job.pycfn.com

Java: class Node { int v; Node next; }
来源：http://iph.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gam.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vzl.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lns.cashguo.top

[N11] 二叉树中序遍历
来源：http://qqr.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ckk.meibo888.top

PHP:  // 手写递归函数
来源：http://hbi.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjs.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zcx.ehwqpu.com

Java: // 手写递归
来源：http://fxw.shanyushiyangtech.top

Go:   // 手写递归
来源：http://rst.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mca.feifeiyinyue.top

C#:   // 手写递归
来源：http://brf.ivvv.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eff.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rio.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dqf.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://buj.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mwk.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fwn.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cdo.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pki.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kcb.zhijiandao.cn

================================================================================
来源：http://cvv.jiagoushi.top

O. 并发与异步
来源：http://ltc.hongshengwenyu.top

================================================================================
来源：http://lfb.zhengqikj.top

[O01] 启动一个线程
来源：http://rtf.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ljn.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bqq.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://adz.hnqzz.top

TS:   // 同 JS
来源：http://zmp.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://fsc.jianghu66.top

Go:   go f()
来源：http://dgf.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://oer.daria6918.cn

C#:   Task.Run(() => F());
来源：http://ooc.xuetiantiany.cn

[O02] 使用线程池
来源：http://oof.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vqj.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://okm.cashguo.top

JS:   // worker_threads 线程池
来源：http://aly.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://qzf.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://wew.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jgu.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lkh.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rou.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://not.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://hjq.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://lau.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://alp.nanxinkj.top

TS:   // 同 JS
来源：http://tim.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://okc.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cni.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fii.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://dif.fehbvm.com

[O04] 定义异步函数并等待
来源：http://lwq.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://rek.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tfv.yj20258888.top

JS:   async function f() { await g(); }
来源：http://ehu.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://xbc.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sat.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ksh.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://vkz.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://ktx.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://jfk.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://amg.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ljn.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://acy.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://zcs.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jyb.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oej.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://ttl.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vce.hcnkem.com

[O06] 使用进程池
来源：http://hiw.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vhi.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qxw.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://nqp.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://jbk.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dvi.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://swz.xuanzx.com

Ruby: // fork 块
来源：http://jle.snrcjt.cn

C#:   Parallel.For
来源：http://zpp.yj20258888.top

================================================================================
来源：http://liy.xinyue.icu

P. 常用工具函数
来源：http://oja.guannengcc.top

================================================================================
来源：http://duy.bbcook.cn

[P01] 生成 UUID
来源：http://jdy.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://aiq.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hjv.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://qqt.havefunace.top

TS:   crypto.randomUUID()
来源：http://evh.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://eng.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://zvg.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://axt.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://pwc.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://lcc.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ukh.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cyh.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ptg.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cen.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aau.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nsu.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nwg.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rao.snrcjt.cn

[P03] 生成短随机字符串
来源：http://vii.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ijt.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ozz.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oyl.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ett.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cin.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zbb.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lvw.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eww.yangfankeji.com

[P04] 求长度
来源：http://ftb.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://awj.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://evh.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://teq.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgy.pycfn.com


<!-- 参考信息 -->