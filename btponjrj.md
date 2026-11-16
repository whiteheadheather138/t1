代发 wailian999

[L03] 设置自定义请求头
来源：http://bhz.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jck.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mce.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zxc.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fyk.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pny.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tar.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zlr.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dew.hnxiangtu.top

[L04] 设置超时
来源：http://mgx.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://fgh.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xyc.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kti.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jip.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://egy.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lmi.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ezn.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yph.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://vwp.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://krl.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zbn.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nvh.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zyw.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rsd.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jkq.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wjr.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hie.daria6918.cn

[L06] 解析响应为 JSON
来源：http://ori.tanke756.top

Py:   resp.json()
来源：http://hbk.guannengcc.top

PHP:  json_decode($body, true);
来源：http://pic.iojbl.cn

JS:   await resp.json()
来源：http://obs.shzxlz.cn

TS:   await resp.json()
来源：http://jjd.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kcd.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oeb.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://vxp.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cke.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://ppa.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tzg.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dkh.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://lph.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://wxf.xziqi.cn

Java: resp.statusCode()
来源：http://hzg.hesvh.cn

Go:   resp.StatusCode
来源：http://tpi.andypj.xyz

Ruby: resp.code.to_i
来源：http://xpz.316326.xyz

C#:   (int)resp.StatusCode
来源：http://trb.dianchejie.cn

[L08] 并发请求多个地址
来源：http://dzl.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fxw.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://maw.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://icy.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://myd.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jry.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wzc.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://opj.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vgg.yonumen.top

================================================================================
来源：http://wzd.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://stc.sweek.top

================================================================================
来源：http://aku.zhengqikj.top

[M01] 读取命令行参数
来源：http://seh.bjfxy.top

Py:   sys.argv[1:]
来源：http://sld.nwbrower.top

PHP:  $argv;  $argc;
来源：http://rfu.aizwys.cn

JS:   process.argv.slice(2)
来源：http://bzm.yongpay.top

TS:   process.argv.slice(2)
来源：http://ulx.ivvv.top

Java: args 数组（main 方法参数）
来源：http://zva.zhongyouzk.top

Go:   os.Args[1:]
来源：http://hls.jinghuilouyu.cn

Ruby: ARGV
来源：http://mmq.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://htr.tianlin.xyz

[M02] 读取环境变量
来源：http://weo.meibo888.top

Py:   os.environ.get("HOME")
来源：http://kjk.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://als.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://lzm.cucudq.cn

TS:   process.env.HOME
来源：http://ikk.xuanzx.com

Java: System.getenv("HOME")
来源：http://cfp.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://utd.tarul.cn

Ruby: ENV["HOME"]
来源：http://fgw.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bjp.yuanzhike.top

[M03] 执行外部命令
来源：http://ufi.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://huz.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fuy.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dnw.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://idq.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xwh.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://iws.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fwn.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://fhv.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://itp.andypj.xyz

Py:   os.getcwd()
来源：http://gjd.cdnleiting.top

PHP:  getcwd();
来源：http://ybx.bjfxy.top

JS:   process.cwd()
来源：http://kwb.daria6918.cn

TS:   process.cwd()
来源：http://mkb.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://fsx.yvedp.cn

Go:   os.Getwd()
来源：http://frl.hcnkem.com

Ruby: Dir.pwd
来源：http://ofr.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://kef.ydjk.org.cn

[M05] 设置退出码
来源：http://itk.meibo888.top

Py:   sys.exit(1)
来源：http://mnp.yj20258888.top

PHP:  exit(1);
来源：http://yrr.tianlin.xyz

JS:   process.exit(1)
来源：http://vve.kuanghao11.cn

TS:   process.exit(1)
来源：http://yxg.sweek.top

Java: System.exit(1)
来源：http://kcn.andypj.xyz

Go:   os.Exit(1)
来源：http://irx.yuanzhike.top

Ruby: exit 1
来源：http://hxo.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wkq.vqdsnc.cn

[M06] 向标准错误输出
来源：http://qix.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://jhy.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://qyi.yueranfly.top

JS:   console.error("err")
来源：http://whv.kuanghao11.cn

TS:   console.error("err")
来源：http://pdt.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://ija.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gzv.tanke756.top

Ruby: warn "err"
来源：http://oyq.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://cse.sufxvd.cn

[M07] 判断是否为主入口
来源：http://cst.yj20258.top

Py:   if __name__ == "__main__":
来源：http://gfh.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://awc.yj20258.top

JS:   require.main === module
来源：http://ykt.havefunace.top

TS:   require.main === module
来源：http://ssp.ydzc1.top

Java: public static void main(String[] args)
来源：http://fgi.yj202588.top

Go:   func main()
来源：http://fil.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sqj.yongpay.top

C#:   static void Main(string[] args)
来源：http://xqv.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://mbj.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://cla.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://qlg.yongpay.top

