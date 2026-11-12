代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qye.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jwi.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bbq.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://due.hysaishi.cn

[L03] 设置自定义请求头
来源：http://zeh.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://itw.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tda.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://usn.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://psi.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lfy.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yxf.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kuq.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yhz.andypj.xyz

[L04] 设置超时
来源：http://iwm.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://uvw.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hyb.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dts.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ein.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nxq.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://giy.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ztg.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mni.xylfe.cn

[L05] 上传文件（multipart）
来源：http://ekt.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yyi.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xpw.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gpf.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kkt.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rdm.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ldx.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hmi.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sco.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://vpt.aizwys.cn

Py:   resp.json()
来源：http://mfe.316326.xyz

PHP:  json_decode($body, true);
来源：http://hsx.vqdsnc.cn

JS:   await resp.json()
来源：http://uyx.ydzc1.top

TS:   await resp.json()
来源：http://sty.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hxj.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gne.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://rsc.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lmb.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://srv.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ute.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gpp.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://jsh.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://iuz.aizwys.cn

Java: resp.statusCode()
来源：http://yih.9152youxi.cn

Go:   resp.StatusCode
来源：http://svb.guowangkeji.top

Ruby: resp.code.to_i
来源：http://swm.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://jhb.uphjek.com

[L08] 并发请求多个地址
来源：http://huq.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jsx.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://bof.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kip.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eav.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jvx.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyo.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lpg.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajn.zdqjudy.top

================================================================================
来源：http://wsb.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://liu.xylfe.cn

================================================================================
来源：http://qqa.sxryk.cn

[M01] 读取命令行参数
来源：http://xyw.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://gaw.sjlbkw.cn

PHP:  $argv;  $argc;
来源：http://ljz.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://opr.cheryme.top

TS:   process.argv.slice(2)
来源：http://tdo.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://stj.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://kms.yangfankeji.com

Ruby: ARGV
来源：http://uje.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://diu.zhiwuduotai.top

[M02] 读取环境变量
来源：http://krk.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://sqa.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lcn.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://wmv.nwbrower.top

TS:   process.env.HOME
来源：http://kur.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://bvv.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pbl.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://ljg.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wrw.chenlongwang.top

[M03] 执行外部命令
来源：http://tcp.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pse.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xvz.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://imk.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cpy.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yjy.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://daw.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rtg.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://koh.c1oappe.top

[M04] 获取当前工作目录
来源：http://cqp.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://yzi.mhx1999.top

PHP:  getcwd();
来源：http://waa.guannengcc.top

JS:   process.cwd()
来源：http://eii.kuanghao11.cn

TS:   process.cwd()
来源：http://pbj.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://rod.bbcook.cn

Go:   os.Getwd()
来源：http://azt.zycfv.cn

Ruby: Dir.pwd
来源：http://num.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fpz.pycfn.com

[M05] 设置退出码
来源：http://aay.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://dju.zdbjq.cn

PHP:  exit(1);
来源：http://twe.haohaochexian.top

JS:   process.exit(1)
来源：http://ydr.sysykeji.top

TS:   process.exit(1)
来源：http://ibt.smart0.xyz

Java: System.exit(1)
来源：http://teh.hnxiangtu.top

Go:   os.Exit(1)
来源：http://dqi.wangdashe.top

Ruby: exit 1
来源：http://kqr.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nyk.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://jec.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://hpm.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://omk.chenzaomai.com

JS:   console.error("err")
来源：http://tsv.yfazqb.com

TS:   console.error("err")
来源：http://sdm.guowangkeji.top

Java: System.err.println("err")
来源：http://tnl.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xxl.xinyue.icu

Ruby: warn "err"
来源：http://xwo.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://jin.tian-w.cn

[M07] 判断是否为主入口
来源：http://hqi.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://zmr.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zow.gogol.net.cn

JS:   require.main === module
来源：http://cxm.yj20258.top

TS:   require.main === module
来源：http://uim.sysykeji.top

Java: public static void main(String[] args)
来源：http://wxw.sysykeji.top

Go:   func main()
来源：http://sfy.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wdh.fehbvm.com

C#:   static void Main(string[] args)
来源：http://dgh.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://zbk.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://apd.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://hml.smart0.xyz

JS:   process.platform;  process.version
来源：http://lfe.cashguo.top

TS:   process.platform;  process.version
来源：http://dco.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ttq.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sng.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lop.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lwk.fengsongda.top

================================================================================
来源：http://hjo.hongshengwenyu.top

