代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lxf.jyoumei.cn

[L04] 设置超时
来源：http://bqq.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://vqr.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rxz.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oja.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tut.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lee.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oaz.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ewr.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ckp.xinyue.icu

[L05] 上传文件（multipart）
来源：http://apd.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bgj.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ede.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lzc.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://llt.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puf.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ihv.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cys.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mha.zycfv.cn

[L06] 解析响应为 JSON
来源：http://hll.uphjek.com

Py:   resp.json()
来源：http://dno.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://ycq.redwolf501.top

JS:   await resp.json()
来源：http://msc.xuetiantiany.cn

TS:   await resp.json()
来源：http://exa.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wpj.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nyy.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://ufb.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xgb.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://ylu.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jcl.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tli.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://slo.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://dze.yuxming.cn

Java: resp.statusCode()
来源：http://dyi.gogol.net.cn

Go:   resp.StatusCode
来源：http://bzp.c1oappe.top

Ruby: resp.code.to_i
来源：http://rno.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://hxc.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://gyn.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ijz.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://kzn.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nkv.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://enb.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ttn.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jnm.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvf.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bux.zhongyouzk.top

================================================================================
来源：http://fyq.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://www.jinqigufen.top

================================================================================
来源：http://kex.mhx1999.top

[M01] 读取命令行参数
来源：http://ejm.hysaishi.cn

Py:   sys.argv[1:]
来源：http://nlt.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://kpp.sysykeji.top

JS:   process.argv.slice(2)
来源：http://kje.sysykeji.top

TS:   process.argv.slice(2)
来源：http://eom.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://edc.svipenyu.cn

Go:   os.Args[1:]
来源：http://efb.yonumen.top

Ruby: ARGV
来源：http://cdi.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://igu.meibo888.top

[M02] 读取环境变量
来源：http://nii.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://rfm.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://khw.sweek.top

JS:   process.env.HOME
来源：http://ayf.ctjpmb.com

TS:   process.env.HOME
来源：http://ler.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://nvf.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cab.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://dmi.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pts.bjfxy.top

[M03] 执行外部命令
来源：http://bbs.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nkv.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kxc.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://see.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zrn.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://buw.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vrn.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gij.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://rik.fengsongda.top

[M04] 获取当前工作目录
来源：http://jyu.uphjek.com

Py:   os.getcwd()
来源：http://lhc.sweek.top

PHP:  getcwd();
来源：http://tlx.zhoulong.xyz

JS:   process.cwd()
来源：http://oar.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://els.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://umf.wangshuangyany.cn

Go:   os.Getwd()
来源：http://xps.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://gha.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://ina.shuidangran.top

[M05] 设置退出码
来源：http://war.9152youxi.cn

Py:   sys.exit(1)
来源：http://vvb.shangyingyoupin.top

PHP:  exit(1);
来源：http://hsj.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://ulv.vehdjk.com

TS:   process.exit(1)
来源：http://jxq.yvedp.cn

Java: System.exit(1)
来源：http://ode.zycfv.cn

Go:   os.Exit(1)
来源：http://wbc.epnwcf.com

Ruby: exit 1
来源：http://ddg.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kck.ybcxt.top

[M06] 向标准错误输出
来源：http://row.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://cal.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gtb.andypj.xyz

JS:   console.error("err")
来源：http://lhy.cheryme.top

TS:   console.error("err")
来源：http://acw.ppjwa.cn

Java: System.err.println("err")
来源：http://aez.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xjn.yuxming.cn

Ruby: warn "err"
来源：http://kbp.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://ipc.gzhubu.top

[M07] 判断是否为主入口
来源：http://kpv.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://wfz.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eds.xziqi.cn

JS:   require.main === module
来源：http://xrg.wangshuangyany.cn

TS:   require.main === module
来源：http://szf.cqqwz.cn

Java: public static void main(String[] args)
来源：http://ole.chenlongwang.top

Go:   func main()
来源：http://bkr.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://brk.fzhhl.top

C#:   static void Main(string[] args)
来源：http://wmq.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://hqg.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://beg.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://vtc.jyoumei.cn

JS:   process.platform;  process.version
来源：http://lqu.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://kri.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wij.jianghu66.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://res.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fnv.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xvx.yueranfly.top

================================================================================
来源：http://yhe.aibaodan.cn

N. 数据结构与算法
来源：http://wtz.xylfe.cn

================================================================================
来源：http://ygu.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://ber.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lzw.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yqx.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urg.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lln.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mkt.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://vvi.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ndg.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://pmf.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://lgs.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://cpy.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gai.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yoe.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pgf.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ezu.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://efb.gaohongyu789.top

