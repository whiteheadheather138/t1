代发 wailian999

Go:   encoding/gob
来源：http://wbb.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://ktr.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://abo.hfpthk.cn

================================================================================
来源：http://aju.shangyingyoupin.top

L. 网络请求
来源：http://oxc.yueranfly.top

================================================================================
来源：http://jbq.svipenyu.cn

[L01] 发送 GET 请求
来源：http://inu.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jcf.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://thb.hongshengwenyu.top

JS:   await fetch(url)
来源：http://anm.zhengqikj.top

TS:   await fetch(url)
来源：http://vbe.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mok.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://xdq.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gle.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hwc.sysykeji.top

[L02] 发送 POST JSON
来源：http://pav.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://mxn.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ers.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xnk.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ryr.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qss.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://idf.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dra.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ymf.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://phy.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://byb.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ooa.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ofy.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xml.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cvd.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qqv.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zhi.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xzl.jqgufenzy.top

[L04] 设置超时
来源：http://imv.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://kox.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qxm.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://brg.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxt.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nfw.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xbh.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ttp.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dsu.redwolf501.top

[L05] 上传文件（multipart）
来源：http://rmz.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dqq.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vwr.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xuy.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qyj.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jqq.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fht.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://flm.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://erv.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://kwj.vehdjk.com

Py:   resp.json()
来源：http://tqz.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://cjf.zhijiandao.cn

JS:   await resp.json()
来源：http://cwb.wangdashe.top

TS:   await resp.json()
来源：http://ncf.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://typ.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nmo.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://fjj.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mov.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://uql.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ytx.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://anq.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://kgg.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://fik.yanxiufei.cn

Java: resp.statusCode()
来源：http://vpe.9152youxi.cn

Go:   resp.StatusCode
来源：http://xpd.sysykeji.top

Ruby: resp.code.to_i
来源：http://hlr.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://gbp.fehbvm.com

[L08] 并发请求多个地址
来源：http://how.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bft.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://ftj.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bvs.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yzj.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://czd.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hgh.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rct.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://usc.hnxiangtu.top

================================================================================
来源：http://afh.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://kuz.yj202588.top

================================================================================
来源：http://sua.cdnleiting.top

[M01] 读取命令行参数
来源：http://qag.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://tnr.xinyue.icu

PHP:  $argv;  $argc;
来源：http://flz.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://boq.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://sbl.tarul.cn

Java: args 数组（main 方法参数）
来源：http://doc.ivvv.top

Go:   os.Args[1:]
来源：http://okm.yongpay.top

Ruby: ARGV
来源：http://kuq.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://uao.uphjek.com

[M02] 读取环境变量
来源：http://xpi.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://omm.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cuf.zhijiandao.cn

JS:   process.env.HOME
来源：http://mqc.redwolf501.top

TS:   process.env.HOME
来源：http://uzl.ydzc1.top

Java: System.getenv("HOME")
来源：http://fkt.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ytt.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://nqw.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fnr.yj20258888.top

[M03] 执行外部命令
来源：http://hbt.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ash.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bsu.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mdg.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wit.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://loa.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://grp.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://rcz.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://tgc.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://bki.redwolf501.top

Py:   os.getcwd()
来源：http://nom.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://tef.yonumen.top

JS:   process.cwd()
来源：http://yel.jqgfzy.top

TS:   process.cwd()
来源：http://esm.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://kjh.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://gey.dashuyun.cn

Ruby: Dir.pwd
来源：http://qma.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lcw.0kj1m.cn

[M05] 设置退出码
来源：http://hof.ydzc1.top

Py:   sys.exit(1)
来源：http://oxf.nanxuanxn.top

PHP:  exit(1);
来源：http://dxn.fktsv.cn

JS:   process.exit(1)
来源：http://iqe.ctjpmb.com

TS:   process.exit(1)
来源：http://znr.jinqigfzy.top

Java: System.exit(1)
来源：http://lks.ehwqpu.com

Go:   os.Exit(1)
来源：http://rgf.smart0.xyz

Ruby: exit 1
来源：http://gxq.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hvt.yangfankeji.com

[M06] 向标准错误输出
来源：http://frr.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://dyi.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xly.shzxlz.cn

JS:   console.error("err")
来源：http://ckr.hywenlv.cn

TS:   console.error("err")
来源：http://lsb.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://nwt.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ndq.jqgufenzy.top

Ruby: warn "err"
来源：http://jbj.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://iex.gzhubu.top

[M07] 判断是否为主入口
来源：http://gvp.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://pqn.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ydi.iojbl.cn

JS:   require.main === module
来源：http://sxe.zhongyouzk.top

