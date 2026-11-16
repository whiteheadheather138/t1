代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qzi.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bkt.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://ztz.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zlu.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://qku.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ygu.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zfd.cheryme.top

JS:   resp.ok;  resp.status
来源：http://rgl.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://cvu.svipenyu.cn

Java: resp.statusCode()
来源：http://muj.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://idh.0kj1m.cn

Ruby: resp.code.to_i
来源：http://vty.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://dyx.jinqigufen.top

[L08] 并发请求多个地址
来源：http://lrq.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yep.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://klq.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxq.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ilm.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zdu.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://prq.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lhx.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qxn.wangshuangyany.cn

================================================================================
来源：http://ofg.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://ump.sjlbkw.cn

================================================================================
来源：http://kfo.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://fvx.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://vnh.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://pdc.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://hej.mhx1999.top

TS:   process.argv.slice(2)
来源：http://rsn.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://wzm.jyoumei.cn

Go:   os.Args[1:]
来源：http://myd.aizwys.cn

Ruby: ARGV
来源：http://ftd.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://ogi.dianchejie.cn

[M02] 读取环境变量
来源：http://iez.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://itl.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rtl.redwolf501.top

JS:   process.env.HOME
来源：http://cpv.yanxiufei.cn

TS:   process.env.HOME
来源：http://ssx.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://mhe.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pza.sxryk.cn

Ruby: ENV["HOME"]
来源：http://gwe.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ime.fktsv.cn

[M03] 执行外部命令
来源：http://dvw.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ezc.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lte.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ypp.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eba.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ifb.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://fwg.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://bgz.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://zoj.cdnleiting.top

[M04] 获取当前工作目录
来源：http://tkn.guowangkeji.top

Py:   os.getcwd()
来源：http://vge.zhijiandao.cn

PHP:  getcwd();
来源：http://ytd.feifeiyinyue.top

JS:   process.cwd()
来源：http://ssd.ybcxt.top

TS:   process.cwd()
来源：http://hol.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://yuk.gotoacloud.top

Go:   os.Getwd()
来源：http://acd.fengsongda.top

Ruby: Dir.pwd
来源：http://sid.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://znk.9152youxi.cn

[M05] 设置退出码
来源：http://chh.pycfn.com

Py:   sys.exit(1)
来源：http://wid.yfazqb.com

PHP:  exit(1);
来源：http://gux.yongpay.top

JS:   process.exit(1)
来源：http://ydr.yuanzhike.top

TS:   process.exit(1)
来源：http://zdg.guannengcc.top

Java: System.exit(1)
来源：http://fzc.jianghu66.top

Go:   os.Exit(1)
来源：http://mnw.zhaomingkeji.xyz

Ruby: exit 1
来源：http://kcj.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bfw.yangfankeji.com

[M06] 向标准错误输出
来源：http://apo.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://jns.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://drc.jinqigufen.top

JS:   console.error("err")
来源：http://vtw.zdqjudy.top

TS:   console.error("err")
来源：http://ueh.sjlbkw.cn

Java: System.err.println("err")
来源：http://obr.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bur.smart0.xyz

Ruby: warn "err"
来源：http://hoh.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://bbk.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://xih.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://edd.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://otc.zhixingplan.top

JS:   require.main === module
来源：http://tfg.yuxming.cn

TS:   require.main === module
来源：http://gdv.pycfn.com

Java: public static void main(String[] args)
来源：http://qxs.shanyushiyangkeji.top

Go:   func main()
来源：http://bal.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qbo.hesvh.cn

C#:   static void Main(string[] args)
来源：http://mrz.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://rel.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://csm.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://ltr.nwbrower.top

JS:   process.platform;  process.version
来源：http://uvu.jinqigufen.top

TS:   process.platform;  process.version
来源：http://iwn.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gnp.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iqj.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://huw.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hru.zhoulong.xyz

================================================================================
来源：http://snk.nanxinkj.top

N. 数据结构与算法
来源：http://fes.bjfxy.top

================================================================================
来源：http://kra.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://byz.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qal.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qkj.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wvz.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://onw.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://sck.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://blq.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://duy.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://yfs.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://nbc.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://xma.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tpw.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://grl.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wfq.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qxw.hammf.cn

Go:   slices.Sort(arr)
来源：http://apl.epnwcf.com

Ruby: arr.sort
来源：http://qnx.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://khy.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://mbn.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kpy.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://uxk.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dzv.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mdb.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pxp.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gay.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lnk.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://qbs.ydjk.org.cn

[N04] 斐波那契数列
来源：http://odc.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xub.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zhp.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yls.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zow.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rcf.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qqp.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wnb.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cty.shuidangran.top

[N05] 最大公约数
来源：http://jni.yfazqb.com

