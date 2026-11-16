代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kbp.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://roq.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mpe.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rno.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vtb.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zea.vehdjk.com

[L05] 上传文件（multipart）
来源：http://tgm.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ygv.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yez.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lim.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uhw.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zdm.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dbw.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ple.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hxg.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://cqx.316326.xyz

Py:   resp.json()
来源：http://fzt.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://mol.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://lgj.jlsjyb.cn

TS:   await resp.json()
来源：http://pas.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dgu.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yvh.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://klo.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sun.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://zat.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nwo.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gmr.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://mbf.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://oqm.shuidangran.top

Java: resp.statusCode()
来源：http://ieq.yangfankeji.com

Go:   resp.StatusCode
来源：http://thd.hesvh.cn

Ruby: resp.code.to_i
来源：http://gfr.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://kts.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://wrw.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yvo.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://phi.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ajj.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hef.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dxl.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qzn.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vhr.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bum.sweek.top

================================================================================
来源：http://fzm.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://rpk.chenlongwang.top

================================================================================
来源：http://sqt.vqdsnc.cn

[M01] 读取命令行参数
来源：http://tzy.epnwcf.com

Py:   sys.argv[1:]
来源：http://lex.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://noq.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://tgy.nwbrower.top

TS:   process.argv.slice(2)
来源：http://cya.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://fsr.vehdjk.com

Go:   os.Args[1:]
来源：http://dro.sysykeji.top

Ruby: ARGV
来源：http://udj.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://ane.yfazqb.com

[M02] 读取环境变量
来源：http://sen.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://hvz.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kxp.cqqwz.cn

JS:   process.env.HOME
来源：http://akv.pengpengdd.cyou

TS:   process.env.HOME
来源：http://bvp.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://sgf.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tut.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://xlf.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://idp.sxryk.cn

[M03] 执行外部命令
来源：http://wcj.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpr.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://utu.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://clq.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ovf.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pgc.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://lev.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://jyg.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://xmy.chenzaomai.com

[M04] 获取当前工作目录
来源：http://oft.zhongyouzk.top

Py:   os.getcwd()
来源：http://aoj.daxiang520.top

PHP:  getcwd();
来源：http://yzb.gogol.net.cn

JS:   process.cwd()
来源：http://zqn.guowangkeji.top

TS:   process.cwd()
来源：http://nbi.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://pqr.cashguo.top

Go:   os.Getwd()
来源：http://mgk.jinqigufen.top

Ruby: Dir.pwd
来源：http://oyu.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hlp.ydjk.org.cn

[M05] 设置退出码
来源：http://jht.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://zzx.shuidangran.top

PHP:  exit(1);
来源：http://eua.hammf.cn

JS:   process.exit(1)
来源：http://xob.epnwcf.com

TS:   process.exit(1)
来源：http://lrt.zycfv.cn

Java: System.exit(1)
来源：http://mei.9152youxi.cn

Go:   os.Exit(1)
来源：http://fkv.jyoumei.cn

Ruby: exit 1
来源：http://zyx.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mht.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://rvd.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://kyd.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://faa.316326.xyz

JS:   console.error("err")
来源：http://twm.fanxiaobao.xyz

TS:   console.error("err")
来源：http://xlp.svipenyu.cn

Java: System.err.println("err")
来源：http://hqy.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uwo.zhongyouzk.top

Ruby: warn "err"
来源：http://sma.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://djx.vehdjk.com

[M07] 判断是否为主入口
来源：http://pwh.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://zae.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tnw.hammf.cn

JS:   require.main === module
来源：http://biy.svipenyu.cn

TS:   require.main === module
来源：http://tzw.zhengqikj.top

Java: public static void main(String[] args)
来源：http://tak.quarkkingdee.top

Go:   func main()
来源：http://jqj.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mqn.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://zfh.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://ofo.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://flz.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://lmx.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://uiq.bbcook.cn

TS:   process.platform;  process.version
来源：http://xyg.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dia.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uic.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pyf.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ivc.daria6918.cn

================================================================================
来源：http://dam.zhijiandao.cn

N. 数据结构与算法
来源：http://ytm.yongpay.top

================================================================================
来源：http://lfk.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://fzp.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sjj.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://asa.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fot.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://efb.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://frp.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://pot.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eto.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://zby.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://ejs.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://acu.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ybc.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://suj.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lgz.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cpe.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://hry.hnxiangtu.top

Ruby: arr.sort
来源：http://hox.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://brz.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://tle.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qpm.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://lmo.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yge.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bqa.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ysv.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zmn.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wbx.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qay.nanxuanxn.top

[N04] 斐波那契数列
来源：http://eek.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rqr.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wzn.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uho.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upv.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xkg.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wsi.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lfq.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dth.hcnkem.com

