代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://shg.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pbu.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lgq.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qqt.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://moi.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rdt.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oww.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://qbs.gzhubu.top

Py:   resp.json()
来源：http://yld.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://fuz.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://css.kuanghao11.cn

TS:   await resp.json()
来源：http://yce.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zge.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qst.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://cih.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nqr.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://owe.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vpc.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bjr.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://gqs.sweek.top

TS:   resp.ok;  resp.status
来源：http://xum.daxiang520.top

Java: resp.statusCode()
来源：http://ugl.fengsongda.top

Go:   resp.StatusCode
来源：http://lpv.cdnleiting.top

Ruby: resp.code.to_i
来源：http://dlg.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://vvy.dianchejie.cn

[L08] 并发请求多个地址
来源：http://hup.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iln.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://ikk.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rei.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mwv.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fhi.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lat.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xeq.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ubf.yuanzhike.top

================================================================================
来源：http://xjs.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://xaw.guannengcc.top

================================================================================
来源：http://lnv.ydjk.org.cn

[M01] 读取命令行参数
来源：http://qcu.cdnleiting.top

Py:   sys.argv[1:]
来源：http://pdr.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://ewk.c1oappe.top

JS:   process.argv.slice(2)
来源：http://boi.yj20258888.top

TS:   process.argv.slice(2)
来源：http://ork.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://xjc.yueranfly.top

Go:   os.Args[1:]
来源：http://qro.dianchejie.cn

Ruby: ARGV
来源：http://bfq.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://irz.hesvh.cn

[M02] 读取环境变量
来源：http://zoi.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://nvh.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dfn.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://gqe.dianchejie.cn

TS:   process.env.HOME
来源：http://tuq.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://yhz.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zll.cucudq.cn

Ruby: ENV["HOME"]
来源：http://yvo.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ozi.feifeiyinyue.top

[M03] 执行外部命令
来源：http://rqn.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kvq.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://swx.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zfj.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ism.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tii.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://shj.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://pir.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://kwz.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://ssl.zhixingplan.top

Py:   os.getcwd()
来源：http://iqo.yonumen.top

PHP:  getcwd();
来源：http://gru.zycfv.cn

JS:   process.cwd()
来源：http://wmk.shzxlz.cn

TS:   process.cwd()
来源：http://wpd.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://fhs.zhiwuduotai.top

Go:   os.Getwd()
来源：http://wmg.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://won.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://gkl.hywenlv.cn

[M05] 设置退出码
来源：http://tvf.9152youxi.cn

Py:   sys.exit(1)
来源：http://kbr.guowangkeji.top

PHP:  exit(1);
来源：http://pjh.jyoumei.cn

JS:   process.exit(1)
来源：http://dmv.redwolf501.top

TS:   process.exit(1)
来源：http://yyn.jlsjyb.cn

Java: System.exit(1)
来源：http://cta.guannengcc.top

Go:   os.Exit(1)
来源：http://ceh.bbcook.cn

Ruby: exit 1
来源：http://wsd.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lwd.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://pdy.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://lri.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uap.andypj.xyz

JS:   console.error("err")
来源：http://kxx.hongshengwenyu.top

TS:   console.error("err")
来源：http://fnz.zhengqikj.top

Java: System.err.println("err")
来源：http://cba.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mzr.hfpthk.cn

Ruby: warn "err"
来源：http://zop.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://bkk.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://tkv.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://vja.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rao.haohaochexian.top

JS:   require.main === module
来源：http://fpc.ydzc1.top

TS:   require.main === module
来源：http://rmv.andypj.xyz

Java: public static void main(String[] args)
来源：http://qan.iojbl.cn

Go:   func main()
来源：http://dbj.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mky.xziqi.cn

C#:   static void Main(string[] args)
来源：http://png.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://qnv.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://kbe.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://gii.sxryk.cn

JS:   process.platform;  process.version
来源：http://mnk.yonumen.top

TS:   process.platform;  process.version
来源：http://qnz.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://czn.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jqq.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vdo.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gwf.guannengcc.top

================================================================================
来源：http://jej.sxryk.cn

N. 数据结构与算法
来源：http://zsx.jianghu66.top

================================================================================
来源：http://xzy.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://lnm.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://jov.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pui.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sdl.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gsx.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hsd.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://noi.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pwj.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pry.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://xyb.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://fdz.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://umd.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://aaw.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://epi.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vvs.uphjek.com

Go:   slices.Sort(arr)
来源：http://sdz.birdmap.top

Ruby: arr.sort
来源：http://ika.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uuh.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://tjv.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fsj.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://bla.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xkk.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aqu.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ney.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tzz.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yzs.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://ftx.ydjk.org.cn

