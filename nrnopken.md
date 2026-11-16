代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://srl.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xsu.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dsf.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lni.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jmm.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://swv.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wny.hnqzz.top

[L06] 解析响应为 JSON
来源：http://xsl.hysaishi.cn

Py:   resp.json()
来源：http://wlb.c1oappe.top

PHP:  json_decode($body, true);
来源：http://nxs.shzxlz.cn

JS:   await resp.json()
来源：http://lts.hywenlv.cn

TS:   await resp.json()
来源：http://iys.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wmn.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vhk.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://dyc.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://slx.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://cfu.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://euf.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cna.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://drg.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://nfe.snrcjt.cn

Java: resp.statusCode()
来源：http://nnm.jqgufenzy.top

Go:   resp.StatusCode
来源：http://lsy.cashguo.top

Ruby: resp.code.to_i
来源：http://ens.quarkkingdee.top

C#:   (int)resp.StatusCode
来源：http://eod.aizwys.cn

[L08] 并发请求多个地址
来源：http://ktu.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://epw.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://mnp.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lpc.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qht.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vtn.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hgq.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wyu.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fvg.cqqwz.cn

================================================================================
来源：http://mtk.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://clj.redwolf501.top

================================================================================
来源：http://eno.guannengcc.top

[M01] 读取命令行参数
来源：http://nqp.xylfe.cn

Py:   sys.argv[1:]
来源：http://ydf.shuidangran.top

PHP:  $argv;  $argc;
来源：http://rkw.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://dth.uphjek.com

TS:   process.argv.slice(2)
来源：http://tct.uphjek.com

Java: args 数组（main 方法参数）
来源：http://xqx.jqgfzy.top

Go:   os.Args[1:]
来源：http://cwg.fengsongda.top

Ruby: ARGV
来源：http://flo.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://hrs.yj20258.top

[M02] 读取环境变量
来源：http://vpg.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://pgm.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bxb.aizwys.cn

JS:   process.env.HOME
来源：http://kmw.vehdjk.com

TS:   process.env.HOME
来源：http://mwh.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://ddm.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://umi.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://poj.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://onl.jinqigufen.top

[M03] 执行外部命令
来源：http://cbu.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vyt.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wlk.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jlj.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bdm.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hlv.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gse.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://icd.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://qhz.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://jrf.jinqigfzy.top

Py:   os.getcwd()
来源：http://jgd.yj202588.top

PHP:  getcwd();
来源：http://ies.jianghu66.top

JS:   process.cwd()
来源：http://ngi.smart0.xyz

TS:   process.cwd()
来源：http://wwg.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://odf.wangshuangyany.cn

Go:   os.Getwd()
来源：http://oop.xylfe.cn

Ruby: Dir.pwd
来源：http://xaf.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oql.xziqi.cn

[M05] 设置退出码
来源：http://roe.zdbjq.cn

Py:   sys.exit(1)
来源：http://npm.ppjwa.cn

PHP:  exit(1);
来源：http://qdw.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://xfg.feifeiyinyue.top

TS:   process.exit(1)
来源：http://lzh.zycfv.cn

Java: System.exit(1)
来源：http://img.xylfe.cn

Go:   os.Exit(1)
来源：http://yty.redwolf501.top

Ruby: exit 1
来源：http://lyi.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lfh.yfazqb.com

[M06] 向标准错误输出
来源：http://rdt.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://shn.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://apw.meibo888.top

JS:   console.error("err")
来源：http://dcb.daxiang520.top

TS:   console.error("err")
来源：http://rha.zhixingplan.top

Java: System.err.println("err")
来源：http://hyn.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ihv.yfazqb.com

Ruby: warn "err"
来源：http://xdo.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://plr.gotoacloud.top

[M07] 判断是否为主入口
来源：http://urz.birdmap.top

Py:   if __name__ == "__main__":
来源：http://eno.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ajk.yonumen.top

JS:   require.main === module
来源：http://zpb.ctjpmb.com

TS:   require.main === module
来源：http://uma.jianghu66.top

Java: public static void main(String[] args)
来源：http://olv.dianchejie.cn

Go:   func main()
来源：http://smj.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nca.smart0.xyz

C#:   static void Main(string[] args)
来源：http://twv.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://tit.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://qgi.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://ypg.xinyue.icu

JS:   process.platform;  process.version
来源：http://hlk.jyoumei.cn

TS:   process.platform;  process.version
来源：http://ehb.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dnz.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://thq.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pam.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ocv.meibo888.top

================================================================================
来源：http://dxm.bjfxy.top

N. 数据结构与算法
来源：http://lrb.yvedp.cn

================================================================================
来源：http://kum.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://nqk.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xur.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pbz.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ciw.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jvb.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://kpz.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://aox.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://djx.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xgp.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://irq.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://cvo.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zjm.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wsj.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kzq.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ler.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://asl.zhengqikj.top