JS:   process.platform;  process.version
来源：http://dwp.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://frc.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zyc.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://efs.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baw.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hrs.jqgfzy.top

================================================================================
来源：http://fix.jinqigufen.top

N. 数据结构与算法
来源：http://dqn.yvedp.cn

================================================================================
来源：http://kzx.tanke756.top

[N01] 二分查找（有序数组）
来源：http://aco.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nab.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lbl.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vme.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rge.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://pdo.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://fke.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gzf.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yxy.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://hze.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://bvl.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jag.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pkb.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ofr.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zsu.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://efp.feifeiyinyue.top

Ruby: arr.sort
来源：http://bdf.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://css.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://wgq.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://muq.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://xst.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://htl.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cfg.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vrg.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wnb.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xhg.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zyi.hammf.cn

[N04] 斐波那契数列
来源：http://acf.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vvk.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://siq.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acu.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rgv.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ems.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pdj.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://byq.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wdo.yj20258.top

[N05] 最大公约数
来源：http://mgv.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://qhi.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wss.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkh.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://clb.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zup.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ulu.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://pcc.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sab.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://gww.gogol.net.cn

Py:   s == s[::-1]
来源：http://akh.hnqzz.top

PHP:  $s === strrev($s);
来源：http://eri.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://vym.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://ydr.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://edi.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://fht.quarkkingdee.top

Ruby: s == s.reverse
来源：http://tja.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ios.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://txt.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kot.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ybe.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hfi.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://dqo.quarkkingdee.top

Java: // 手写 HashMap
来源：http://smv.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://hkt.0kj1m.cn

Ruby: // 手写 Hash
来源：http://bcf.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://sww.fzhhl.top

[N08] 生成全排列
来源：http://vuo.316326.xyz

Py:   itertools.permutations(arr)
来源：http://zia.haohaochexian.top

PHP:  // 手写递归交换
来源：http://pco.bbcook.cn

JS:   // 手写回溯递归
来源：http://yqh.hysaishi.cn

TS:   // 手写回溯递归
来源：http://ldf.jiagoushi.top

Java: // 手写回溯递归
来源：http://gjs.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://ppt.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://nun.ybcxt.top

C#:   // 手写回溯递归
来源：http://mmh.shzxlz.cn

[N09] 栈与队列
来源：http://oev.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ejx.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vuf.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wqu.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dlu.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wuk.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jzw.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fro.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rvj.fktsv.cn

[N10] 链表节点定义
来源：http://csh.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iti.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cqx.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rrp.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://swj.cashguo.top

Java: class Node { int v; Node next; }
来源：http://cbk.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://jcv.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://asq.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vmo.52xcode.cn

[N11] 二叉树中序遍历
来源：http://sle.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://acb.tarul.cn

PHP:  // 手写递归函数
来源：http://fya.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ezy.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lvx.sufxvd.cn

Java: // 手写递归
来源：http://rth.ybcxt.top

Go:   // 手写递归
来源：http://bog.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://peo.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://qde.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nok.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ynw.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bvk.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dhm.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmp.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wwg.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wip.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tva.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hif.gogol.net.cn

================================================================================
来源：http://myk.ywan-chungtsiang.top

O. 并发与异步
来源：http://cyc.yvedp.cn

================================================================================
来源：http://ewy.jiagoushi.top

[O01] 启动一个线程
来源：http://cxc.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wcx.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ubn.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fhb.yj20258888.top

TS:   // 同 JS
来源：http://unl.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://mfq.xingfuxueyuan.xyz

Go:   go f()
来源：http://dsv.guowangkeji.top

Ruby: Thread.new { f }
来源：http://zsm.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://iha.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://dsz.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mgy.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pbd.yvedp.cn

JS:   // worker_threads 线程池
来源：http://qmm.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://ged.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://rwc.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mpj.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ngq.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rbo.sxryk.cn

[O03] 加锁保护共享数据
来源：http://hrs.ehwqpu.com

Py:   with lock: shared += 1
来源：http://izz.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://xac.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uck.jiagoushi.top

TS:   // 同 JS
来源：http://yzu.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://bvo.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rqp.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://viu.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://jnr.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://iue.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://hnn.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uqx.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://ile.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://wwg.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bix.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bds.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rtx.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://amm.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://wfq.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://pay.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cuj.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://ngp.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://yel.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://daf.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://htd.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://mbf.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ixh.kuanghao11.cn

[O06] 使用进程池
来源：http://jmi.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mdl.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://htl.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://sie.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://mqa.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wyt.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dgg.0kj1m.cn

Ruby: // fork 块
来源：http://ukk.sjlbkw.cn

C#:   Parallel.For
来源：http://foi.haohaochexian.top

================================================================================
来源：http://gcv.xylfe.cn

P. 常用工具函数
来源：http://opo.wangshuangyany.cn

================================================================================
来源：http://tlh.gaohongyu789.top


<!-- 参考信息 -->