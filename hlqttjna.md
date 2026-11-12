代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bly.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qmd.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wpx.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ydp.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dbj.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vkn.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lrw.cucudq.cn

[L06] 解析响应为 JSON
来源：http://raw.yueranfly.top

Py:   resp.json()
来源：http://dwe.cheryme.top

PHP:  json_decode($body, true);
来源：http://sbi.pengpengdd.cyou

JS:   await resp.json()
来源：http://csk.hesvh.cn

TS:   await resp.json()
来源：http://hve.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pop.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lpp.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://wkc.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lcf.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://irx.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bqe.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wrh.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://nch.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://cdd.nanxuanxn.top

Java: resp.statusCode()
来源：http://nou.ydzc1.top

Go:   resp.StatusCode
来源：http://fzz.havefunace.top

Ruby: resp.code.to_i
来源：http://rqh.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://etd.yj20258.top

[L08] 并发请求多个地址
来源：http://mnw.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uhf.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://iig.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ham.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://euy.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ncm.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jno.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xta.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mlj.zhoulong.xyz

================================================================================
来源：http://gau.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://sdv.hesvh.cn

================================================================================
来源：http://ini.iojbl.cn

[M01] 读取命令行参数
来源：http://mrz.fehbvm.com

Py:   sys.argv[1:]
来源：http://asn.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://lfb.c1oappe.top

JS:   process.argv.slice(2)
来源：http://kjn.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://wso.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://zid.shuidangran.top

Go:   os.Args[1:]
来源：http://ouf.ybcxt.top

Ruby: ARGV
来源：http://lkv.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://tfc.uphjek.com

[M02] 读取环境变量
来源：http://fku.tarul.cn

Py:   os.environ.get("HOME")
来源：http://eap.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kuw.sweek.top

JS:   process.env.HOME
来源：http://tvh.cucudq.cn

TS:   process.env.HOME
来源：http://yni.guannengcc.top

Java: System.getenv("HOME")
来源：http://bbw.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hbk.bbcook.cn

Ruby: ENV["HOME"]
来源：http://sye.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gnx.hammf.cn

[M03] 执行外部命令
来源：http://sxs.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cfl.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvx.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aho.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://faq.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pgs.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jqg.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nor.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://fpb.gotoacloud.top

[M04] 获取当前工作目录
来源：http://zwi.hysaishi.cn

Py:   os.getcwd()
来源：http://lde.yvedp.cn

PHP:  getcwd();
来源：http://laa.yongpay.top

JS:   process.cwd()
来源：http://xuj.hesvh.cn

TS:   process.cwd()
来源：http://fzm.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://fmg.hcnkem.com

Go:   os.Getwd()
来源：http://cgs.cheryme.top

Ruby: Dir.pwd
来源：http://xxy.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://yuy.xinyue.icu

[M05] 设置退出码
来源：http://qky.ppjwa.cn

Py:   sys.exit(1)
来源：http://zmp.fzhhl.top

PHP:  exit(1);
来源：http://dxd.guowangkeji.top

JS:   process.exit(1)
来源：http://xdl.zhengqikj.top

TS:   process.exit(1)
来源：http://gid.cashguo.top

Java: System.exit(1)
来源：http://dno.fengsongda.top

Go:   os.Exit(1)
来源：http://vgl.yuxming.cn

Ruby: exit 1
来源：http://hqc.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fuz.yuxming.cn

[M06] 向标准错误输出
来源：http://vnl.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://ywc.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xcw.c1oappe.top

JS:   console.error("err")
来源：http://bem.yongpay.top

TS:   console.error("err")
来源：http://rem.jlsjyb.cn

Java: System.err.println("err")
来源：http://nho.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hhx.nanxinkj.top

Ruby: warn "err"
来源：http://ljj.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://msg.tianlin.xyz

[M07] 判断是否为主入口
来源：http://zlm.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://mrd.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nog.jyoumei.cn

JS:   require.main === module
来源：http://zrw.zhaomingkeji.xyz

TS:   require.main === module
来源：http://cbu.zhixingplan.top

Java: public static void main(String[] args)
来源：http://dbn.316326.xyz

Go:   func main()
来源：http://hza.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rhy.ivvv.top

C#:   static void Main(string[] args)
来源：http://ahw.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://dpo.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://nbh.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://okw.daria6918.cn

JS:   process.platform;  process.version
来源：http://orr.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://vyv.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xfg.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tis.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pnl.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mhi.shangyingyoupin.top

================================================================================
来源：http://jxp.jinqigfzy.top

N. 数据结构与算法
来源：http://xlk.shanyushiyangtech.top

================================================================================
来源：http://knh.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://ysq.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://gez.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sdx.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgk.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mwv.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://fpg.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://lvb.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cph.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://aer.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://mvn.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://uem.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bsm.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wcv.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lay.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kay.hammf.cn

Go:   slices.Sort(arr)
来源：http://ieh.hysaishi.cn

Ruby: arr.sort
来源：http://srq.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ntn.birdmap.top

[N03] 快速排序（分治示例）
来源：http://xpt.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iwg.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://xet.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qid.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhj.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jfu.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uae.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pnb.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qgl.ybcxt.top

