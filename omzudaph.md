代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://elv.daxiang520.top

JS:   await fetch(url)
来源：http://bzy.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://iko.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kud.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://ogd.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ogr.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ayg.fzhhl.top

[L02] 发送 POST JSON
来源：http://mdu.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://gdq.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lwd.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ksc.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://all.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eny.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tyh.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qlp.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://spb.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://zbd.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qfo.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://niz.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gdz.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qjq.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iam.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rjc.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mqj.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jwh.yj202588.top

[L04] 设置超时
来源：http://tbx.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://hof.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://noq.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egy.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nkl.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vqn.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mbl.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://orj.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sgz.c1oappe.top

[L05] 上传文件（multipart）
来源：http://qil.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wbo.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zbh.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ezb.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://efv.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aod.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cdb.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xyn.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qvt.sxryk.cn

[L06] 解析响应为 JSON
来源：http://wdr.ctjpmb.com

Py:   resp.json()
来源：http://mlw.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://pch.jqgfzy.top

JS:   await resp.json()
来源：http://xbi.xuanzx.com

TS:   await resp.json()
来源：http://shj.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bzl.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gyu.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://alw.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kyu.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://uuh.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xbp.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzj.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://nkk.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://riv.hnqzz.top

Java: resp.statusCode()
来源：http://ggs.smart0.xyz

Go:   resp.StatusCode
来源：http://ebp.sysykeji.top

Ruby: resp.code.to_i
来源：http://ibb.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://dhs.52xcode.cn

[L08] 并发请求多个地址
来源：http://yxu.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kjw.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://hjo.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fhd.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wwz.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hrt.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dlr.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gbd.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kqi.mhx1999.top

================================================================================
来源：http://sfr.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://fkl.cashguo.top

================================================================================
来源：http://fnw.tian-w.cn

[M01] 读取命令行参数
来源：http://wbe.gotoacloud.top

Py:   sys.argv[1:]
来源：http://psu.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://hdz.daria6918.cn

JS:   process.argv.slice(2)
来源：http://ywx.hammf.cn

TS:   process.argv.slice(2)
来源：http://wbq.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://qjp.gogol.net.cn

Go:   os.Args[1:]
来源：http://pwx.nanxuanxn.top

Ruby: ARGV
来源：http://xqs.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://wwp.vqdsnc.cn

[M02] 读取环境变量
来源：http://qak.uphjek.com

Py:   os.environ.get("HOME")
来源：http://jdj.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vsz.zhiwuduotai.top

JS:   process.env.HOME
来源：http://icb.hesvh.cn

TS:   process.env.HOME
来源：http://ifo.yj20258.top

Java: System.getenv("HOME")
来源：http://biw.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ett.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://hbb.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pqu.9152youxi.cn

[M03] 执行外部命令
来源：http://njq.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rum.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ghf.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fyq.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vyp.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bsp.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wsd.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://ssx.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://bzr.jiagoushi.top

[M04] 获取当前工作目录
来源：http://vkh.yfazqb.com

Py:   os.getcwd()
来源：http://tmt.fengsongda.top

PHP:  getcwd();
来源：http://reb.jqgufenzy.top

JS:   process.cwd()
来源：http://fwr.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://rgs.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ujs.yangfankeji.com

Go:   os.Getwd()
来源：http://twr.jqgufenzy.top

Ruby: Dir.pwd
来源：http://xfz.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://ivv.hongshengwenyu.top

[M05] 设置退出码
来源：http://ubn.316326.xyz

Py:   sys.exit(1)
来源：http://vhc.mhx1999.top

PHP:  exit(1);
来源：http://hyw.yvedp.cn

JS:   process.exit(1)
来源：http://vgt.zdbjq.cn

TS:   process.exit(1)
来源：http://nyx.wangdashe.top

Java: System.exit(1)
来源：http://huz.bbcook.cn

Go:   os.Exit(1)
来源：http://vry.nanxuanxn.top

Ruby: exit 1
来源：http://diz.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hjv.cdnleiting.top

[M06] 向标准错误输出
来源：http://jke.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://zfm.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kmi.jqgfzy.top

JS:   console.error("err")
来源：http://uzw.jianghu66.top

TS:   console.error("err")
来源：http://hwl.c1oappe.top

Java: System.err.println("err")
来源：http://you.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ibk.ctjpmb.com

Ruby: warn "err"
来源：http://hnx.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://zwv.sufxvd.cn

[M07] 判断是否为主入口
来源：http://jaz.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://udn.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yxy.cheryme.top

JS:   require.main === module
来源：http://cfz.yvedp.cn

TS:   require.main === module
来源：http://hzc.fktsv.cn