[N05] 最大公约数
来源：http://hjn.tarul.cn

Py:   math.gcd(a, b)
来源：http://mll.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mtl.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kig.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qif.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://trs.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nex.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://ais.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hct.quarkkingdee.top

[N06] 判断回文字符串
来源：http://aij.zhongyouzk.top

Py:   s == s[::-1]
来源：http://pbz.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://wvu.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://scy.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://pmt.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dhc.sweek.top

Go:   // 双指针从两端比较
来源：http://eak.aibaodan.cn

Ruby: s == s.reverse
来源：http://rca.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cjq.pycfn.com

[N07] 两数之和（返回下标）
来源：http://ihj.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://syy.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://upj.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dcq.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://wcy.hesvh.cn

Java: // 手写 HashMap
来源：http://kbn.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://hbi.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://dop.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://niv.jqgfzy.top

[N08] 生成全排列
来源：http://njo.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://cea.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://ixm.bjfxy.top

JS:   // 手写回溯递归
来源：http://riv.yonumen.top

TS:   // 手写回溯递归
来源：http://biv.haohaochexian.top

Java: // 手写回溯递归
来源：http://zvz.redwolf501.top

Go:   // 手写回溯递归
来源：http://sll.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://rnc.yj202588.top

C#:   // 手写回溯递归
来源：http://ges.hesvh.cn

[N09] 栈与队列
来源：http://nhz.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://evo.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mdo.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gws.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vnu.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fra.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tjb.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jbp.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gxe.c1oappe.top

[N10] 链表节点定义
来源：http://pmf.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bqz.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sfp.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fns.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lik.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://nrl.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://bxd.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mrh.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pkb.hammf.cn

[N11] 二叉树中序遍历
来源：http://lzn.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wtc.redwolf501.top

PHP:  // 手写递归函数
来源：http://vkb.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vyv.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ufl.feifeiyinyue.top

Java: // 手写递归
来源：http://wag.sufxvd.cn

Go:   // 手写递归
来源：http://aqu.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://czc.zhoulong.xyz

C#:   // 手写递归
来源：http://fah.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iro.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://byz.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aqv.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hrz.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvv.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bqr.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sls.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zsu.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yez.zycfv.cn

================================================================================
来源：http://dpd.iojbl.cn

O. 并发与异步
来源：http://yey.dianchejie.cn

================================================================================
来源：http://yql.sweek.top

[O01] 启动一个线程
来源：http://pet.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fbt.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://prj.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pmf.xuetiantiany.cn

TS:   // 同 JS
来源：http://mne.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://zxt.tian-w.cn

Go:   go f()
来源：http://nfm.dashuyun.cn

Ruby: Thread.new { f }
来源：http://hjc.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://apb.sweek.top

[O02] 使用线程池
来源：http://evb.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gwp.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qat.ivvv.top

JS:   // worker_threads 线程池
来源：http://eng.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://cja.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wdj.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fwj.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sen.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://htl.vehdjk.com

[O03] 加锁保护共享数据
来源：http://ygr.ydzc1.top

Py:   with lock: shared += 1
来源：http://uzu.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://bvc.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yxe.cqqwz.cn

TS:   // 同 JS
来源：http://oek.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://wte.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pnj.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nop.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://gyg.yonumen.top

[O04] 定义异步函数并等待
来源：http://zdk.yonumen.top

Py:   async def f():⏎    await g()
来源：http://joj.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ram.vehdjk.com

JS:   async function f() { await g(); }
来源：http://zib.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gzh.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xok.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ecl.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://pzd.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://hgk.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://bxi.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://ovs.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lur.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://yhv.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://vog.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wwd.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://egf.52xcode.cn

Ruby: threads.map(&:join)
来源：http://tze.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mmy.xuetiantiany.cn

[O06] 使用进程池
来源：http://ezc.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dhc.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nds.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://gxl.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://eja.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jww.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bsv.zdqjudy.top

Ruby: // fork 块
来源：http://uce.jinyuanbaomall.cn

C#:   Parallel.For
来源：http://hsb.ctjpmb.com

================================================================================
来源：http://ncf.cqqwz.cn

P. 常用工具函数
来源：http://yfd.ppjwa.cn

================================================================================
来源：http://hxm.daxiang520.top

[P01] 生成 UUID
来源：http://rlo.ivvv.top

Py:   str(uuid.uuid4())
来源：http://clx.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jyo.yj202588.top

JS:   crypto.randomUUID()
来源：http://rwx.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://ztd.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://lhq.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://oyc.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://cqo.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://dsd.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://apb.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://och.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://lui.ivvv.top


<!-- 参考信息 -->