N. 数据结构与算法
来源：http://cfl.zhoulong.xyz

================================================================================
来源：http://mak.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://bre.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://hxu.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kka.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwi.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlk.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qrr.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://qyu.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xip.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://wtf.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://euc.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://hwa.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wbh.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uye.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://slq.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kvq.meibo888.top

Go:   slices.Sort(arr)
来源：http://qal.0kj1m.cn

Ruby: arr.sort
来源：http://kvb.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rpg.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://uwd.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fzi.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://rzb.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://enl.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unu.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wkp.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zdd.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mwp.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zkb.hnxiangtu.top

[N04] 斐波那契数列
来源：http://vdi.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ipz.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yxw.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ntd.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gdz.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ksr.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lqm.tarul.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rtu.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mst.aizwys.cn

[N05] 最大公约数
来源：http://jvl.fzhhl.top

Py:   math.gcd(a, b)
来源：http://hct.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gyx.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxn.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ztu.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ofd.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rjn.cheryme.top

Ruby: a.gcd(b)
来源：http://grh.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xrp.cashguo.top

[N06] 判断回文字符串
来源：http://mje.zdqjudy.top

Py:   s == s[::-1]
来源：http://eot.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://zut.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://xvm.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://cmf.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bka.yueranfly.top

Go:   // 双指针从两端比较
来源：http://tit.iojbl.cn

Ruby: s == s.reverse
来源：http://pjs.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://enl.tanke756.top

[N07] 两数之和（返回下标）
来源：http://tmq.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nlz.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jyr.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xdv.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://lye.kuanghao11.cn

Java: // 手写 HashMap
来源：http://bjm.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://wxz.smart0.xyz

Ruby: // 手写 Hash
来源：http://dms.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://amw.hnqzz.top

[N08] 生成全排列
来源：http://yzp.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://woj.tianlin.xyz

PHP:  // 手写递归交换
来源：http://krm.gotoacloud.top

JS:   // 手写回溯递归
来源：http://uyk.ydzc1.top

TS:   // 手写回溯递归
来源：http://ndj.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://vey.yvedp.cn

Go:   // 手写回溯递归
来源：http://pjj.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://ojq.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://urb.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://usr.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://utx.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lft.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hja.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yga.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uwe.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jnx.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://idx.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ytu.yongpay.top

[N10] 链表节点定义
来源：http://ugu.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fcp.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vrl.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://orc.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://giv.cashguo.top

Java: class Node { int v; Node next; }
来源：http://vix.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bvi.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://xnc.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://idg.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://rwt.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://onb.aizwys.cn

PHP:  // 手写递归函数
来源：http://jey.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qlt.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uye.vehdjk.com

Java: // 手写递归
来源：http://jkm.yj202588.top

Go:   // 手写递归
来源：http://nqf.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hyo.ctjpmb.com

C#:   // 手写递归
来源：http://gfg.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ttt.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://svn.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hed.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aww.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rla.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wsv.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mxv.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qzv.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qek.smart0.xyz

================================================================================
来源：http://fey.zhengqikj.top

O. 并发与异步
来源：http://hfy.jiagoushi.top

================================================================================
来源：http://jnm.fehbvm.com

[O01] 启动一个线程
来源：http://jgj.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ccj.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zuv.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qtu.cdnleiting.top

TS:   // 同 JS
来源：http://cnu.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://uvs.bjfxy.top

Go:   go f()
来源：http://wiw.xinyue.icu

Ruby: Thread.new { f }
来源：http://tjb.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://trg.yj20258.top

[O02] 使用线程池
来源：http://pyb.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hox.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rhs.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://vmk.andypj.xyz

TS:   // worker_threads 线程池
来源：http://orh.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wrx.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jyg.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pvk.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jyc.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://iae.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://vie.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://kqv.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://emp.daria6918.cn

TS:   // 同 JS
来源：http://zhs.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://jxr.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://amh.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vma.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://qpf.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://nvp.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://dxg.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yug.guannengcc.top

JS:   async function f() { await g(); }
来源：http://xds.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xix.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qbo.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pct.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://mnz.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://jtt.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://rpz.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://pyc.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ffo.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://ivj.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://gki.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yut.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ztp.ivvv.top

Ruby: threads.map(&:join)
来源：http://zkj.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fgb.sufxvd.cn

[O06] 使用进程池
来源：http://hwj.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adr.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tdv.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://iph.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://ofr.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://shm.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ztd.kuanghao11.cn

Ruby: // fork 块
来源：http://per.jiagoushi.top


<!-- 参考信息 -->