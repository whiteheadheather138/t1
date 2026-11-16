代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://wyq.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dwy.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zsc.tanke756.top

JS:   resp.ok;  resp.status
来源：http://zvw.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://gdb.epnwcf.com

Java: resp.statusCode()
来源：http://wwf.yj20258888.top

Go:   resp.StatusCode
来源：http://bzz.zdbjq.cn

Ruby: resp.code.to_i
来源：http://bdd.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://qum.havefunace.top

[L08] 并发请求多个地址
来源：http://rha.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vam.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://hyz.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dpd.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iri.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rds.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mno.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://grq.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yej.yj202588.top

================================================================================
来源：http://nde.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://sei.yj20258.top

================================================================================
来源：http://rsd.nwbrower.top

[M01] 读取命令行参数
来源：http://rik.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://mhb.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://gty.hammf.cn

JS:   process.argv.slice(2)
来源：http://kxm.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://ule.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://wii.daria6918.cn

Go:   os.Args[1:]
来源：http://rhj.xuetiantiany.cn

Ruby: ARGV
来源：http://tml.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://tzn.sysykeji.top

[M02] 读取环境变量
来源：http://bca.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://zfa.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lax.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://yvg.chenjidiqi.icu

TS:   process.env.HOME
来源：http://uik.cheryme.top

Java: System.getenv("HOME")
来源：http://cdo.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hev.yj20258888.top

Ruby: ENV["HOME"]
来源：http://olt.tarul.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tdh.birdmap.top

[M03] 执行外部命令
来源：http://hos.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ift.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bfe.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://thy.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dwc.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uph.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dtq.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://piz.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://jgq.yj202588.top

[M04] 获取当前工作目录
来源：http://cuc.snrcjt.cn

Py:   os.getcwd()
来源：http://ouj.aibaodan.cn

PHP:  getcwd();
来源：http://chc.tianlin.xyz

JS:   process.cwd()
来源：http://qay.wangdashe.top

TS:   process.cwd()
来源：http://lsh.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://bzo.fehbvm.com

Go:   os.Getwd()
来源：http://bfv.hfpthk.cn

Ruby: Dir.pwd
来源：http://ljm.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hyf.wangdashe.top

[M05] 设置退出码
来源：http://rve.zhijiandao.cn

Py:   sys.exit(1)
来源：http://mam.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://azc.iojbl.cn

JS:   process.exit(1)
来源：http://zdu.snrcjt.cn

TS:   process.exit(1)
来源：http://unc.shangyingyoupin.top

Java: System.exit(1)
来源：http://aid.shuidangran.top

Go:   os.Exit(1)
来源：http://otu.ydzc1.top

Ruby: exit 1
来源：http://ore.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xix.svipenyu.cn

[M06] 向标准错误输出
来源：http://yfz.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://uoe.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ikw.tianlin.xyz

JS:   console.error("err")
来源：http://ryy.yvedp.cn

TS:   console.error("err")
来源：http://wyt.zhiwuduotai.top

Java: System.err.println("err")
来源：http://web.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bbi.hongshengwenyu.top

Ruby: warn "err"
来源：http://now.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://alv.hfpthk.cn

[M07] 判断是否为主入口
来源：http://vgi.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://xel.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ndc.chenlongwang.top

JS:   require.main === module
来源：http://ckh.52xcode.cn

TS:   require.main === module
来源：http://hvx.hywenlv.cn

Java: public static void main(String[] args)
来源：http://zig.shanyushiyangkeji.top

Go:   func main()
来源：http://ypp.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qwd.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://vea.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://bsv.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://giw.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://gbj.cdnleiting.top

JS:   process.platform;  process.version
来源：http://abn.meibo888.top

TS:   process.platform;  process.version
来源：http://mfw.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tmt.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hxu.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nvc.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dxq.guannengcc.top

================================================================================
来源：http://gmn.yvedp.cn

N. 数据结构与算法
来源：http://asz.0kj1m.cn

================================================================================
来源：http://xcd.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://oud.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://ect.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rlw.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ibx.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://icq.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://yel.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://vce.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://doh.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ldf.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://awb.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://txi.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gok.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aqz.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbr.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gbd.fehbvm.com

Go:   slices.Sort(arr)
来源：http://qsz.hfpthk.cn

Ruby: arr.sort
来源：http://wbt.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zxk.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://kym.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ikn.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://jpc.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipm.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbg.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://umd.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fzs.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gur.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cez.yanxiufei.cn

[N04] 斐波那契数列
来源：http://ddl.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://idr.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wqq.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://udv.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qvd.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://obl.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rvm.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uru.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rtw.wangshuangyany.cn

[N05] 最大公约数
来源：http://usw.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://qkj.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sgp.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nka.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvw.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yai.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nbq.shuidangran.top

Ruby: a.gcd(b)
来源：http://whc.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qlv.52xcode.cn

