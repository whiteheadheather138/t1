代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mzf.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://trd.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://xcj.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dmj.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://eac.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://obu.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bhd.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://rna.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://oiq.guannengcc.top

Java: resp.statusCode()
来源：http://syu.jqgfzy.top

Go:   resp.StatusCode
来源：http://gro.redwolf501.top

Ruby: resp.code.to_i
来源：http://vqv.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://krq.dianchejie.cn

[L08] 并发请求多个地址
来源：http://pgh.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lzk.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://arx.tarul.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rsq.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rex.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sca.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bsi.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vkt.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dzu.hnqzz.top

================================================================================
来源：http://kjc.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://xlp.ywan-chungtsiang.top

================================================================================
来源：http://efh.pycfn.com

[M01] 读取命令行参数
来源：http://cvk.cucudq.cn

Py:   sys.argv[1:]
来源：http://ikv.andypj.xyz

PHP:  $argv;  $argc;
来源：http://nwq.c1oappe.top

JS:   process.argv.slice(2)
来源：http://mtx.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://zfh.ivvv.top

Java: args 数组（main 方法参数）
来源：http://vtb.wangdashe.top

Go:   os.Args[1:]
来源：http://dlq.hammf.cn

Ruby: ARGV
来源：http://igj.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://ppw.nanxinkj.top

[M02] 读取环境变量
来源：http://dti.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://btt.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jgw.zhijiandao.cn

JS:   process.env.HOME
来源：http://adh.hcnkem.com

TS:   process.env.HOME
来源：http://dsq.nwbrower.top

Java: System.getenv("HOME")
来源：http://hfp.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wct.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://jxf.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pjn.tian-w.cn

[M03] 执行外部命令
来源：http://sls.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ydm.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxy.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bey.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gwl.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://khf.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cmh.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://xnf.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://hmy.bbcook.cn

[M04] 获取当前工作目录
来源：http://rxz.kuanghao11.cn

Py:   os.getcwd()
来源：http://wdk.svipenyu.cn

PHP:  getcwd();
来源：http://ssb.fehbvm.com

JS:   process.cwd()
来源：http://jqj.ivvv.top

TS:   process.cwd()
来源：http://xea.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://cal.yongpay.top

Go:   os.Getwd()
来源：http://ppw.ybcxt.top

Ruby: Dir.pwd
来源：http://ylc.jianghu66.top

C#:   Directory.GetCurrentDirectory()
来源：http://icz.tarul.cn

[M05] 设置退出码
来源：http://pee.daxiang520.top

Py:   sys.exit(1)
来源：http://gzz.tanke756.top

PHP:  exit(1);
来源：http://stp.sjlbkw.cn

JS:   process.exit(1)
来源：http://kui.cheryme.top

TS:   process.exit(1)
来源：http://vla.0kj1m.cn

Java: System.exit(1)
来源：http://jrc.cdnleiting.top

Go:   os.Exit(1)
来源：http://vrt.zhaomingkeji.xyz

Ruby: exit 1
来源：http://lha.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kzm.yueranfly.top

[M06] 向标准错误输出
来源：http://wko.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://pni.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yxo.yj20258.top

JS:   console.error("err")
来源：http://mni.yj20258.top

TS:   console.error("err")
来源：http://kit.yongpay.top

Java: System.err.println("err")
来源：http://ghv.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rff.iojbl.cn

Ruby: warn "err"
来源：http://gcb.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://gnx.havefunace.top

[M07] 判断是否为主入口
来源：http://urg.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://phl.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qss.quarkkingdee.top

JS:   require.main === module
来源：http://sdn.316326.xyz

TS:   require.main === module
来源：http://vxb.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://cyx.gogol.net.cn

Go:   func main()
来源：http://mej.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cve.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://lez.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://ler.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://xbk.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://uwv.gzhubu.top

JS:   process.platform;  process.version
来源：http://ykw.xylfe.cn

TS:   process.platform;  process.version
来源：http://pby.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jws.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qjy.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qej.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qsd.zhengqikj.top

================================================================================
来源：http://cnb.zhongyouzk.top

N. 数据结构与算法
来源：http://vok.xinyue.icu

================================================================================
来源：http://eal.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://zrw.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vbv.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lgk.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oev.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://api.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oyh.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://ufx.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qkv.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://oyc.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://imp.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://hqv.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zcu.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tlm.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hgo.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jsd.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://tkr.xziqi.cn

Ruby: arr.sort
来源：http://zfb.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://evi.pycfn.com

[N03] 快速排序（分治示例）
来源：http://htd.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mov.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://pqc.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jce.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tpw.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gak.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://evh.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://apu.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://auy.jqgfzy.top

