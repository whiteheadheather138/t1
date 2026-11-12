代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://klj.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lvj.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://cwx.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fcs.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://hjd.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://maz.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hpu.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://las.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://tbo.ppjwa.cn

Java: resp.statusCode()
来源：http://qrp.vehdjk.com

Go:   resp.StatusCode
来源：http://brj.hysaishi.cn

Ruby: resp.code.to_i
来源：http://hci.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://brt.c1oappe.top

[L08] 并发请求多个地址
来源：http://upf.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ked.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://oaw.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zef.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nfk.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://phi.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wmz.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dlt.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mck.bbcook.cn

================================================================================
来源：http://slt.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://gho.hysaishi.cn

================================================================================
来源：http://kxh.sjlbkw.cn

[M01] 读取命令行参数
来源：http://wxq.ppjwa.cn

Py:   sys.argv[1:]
来源：http://zgi.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://rev.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://qiw.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://mef.uphjek.com

Java: args 数组（main 方法参数）
来源：http://evi.bjfxy.top

Go:   os.Args[1:]
来源：http://rhb.cdnleiting.top

Ruby: ARGV
来源：http://lyn.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://bkn.guowangkeji.top

[M02] 读取环境变量
来源：http://tko.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://dsq.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jwl.cheryme.top

JS:   process.env.HOME
来源：http://ili.316326.xyz

TS:   process.env.HOME
来源：http://vzu.fengsongda.top

Java: System.getenv("HOME")
来源：http://cxv.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rns.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://wek.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bdb.yongpay.top

[M03] 执行外部命令
来源：http://ssm.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xmw.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yze.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nfo.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lem.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tpm.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fnw.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://wyc.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://mby.yongpay.top

[M04] 获取当前工作目录
来源：http://jbx.yvedp.cn

Py:   os.getcwd()
来源：http://rdb.zhengqikj.top

PHP:  getcwd();
来源：http://uei.0kj1m.cn

JS:   process.cwd()
来源：http://mku.0kj1m.cn

TS:   process.cwd()
来源：http://uye.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://xah.hfpthk.cn

Go:   os.Getwd()
来源：http://nwl.tanke756.top

Ruby: Dir.pwd
来源：http://pzz.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://lxk.cucudq.cn

[M05] 设置退出码
来源：http://rbm.smart0.xyz

Py:   sys.exit(1)
来源：http://rll.hfpthk.cn

PHP:  exit(1);
来源：http://dyk.xylfe.cn

JS:   process.exit(1)
来源：http://mua.yj202588.top

TS:   process.exit(1)
来源：http://syh.uphjek.com

Java: System.exit(1)
来源：http://fdc.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://rmc.gzhubu.top

Ruby: exit 1
来源：http://cwn.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fvg.fehbvm.com

[M06] 向标准错误输出
来源：http://ykh.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://mdx.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://upm.fehbvm.com

JS:   console.error("err")
来源：http://mlq.cheryme.top

TS:   console.error("err")
来源：http://smw.xziqi.cn

Java: System.err.println("err")
来源：http://mtc.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zgd.yj20258.top

Ruby: warn "err"
来源：http://byl.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://wgd.xinyue.icu

[M07] 判断是否为主入口
来源：http://bef.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://jvr.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://izp.mhx1999.top

JS:   require.main === module
来源：http://cfq.vehdjk.com

TS:   require.main === module
来源：http://ywe.xziqi.cn

Java: public static void main(String[] args)
来源：http://mcn.havefunace.top

Go:   func main()
来源：http://skp.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://euv.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://noj.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://ydm.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://pjl.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://wab.316326.xyz

JS:   process.platform;  process.version
来源：http://hai.hesvh.cn

TS:   process.platform;  process.version
来源：http://klo.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mgz.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tpi.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eak.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mxv.jinqigfzy.top

================================================================================
来源：http://vyd.pycfn.com

N. 数据结构与算法
来源：http://hlj.hammf.cn

================================================================================
来源：http://hgc.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://tpl.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://jlo.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yda.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xxs.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cxg.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://ysr.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://ptt.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ijx.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tfb.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://hqu.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://aak.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bzj.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ece.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ayd.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://osd.uphjek.com

Go:   slices.Sort(arr)
来源：http://vxe.hesvh.cn

Ruby: arr.sort
来源：http://ksg.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ang.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://roa.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nri.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://wuf.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kjo.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ads.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://upp.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://srp.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pcn.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://exc.aibaodan.cn

[N04] 斐波那契数列
来源：http://buy.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://how.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kpn.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tas.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnp.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uec.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://shj.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mor.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tyu.yongpay.top