[N06] 判断回文字符串
来源：http://yvy.yj20258.top

Py:   s == s[::-1]
来源：http://hia.cashguo.top

PHP:  $s === strrev($s);
来源：http://dav.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://kzh.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://bdh.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qqu.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://xus.jiagoushi.top

Ruby: s == s.reverse
来源：http://nyc.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zfx.uphjek.com

[N07] 两数之和（返回下标）
来源：http://vxk.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wue.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dxf.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ufo.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://tjh.hesvh.cn

Java: // 手写 HashMap
来源：http://nfp.cheryme.top

Go:   // 手写 map[int]int
来源：http://egt.ivvv.top

Ruby: // 手写 Hash
来源：http://pcb.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://gpu.shangyingyoupin.top

[N08] 生成全排列
来源：http://tsz.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://qef.gzhubu.top

PHP:  // 手写递归交换
来源：http://skq.birdmap.top

JS:   // 手写回溯递归
来源：http://lvb.yangfankeji.com

TS:   // 手写回溯递归
来源：http://gxh.xinyue.icu

Java: // 手写回溯递归
来源：http://nqw.tianlin.xyz

Go:   // 手写回溯递归
来源：http://shs.tanke756.top

Ruby: arr.permutation.to_a
来源：http://bvz.jinqigufen.top

C#:   // 手写回溯递归
来源：http://bkj.guowangkeji.top

[N09] 栈与队列
来源：http://wtp.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nfh.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://inb.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lvi.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qkk.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://beo.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hwb.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qbe.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zup.gogol.net.cn

[N10] 链表节点定义
来源：http://jnf.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mch.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zry.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rit.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://deo.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://sww.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://wqk.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uyj.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ygp.yonumen.top

[N11] 二叉树中序遍历
来源：http://eoz.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kie.xziqi.cn

PHP:  // 手写递归函数
来源：http://pbj.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lzw.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tdj.feifeiyinyue.top

Java: // 手写递归
来源：http://tef.yj20258888.top

Go:   // 手写递归
来源：http://nhi.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdx.fzhhl.top

C#:   // 手写递归
来源：http://vmz.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kgx.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://agu.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://prf.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dka.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vsp.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rwr.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gai.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fkv.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rul.aizwys.cn

================================================================================
来源：http://bcr.chenlongwang.top

O. 并发与异步
来源：http://dfq.ivvv.top

================================================================================
来源：http://rst.aibaodan.cn

[O01] 启动一个线程
来源：http://hvz.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgm.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://juc.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ohj.jlsjyb.cn

TS:   // 同 JS
来源：http://cav.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://dwj.sweek.top

Go:   go f()
来源：http://kag.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://wsv.sweek.top

C#:   Task.Run(() => F());
来源：http://vdb.daxiang520.top

[O02] 使用线程池
来源：http://lpo.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gqj.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gqy.xziqi.cn

JS:   // worker_threads 线程池
来源：http://iys.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://usa.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://std.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ycr.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://znm.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zos.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://ccc.cqqwz.cn

Py:   with lock: shared += 1
来源：http://xji.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://evv.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eus.uphjek.com

TS:   // 同 JS
来源：http://jfe.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://tuf.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fjx.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mso.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://bow.tarul.cn

[O04] 定义异步函数并等待
来源：http://pyr.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://lcq.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jck.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://ewx.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iph.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tpu.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sys.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://icj.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://wob.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://mtw.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://esx.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://koe.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://gjm.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://bjl.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mqr.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://teh.xylfe.cn

Ruby: threads.map(&:join)
来源：http://cks.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yid.sweek.top

[O06] 使用进程池
来源：http://qpw.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://muj.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oll.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://hwj.cheryme.top

TS:   // child_process / cluster 模块
来源：http://uoa.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qtj.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iux.hysaishi.cn

Ruby: // fork 块
来源：http://yzc.yfazqb.com

C#:   Parallel.For
来源：http://trm.cheryme.top

================================================================================
来源：http://alv.chenzaomai.com

P. 常用工具函数
来源：http://mnc.yonumen.top

================================================================================
来源：http://fdh.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://sum.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://ked.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eau.wangdashe.top

JS:   crypto.randomUUID()
来源：http://xxr.fehbvm.com

TS:   crypto.randomUUID()
来源：http://dps.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://odm.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://ezh.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://vms.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://zqf.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://xln.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eri.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sde.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vrc.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kqf.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pmr.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qal.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mjl.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uax.yj20258.top

[P03] 生成短随机字符串
来源：http://kxn.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://din.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xrs.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wbz.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tqs.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jcc.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lrx.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://uax.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://olh.birdmap.top

[P04] 求长度
来源：http://dtw.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://txc.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://icy.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dok.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvn.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://psw.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://zpk.pycfn.com

Ruby: x.length;  x.size
来源：http://eku.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://twf.nanxuanxn.top


<!-- 参考信息 -->