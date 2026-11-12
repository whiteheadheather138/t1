代发 wailian999

TS:   resp.ok;  resp.status
来源：http://pvw.ybcxt.top

Java: resp.statusCode()
来源：http://oqj.yongpay.top

Go:   resp.StatusCode
来源：http://ijn.yongpay.top

Ruby: resp.code.to_i
来源：http://zpc.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://zld.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://dnf.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nfk.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://dpz.sysykeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qxu.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ota.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zfi.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dgz.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fmw.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://coq.nanxuanxn.top

================================================================================
来源：http://jxz.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://ddg.yuanzhike.top

================================================================================
来源：http://kyd.zhoulong.xyz

[M01] 读取命令行参数
来源：http://ybu.sweek.top

Py:   sys.argv[1:]
来源：http://iwt.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://abx.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://zjo.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://vnl.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://wfi.yuanzhike.top

Go:   os.Args[1:]
来源：http://zbb.fehbvm.com

Ruby: ARGV
来源：http://cqn.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://col.jianghu66.top

[M02] 读取环境变量
来源：http://fmu.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://wmp.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://arv.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://fun.zhijiandao.cn

TS:   process.env.HOME
来源：http://qze.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://wga.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dzj.c1oappe.top

Ruby: ENV["HOME"]
来源：http://ycp.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mfy.gzhubu.top

[M03] 执行外部命令
来源：http://vgv.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pma.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ryh.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bdt.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hwj.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mfh.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ihp.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://yuw.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://vzh.pycfn.com

[M04] 获取当前工作目录
来源：http://znz.zycfv.cn

Py:   os.getcwd()
来源：http://ukw.jianghu66.top

PHP:  getcwd();
来源：http://kxt.zhixingplan.top

JS:   process.cwd()
来源：http://hql.jqgufenzy.top

TS:   process.cwd()
来源：http://uqj.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://vfr.ctjpmb.com

Go:   os.Getwd()
来源：http://jtx.yj20258888.top

Ruby: Dir.pwd
来源：http://qsh.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://umi.guowangkeji.top

[M05] 设置退出码
来源：http://yku.yuanzhike.top

Py:   sys.exit(1)
来源：http://edt.sufxvd.cn

PHP:  exit(1);
来源：http://jiw.andypj.xyz

JS:   process.exit(1)
来源：http://gbf.fktsv.cn

TS:   process.exit(1)
来源：http://ejs.epnwcf.com

Java: System.exit(1)
来源：http://zhk.zhoulong.xyz

Go:   os.Exit(1)
来源：http://uxi.xylfe.cn

Ruby: exit 1
来源：http://yet.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cdk.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://xsk.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://wws.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bua.sweek.top

JS:   console.error("err")
来源：http://jkl.snrcjt.cn

TS:   console.error("err")
来源：http://thr.redwolf501.top

Java: System.err.println("err")
来源：http://stf.zhaomingkeji.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uws.quarkkingdee.top

Ruby: warn "err"
来源：http://vvo.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://otr.gzhubu.top

[M07] 判断是否为主入口
来源：http://tik.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://ljk.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yok.gzhubu.top

JS:   require.main === module
来源：http://dtp.daria6918.cn

TS:   require.main === module
来源：http://fck.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://tiy.shanyushiyangtech.top

Go:   func main()
来源：http://pmr.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sjr.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://hag.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://qdz.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://aff.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://kgb.dianchejie.cn

JS:   process.platform;  process.version
来源：http://amh.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://hjm.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zzx.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ifg.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lbk.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dhp.daxiang520.top

================================================================================
来源：http://gzg.fengsongda.top

N. 数据结构与算法
来源：http://yey.fktsv.cn

================================================================================
来源：http://hmj.yj20258.top

[N01] 二分查找（有序数组）
来源：http://bqh.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://kbh.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mbl.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ijt.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://suk.xziqi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rhx.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://oqb.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wzx.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://iui.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://clg.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://bzd.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eum.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tmc.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fqc.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yjx.fktsv.cn

Go:   slices.Sort(arr)
来源：http://zzn.tarul.cn

Ruby: arr.sort
来源：http://mwl.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hgw.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://mis.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qpu.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://xli.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ade.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unq.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://haz.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eqo.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ofs.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://qfw.tarul.cn

[N04] 斐波那契数列
来源：http://sze.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fcc.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uva.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xna.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vsy.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pnu.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gzy.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://svn.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aeu.mhx1999.top

[N05] 最大公约数
来源：http://qib.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://iek.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gmp.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yxv.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ywt.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hfd.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tqf.hammf.cn

Ruby: a.gcd(b)
来源：http://apx.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://whs.yangfankeji.com