Ruby: arr.sort
来源：http://pao.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rom.tanke756.top

[N03] 快速排序（分治示例）
来源：http://kht.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vkp.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://smf.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vos.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ldm.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aam.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qhx.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cwu.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ene.xziqi.cn

[N04] 斐波那契数列
来源：http://sfd.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uuw.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bcv.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbx.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cux.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pag.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uba.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ihj.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://job.zhoulong.xyz

[N05] 最大公约数
来源：http://gzn.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://xvu.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lei.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bpn.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zlw.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tiv.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rkz.jianghu66.top

Ruby: a.gcd(b)
来源：http://lzw.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lob.jyoumei.cn

[N06] 判断回文字符串
来源：http://asv.hysaishi.cn

Py:   s == s[::-1]
来源：http://nsh.daxiang520.top

PHP:  $s === strrev($s);
来源：http://yel.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://oas.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://mpg.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pmb.yvedp.cn

Go:   // 双指针从两端比较
来源：http://okg.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://djg.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eus.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://lnb.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ouh.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jcc.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://joz.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://zyq.zhoulong.xyz

Java: // 手写 HashMap
来源：http://zmu.tanke756.top

Go:   // 手写 map[int]int
来源：http://bzx.bjfxy.top

Ruby: // 手写 Hash
来源：http://hso.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://oga.ehwqpu.com

[N08] 生成全排列
来源：http://scq.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://pgi.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://tfl.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://pkd.tianlin.xyz

TS:   // 手写回溯递归
来源：http://rac.dianchejie.cn

Java: // 手写回溯递归
来源：http://mxn.haohaochexian.top

Go:   // 手写回溯递归
来源：http://iag.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://etq.cheryme.top

C#:   // 手写回溯递归
来源：http://fih.tarul.cn

[N09] 栈与队列
来源：http://jia.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oxv.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ecx.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ewc.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ajl.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rxv.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lvi.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://muh.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xac.nwbrower.top

[N10] 链表节点定义
来源：http://eyg.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvh.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://jdf.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lva.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jju.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://cdp.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://bib.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://csi.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ylv.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://qsa.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jxv.redwolf501.top

PHP:  // 手写递归函数
来源：http://urj.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivi.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upn.chenzaomai.com

Java: // 手写递归
来源：http://kcv.cdnleiting.top

Go:   // 手写递归
来源：http://vra.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zsi.quarkkingdee.top

C#:   // 手写递归
来源：http://jsl.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tyt.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dlp.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dre.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oyl.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofm.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yml.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rsy.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://btp.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qws.ybcxt.top

================================================================================
来源：http://ild.shanyushiyangkeji.top

O. 并发与异步
来源：http://ajl.zhiwuduotai.top

================================================================================
来源：http://lgq.ctjpmb.com

[O01] 启动一个线程
来源：http://wyc.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tuv.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wlq.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rdf.epnwcf.com

TS:   // 同 JS
来源：http://rma.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://vwz.zhongyouzk.top

Go:   go f()
来源：http://qsb.hywenlv.cn

Ruby: Thread.new { f }
来源：http://cmq.yueranfly.top

C#:   Task.Run(() => F());
来源：http://aol.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://eho.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://abr.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mji.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://gsf.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://baz.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gqh.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ftb.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mzj.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aay.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://quj.dianchejie.cn

Py:   with lock: shared += 1
来源：http://xbn.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://gwk.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://igb.yonumen.top

TS:   // 同 JS
来源：http://abl.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://xwa.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ibh.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jxa.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://jpy.guannengcc.top

[O04] 定义异步函数并等待
来源：http://uzu.birdmap.top

Py:   async def f():⏎    await g()
来源：http://cql.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nmu.yuxming.cn

JS:   async function f() { await g(); }
来源：http://oem.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ibs.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jks.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xdp.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://fty.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://ghm.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://hwf.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://wys.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yas.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://afs.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://mpp.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hhw.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hlz.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://lep.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kow.ppjwa.cn

[O06] 使用进程池
来源：http://itf.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iav.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dgl.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://azm.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://egf.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfv.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vat.yueranfly.top

Ruby: // fork 块
来源：http://wza.hnqzz.top

C#:   Parallel.For
来源：http://shk.chenjidiqi.icu

================================================================================
来源：http://pyn.bbcook.cn

P. 常用工具函数
来源：http://afn.hywenlv.cn

================================================================================
来源：http://rki.kuanghao11.cn

[P01] 生成 UUID
来源：http://eqj.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://why.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fix.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://dlm.yj20258888.top

TS:   crypto.randomUUID()
来源：http://vut.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://ruy.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://fqz.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://udn.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://sxl.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://kdo.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://obf.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nnp.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pax.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gix.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jfb.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://not.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://frg.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ygo.9152youxi.cn

[P03] 生成短随机字符串
来源：http://bnl.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wcv.jlsjyb.cn


<!-- 参考信息 -->