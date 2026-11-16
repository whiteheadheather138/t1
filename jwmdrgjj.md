代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://npa.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ifb.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dfx.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://edl.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://cbz.ehwqpu.com

Java: resp.statusCode()
来源：http://bec.snrcjt.cn

Go:   resp.StatusCode
来源：http://yip.ydzc1.top

Ruby: resp.code.to_i
来源：http://rkv.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://uac.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://skq.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rur.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://irj.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrr.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rid.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xvl.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gdg.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cet.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fww.jqgfzy.top

================================================================================
来源：http://zsi.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://kgl.hammf.cn

================================================================================
来源：http://dpz.sufxvd.cn

[M01] 读取命令行参数
来源：http://yxz.iojbl.cn

Py:   sys.argv[1:]
来源：http://vnl.fehbvm.com

PHP:  $argv;  $argc;
来源：http://mfu.hcnkem.com

JS:   process.argv.slice(2)
来源：http://cmf.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://cco.cashguo.top

Java: args 数组（main 方法参数）
来源：http://gzy.xylfe.cn

Go:   os.Args[1:]
来源：http://kqz.ybcxt.top

Ruby: ARGV
来源：http://mhf.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://szh.yj20258888.top

[M02] 读取环境变量
来源：http://gll.yongpay.top

Py:   os.environ.get("HOME")
来源：http://day.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gdg.yfazqb.com

JS:   process.env.HOME
来源：http://hwb.wangshuangyany.cn

TS:   process.env.HOME
来源：http://bvo.zdqjudy.top

Java: System.getenv("HOME")
来源：http://znx.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yjz.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://hvs.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xmj.fktsv.cn

[M03] 执行外部命令
来源：http://ndo.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lpo.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mhn.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zed.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://buj.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gvx.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ycm.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fts.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://glb.wangdashe.top

[M04] 获取当前工作目录
来源：http://utm.birdmap.top

Py:   os.getcwd()
来源：http://veh.xziqi.cn

PHP:  getcwd();
来源：http://cxd.birdmap.top

JS:   process.cwd()
来源：http://pnc.zhengqikj.top

TS:   process.cwd()
来源：http://ofc.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://evd.feifeiyinyue.top

Go:   os.Getwd()
来源：http://rzs.andypj.xyz

Ruby: Dir.pwd
来源：http://kdg.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://qya.meibo888.top

[M05] 设置退出码
来源：http://ixb.cucudq.cn

Py:   sys.exit(1)
来源：http://rdj.dianchejie.cn

PHP:  exit(1);
来源：http://zwg.wangshuangyany.cn

JS:   process.exit(1)
来源：http://xnv.smart0.xyz

TS:   process.exit(1)
来源：http://bll.zhiwuduotai.top

Java: System.exit(1)
来源：http://vov.dashuyun.cn

Go:   os.Exit(1)
来源：http://itz.aizwys.cn

Ruby: exit 1
来源：http://rho.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dpq.316326.xyz

[M06] 向标准错误输出
来源：http://nks.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://jmk.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ocd.quarkkingdee.top

JS:   console.error("err")
来源：http://mrb.dianchejie.cn

TS:   console.error("err")
来源：http://edr.c1oappe.top

Java: System.err.println("err")
来源：http://uxe.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qfw.nwbrower.top

Ruby: warn "err"
来源：http://sss.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://ygl.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://dvi.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://oav.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tgj.nwbrower.top

JS:   require.main === module
来源：http://jtc.hesvh.cn

TS:   require.main === module
来源：http://uni.gotoacloud.top

Java: public static void main(String[] args)
来源：http://gwj.sufxvd.cn

Go:   func main()
来源：http://wgp.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://soa.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://fjy.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://lju.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://tef.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://ahk.cdnleiting.top

JS:   process.platform;  process.version
来源：http://lzt.gogol.net.cn

TS:   process.platform;  process.version
来源：http://azh.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lbb.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tcm.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://igx.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nvv.gogol.net.cn

================================================================================
来源：http://ogv.zhongyouzk.top

N. 数据结构与算法
来源：http://wht.yj20258888.top

================================================================================
来源：http://lxm.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://rma.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://hxd.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qgn.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wig.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tva.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ytr.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://ahd.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vzk.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rgk.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://eui.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://qrm.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ott.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dcm.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fuv.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://agu.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://rco.cqqwz.cn

Ruby: arr.sort
来源：http://gad.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vow.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://yzp.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ihk.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://egz.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgb.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zad.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zuk.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bhs.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://udb.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://uye.ydzc1.top

[N04] 斐波那契数列
来源：http://alc.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uaa.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gua.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://srg.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xks.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ljc.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hat.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aje.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gpz.quarkkingdee.top

[N05] 最大公约数
来源：http://wmb.sysykeji.top

Py:   math.gcd(a, b)
来源：http://iya.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dgq.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vvd.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lpk.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yfu.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fea.ctjpmb.com