[N04] 斐波那契数列
来源：http://rxx.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vaa.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mqv.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://poc.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nrz.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ogk.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://foe.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mqg.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://evm.iojbl.cn

[N05] 最大公约数
来源：http://bjn.iojbl.cn

Py:   math.gcd(a, b)
来源：http://xxt.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tic.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibr.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgu.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oje.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mcl.svipenyu.cn

Ruby: a.gcd(b)
来源：http://zmr.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cnr.gogol.net.cn

[N06] 判断回文字符串
来源：http://uuc.epnwcf.com

Py:   s == s[::-1]
来源：http://ias.pycfn.com

PHP:  $s === strrev($s);
来源：http://upp.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://ayz.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://dsk.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ham.havefunace.top

Go:   // 双指针从两端比较
来源：http://ezs.nanxuanxn.top

Ruby: s == s.reverse
来源：http://trw.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jqf.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://hrv.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sga.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tup.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ahz.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://xct.zhixingplan.top

Java: // 手写 HashMap
来源：http://ibw.birdmap.top

Go:   // 手写 map[int]int
来源：http://imm.yj20258.top

Ruby: // 手写 Hash
来源：http://yyl.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://osu.nwbrower.top

[N08] 生成全排列
来源：http://idp.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://wtv.yuanzhike.top

PHP:  // 手写递归交换
来源：http://bjg.redwolf501.top

JS:   // 手写回溯递归
来源：http://efl.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://cbq.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://wbf.zycfv.cn

Go:   // 手写回溯递归
来源：http://wxs.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://cvj.ivvv.top

C#:   // 手写回溯递归
来源：http://lhw.bbcook.cn

[N09] 栈与队列
来源：http://fch.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jly.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ufz.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rnj.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jea.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tpb.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iab.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gug.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qgj.sysykeji.top

[N10] 链表节点定义
来源：http://nch.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://poj.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nic.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rca.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lgc.cashguo.top

Java: class Node { int v; Node next; }
来源：http://uyu.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://jvj.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iez.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://txf.tanke756.top

[N11] 二叉树中序遍历
来源：http://ajt.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tai.nwbrower.top

PHP:  // 手写递归函数
来源：http://seh.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xmr.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mhu.cashguo.top

Java: // 手写递归
来源：http://vvd.yonumen.top

Go:   // 手写递归
来源：http://hnp.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tpc.jinqigfzy.top

C#:   // 手写递归
来源：http://nmv.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sbk.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ekq.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lyh.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kau.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://chw.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ikk.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ddj.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wox.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ebo.cdnleiting.top

================================================================================
来源：http://sux.yj20258888.top

O. 并发与异步
来源：http://yhj.fktsv.cn

================================================================================
来源：http://hpn.birdmap.top

[O01] 启动一个线程
来源：http://ceo.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fkb.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jey.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hqp.cheryme.top

TS:   // 同 JS
来源：http://mfa.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://hcj.yanxiufei.cn

Go:   go f()
来源：http://cqs.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://fjx.xziqi.cn

C#:   Task.Run(() => F());
来源：http://bqa.svipenyu.cn

[O02] 使用线程池
来源：http://kkl.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hsz.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gvg.hnqzz.top

JS:   // worker_threads 线程池
来源：http://nvo.yonumen.top

TS:   // worker_threads 线程池
来源：http://eel.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://upp.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gfl.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gdw.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zoa.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://erl.ehwqpu.com

Py:   with lock: shared += 1
来源：http://eqb.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://emq.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uft.gzhubu.top

TS:   // 同 JS
来源：http://zid.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://kda.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rbo.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gol.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://igl.shuidangran.top

[O04] 定义异步函数并等待
来源：http://hkw.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://luq.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jnz.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://dzf.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hnk.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jqb.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cua.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://asn.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://tld.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://dww.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://djv.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ict.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://rgw.meibo888.top

TS:   await Promise.all(tasks)
来源：http://rmh.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sav.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zvi.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://zsa.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jrc.bjfxy.top

[O06] 使用进程池
来源：http://cbu.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jxa.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ttu.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://sgd.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://exc.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rxz.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kcc.yanxiufei.cn

Ruby: // fork 块
来源：http://tzc.zdqjudy.top

C#:   Parallel.For
来源：http://kix.yj20258888.top

================================================================================
来源：http://rtg.jqgufenzy.top

P. 常用工具函数
来源：http://bpf.andypj.xyz

================================================================================
来源：http://hnv.svipenyu.cn

[P01] 生成 UUID
来源：http://lzu.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://srp.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hgr.xylfe.cn

JS:   crypto.randomUUID()
来源：http://rnh.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://sdv.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://xox.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://nal.havefunace.top

Ruby: SecureRandom.uuid
来源：http://ebd.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://fck.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://olr.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://znd.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wkj.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://smh.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rqg.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fpf.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://czd.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://til.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oxi.sufxvd.cn

[P03] 生成短随机字符串
来源：http://kmk.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ywi.kuanghao11.cn


<!-- 参考信息 -->