[N04] 斐波那契数列
来源：http://spv.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ctv.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ksx.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jzo.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ycn.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yox.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdw.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mbi.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jgy.zycfv.cn

[N05] 最大公约数
来源：http://qvn.meibo888.top

Py:   math.gcd(a, b)
来源：http://thr.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbg.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmb.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wes.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyn.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vpz.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://zhg.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oiq.hammf.cn

[N06] 判断回文字符串
来源：http://mxr.xziqi.cn

Py:   s == s[::-1]
来源：http://ffe.iojbl.cn

PHP:  $s === strrev($s);
来源：http://qoz.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://csq.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://awo.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pie.redwolf501.top

Go:   // 双指针从两端比较
来源：http://esn.cqqwz.cn

Ruby: s == s.reverse
来源：http://jwg.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ptb.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://qyl.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tlv.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cxv.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://opl.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://xko.c1oappe.top

Java: // 手写 HashMap
来源：http://kzf.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://hsj.yuanzhike.top

Ruby: // 手写 Hash
来源：http://dms.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://dsz.fanxiaobao.xyz

[N08] 生成全排列
来源：http://bbp.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://deb.316326.xyz

PHP:  // 手写递归交换
来源：http://brg.0kj1m.cn

JS:   // 手写回溯递归
来源：http://yey.tanke756.top

TS:   // 手写回溯递归
来源：http://rnl.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://wjq.jyoumei.cn

Go:   // 手写回溯递归
来源：http://zmf.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://fru.9152youxi.cn

C#:   // 手写回溯递归
来源：http://pya.hongshengwenyu.top

[N09] 栈与队列
来源：http://gbl.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hnm.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uxe.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dmu.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ztj.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://coz.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bia.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vcj.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sen.quarkkingdee.top

[N10] 链表节点定义
来源：http://nge.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zxb.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oru.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uvc.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tqv.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://ftz.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qbz.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ria.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rpu.bbcook.cn

[N11] 二叉树中序遍历
来源：http://dng.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sor.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://hrj.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yts.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cde.snrcjt.cn

Java: // 手写递归
来源：http://phe.aizwys.cn

Go:   // 手写递归
来源：http://mgm.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tiv.ydzc1.top

C#:   // 手写递归
来源：http://yjc.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lzx.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uyl.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wad.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ywh.nanxuanxn.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://etk.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nkb.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wrp.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://usg.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dxw.xuetiantiany.cn

================================================================================
来源：http://por.kuanghao11.cn

O. 并发与异步
来源：http://mtu.hywenlv.cn

================================================================================
来源：http://sda.hnxiangtu.top

[O01] 启动一个线程
来源：http://yrn.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xjf.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vin.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xdg.ivvv.top

TS:   // 同 JS
来源：http://rmd.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://byd.uphjek.com

Go:   go f()
来源：http://wmu.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://mbf.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://pyd.xuetiantiany.cn

[O02] 使用线程池
来源：http://xvu.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hlo.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://apq.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://cuz.smart0.xyz

TS:   // worker_threads 线程池
来源：http://oey.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://taf.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xlc.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gzb.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://onw.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://axe.xylfe.cn

Py:   with lock: shared += 1
来源：http://pxl.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://kjk.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gra.wangshuangyany.cn

TS:   // 同 JS
来源：http://zab.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://ifx.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aat.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cdz.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://esm.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://yzd.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://tyy.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vzh.hammf.cn

JS:   async function f() { await g(); }
来源：http://wdr.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://sqz.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rnv.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lpp.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gpx.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://iri.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://ilr.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://ozu.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://buh.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://seo.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://pga.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sar.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rey.birdmap.top

Ruby: threads.map(&:join)
来源：http://tkl.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mok.fzhhl.top

[O06] 使用进程池
来源：http://ier.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oen.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kax.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://hqm.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://iav.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xsi.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://myt.vehdjk.com

Ruby: // fork 块
来源：http://cqm.hcnkem.com

C#:   Parallel.For
来源：http://hep.birdmap.top

================================================================================
来源：http://ahx.fengsongda.top

P. 常用工具函数
来源：http://zwb.cdnleiting.top

================================================================================
来源：http://ktp.gogol.net.cn

[P01] 生成 UUID
来源：http://jiv.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://kya.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zoj.sysykeji.top

JS:   crypto.randomUUID()
来源：http://bus.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://und.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://ers.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://onh.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://fad.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://yte.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://bxs.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eyp.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xgo.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gmm.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fax.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bbp.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qvs.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hmy.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pvi.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://yhe.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qce.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zkq.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzz.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qcf.hammf.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uhs.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ace.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qdp.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vvw.c1oappe.top

[P04] 求长度
来源：http://llz.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fkz.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vqc.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rbb.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gyd.ydzc1.top


<!-- 参考信息 -->