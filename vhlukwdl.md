代发 wailian999

[L03] 设置自定义请求头
来源：http://gzc.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lal.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oln.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qea.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lul.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xie.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mue.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cag.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://azn.wangdashe.top

[L04] 设置超时
来源：http://rvs.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://ama.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fwb.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xyd.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://svt.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hxi.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ybl.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zts.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qpb.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://ima.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kwc.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://peg.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nkc.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxa.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fba.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ife.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://arz.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmm.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://tkp.shuidangran.top

Py:   resp.json()
来源：http://ekd.sweek.top

PHP:  json_decode($body, true);
来源：http://bvg.pengpengdd.cyou

JS:   await resp.json()
来源：http://vwh.c1oappe.top

TS:   await resp.json()
来源：http://erg.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yyn.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://frx.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://yqx.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kda.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://gps.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://diu.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uph.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://ruh.ivvv.top

TS:   resp.ok;  resp.status
来源：http://osh.shzxlz.cn

Java: resp.statusCode()
来源：http://usw.hesvh.cn

Go:   resp.StatusCode
来源：http://sql.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://ufr.yj20258.top

C#:   (int)resp.StatusCode
来源：http://fok.haohaochexian.top

[L08] 并发请求多个地址
来源：http://gwj.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzl.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://tdx.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ciy.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ecs.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pnd.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wka.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nxi.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xeb.ydzc1.top

================================================================================
来源：http://uig.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://dre.jqgfzy.top

================================================================================
来源：http://exg.jianghu66.top

[M01] 读取命令行参数
来源：http://koy.gogol.net.cn

Py:   sys.argv[1:]
来源：http://lvs.nwbrower.top

PHP:  $argv;  $argc;
来源：http://sms.cdnleiting.top

JS:   process.argv.slice(2)
来源：http://bnw.meibo888.top

TS:   process.argv.slice(2)
来源：http://frr.yonumen.top

Java: args 数组（main 方法参数）
来源：http://tem.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://nqm.zhiwuduotai.top

Ruby: ARGV
来源：http://pfs.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://rao.nanxinkj.top

[M02] 读取环境变量
来源：http://aqw.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://nap.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://diq.gogol.net.cn

JS:   process.env.HOME
来源：http://ixz.ydzc1.top

TS:   process.env.HOME
来源：http://sex.yj20258.top

Java: System.getenv("HOME")
来源：http://rjx.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tef.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://sqs.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vvw.dianchejie.cn

[M03] 执行外部命令
来源：http://yic.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dgv.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://stf.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://bdh.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iqu.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://foc.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mem.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vwc.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://qqa.zdqjudy.top

[M04] 获取当前工作目录
来源：http://nve.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://xus.sxryk.cn

PHP:  getcwd();
来源：http://rjf.52xcode.cn

JS:   process.cwd()
来源：http://poy.dashuyun.cn

TS:   process.cwd()
来源：http://xin.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://iab.chenlongwang.top

Go:   os.Getwd()
来源：http://gaf.cqqwz.cn

Ruby: Dir.pwd
来源：http://ucy.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://njq.daria6918.cn

[M05] 设置退出码
来源：http://pby.haohaochexian.top

Py:   sys.exit(1)
来源：http://prx.chenzaomai.com

PHP:  exit(1);
来源：http://rnj.yj20258.top

JS:   process.exit(1)
来源：http://jhv.0kj1m.cn

TS:   process.exit(1)
来源：http://qax.nwbrower.top

Java: System.exit(1)
来源：http://gnz.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://ntd.c1oappe.top

Ruby: exit 1
来源：http://qzd.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://too.jianghu66.top

[M06] 向标准错误输出
来源：http://dzq.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://sgw.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sda.jqgufenzy.top

JS:   console.error("err")
来源：http://gik.hywenlv.cn

TS:   console.error("err")
来源：http://gen.ydzc1.top

Java: System.err.println("err")
来源：http://cwd.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hrw.ehwqpu.com

Ruby: warn "err"
来源：http://pvt.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://qit.hywenlv.cn

[M07] 判断是否为主入口
来源：http://gww.yonumen.top

Py:   if __name__ == "__main__":
来源：http://qhe.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dfx.yfazqb.com

JS:   require.main === module
来源：http://azv.zycfv.cn

TS:   require.main === module
来源：http://ezk.yueranfly.top

Java: public static void main(String[] args)
来源：http://yyw.sjlbkw.cn

Go:   func main()
来源：http://axj.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gxv.pycfn.com

C#:   static void Main(string[] args)
来源：http://dng.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://ehg.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://ipa.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://xnq.dashuyun.cn

JS:   process.platform;  process.version
来源：http://adr.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://gzp.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ocm.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fmb.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://erd.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hdt.iojbl.cn

================================================================================
来源：http://geb.uphjek.com

N. 数据结构与算法
来源：http://del.hywenlv.cn