Java: public static void main(String[] args)
来源：http://vlh.snrcjt.cn

Go:   func main()
来源：http://jhm.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ayd.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://vdk.tarul.cn

[M08] 获取系统与运行时信息
来源：http://pjw.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://qea.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://xut.bjfxy.top

JS:   process.platform;  process.version
来源：http://eoa.hfpthk.cn

TS:   process.platform;  process.version
来源：http://qvt.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://deu.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qyi.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gpx.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://fwk.daxiang520.top

================================================================================
来源：http://evd.havefunace.top

N. 数据结构与算法
来源：http://tmi.yongpay.top

================================================================================
来源：http://kaf.chenzaomai.com

[N01] 二分查找（有序数组）
来源：http://oos.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://ucg.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hrg.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kaq.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfb.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://cvx.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://mdk.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://qod.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://szp.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://crp.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xuf.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cnl.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bat.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xlu.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iqa.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://ewk.gotoacloud.top

Ruby: arr.sort
来源：http://ofx.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gvg.uphjek.com

[N03] 快速排序（分治示例）
来源：http://pnp.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fcx.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://idw.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fie.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mmh.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yzv.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhx.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tgc.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://dmu.xuanzx.com

[N04] 斐波那契数列
来源：http://owt.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lhy.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cau.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://giw.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://irc.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iwi.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rlu.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ays.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qzn.xziqi.cn

[N05] 最大公约数
来源：http://wid.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://eto.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://njc.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yhl.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqx.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zgv.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://syj.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://rcq.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zhv.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://iwq.havefunace.top

Py:   s == s[::-1]
来源：http://wlt.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://pze.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://xdd.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://gvz.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://npv.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://tew.sjlbkw.cn

Ruby: s == s.reverse
来源：http://jih.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hdo.pycfn.com

[N07] 两数之和（返回下标）
来源：http://nqc.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://doz.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ulx.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ark.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://qxq.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://hqr.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://ewu.ppjwa.cn

Ruby: // 手写 Hash
来源：http://oio.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cvc.jinqigufen.top

[N08] 生成全排列
来源：http://dgb.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://kvl.redwolf501.top

PHP:  // 手写递归交换
来源：http://hau.fengsongda.top

JS:   // 手写回溯递归
来源：http://fsy.ehwqpu.com

TS:   // 手写回溯递归
来源：http://ckz.zycfv.cn

Java: // 手写回溯递归
来源：http://vvj.ydjk.org.cn

Go:   // 手写回溯递归
来源：http://prw.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://jqu.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://zac.yongpay.top

[N09] 栈与队列
来源：http://xko.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zbn.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pqb.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rhs.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tly.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lrr.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://smo.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vjd.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xaa.hywenlv.cn

[N10] 链表节点定义
来源：http://ypg.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://stq.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fwe.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tbc.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hce.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://txl.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://lyc.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rfx.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://syb.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://kmh.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://but.kuanghao11.cn

PHP:  // 手写递归函数
来源：http://ieg.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qsd.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rtz.shuidangran.top

Java: // 手写递归
来源：http://vib.gzhubu.top

Go:   // 手写递归
来源：http://hwy.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xwv.epnwcf.com

C#:   // 手写递归
来源：http://ukn.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jqs.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kpv.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ttx.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kml.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://few.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jsk.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ygh.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ekb.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cbt.birdmap.top

================================================================================
来源：http://yew.cucudq.cn

O. 并发与异步
来源：http://vfm.bjfxy.top

================================================================================
来源：http://lto.svipenyu.cn

[O01] 启动一个线程
来源：http://ykb.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ufb.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uza.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sds.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://izy.yongpay.top

Java: new Thread(() -> f()).start()
来源：http://dhy.sxryk.cn

Go:   go f()
来源：http://hxg.tarul.cn

Ruby: Thread.new { f }
来源：http://wzo.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://gcl.aibaodan.cn

[O02] 使用线程池
来源：http://izr.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ckz.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tqh.c1oappe.top

JS:   // worker_threads 线程池
来源：http://kgv.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://ntw.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://lgp.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://whp.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xdp.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://geu.tanke756.top

[O03] 加锁保护共享数据
来源：http://njm.ybcxt.top

Py:   with lock: shared += 1
来源：http://etu.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://bjq.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lld.0kj1m.cn

TS:   // 同 JS
来源：http://tnd.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://idy.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ala.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ogy.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://fbh.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://mis.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://oxv.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yld.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://bby.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://txt.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tyb.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mrx.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://ddc.hammf.cn

C#:   async Task F() { await G(); }
来源：http://jxf.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://iim.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://woe.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nyt.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://msf.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://ccz.ppjwa.cn


<!-- 参考信息 -->