[N04] 斐波那契数列
来源：http://iwd.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aiw.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rbn.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugq.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exj.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kjr.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bal.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://out.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kdu.tianlin.xyz

[N05] 最大公约数
来源：http://bwb.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://cor.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qea.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rpj.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbo.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cww.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kph.hnqzz.top

Ruby: a.gcd(b)
来源：http://xko.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sbp.hnxiangtu.top

[N06] 判断回文字符串
来源：http://zyz.cashguo.top

Py:   s == s[::-1]
来源：http://bte.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://bre.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://npd.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://xhg.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xaf.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://zds.yvedp.cn

Ruby: s == s.reverse
来源：http://txb.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ptt.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://xwc.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvx.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fai.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zku.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://onr.sufxvd.cn

Java: // 手写 HashMap
来源：http://xhw.zycfv.cn

Go:   // 手写 map[int]int
来源：http://sqt.dashuyun.cn

Ruby: // 手写 Hash
来源：http://wwm.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dmf.fktsv.cn

[N08] 生成全排列
来源：http://wxo.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://jye.hywenlv.cn

PHP:  // 手写递归交换
来源：http://drp.dashuyun.cn

JS:   // 手写回溯递归
来源：http://mqy.iojbl.cn

TS:   // 手写回溯递归
来源：http://eay.yongpay.top

Java: // 手写回溯递归
来源：http://rmf.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://cyh.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://quo.chenzaomai.com

C#:   // 手写回溯递归
来源：http://ctt.zhiwuduotai.top

[N09] 栈与队列
来源：http://drg.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nxj.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cbt.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zvb.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nzg.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vbq.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nzd.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vfg.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://coz.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://ckx.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cxf.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://sme.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sqy.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hyy.bbcook.cn

Java: class Node { int v; Node next; }
来源：http://ikx.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://ofr.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hng.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bed.tanke756.top

[N11] 二叉树中序遍历
来源：http://bfn.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://djx.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://dmf.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndf.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nhq.vehdjk.com

Java: // 手写递归
来源：http://wwe.ehwqpu.com

Go:   // 手写递归
来源：http://zyi.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vfr.hnxiangtu.top

C#:   // 手写递归
来源：http://wwm.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ier.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rcm.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fjq.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffr.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbb.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvx.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ono.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://enz.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rhy.yonumen.top

================================================================================
来源：http://ysz.shangyingyoupin.top

O. 并发与异步
来源：http://sjh.ivvv.top

================================================================================
来源：http://qce.birdmap.top

[O01] 启动一个线程
来源：http://zwu.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zgf.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iwd.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nsm.zhengqikj.top

TS:   // 同 JS
来源：http://waj.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://qhx.fktsv.cn

Go:   go f()
来源：http://swq.xziqi.cn

Ruby: Thread.new { f }
来源：http://gys.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://zrl.yj20258888.top

[O02] 使用线程池
来源：http://ljg.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cww.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tal.jianghu66.top

JS:   // worker_threads 线程池
来源：http://imh.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://ovo.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://szo.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ovg.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eqq.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oxz.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://dnt.sufxvd.cn

Py:   with lock: shared += 1
来源：http://afw.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://iqq.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lks.snrcjt.cn

TS:   // 同 JS
来源：http://obp.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://ucv.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zye.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mxs.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://yzy.epnwcf.com

[O04] 定义异步函数并等待
来源：http://iam.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://xfa.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qdr.bbcook.cn

JS:   async function f() { await g(); }
来源：http://oku.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kky.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uaw.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ttg.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eob.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://tto.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://eja.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://wpx.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wod.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://zdh.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://pns.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nmh.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fny.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://udq.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://hmw.jiagoushi.top

[O06] 使用进程池
来源：http://hte.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uzi.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://agn.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://jaq.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://tcd.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ufe.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ykn.shangyingyoupin.top

Ruby: // fork 块
来源：http://neu.xinyue.icu

C#:   Parallel.For
来源：http://ukn.yongpay.top

================================================================================
来源：http://tpz.shanyushiyangtech.top

P. 常用工具函数
来源：http://zbf.gotoacloud.top

================================================================================
来源：http://cbd.gogol.net.cn

[P01] 生成 UUID
来源：http://tca.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://cyn.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://non.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://rbw.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://ane.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://zue.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://fcr.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://aqo.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://wup.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://igr.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mtn.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qbc.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mtd.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tyr.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mna.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wza.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uar.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xdv.pycfn.com

[P03] 生成短随机字符串
来源：http://dsy.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nyx.dianchejie.cn


<!-- 参考信息 -->