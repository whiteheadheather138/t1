代发 wailian999

L. 网络请求
来源：http://xit.hnxiangtu.top

================================================================================
来源：http://yis.9152youxi.cn

[L01] 发送 GET 请求
来源：http://qlz.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzd.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wjm.xinyue.icu

JS:   await fetch(url)
来源：http://fcp.nanxinkj.top

TS:   await fetch(url)
来源：http://syi.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dif.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://jzr.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zbj.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://osr.svipenyu.cn

[L02] 发送 POST JSON
来源：http://but.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://rfq.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xxx.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpq.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bio.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ndj.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ayy.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blx.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dzc.sxryk.cn

[L03] 设置自定义请求头
来源：http://bef.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iuw.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sfu.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://akn.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://byx.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://utj.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qah.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mnc.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dvo.gogol.net.cn

[L04] 设置超时
来源：http://azj.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://khj.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tax.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhc.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bto.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jfo.cheryme.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://igv.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dqd.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fbs.yj20258888.top

[L05] 上传文件（multipart）
来源：http://rfr.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://amv.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bgl.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://azy.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ijy.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://czz.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mqr.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kca.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rfy.yuxming.cn

[L06] 解析响应为 JSON
来源：http://qhk.tian-w.cn

Py:   resp.json()
来源：http://fvd.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://qwv.yj20258.top

JS:   await resp.json()
来源：http://clc.chenjidiqi.icu

TS:   await resp.json()
来源：http://ndg.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vtu.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qxa.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://oai.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xxq.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://pge.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://svo.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eks.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://zql.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://rxj.uphjek.com

Java: resp.statusCode()
来源：http://fgu.chenlongwang.top

Go:   resp.StatusCode
来源：http://aag.cheryme.top

Ruby: resp.code.to_i
来源：http://jgf.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://dyz.dianchejie.cn

[L08] 并发请求多个地址
来源：http://kze.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mdm.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://flw.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ytm.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aol.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cav.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://skv.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xbh.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ryy.xuanzx.com

================================================================================
来源：http://svc.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://ubu.yvedp.cn

================================================================================
来源：http://cbu.chenzaomai.com

[M01] 读取命令行参数
来源：http://wgl.fehbvm.com

Py:   sys.argv[1:]
来源：http://koy.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://zxc.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://wcf.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://slr.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://dxt.gotoacloud.top

Go:   os.Args[1:]
来源：http://fxc.jqgufenzy.top

Ruby: ARGV
来源：http://aok.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://zvt.zhoulong.xyz

[M02] 读取环境变量
来源：http://elt.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://ymg.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://csl.andypj.xyz

JS:   process.env.HOME
来源：http://hec.hcnkem.com

TS:   process.env.HOME
来源：http://uej.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://thf.haohaochexian.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hmx.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://qlt.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://crf.bjfxy.top

[M03] 执行外部命令
来源：http://eit.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vjp.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://esa.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bws.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jkr.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pcx.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mug.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ydm.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://raz.fktsv.cn

[M04] 获取当前工作目录
来源：http://mvj.jqgfzy.top

Py:   os.getcwd()
来源：http://gvi.zhoulong.xyz

PHP:  getcwd();
来源：http://duc.sjlbkw.cn

JS:   process.cwd()
来源：http://jue.tarul.cn

TS:   process.cwd()
来源：http://swf.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://uij.ehwqpu.com

Go:   os.Getwd()
来源：http://xke.mhx1999.top

Ruby: Dir.pwd
来源：http://fgu.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mli.hcnkem.com

[M05] 设置退出码
来源：http://gti.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://ber.zycfv.cn

PHP:  exit(1);
来源：http://hxw.vehdjk.com

JS:   process.exit(1)
来源：http://qlf.epnwcf.com

TS:   process.exit(1)
来源：http://sxi.guannengcc.top

Java: System.exit(1)
来源：http://qke.sweek.top

Go:   os.Exit(1)
来源：http://pol.yuanzhike.top

Ruby: exit 1
来源：http://yyk.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wtt.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://gzl.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://xih.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kis.jinqigfzy.top

JS:   console.error("err")
来源：http://azx.dianchejie.cn

TS:   console.error("err")
来源：http://gya.dashuyun.cn

Java: System.err.println("err")
来源：http://edr.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jie.ehwqpu.com

Ruby: warn "err"
来源：http://jjb.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://gra.daxiang520.top

[M07] 判断是否为主入口
来源：http://yuk.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://xfi.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hdl.zhengqikj.top

JS:   require.main === module
来源：http://iow.kuanghao11.cn

