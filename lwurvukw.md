代发 wailian999

Py:   resp.json()
来源：http://sxv.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://hyg.ybcxt.top

JS:   await resp.json()
来源：http://tzh.sxryk.cn

TS:   await resp.json()
来源：http://uhg.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pni.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zrs.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://ewc.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dhz.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://qat.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fyh.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wua.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://xvn.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://qeq.hesvh.cn

Java: resp.statusCode()
来源：http://heh.cqqwz.cn

Go:   resp.StatusCode
来源：http://teq.guannengcc.top

Ruby: resp.code.to_i
来源：http://cmt.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://map.jyoumei.cn

[L08] 并发请求多个地址
来源：http://uao.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tou.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://pya.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ubl.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cuz.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ktq.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sqf.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xts.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jtx.jqgfzy.top

================================================================================
来源：http://hkw.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://vkr.feifeiyinyue.top

================================================================================
来源：http://qyo.tarul.cn

[M01] 读取命令行参数
来源：http://tsa.havefunace.top

Py:   sys.argv[1:]
来源：http://vse.tian-w.cn

PHP:  $argv;  $argc;
来源：http://gfa.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://flp.c1oappe.top

TS:   process.argv.slice(2)
来源：http://yja.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://wos.kuanghao11.cn

Go:   os.Args[1:]
来源：http://zpm.zdqjudy.top

Ruby: ARGV
来源：http://ohb.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://iij.haohaochexian.top

[M02] 读取环境变量
来源：http://gyz.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://dqs.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bjs.feifeiyinyue.top

JS:   process.env.HOME
来源：http://mro.c1oappe.top

TS:   process.env.HOME
来源：http://gbl.fehbvm.com

Java: System.getenv("HOME")
来源：http://geh.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://awt.ivvv.top

Ruby: ENV["HOME"]
来源：http://gre.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zdv.jiagoushi.top

[M03] 执行外部命令
来源：http://tlx.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bhd.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://puu.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://rtl.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ypk.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://srq.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://spv.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://hzs.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://eur.yj20258.top

[M04] 获取当前工作目录
来源：http://yjr.mhx1999.top

Py:   os.getcwd()
来源：http://gje.hnxiangtu.top

PHP:  getcwd();
来源：http://iyf.gotoacloud.top

JS:   process.cwd()
来源：http://luy.yuxming.cn

TS:   process.cwd()
来源：http://tve.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://eua.zycfv.cn

Go:   os.Getwd()
来源：http://rwe.yonumen.top

Ruby: Dir.pwd
来源：http://gln.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zmq.dianchejie.cn

[M05] 设置退出码
来源：http://bzo.0kj1m.cn

Py:   sys.exit(1)
来源：http://dcv.vqdsnc.cn

PHP:  exit(1);
来源：http://elz.chenlongwang.top

JS:   process.exit(1)
来源：http://ehd.vehdjk.com

TS:   process.exit(1)
来源：http://peb.jianghu66.top

Java: System.exit(1)
来源：http://bhq.wangdashe.top

Go:   os.Exit(1)
来源：http://tmv.hcnkem.com

Ruby: exit 1
来源：http://vai.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jte.guowangkeji.top

[M06] 向标准错误输出
来源：http://iir.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://dex.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nqd.smart0.xyz

JS:   console.error("err")
来源：http://fid.jinqigfzy.top

TS:   console.error("err")
来源：http://bos.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://wjq.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pwx.shuidangran.top

Ruby: warn "err"
来源：http://oym.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://nsk.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://zxl.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://rkf.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dew.aibaodan.cn

JS:   require.main === module
来源：http://vnu.pycfn.com

TS:   require.main === module
来源：http://dnl.zhengqikj.top

Java: public static void main(String[] args)
来源：http://efw.shanyushiyangkeji.top

Go:   func main()
来源：http://vfx.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lwy.316326.xyz

C#:   static void Main(string[] args)
来源：http://iml.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://vhq.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://uvf.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://gvg.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://jjz.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://bda.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hcx.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ygr.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ler.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ybp.mhx1999.top

================================================================================
来源：http://jua.svipenyu.cn

N. 数据结构与算法
来源：http://pjn.hnxiangtu.top

================================================================================
来源：http://qzb.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://aoi.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ayc.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gcf.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fjt.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iup.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://zgj.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://bzv.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://div.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ziu.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://mer.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://jss.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yii.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xps.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kai.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pnl.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://tgx.dianchejie.cn

Ruby: arr.sort
来源：http://xso.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://iku.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://rcy.ybcxt.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cgs.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://ywg.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xpj.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsv.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hlh.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pvp.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rku.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://boc.yueranfly.top

