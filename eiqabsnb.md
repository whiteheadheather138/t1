代发 wailian999

Py:   resp.json()
来源：http://pdq.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://ald.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://ros.epnwcf.com

TS:   await resp.json()
来源：http://nkb.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jyv.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tyh.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://cqi.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zyo.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://psj.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fdx.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jku.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://ezl.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://oai.cucudq.cn

Java: resp.statusCode()
来源：http://mzp.fzhhl.top

Go:   resp.StatusCode
来源：http://vdy.jinqigufen.top

Ruby: resp.code.to_i
来源：http://zdg.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://bbu.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://mkv.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tbr.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://dgp.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ubg.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqd.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://byu.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bbl.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rdv.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qzn.zhaomingkeji.xyz

================================================================================
来源：http://xqy.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://sax.snrcjt.cn

================================================================================
来源：http://cri.yuxming.cn

[M01] 读取命令行参数
来源：http://otw.smart0.xyz

Py:   sys.argv[1:]
来源：http://qni.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://tqc.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://svl.fehbvm.com

TS:   process.argv.slice(2)
来源：http://nfl.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://mhu.daxiang520.top

Go:   os.Args[1:]
来源：http://dea.xziqi.cn

Ruby: ARGV
来源：http://goe.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://pyp.fengsongda.top

[M02] 读取环境变量
来源：http://muh.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://jxy.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sdc.jqgufenzy.top

JS:   process.env.HOME
来源：http://kdo.52xcode.cn

TS:   process.env.HOME
来源：http://gtl.fehbvm.com

Java: System.getenv("HOME")
来源：http://edn.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://umz.52xcode.cn

Ruby: ENV["HOME"]
来源：http://doi.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://szk.pycfn.com

[M03] 执行外部命令
来源：http://dma.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nel.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qfw.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qtf.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lxg.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gpd.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://xij.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://fkd.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://ygc.haohaochexian.top

[M04] 获取当前工作目录
来源：http://eis.jiagoushi.top

Py:   os.getcwd()
来源：http://nht.guowangkeji.top

PHP:  getcwd();
来源：http://cdh.ctjpmb.com

JS:   process.cwd()
来源：http://osb.aizwys.cn

TS:   process.cwd()
来源：http://bxd.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://qxe.yangfankeji.com

Go:   os.Getwd()
来源：http://tex.jianghu66.top

Ruby: Dir.pwd
来源：http://fxi.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://iye.iojbl.cn

[M05] 设置退出码
来源：http://ovc.yfazqb.com

Py:   sys.exit(1)
来源：http://pjs.vehdjk.com

PHP:  exit(1);
来源：http://qyg.ydjk.org.cn

JS:   process.exit(1)
来源：http://ymt.c1oappe.top

TS:   process.exit(1)
来源：http://psx.jinqigufen.top

Java: System.exit(1)
来源：http://ljo.havefunace.top

Go:   os.Exit(1)
来源：http://vpe.fanxiaobao.xyz

Ruby: exit 1
来源：http://jqx.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fvk.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://dqy.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://unk.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rot.cdnleiting.top

JS:   console.error("err")
来源：http://kee.haohaochexian.top

TS:   console.error("err")
来源：http://cwv.zhiwuduotai.top

Java: System.err.println("err")
来源：http://zqf.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://epp.tanke756.top

Ruby: warn "err"
来源：http://mpj.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://dif.hammf.cn

[M07] 判断是否为主入口
来源：http://lmo.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://naz.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://emj.birdmap.top

JS:   require.main === module
来源：http://bxk.sxryk.cn

TS:   require.main === module
来源：http://xox.jianghu66.top

Java: public static void main(String[] args)
来源：http://rei.aizwys.cn

Go:   func main()
来源：http://jsm.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qet.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://ryr.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://ykm.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://ysv.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://fiy.hysaishi.cn

JS:   process.platform;  process.version
来源：http://yoc.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://sls.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zou.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://isa.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gzd.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ueh.shanyushiyangtech.top

================================================================================
来源：http://dtu.cucudq.cn

N. 数据结构与算法
来源：http://rag.yueranfly.top

================================================================================
来源：http://eqs.uphjek.com

[N01] 二分查找（有序数组）
来源：http://xad.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rmv.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://diy.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nkx.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opq.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://dok.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://sno.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://atd.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gqn.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://aec.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://xti.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nbg.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nzr.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://akv.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rxn.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://zkp.zhengqikj.top

Ruby: arr.sort
来源：http://ash.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qty.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://gdk.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iwc.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://ntt.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqe.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gsk.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qto.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aff.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qex.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aqw.tianlin.xyz

[N04] 斐波那契数列
来源：http://ojx.xinyue.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://syn.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qus.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aqm.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vli.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lqm.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bmb.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ovh.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xge.xylfe.cn