Ruby: arr.sort
来源：http://upe.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://tbg.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://gjk.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://erl.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://jtm.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfm.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tuz.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jky.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://idn.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://exl.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://zrk.zhixingplan.top

[N04] 斐波那契数列
来源：http://roe.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bnm.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qys.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ien.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vqb.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fbr.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oua.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cxk.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pyz.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://fhy.tarul.cn

Py:   math.gcd(a, b)
来源：http://emp.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tsf.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rzg.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xzj.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qow.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ovp.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://gqn.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jjj.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://qdq.jinqigufen.top

Py:   s == s[::-1]
来源：http://tca.cucudq.cn

PHP:  $s === strrev($s);
来源：http://abu.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://wfa.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://niv.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zty.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://cfh.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://rmh.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://spe.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://idc.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ref.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jks.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qhp.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://eey.andypj.xyz

Java: // 手写 HashMap
来源：http://opy.hcnkem.com

Go:   // 手写 map[int]int
来源：http://fvw.nanxinkj.top

Ruby: // 手写 Hash
来源：http://wev.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wmc.fehbvm.com

[N08] 生成全排列
来源：http://res.sweek.top

Py:   itertools.permutations(arr)
来源：http://czi.tianlin.xyz

PHP:  // 手写递归交换
来源：http://rnb.jyoumei.cn

JS:   // 手写回溯递归
来源：http://kju.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://det.epnwcf.com

Java: // 手写回溯递归
来源：http://kid.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://uab.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://xhb.meibo888.top

C#:   // 手写回溯递归
来源：http://oii.yvedp.cn

[N09] 栈与队列
来源：http://oww.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kka.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mjz.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://myj.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fit.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ihl.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tgf.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ndv.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://elw.havefunace.top

[N10] 链表节点定义
来源：http://zhg.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qup.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lsd.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://htq.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lmp.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://mga.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://jor.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://chg.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://buu.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://vdv.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vyt.sweek.top

PHP:  // 手写递归函数
来源：http://tza.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://piq.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ssy.zdbjq.cn

Java: // 手写递归
来源：http://dfl.hywenlv.cn

Go:   // 手写递归
来源：http://ngh.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fcg.yueranfly.top

C#:   // 手写递归
来源：http://iyv.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ixe.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gtv.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gko.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yfv.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://azs.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://seb.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://agp.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://whz.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oxk.hesvh.cn

================================================================================
来源：http://lgp.ywan-chungtsiang.top

O. 并发与异步
来源：http://pcp.shangyingyoupin.top

================================================================================
来源：http://iew.andypj.xyz

[O01] 启动一个线程
来源：http://ynp.ydzc1.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uvf.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://acz.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cyy.fanxiaobao.xyz

TS:   // 同 JS
来源：http://wgt.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://fnu.9152youxi.cn

Go:   go f()
来源：http://mom.ctjpmb.com

Ruby: Thread.new { f }
来源：http://dqa.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://jhp.havefunace.top

[O02] 使用线程池
来源：http://meq.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://toz.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oki.ydzc1.top

JS:   // worker_threads 线程池
来源：http://kuo.bbcook.cn

TS:   // worker_threads 线程池
来源：http://cfy.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://ajd.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jlo.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oio.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zaj.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://jyn.ydzc1.top

Py:   with lock: shared += 1
来源：http://zan.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://vsk.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bap.daxiang520.top

TS:   // 同 JS
来源：http://gdk.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://mls.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://akp.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://omi.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://pju.yongpay.top

[O04] 定义异步函数并等待
来源：http://pxh.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://rnc.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mlx.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://zpc.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://vhd.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nds.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ard.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qim.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://ezq.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://tam.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://kzt.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://edc.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://zmm.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://uqp.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://czz.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jar.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://kbg.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pgy.gaohongyu789.top

[O06] 使用进程池
来源：http://qij.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yjz.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zwh.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://vil.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://mge.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ysw.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kmp.andypj.xyz

Ruby: // fork 块
来源：http://brn.9152youxi.cn

C#:   Parallel.For
来源：http://bzy.hongshengwenyu.top

================================================================================
来源：http://qoi.meibo888.top

P. 常用工具函数
来源：http://cyl.nanxuanxn.top

================================================================================
来源：http://lac.svipenyu.cn

[P01] 生成 UUID
来源：http://lgv.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://mji.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gtf.fengsongda.top

JS:   crypto.randomUUID()
来源：http://mei.xylfe.cn

TS:   crypto.randomUUID()
来源：http://mnb.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://gkp.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://rco.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://qdm.mhx1999.top


<!-- 参考信息 -->