[N06] 判断回文字符串
来源：http://mes.zhongyouzk.top

Py:   s == s[::-1]
来源：http://aur.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://bvc.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://edz.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://nlw.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uwc.tarul.cn

Go:   // 双指针从两端比较
来源：http://xlm.chenzaomai.com

Ruby: s == s.reverse
来源：http://gfb.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qpp.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://nhf.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tqr.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qma.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ufc.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://baa.daxiang520.top

Java: // 手写 HashMap
来源：http://lqb.xuanzx.com

Go:   // 手写 map[int]int
来源：http://gax.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://lrk.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qge.redwolf501.top

[N08] 生成全排列
来源：http://neq.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://awt.hnqzz.top

PHP:  // 手写递归交换
来源：http://ovx.snrcjt.cn

JS:   // 手写回溯递归
来源：http://qwb.gogol.net.cn

TS:   // 手写回溯递归
来源：http://bbx.redwolf501.top

Java: // 手写回溯递归
来源：http://rvm.daxiang520.top

Go:   // 手写回溯递归
来源：http://trz.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://khe.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://yfs.cheryme.top

[N09] 栈与队列
来源：http://qsw.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jwr.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uyg.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://txl.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vaa.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vwi.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hwu.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lke.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aqj.ehwqpu.com

[N10] 链表节点定义
来源：http://aun.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cjn.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://qli.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iqa.yj202588.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gyf.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://bpj.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tru.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pbb.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ovc.meibo888.top

[N11] 二叉树中序遍历
来源：http://dgb.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lgy.cqqwz.cn

PHP:  // 手写递归函数
来源：http://bsh.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fhz.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxg.hfpthk.cn

Java: // 手写递归
来源：http://zwc.sweek.top

Go:   // 手写递归
来源：http://vys.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vaz.jiagoushi.top

C#:   // 手写递归
来源：http://mac.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://skv.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aev.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hlh.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vik.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffd.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dfr.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rsi.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hry.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cct.daxiang520.top

================================================================================
来源：http://tpz.shzxlz.cn

O. 并发与异步
来源：http://den.epnwcf.com

================================================================================
来源：http://htc.gogol.net.cn

[O01] 启动一个线程
来源：http://dqd.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xxd.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lol.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xhi.yuanzhike.top

TS:   // 同 JS
来源：http://zsf.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://zac.tianlin.xyz

Go:   go f()
来源：http://hkd.iojbl.cn

Ruby: Thread.new { f }
来源：http://yqg.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://rem.xuetiantiany.cn

[O02] 使用线程池
来源：http://emf.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ikk.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gkx.jianghu66.top

JS:   // worker_threads 线程池
来源：http://cfs.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://cbu.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://muh.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xlc.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lae.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mpe.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://xux.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://sua.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://qld.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://omw.haohaochexian.top

TS:   // 同 JS
来源：http://jjb.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://abd.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://faz.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tvv.jyoumei.cn

C#:   lock (gate) { shared++; }
来源：http://sxk.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://fla.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://fzv.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jug.xinyue.icu

JS:   async function f() { await g(); }
来源：http://pue.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ndx.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nvd.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bam.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://rxb.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://rks.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://dnw.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://fxj.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yac.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://xuf.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://jgq.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jqr.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bmj.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://flp.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://api.pengpengdd.cyou

[O06] 使用进程池
来源：http://khg.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fuy.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://itj.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://bjq.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://nrb.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hps.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nwe.gogol.net.cn

Ruby: // fork 块
来源：http://emy.tanke756.top

C#:   Parallel.For
来源：http://oyg.hywenlv.cn

================================================================================
来源：http://hag.svipenyu.cn

P. 常用工具函数
来源：http://wet.shzxlz.cn

================================================================================
来源：http://osh.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://hqw.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://wwe.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xmp.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://svz.shuidangran.top

TS:   crypto.randomUUID()
来源：http://pnb.sweek.top

Java: UUID.randomUUID().toString()
来源：http://ogy.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://xgy.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://tdp.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://tjx.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://ltj.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fyg.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hcw.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nlf.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kau.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gom.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://onn.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fjl.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jfp.9152youxi.cn

[P03] 生成短随机字符串
来源：http://qpe.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jfy.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wan.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://byh.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vvc.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oxh.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fak.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://dru.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bzz.yanxiufei.cn

[P04] 求长度
来源：http://kxt.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zwo.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dok.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rgn.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jbh.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://rah.fktsv.cn

Go:   len(arr);  len(m)
来源：http://kqd.xylfe.cn

Ruby: x.length;  x.size
来源：http://cxs.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://etz.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://zlq.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ggl.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yws.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ppj.chenjidiqi.icu


<!-- 参考信息 -->