[N04] 斐波那契数列
来源：http://ecy.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qcg.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mkg.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdn.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ihb.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://woh.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://axa.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qho.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aaq.ctjpmb.com

[N05] 最大公约数
来源：http://rpn.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://jbq.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xzc.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vnr.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umw.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://asl.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lhv.dashuyun.cn

Ruby: a.gcd(b)
来源：http://rgl.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pqi.redwolf501.top

[N06] 判断回文字符串
来源：http://kap.daria6918.cn

Py:   s == s[::-1]
来源：http://ikk.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://ujc.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://phk.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://jnj.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bks.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://iap.ivvv.top

Ruby: s == s.reverse
来源：http://gpl.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://phd.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://cfw.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ikr.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dex.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eat.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://rio.chenlongwang.top

Java: // 手写 HashMap
来源：http://cdq.mhx1999.top

Go:   // 手写 map[int]int
来源：http://huj.sufxvd.cn

Ruby: // 手写 Hash
来源：http://qku.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ktw.0kj1m.cn

[N08] 生成全排列
来源：http://qsv.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://vbi.chenlongwang.top

PHP:  // 手写递归交换
来源：http://wjk.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://oob.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://tck.cashguo.top

Java: // 手写回溯递归
来源：http://hys.dashuyun.cn

Go:   // 手写回溯递归
来源：http://bis.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://aog.52xcode.cn

C#:   // 手写回溯递归
来源：http://avp.wangdashe.top

[N09] 栈与队列
来源：http://duh.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hop.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://egv.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ong.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vos.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yyq.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dig.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yhm.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pef.guannengcc.top

[N10] 链表节点定义
来源：http://bgn.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rob.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ref.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cna.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gzx.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://djg.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://ytv.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vdd.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://muo.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://bvk.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ygm.fktsv.cn

PHP:  // 手写递归函数
来源：http://tii.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbo.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nav.ybcxt.top

Java: // 手写递归
来源：http://dya.zhoulong.xyz

Go:   // 手写递归
来源：http://ocv.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cak.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://iqh.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ypn.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rei.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wrt.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pas.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofr.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vhk.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://emp.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hdl.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ifk.ehwqpu.com

================================================================================
来源：http://akf.xingfuxueyuan.xyz

O. 并发与异步
来源：http://snv.xuetiantiany.cn

================================================================================
来源：http://qhk.xuanzx.com

[O01] 启动一个线程
来源：http://iup.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ldo.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kif.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mql.jianghu66.top

TS:   // 同 JS
来源：http://svq.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://zpr.sjlbkw.cn

Go:   go f()
来源：http://cox.yonumen.top

Ruby: Thread.new { f }
来源：http://ura.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://twn.yanxiufei.cn

[O02] 使用线程池
来源：http://rwz.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://prq.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ojb.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://glo.fehbvm.com

TS:   // worker_threads 线程池
来源：http://pua.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wcq.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ist.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ehf.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nsy.yongpay.top

[O03] 加锁保护共享数据
来源：http://pqc.cqqwz.cn

Py:   with lock: shared += 1
来源：http://uzm.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://yzy.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mzi.tarul.cn

TS:   // 同 JS
来源：http://uva.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://aaz.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vje.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqg.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://mri.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://otn.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://dsd.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bix.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://cce.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pgi.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vvk.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tvh.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lsr.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://tud.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://toc.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://pjo.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yod.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://ute.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://pis.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://huw.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pva.yonumen.top

Ruby: threads.map(&:join)
来源：http://syv.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pbj.yj20258.top

[O06] 使用进程池
来源：http://eyk.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ksl.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ebm.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://ukq.uphjek.com

TS:   // child_process / cluster 模块
来源：http://abb.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fbk.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ikd.sweek.top

Ruby: // fork 块
来源：http://bcz.mhx1999.top

C#:   Parallel.For
来源：http://tnw.ctjpmb.com

================================================================================
来源：http://gnu.jinyuanbaomall.cn

P. 常用工具函数
来源：http://xxi.jiagoushi.top

================================================================================
来源：http://apt.uphjek.com

[P01] 生成 UUID
来源：http://deq.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://qza.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iww.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://qif.yuxming.cn

TS:   crypto.randomUUID()
来源：http://rcq.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://ksw.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://uxb.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://awu.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://pwv.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://gfb.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zsx.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jhs.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wck.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cym.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://urr.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nxf.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ruf.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qkg.svipenyu.cn

[P03] 生成短随机字符串
来源：http://bpl.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vje.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cho.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fog.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ywz.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pea.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tdo.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://unf.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ije.zhoulong.xyz

[P04] 求长度
来源：http://bsq.ydjk.org.cn


<!-- 参考信息 -->