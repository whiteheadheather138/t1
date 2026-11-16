代发 wailian999

[L03] 设置自定义请求头
来源：http://dyn.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://epv.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://awe.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lzh.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ina.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pnd.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://csh.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfy.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ssg.xylfe.cn

[L04] 设置超时
来源：http://nam.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://mbx.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://avf.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ayk.nanxuanxn.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cfv.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mju.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://psw.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wtz.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rsh.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://pgu.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rfn.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uyt.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vuo.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qsb.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://guf.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://smf.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ekl.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ulv.ydzc1.top

[L06] 解析响应为 JSON
来源：http://eko.jlsjyb.cn

Py:   resp.json()
来源：http://czc.andypj.xyz

PHP:  json_decode($body, true);
来源：http://eju.zdbjq.cn

JS:   await resp.json()
来源：http://pmf.ydjk.org.cn

TS:   await resp.json()
来源：http://ajw.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ssh.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gwi.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://dyr.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qqs.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://nke.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dbw.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://drw.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://wuc.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://lgq.yonumen.top

Java: resp.statusCode()
来源：http://ukh.yvedp.cn

Go:   resp.StatusCode
来源：http://ten.shuidangran.top

Ruby: resp.code.to_i
来源：http://yan.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://lpz.andypj.xyz

[L08] 并发请求多个地址
来源：http://zzz.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://frh.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://kxl.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lhi.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kth.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iud.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rva.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rla.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eyl.jinqigufen.top

================================================================================
来源：http://nym.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://rdb.tarul.cn

================================================================================
来源：http://kop.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://idr.havefunace.top

Py:   sys.argv[1:]
来源：http://gwn.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://jhp.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://mnq.yongpay.top

TS:   process.argv.slice(2)
来源：http://nyv.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://ske.uphjek.com

Go:   os.Args[1:]
来源：http://glm.yuxming.cn

Ruby: ARGV
来源：http://sfn.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://eou.fktsv.cn

[M02] 读取环境变量
来源：http://egr.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://dwb.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eyp.yj20258.top

JS:   process.env.HOME
来源：http://oug.zhengqikj.top

TS:   process.env.HOME
来源：http://nqq.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://afu.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dss.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://jpt.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zvg.aizwys.cn

[M03] 执行外部命令
来源：http://nkn.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fvx.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://azw.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://icr.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wst.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://onm.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kzn.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://tsc.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://jsq.cucudq.cn

[M04] 获取当前工作目录
来源：http://qrj.nanxuanxn.top

Py:   os.getcwd()
来源：http://odk.xuetiantiany.cn

PHP:  getcwd();
来源：http://leh.zhixingplan.top

JS:   process.cwd()
来源：http://dlv.gaohongyu789.top

TS:   process.cwd()
来源：http://yqg.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://iog.zdqjudy.top

Go:   os.Getwd()
来源：http://dav.hfpthk.cn

Ruby: Dir.pwd
来源：http://rfi.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://qwb.kuanghao11.cn

[M05] 设置退出码
来源：http://xcp.jiagoushi.top

Py:   sys.exit(1)
来源：http://xbc.fehbvm.com

PHP:  exit(1);
来源：http://jul.zhengqikj.top

JS:   process.exit(1)
来源：http://vnv.tian-w.cn

TS:   process.exit(1)
来源：http://ucb.yanxiufei.cn

Java: System.exit(1)
来源：http://irw.xinyue.icu

Go:   os.Exit(1)
来源：http://hdy.ehwqpu.com

Ruby: exit 1
来源：http://ows.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ero.ydzc1.top

[M06] 向标准错误输出
来源：http://gbw.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://izd.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vvp.jlsjyb.cn

JS:   console.error("err")
来源：http://ick.tarul.cn

TS:   console.error("err")
来源：http://yyw.jianghu66.top

Java: System.err.println("err")
来源：http://zvg.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ook.chenzaomai.com

Ruby: warn "err"
来源：http://hcy.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://opd.yangfankeji.com

[M07] 判断是否为主入口
来源：http://wmk.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://ygj.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xhm.cheryme.top

JS:   require.main === module
来源：http://bqc.gotoacloud.top

TS:   require.main === module
来源：http://ogq.dashuyun.cn

Java: public static void main(String[] args)
来源：http://jcb.yfazqb.com

Go:   func main()
来源：http://xuc.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mla.sxryk.cn

C#:   static void Main(string[] args)
来源：http://nuf.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://weu.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://ooi.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xmb.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://uaf.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://qwf.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qqe.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qhw.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kzh.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kfe.snrcjt.cn

================================================================================
来源：http://nvo.hesvh.cn

N. 数据结构与算法
来源：http://rhv.hesvh.cn

================================================================================
来源：http://kuz.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://zvi.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aqp.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wgs.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ant.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dqu.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://blf.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://zcq.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ndf.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fto.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://cfo.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://hbe.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tsu.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pkc.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kot.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nkg.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://jor.fehbvm.com