[N05] 最大公约数
来源：http://oqr.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://yiz.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wza.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idt.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://myc.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vgc.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tis.daria6918.cn

Ruby: a.gcd(b)
来源：http://bai.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qbu.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://agp.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://lpr.yonumen.top

PHP:  $s === strrev($s);
来源：http://exf.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://xqu.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://qyc.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://add.tarul.cn

Go:   // 双指针从两端比较
来源：http://hzy.9152youxi.cn

Ruby: s == s.reverse
来源：http://jmz.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fvv.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://cwm.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tnh.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qfb.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jaa.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://akk.dianchejie.cn

Java: // 手写 HashMap
来源：http://vsp.quarkkingdee.top

Go:   // 手写 map[int]int
来源：http://jgu.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://rrv.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://kpx.xinyue.icu

[N08] 生成全排列
来源：http://bhq.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://qur.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://zkz.ybcxt.top

JS:   // 手写回溯递归
来源：http://ezk.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://iwb.jianghu66.top

Java: // 手写回溯递归
来源：http://ztk.chenzaomai.com

Go:   // 手写回溯递归
来源：http://tiv.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://jiz.nanxinkj.top

C#:   // 手写回溯递归
来源：http://zjv.fanxiaobao.xyz

[N09] 栈与队列
来源：http://mzc.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gss.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cgu.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kys.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mrh.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tcb.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wew.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nyx.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://icw.yuxming.cn

[N10] 链表节点定义
来源：http://hfg.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mcw.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lnk.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oaa.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://udq.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://aym.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://jjg.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cqf.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qim.aizwys.cn

[N11] 二叉树中序遍历
来源：http://wvg.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bdl.daria6918.cn

PHP:  // 手写递归函数
来源：http://fxr.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hup.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rtm.yvedp.cn

Java: // 手写递归
来源：http://vce.bjfxy.top

Go:   // 手写递归
来源：http://blc.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vzb.hfpthk.cn

C#:   // 手写递归
来源：http://zst.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tgo.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://anh.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tdp.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpr.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjv.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xrd.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://msa.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://idv.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://inx.jianghu66.top

================================================================================
来源：http://enc.ybcxt.top

O. 并发与异步
来源：http://pfb.xuanzx.com

================================================================================
来源：http://yal.daxiang520.top

[O01] 启动一个线程
来源：http://zqe.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wlt.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://szc.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://luc.cashguo.top

TS:   // 同 JS
来源：http://afw.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://zob.snrcjt.cn

Go:   go f()
来源：http://smf.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://hba.smart0.xyz

C#:   Task.Run(() => F());
来源：http://tzh.c1oappe.top

[O02] 使用线程池
来源：http://zdv.jqgufenzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qrj.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fqp.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://fdc.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://fjt.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://bgf.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xji.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yya.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://krk.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://exu.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://cvp.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://ctu.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://koh.jqgfzy.top

TS:   // 同 JS
来源：http://rqj.sxryk.cn

Java: synchronized (this) { shared++; }
来源：http://cgx.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://toi.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://pga.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://faq.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://tfm.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://tna.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://czq.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://vfr.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ile.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://avm.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hqg.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://two.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://lsp.daxiang520.top

[O05] 并发执行并等待全部完成
来源：http://eym.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://rvv.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xdn.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://puq.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://hvn.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tqz.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mkz.xinyue.icu

Ruby: threads.map(&:join)
来源：http://lrj.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tby.cheryme.top

[O06] 使用进程池
来源：http://ihi.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mhi.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bof.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://hxd.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://brn.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gah.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kfs.zycfv.cn

Ruby: // fork 块
来源：http://yfd.zhijiandao.cn

C#:   Parallel.For
来源：http://ejf.hnxiangtu.top

================================================================================
来源：http://jvb.gogol.net.cn

P. 常用工具函数
来源：http://dvb.jianghu66.top

================================================================================
来源：http://acx.jinqigfzy.top

[P01] 生成 UUID
来源：http://nmo.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://tbx.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://syt.daxiang520.top

JS:   crypto.randomUUID()
来源：http://zco.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://fjw.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://roc.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://vsn.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://xjz.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://wag.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://gyc.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ofn.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://rgk.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tqb.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nyr.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vvm.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iwc.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ljb.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dio.fehbvm.com

[P03] 生成短随机字符串
来源：http://ivi.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wum.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://svy.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xmq.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://por.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zfb.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ves.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://urq.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://exl.c1oappe.top

[P04] 求长度
来源：http://opv.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xyc.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xcj.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hkd.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pis.bjfxy.top


<!-- 参考信息 -->