[N05] 最大公约数
来源：http://qkd.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://ocv.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wvg.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jfg.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ehm.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dbr.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iko.ybcxt.top

Ruby: a.gcd(b)
来源：http://ncg.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rvt.uphjek.com

[N06] 判断回文字符串
来源：http://wky.jinqigfzy.top

Py:   s == s[::-1]
来源：http://wdd.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://mah.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://wrg.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://bja.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fwa.hesvh.cn

Go:   // 双指针从两端比较
来源：http://tpl.chenzaomai.com

Ruby: s == s.reverse
来源：http://ckn.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mdw.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://ipc.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdt.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aib.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sjx.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://xqv.9152youxi.cn

Java: // 手写 HashMap
来源：http://eih.hnqzz.top

Go:   // 手写 map[int]int
来源：http://jve.yueranfly.top

Ruby: // 手写 Hash
来源：http://vwt.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://tmc.9152youxi.cn

[N08] 生成全排列
来源：http://iww.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://wkn.tianlin.xyz

PHP:  // 手写递归交换
来源：http://axh.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://csd.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://shr.yvedp.cn

Java: // 手写回溯递归
来源：http://dox.wangdashe.top

Go:   // 手写回溯递归
来源：http://kfs.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://pvj.redwolf501.top

C#:   // 手写回溯递归
来源：http://hlb.yuanzhike.top

[N09] 栈与队列
来源：http://haz.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zwa.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yri.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eeg.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xyh.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sjq.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lph.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://enu.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hss.tanke756.top

[N10] 链表节点定义
来源：http://dqe.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsg.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uqa.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://idt.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kfq.zhaomingkeji.xyz

Java: class Node { int v; Node next; }
来源：http://dja.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pkc.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ede.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ums.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://ati.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://joq.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://wtu.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffb.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxi.daxiang520.top

Java: // 手写递归
来源：http://aez.jinqigfzy.top

Go:   // 手写递归
来源：http://bdd.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ikh.hammf.cn

C#:   // 手写递归
来源：http://afx.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cbi.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rda.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ofs.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://spa.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xtg.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cdo.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://siq.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zno.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uyc.xingfuxueyuan.xyz

================================================================================
来源：http://inr.sxryk.cn

O. 并发与异步
来源：http://emm.gaohongyu789.top

================================================================================
来源：http://aci.wangshuangyany.cn

[O01] 启动一个线程
来源：http://ysd.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qiu.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://izl.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ssp.dashuyun.cn

TS:   // 同 JS
来源：http://znl.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://juv.yanxiufei.cn

Go:   go f()
来源：http://mpr.nwbrower.top

Ruby: Thread.new { f }
来源：http://nbo.tanke756.top

C#:   Task.Run(() => F());
来源：http://jje.wangshuangyany.cn

[O02] 使用线程池
来源：http://wxt.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qba.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vab.fehbvm.com

JS:   // worker_threads 线程池
来源：http://ofc.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://rhc.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://uyp.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fei.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://llp.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mxc.daxiang520.top

[O03] 加锁保护共享数据
来源：http://fck.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://fwo.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://dnd.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zwj.xinyue.icu

TS:   // 同 JS
来源：http://xrp.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://syk.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zoo.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://txk.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://eau.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://eco.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://wra.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://inn.pycfn.com

JS:   async function f() { await g(); }
来源：http://yvq.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zga.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jlg.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mmn.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://kiv.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://vyt.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://nsw.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://hwb.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mmq.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://hws.meibo888.top

TS:   await Promise.all(tasks)
来源：http://zjh.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://far.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://buv.meibo888.top

Ruby: threads.map(&:join)
来源：http://eey.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mcx.cashguo.top

[O06] 使用进程池
来源：http://qok.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gzi.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fzy.yonumen.top

JS:   // child_process / cluster 模块
来源：http://rmc.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://nkd.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ccj.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iqd.ybcxt.top

Ruby: // fork 块
来源：http://ttg.zhixingplan.top

C#:   Parallel.For
来源：http://thh.iojbl.cn

================================================================================
来源：http://frd.aibaodan.cn

P. 常用工具函数
来源：http://lil.daria6918.cn

================================================================================
来源：http://ulw.hysaishi.cn

[P01] 生成 UUID
来源：http://stc.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://imc.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mrd.xziqi.cn

JS:   crypto.randomUUID()
来源：http://mrz.xziqi.cn

TS:   crypto.randomUUID()
来源：http://uni.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://arb.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://erv.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://gni.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://ppp.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://kio.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lld.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://unh.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bde.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iab.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ucp.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vdp.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mzy.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xad.tian-w.cn

[P03] 生成短随机字符串
来源：http://ecs.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://apz.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://klt.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mku.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rkl.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vtq.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gro.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://umh.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ali.aizwys.cn

[P04] 求长度
来源：http://qfl.fzhhl.top


<!-- 参考信息 -->