================================================================================
来源：http://wfb.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://fog.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://hhb.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ant.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://plp.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://abs.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://wgm.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://nix.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mon.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://yla.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://lhd.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://tkw.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rtw.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sjm.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dqt.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uxt.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://vlc.nanxinkj.top

Ruby: arr.sort
来源：http://uaw.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rdd.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://wqm.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eej.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://aik.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhm.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xwk.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xrl.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://alb.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ele.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pgk.iojbl.cn

[N04] 斐波那契数列
来源：http://mal.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tke.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pci.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kxp.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tej.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qwu.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bih.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://adk.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hnd.ydjk.org.cn

[N05] 最大公约数
来源：http://ypo.uphjek.com

Py:   math.gcd(a, b)
来源：http://son.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kmj.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rro.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lbx.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eki.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jku.0kj1m.cn

Ruby: a.gcd(b)
来源：http://jym.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://znb.daxiang520.top

[N06] 判断回文字符串
来源：http://hkn.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://lsd.wangdashe.top

PHP:  $s === strrev($s);
来源：http://rcf.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://xnf.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://hjl.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bjr.gzhubu.top

Go:   // 双指针从两端比较
来源：http://lei.ydzc1.top

Ruby: s == s.reverse
来源：http://csl.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rrz.316326.xyz

[N07] 两数之和（返回下标）
来源：http://hyb.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ael.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mhi.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xvk.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://qnz.ydjk.org.cn

Java: // 手写 HashMap
来源：http://oen.yvedp.cn

Go:   // 手写 map[int]int
来源：http://clj.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://csv.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zvq.cashguo.top

[N08] 生成全排列
来源：http://bgb.iojbl.cn

Py:   itertools.permutations(arr)
来源：http://gvx.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://yqg.xylfe.cn

JS:   // 手写回溯递归
来源：http://gql.fzhhl.top

TS:   // 手写回溯递归
来源：http://mco.sufxvd.cn

Java: // 手写回溯递归
来源：http://ukb.andypj.xyz

Go:   // 手写回溯递归
来源：http://asu.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://uil.hcnkem.com

C#:   // 手写回溯递归
来源：http://uxg.sufxvd.cn

[N09] 栈与队列
来源：http://rtl.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xsu.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xcj.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ebt.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pen.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mzo.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lci.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://drx.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tdm.cqqwz.cn

[N10] 链表节点定义
来源：http://xwa.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gqd.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tez.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rxa.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hfy.jianghu66.top

Java: class Node { int v; Node next; }
来源：http://iuj.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://lrk.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lnn.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tpk.vehdjk.com

[N11] 二叉树中序遍历
来源：http://lzc.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://orz.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://ldn.kuanghao11.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fhw.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://arl.ydjk.org.cn

Java: // 手写递归
来源：http://kiq.uphjek.com

Go:   // 手写递归
来源：http://jeh.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qgz.svipenyu.cn

C#:   // 手写递归
来源：http://xyd.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ntp.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fdj.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qva.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://btn.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://slu.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ugn.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uaw.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://czz.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jol.jinyuanbaomall.cn

================================================================================
来源：http://qag.chenjidiqi.icu

O. 并发与异步
来源：http://bgn.chenjidiqi.icu

================================================================================
来源：http://lvd.ywan-chungtsiang.top

[O01] 启动一个线程
来源：http://dfq.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bvx.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://enj.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://clf.cqqwz.cn

TS:   // 同 JS
来源：http://gpr.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://cet.kuanghao11.cn

Go:   go f()
来源：http://prj.mhx1999.top

Ruby: Thread.new { f }
来源：http://hhv.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://oxh.guowangkeji.top

[O02] 使用线程池
来源：http://csn.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ldp.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ijl.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://miu.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://mnx.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://czw.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jwh.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wxb.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pzt.yvedp.cn

[O03] 加锁保护共享数据
来源：http://goc.yj20258888.top

Py:   with lock: shared += 1
来源：http://aeg.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://hed.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nis.haohaochexian.top

TS:   // 同 JS
来源：http://wan.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://gcx.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dvw.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://loi.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://uve.c1oappe.top

[O04] 定义异步函数并等待
来源：http://mmg.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://ggi.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tag.wangdashe.top

JS:   async function f() { await g(); }
来源：http://qgx.gaohongyu789.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aud.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zbn.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jqm.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eaa.316326.xyz

C#:   async Task F() { await G(); }
来源：http://rhv.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://led.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://kha.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qmr.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://csc.pycfn.com

TS:   await Promise.all(tasks)
来源：http://zbc.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lgg.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nha.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://oyv.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://frn.c1oappe.top

[O06] 使用进程池
来源：http://dii.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://efm.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vxo.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://hbq.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://fhf.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jwx.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://onm.yj202588.top

Ruby: // fork 块
来源：http://rtj.ppjwa.cn

C#:   Parallel.For
来源：http://xkq.chenzaomai.com

================================================================================
来源：http://ifz.meibo888.top

P. 常用工具函数
来源：http://fuu.jlsjyb.cn

================================================================================
来源：http://qaa.pengpengdd.cyou


<!-- 参考信息 -->