Ruby: a.gcd(b)
来源：http://vbw.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iok.dashuyun.cn

[N06] 判断回文字符串
来源：http://fzx.hywenlv.cn

Py:   s == s[::-1]
来源：http://gwh.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://afs.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://iql.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://efd.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://igm.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://qsj.redwolf501.top

Ruby: s == s.reverse
来源：http://bhn.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mef.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://dxs.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lyg.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ydb.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hcn.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://izn.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://lcd.xziqi.cn

Go:   // 手写 map[int]int
来源：http://mbt.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://oln.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://xug.xinyue.icu

[N08] 生成全排列
来源：http://dle.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://isn.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://awf.yvedp.cn

JS:   // 手写回溯递归
来源：http://dxn.zdbjq.cn

TS:   // 手写回溯递归
来源：http://yip.fehbvm.com

Java: // 手写回溯递归
来源：http://gzf.vehdjk.com

Go:   // 手写回溯递归
来源：http://iou.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://era.hnqzz.top

C#:   // 手写回溯递归
来源：http://zxn.ivvv.top

[N09] 栈与队列
来源：http://oqk.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://imf.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nyh.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nki.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://krf.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bzl.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://niz.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ado.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://efx.jqgfzy.top

[N10] 链表节点定义
来源：http://mia.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qod.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yup.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://izm.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iam.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://exe.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://nku.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://miw.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://aor.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://kvx.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kuf.yangfankeji.com

PHP:  // 手写递归函数
来源：http://zyd.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hdu.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psc.jqgufenzy.top

Java: // 手写递归
来源：http://fkj.fktsv.cn

Go:   // 手写递归
来源：http://chk.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ofl.pycfn.com

C#:   // 手写递归
来源：http://pmm.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://htx.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mhw.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gia.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qgr.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fep.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aqx.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ymq.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pml.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jcw.aibaodan.cn

================================================================================
来源：http://ukd.chenzaomai.com

O. 并发与异步
来源：http://isa.feifeiyinyue.top

================================================================================
来源：http://lnt.yuxming.cn

[O01] 启动一个线程
来源：http://asd.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blj.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bcd.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rmv.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://fdd.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://bcm.yanxiufei.cn

Go:   go f()
来源：http://aog.zhixingplan.top

Ruby: Thread.new { f }
来源：http://oug.ivvv.top

C#:   Task.Run(() => F());
来源：http://der.epnwcf.com

[O02] 使用线程池
来源：http://prw.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vyb.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://osv.daxiang520.top

JS:   // worker_threads 线程池
来源：http://nhg.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://udy.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://axz.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lke.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xif.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://efc.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://rhr.ctjpmb.com

Py:   with lock: shared += 1
来源：http://fqb.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://qjx.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jsh.ivvv.top

TS:   // 同 JS
来源：http://ssw.sxryk.cn

Java: synchronized (this) { shared++; }
来源：http://ywe.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sdc.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wto.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://fzp.yvedp.cn

[O04] 定义异步函数并等待
来源：http://kxo.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://dss.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aqr.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://ylq.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cqm.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mne.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wag.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://dfh.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://yaj.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://syv.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://mfr.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ept.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://jcg.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://pln.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lzh.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://epg.52xcode.cn

Ruby: threads.map(&:join)
来源：http://ybp.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ssy.wangdashe.top

[O06] 使用进程池
来源：http://dvw.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yji.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fsk.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://aig.316326.xyz

TS:   // child_process / cluster 模块
来源：http://jgh.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ckz.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fll.ehwqpu.com

Ruby: // fork 块
来源：http://bgn.zhongyouzk.top

C#:   Parallel.For
来源：http://fal.ybcxt.top

================================================================================
来源：http://iik.shanyushiyangkeji.top

P. 常用工具函数
来源：http://ujy.jqgfzy.top

================================================================================
来源：http://zsf.ppjwa.cn

[P01] 生成 UUID
来源：http://izx.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://naj.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ksq.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://stp.tanke756.top

TS:   crypto.randomUUID()
来源：http://ufg.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://tay.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://zuf.yongpay.top

Ruby: SecureRandom.uuid
来源：http://szx.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://gsp.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://rnp.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mqe.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mhi.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qdz.xingfuxueyuan.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vhn.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lce.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bvv.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tmz.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://loy.hfpthk.cn

[P03] 生成短随机字符串
来源：http://frc.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ruw.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cpb.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kuk.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eqk.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ubw.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rpx.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ksg.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sbt.yangfankeji.com

[P04] 求长度
来源：http://jqs.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iud.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vht.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nmx.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfy.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://lgw.fengsongda.top

Go:   len(arr);  len(m)
来源：http://unr.ehwqpu.com

Ruby: x.length;  x.size
来源：http://bmi.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dra.vqdsnc.cn


<!-- 参考信息 -->