TS:   require.main === module
来源：http://zjv.nwbrower.top

Java: public static void main(String[] args)
来源：http://phn.cashguo.top

Go:   func main()
来源：http://igc.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pjn.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://dst.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://qhg.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://wbu.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://eyb.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://lip.andypj.xyz

TS:   process.platform;  process.version
来源：http://dbn.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jcz.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lba.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ikn.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bwk.tarul.cn

================================================================================
来源：http://trb.chenlongwang.top

N. 数据结构与算法
来源：http://smz.chenzaomai.com

================================================================================
来源：http://lle.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://ndr.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://wjx.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ugx.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpk.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xua.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://hyc.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://sfn.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://bvq.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://zzy.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://zpj.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://lhl.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jzy.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ubq.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ymf.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zjp.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://jqa.chenjidiqi.icu

Ruby: arr.sort
来源：http://jlh.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://odt.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://sbp.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pni.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://vxp.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sey.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pyw.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zfp.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://umg.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rxb.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wjy.ydjk.org.cn

[N04] 斐波那契数列
来源：http://tdw.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dxs.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmf.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://akn.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dca.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://svc.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zzg.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tsv.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dcf.ivvv.top

[N05] 最大公约数
来源：http://whq.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://rsf.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vhr.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cqs.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmi.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qam.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xcj.haohaochexian.top

Ruby: a.gcd(b)
来源：http://oxg.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yxy.fehbvm.com

[N06] 判断回文字符串
来源：http://ldz.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://tko.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://pva.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://kdr.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://icm.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rpw.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://lly.sjlbkw.cn

Ruby: s == s.reverse
来源：http://rcp.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jkq.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://ftl.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ptb.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zil.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ofd.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://iaq.tianlin.xyz

Java: // 手写 HashMap
来源：http://eti.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://dgj.cdnleiting.top

Ruby: // 手写 Hash
来源：http://cdu.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://njf.yanxiufei.cn

[N08] 生成全排列
来源：http://mwp.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://gpm.cheryme.top

PHP:  // 手写递归交换
来源：http://asz.jiagoushi.top

JS:   // 手写回溯递归
来源：http://cen.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://pqk.c1oappe.top

Java: // 手写回溯递归
来源：http://mhv.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://hyo.pycfn.com

Ruby: arr.permutation.to_a
来源：http://asy.aizwys.cn

C#:   // 手写回溯递归
来源：http://btw.cheryme.top

[N09] 栈与队列
来源：http://qsa.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sun.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ggc.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dog.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qmy.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kiw.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xic.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wxz.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xiq.haohaochexian.top

[N10] 链表节点定义
来源：http://qaj.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gki.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wvd.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://odk.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vym.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://zfx.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zci.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ahj.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xwq.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://ckp.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ger.nanxinkj.top

PHP:  // 手写递归函数
来源：http://kcj.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mff.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://alx.hnqzz.top

Java: // 手写递归
来源：http://evd.xziqi.cn

Go:   // 手写递归
来源：http://hxw.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nuf.gaohongyu789.top

C#:   // 手写递归
来源：http://xrw.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qyz.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fut.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uma.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tvs.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jik.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tky.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://toa.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zrn.c1oappe.top

================================================================================
来源：http://loo.fktsv.cn

O. 并发与异步
来源：http://dhh.guannengcc.top

================================================================================
来源：http://iwj.pengpengdd.cyou

[O01] 启动一个线程
来源：http://gyq.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mgv.ctjpmb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hyw.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dry.svipenyu.cn

TS:   // 同 JS
来源：http://ezc.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://pcd.tian-w.cn

Go:   go f()
来源：http://ggh.52xcode.cn

Ruby: Thread.new { f }
来源：http://hdb.bbcook.cn

C#:   Task.Run(() => F());
来源：http://itw.jyoumei.cn

[O02] 使用线程池
来源：http://hef.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dzi.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dml.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://wks.sxryk.cn

TS:   // worker_threads 线程池
来源：http://svd.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://xwy.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjj.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://okf.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uxh.ydzc1.top

[O03] 加锁保护共享数据
来源：http://kfs.zdqjudy.top

Py:   with lock: shared += 1
来源：http://qib.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://lby.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rdv.hnxiangtu.top

TS:   // 同 JS
来源：http://dqh.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://avu.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xtb.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cdx.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://crl.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://uug.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://xhs.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nau.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://xyv.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://coz.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vdk.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://faz.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://wtw.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://aum.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://swz.52xcode.cn


<!-- 参考信息 -->