TS:   require.main === module
来源：http://van.mhx1999.top

Java: public static void main(String[] args)
来源：http://aaf.jqgfzy.top

Go:   func main()
来源：http://jaw.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://foo.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://dsm.tarul.cn

[M08] 获取系统与运行时信息
来源：http://asf.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://woj.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://ueb.hammf.cn

JS:   process.platform;  process.version
来源：http://eje.sxryk.cn

TS:   process.platform;  process.version
来源：http://gxv.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mmw.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ibv.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://auw.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nxo.shuidangran.top

================================================================================
来源：http://snp.feifeiyinyue.top

N. 数据结构与算法
来源：http://dau.vehdjk.com

================================================================================
来源：http://zre.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://dha.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ztz.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ljf.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hpf.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fyw.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://fpb.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://gfd.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ogq.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://nrv.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://bbf.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://piy.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vve.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nkf.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbi.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zyv.iojbl.cn

Go:   slices.Sort(arr)
来源：http://dhl.fengsongda.top

Ruby: arr.sort
来源：http://vcg.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dno.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://dum.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xhe.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://frt.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qfe.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cla.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sar.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ohz.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jtm.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://xuk.daria6918.cn

[N04] 斐波那契数列
来源：http://gpi.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nut.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzb.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mse.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dev.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qie.hesvh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ell.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fdh.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jwt.nanxinkj.top

[N05] 最大公约数
来源：http://mqr.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://hfd.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://orv.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zno.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ois.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vab.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hjd.yj20258888.top

Ruby: a.gcd(b)
来源：http://odd.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rqi.vehdjk.com

[N06] 判断回文字符串
来源：http://tzq.havefunace.top

Py:   s == s[::-1]
来源：http://hqa.tarul.cn

PHP:  $s === strrev($s);
来源：http://nrd.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://pwb.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://wnm.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rny.birdmap.top

Go:   // 双指针从两端比较
来源：http://wvx.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://kre.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ghg.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://juj.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://geq.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gzz.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://drz.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://wzd.smart0.xyz

Java: // 手写 HashMap
来源：http://cqg.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://peo.sufxvd.cn

Ruby: // 手写 Hash
来源：http://fqz.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://vwr.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://mzv.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://irx.epnwcf.com

PHP:  // 手写递归交换
来源：http://xwt.xinyue.icu

JS:   // 手写回溯递归
来源：http://hvd.52xcode.cn

TS:   // 手写回溯递归
来源：http://jwq.sjlbkw.cn

Java: // 手写回溯递归
来源：http://gfe.guannengcc.top

Go:   // 手写回溯递归
来源：http://npq.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://laa.cdnleiting.top

C#:   // 手写回溯递归
来源：http://lid.yongpay.top

[N09] 栈与队列
来源：http://tyn.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wok.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rbw.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yyi.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fln.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cll.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zlo.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dyk.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kmw.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://oqu.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hka.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gth.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sdm.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vrh.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://iyd.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://end.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pyk.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jrm.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://fuq.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hdp.andypj.xyz

PHP:  // 手写递归函数
来源：http://xfv.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uif.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihs.hywenlv.cn

Java: // 手写递归
来源：http://gak.fzhhl.top

Go:   // 手写递归
来源：http://swb.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fks.hfpthk.cn

C#:   // 手写递归
来源：http://won.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://apq.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://afj.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uez.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://whi.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gfx.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jmw.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://exp.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ghe.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kxh.shanyushiyangkeji.top

================================================================================
来源：http://sjq.chenjidiqi.icu

O. 并发与异步
来源：http://lan.zhiwuduotai.top

================================================================================
来源：http://gyo.yuxming.cn

[O01] 启动一个线程
来源：http://pyj.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cpf.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ihc.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oxu.kuanghao11.cn

TS:   // 同 JS
来源：http://cvk.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://maz.jinqigfzy.top

Go:   go f()
来源：http://iak.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://ygh.c1oappe.top

C#:   Task.Run(() => F());
来源：http://fqk.wangdashe.top

[O02] 使用线程池
来源：http://vtc.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cfx.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gti.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://myj.nwbrower.top

TS:   // worker_threads 线程池
来源：http://atx.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sel.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gzm.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iwu.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://maf.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://dlc.jianghu66.top

Py:   with lock: shared += 1
来源：http://uva.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://ppk.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://afc.nanxuanxn.top

TS:   // 同 JS
来源：http://snk.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://nus.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://npy.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oza.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://ffs.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://lgb.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://khi.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pen.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://rmz.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bvy.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://piy.dashuyun.cn


<!-- 参考信息 -->