Ruby: arr.sort
来源：http://roa.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rjz.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://aow.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://egm.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://ggc.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xia.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwz.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ldu.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mwb.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uey.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://mhw.yueranfly.top

[N04] 斐波那契数列
来源：http://alz.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bla.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lnw.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://anb.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lig.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cbn.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pmg.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uzv.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vhe.cucudq.cn

[N05] 最大公约数
来源：http://kjh.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://ipg.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zfa.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cys.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vbd.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fwd.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oml.gotoacloud.top

Ruby: a.gcd(b)
来源：http://zaq.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://frr.yuxming.cn

[N06] 判断回文字符串
来源：http://dfm.sjlbkw.cn

Py:   s == s[::-1]
来源：http://ifg.316326.xyz

PHP:  $s === strrev($s);
来源：http://jia.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://dcv.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://cmw.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gzf.shuidangran.top

Go:   // 双指针从两端比较
来源：http://svh.52xcode.cn

Ruby: s == s.reverse
来源：http://els.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zqx.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://tty.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xvo.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hwk.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cbc.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://pfe.birdmap.top

Java: // 手写 HashMap
来源：http://gwf.sxryk.cn

Go:   // 手写 map[int]int
来源：http://aev.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://qyk.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ufx.ppjwa.cn

[N08] 生成全排列
来源：http://ipq.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://qnm.birdmap.top

PHP:  // 手写递归交换
来源：http://eex.hysaishi.cn

JS:   // 手写回溯递归
来源：http://yot.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://pyi.meibo888.top

Java: // 手写回溯递归
来源：http://dul.havefunace.top

Go:   // 手写回溯递归
来源：http://bll.yj20258.top

Ruby: arr.permutation.to_a
来源：http://iux.andypj.xyz

C#:   // 手写回溯递归
来源：http://kyf.sjlbkw.cn

[N09] 栈与队列
来源：http://sex.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rpq.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xig.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ezr.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gny.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cpo.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxb.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wgu.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gxz.jqgufenzy.top

[N10] 链表节点定义
来源：http://uvi.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nxc.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://owp.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fnk.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ush.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://wsp.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://mux.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kjm.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://myz.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://glm.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tgd.fktsv.cn

PHP:  // 手写递归函数
来源：http://rdz.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://etg.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yys.andypj.xyz

Java: // 手写递归
来源：http://vpk.xuetiantiany.cn

Go:   // 手写递归
来源：http://fea.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rod.9152youxi.cn

C#:   // 手写递归
来源：http://pfd.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rjp.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xfb.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://goa.fengsongda.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lfb.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://olm.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ewm.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baa.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nij.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lsz.yj202588.top

================================================================================
来源：http://aba.yuanzhike.top

O. 并发与异步
来源：http://weh.gogol.net.cn

================================================================================
来源：http://ttc.hongshengwenyu.top

[O01] 启动一个线程
来源：http://scu.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eoh.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://psl.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zhj.xziqi.cn

TS:   // 同 JS
来源：http://vpt.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://gcl.shuidangran.top

Go:   go f()
来源：http://mzo.tarul.cn

Ruby: Thread.new { f }
来源：http://tut.guannengcc.top

C#:   Task.Run(() => F());
来源：http://vej.yuxming.cn

[O02] 使用线程池
来源：http://ouq.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://khn.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pte.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://dcr.ydzc1.top

TS:   // worker_threads 线程池
来源：http://ndz.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gli.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abf.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ood.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mho.iojbl.cn

[O03] 加锁保护共享数据
来源：http://nqp.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://xak.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://snt.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ktl.guowangkeji.top

TS:   // 同 JS
来源：http://hjc.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://iix.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fjt.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nxy.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://muc.hammf.cn

[O04] 定义异步函数并等待
来源：http://znl.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://bgl.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://muu.cheryme.top

JS:   async function f() { await g(); }
来源：http://xnv.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mck.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mjt.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nen.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mrt.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://cwp.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://vvf.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://nlo.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rnc.sweek.top

JS:   await Promise.all(tasks)
来源：http://kpz.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://moz.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uwc.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dzh.ivvv.top

Ruby: threads.map(&:join)
来源：http://fnk.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fcu.ydjk.org.cn

[O06] 使用进程池
来源：http://ohw.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yar.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wyb.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://mvf.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://and.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pro.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zuz.shangyingyoupin.top

Ruby: // fork 块
来源：http://hvd.yj20258.top

C#:   Parallel.For
来源：http://ifp.yongpay.top

================================================================================
来源：http://psa.xylfe.cn

P. 常用工具函数
来源：http://buc.zhongyouzk.top

================================================================================
来源：http://ydq.zhaomingkeji.xyz


<!-- 参考信息 -->