Py:   math.gcd(a, b)
来源：http://bas.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vfz.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zjk.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbh.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rct.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mwz.daxiang520.top

Ruby: a.gcd(b)
来源：http://cgw.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sty.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://wnc.ydjk.org.cn

Py:   s == s[::-1]
来源：http://lwg.yj20258.top

PHP:  $s === strrev($s);
来源：http://ppz.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://ivv.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://zkd.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ywj.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://nxa.yuanzhike.top

Ruby: s == s.reverse
来源：http://eku.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ftc.hammf.cn

[N07] 两数之和（返回下标）
来源：http://fov.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://npe.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rxv.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ask.gzhubu.top

TS:   // 手写 Map<string, number>
来源：http://iuw.hammf.cn

Java: // 手写 HashMap
来源：http://iox.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://lfs.snrcjt.cn

Ruby: // 手写 Hash
来源：http://ocs.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vwi.cqqwz.cn

[N08] 生成全排列
来源：http://krx.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://fhn.hnqzz.top

PHP:  // 手写递归交换
来源：http://qzt.uphjek.com

JS:   // 手写回溯递归
来源：http://nku.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://dbk.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://jvw.ydjk.org.cn

Go:   // 手写回溯递归
来源：http://icz.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://ghj.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://wab.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://zpf.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dlq.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vgp.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://taa.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xcf.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://csu.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kyw.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://akr.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pcx.nanxuanxn.top

[N10] 链表节点定义
来源：http://yil.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ibe.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ufu.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xxe.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pdf.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://ipq.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://evt.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sof.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bdz.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://qlv.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ond.snrcjt.cn

PHP:  // 手写递归函数
来源：http://ehr.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbz.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ajd.chenlongwang.top

Java: // 手写递归
来源：http://gbg.yvedp.cn

Go:   // 手写递归
来源：http://lly.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nyu.ivvv.top

C#:   // 手写递归
来源：http://rop.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rrt.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lbc.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sfa.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ytv.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffn.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nct.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xah.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hfm.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ija.wangdashe.top

================================================================================
来源：http://aor.ppjwa.cn

O. 并发与异步
来源：http://xhi.chenzaomai.com

================================================================================
来源：http://zzp.shzxlz.cn

[O01] 启动一个线程
来源：http://itk.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wxp.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://duu.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hhz.chenjidiqi.icu

TS:   // 同 JS
来源：http://fwd.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://mnv.dianchejie.cn

Go:   go f()
来源：http://ydh.birdmap.top

Ruby: Thread.new { f }
来源：http://pdz.yj202588.top

C#:   Task.Run(() => F());
来源：http://pfm.nanxuanxn.top

[O02] 使用线程池
来源：http://quj.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tin.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bvc.cheryme.top

JS:   // worker_threads 线程池
来源：http://htx.redwolf501.top

TS:   // worker_threads 线程池
来源：http://fjy.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://dqn.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qdc.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://erm.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://csm.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://gxe.aibaodan.cn

Py:   with lock: shared += 1
来源：http://zfe.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://uuo.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sxz.aibaodan.cn

TS:   // 同 JS
来源：http://qvd.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://szn.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://omw.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hwa.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://zbn.xinyue.icu

[O04] 定义异步函数并等待
来源：http://zro.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://mvd.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ljs.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://jzx.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kpz.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ryc.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yme.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zuu.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://wmm.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://fxx.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://aji.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iiq.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://hld.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://acq.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://psk.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://clf.cashguo.top

Ruby: threads.map(&:join)
来源：http://lto.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mmh.yangfankeji.com

[O06] 使用进程池
来源：http://vee.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nhn.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yla.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://tmw.yj20258.top

TS:   // child_process / cluster 模块
来源：http://dyv.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ppo.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kqk.tarul.cn

Ruby: // fork 块
来源：http://npm.shuidangran.top

C#:   Parallel.For
来源：http://aiy.shangyingyoupin.top

================================================================================
来源：http://hec.0kj1m.cn

P. 常用工具函数
来源：http://cfn.dashuyun.cn

================================================================================
来源：http://rmj.iojbl.cn

[P01] 生成 UUID
来源：http://yzn.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://fpc.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://otg.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://zon.cashguo.top

TS:   crypto.randomUUID()
来源：http://itz.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://tww.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://kyn.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://jhn.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://zxj.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://too.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ljj.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://rwb.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xlh.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wuj.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lpp.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://odk.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vcv.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lwf.iojbl.cn

[P03] 生成短随机字符串
来源：http://agt.xingfuxueyuan.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pbs.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bvw.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rpk.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wby.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sta.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bfp.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://qax.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ugv.xuetiantiany.cn

[P04] 求长度
来源：http://huv.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rpr.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://teq.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smb.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgw.zhoulong.xyz


<!-- 参考信息 -->