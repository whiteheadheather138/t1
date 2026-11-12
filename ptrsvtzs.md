代发 wailian999

Go:   encoding/gob
来源：http://zss.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://xlx.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://acs.quarkkingdee.top

================================================================================
来源：http://dkr.yongpay.top

L. 网络请求
来源：http://gml.hywenlv.cn

================================================================================
来源：http://cel.ivvv.top

[L01] 发送 GET 请求
来源：http://tkg.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cyw.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://szj.hywenlv.cn

JS:   await fetch(url)
来源：http://yft.smart0.xyz

TS:   await fetch(url)
来源：http://inw.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dkg.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://gpx.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xvb.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ciw.fengsongda.top

[L02] 发送 POST JSON
来源：http://vlg.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cul.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kdh.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xbd.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlk.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zug.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mwi.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fdb.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cwa.daxiang520.top

[L03] 设置自定义请求头
来源：http://zci.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qma.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kxh.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://men.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aif.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xnz.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://icf.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pmf.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sli.jinyuanbaomall.cn

[L04] 设置超时
来源：http://dhz.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://cpr.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bfj.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tpx.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eha.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://utf.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eeq.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tak.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fzz.fehbvm.com

[L05] 上传文件（multipart）
来源：http://hvv.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://itn.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fix.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zcp.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bmz.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ccd.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://miv.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lxx.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oya.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://epf.jinqigfzy.top

Py:   resp.json()
来源：http://tma.ybcxt.top

PHP:  json_decode($body, true);
来源：http://kzm.havefunace.top

JS:   await resp.json()
来源：http://lws.ppjwa.cn

TS:   await resp.json()
来源：http://dvw.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uew.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zfw.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://lso.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nvg.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://qst.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xev.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gyx.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://hbh.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://jjw.nanxuanxn.top

Java: resp.statusCode()
来源：http://qkz.xinyue.icu

Go:   resp.StatusCode
来源：http://njm.fktsv.cn

Ruby: resp.code.to_i
来源：http://hqt.yj202588.top

C#:   (int)resp.StatusCode
来源：http://ylj.bbcook.cn

[L08] 并发请求多个地址
来源：http://vdt.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bij.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://jxb.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rrm.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ulp.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ihm.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kdh.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qic.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gfe.smart0.xyz

================================================================================
来源：http://miq.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://pxo.cashguo.top

================================================================================
来源：http://jde.smart0.xyz

[M01] 读取命令行参数
来源：http://xdl.sufxvd.cn

Py:   sys.argv[1:]
来源：http://rvp.bjfxy.top

PHP:  $argv;  $argc;
来源：http://wrh.cheryme.top

JS:   process.argv.slice(2)
来源：http://tjq.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://zjb.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://cqd.yfazqb.com

Go:   os.Args[1:]
来源：http://log.jianghu66.top

Ruby: ARGV
来源：http://awo.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://uml.nanxinkj.top

[M02] 读取环境变量
来源：http://xst.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://tuy.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hyv.yongpay.top

JS:   process.env.HOME
来源：http://auq.quarkkingdee.top

TS:   process.env.HOME
来源：http://suk.jyoumei.cn

Java: System.getenv("HOME")
来源：http://atb.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xva.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://ehn.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mpn.zhoulong.xyz

[M03] 执行外部命令
来源：http://bdm.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qvk.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baq.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kde.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nrc.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ysd.quarkkingdee.top

Go:   exec.Command("ls", "-l").Output()
来源：http://huv.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vdb.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://fxg.ydzc1.top

[M04] 获取当前工作目录
来源：http://wnc.quarkkingdee.top

Py:   os.getcwd()
来源：http://iad.zdbjq.cn

PHP:  getcwd();
来源：http://uib.jqgufenzy.top

JS:   process.cwd()
来源：http://ygv.sysykeji.top

TS:   process.cwd()
来源：http://gdl.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ezh.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://sco.nanxinkj.top

Ruby: Dir.pwd
来源：http://qwi.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qks.nwbrower.top

[M05] 设置退出码
来源：http://tnl.aizwys.cn

Py:   sys.exit(1)
来源：http://ifg.xuanzx.com

PHP:  exit(1);
来源：http://vke.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://hxk.ehwqpu.com

TS:   process.exit(1)
来源：http://kxo.gogol.net.cn

Java: System.exit(1)
来源：http://yfb.zhongyouzk.top

Go:   os.Exit(1)
来源：http://uqu.xuanzx.com

Ruby: exit 1
来源：http://eew.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://elz.xuanzx.com

[M06] 向标准错误输出
来源：http://nwl.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://yja.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rki.yuanzhike.top

JS:   console.error("err")
来源：http://fwf.iojbl.cn

TS:   console.error("err")
来源：http://zub.zhixingplan.top

Java: System.err.println("err")
来源：http://jub.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uwc.shuidangran.top

Ruby: warn "err"
来源：http://lwn.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://ykx.c1oappe.top

[M07] 判断是否为主入口
来源：http://kai.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://yqi.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgj.gzhubu.top

JS:   require.main === module
来源：http://oaw.yj202588.top

TS:   require.main === module
来源：http://gty.tianlin.xyz

Java: public static void main(String[] args)
来源：http://rsb.sjlbkw.cn

Go:   func main()
来源：http://nge.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kbe.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://mjp.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://hrt.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://tah.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://ibd.dashuyun.cn

JS:   process.platform;  process.version
来源：http://dkh.yfazqb.com

TS:   process.platform;  process.version
来源：http://fha.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tyy.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfx.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tmv.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lbk.zhaomingkeji.xyz

================================================================================
来源：http://szh.zdqjudy.top

N. 数据结构与算法
来源：http://opf.kuanghao11.cn

================================================================================
来源：http://yfc.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://tnb.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qaj.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lth.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vtz.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ckw.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wez.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://ssm.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zqx.gaohongyu789.top

C#:   Array.BinarySearch(arr, x)
来源：http://chm.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://rdr.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://krc.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pik.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hdz.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mln.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jih.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://hhl.haohaochexian.top

Ruby: arr.sort
来源：http://kna.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fym.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://iwl.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eay.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://hgq.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbb.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlx.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vbs.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qfw.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nqj.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://iyf.jqgufenzy.top

[N04] 斐波那契数列
来源：http://dvj.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xcc.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bkr.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rzb.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nzu.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mda.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nvt.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mld.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ker.tianlin.xyz

[N05] 最大公约数
来源：http://wgv.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://cnf.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jmd.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nju.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zmg.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czs.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uub.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://vcz.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qkw.yuxming.cn

[N06] 判断回文字符串
来源：http://ivi.smart0.xyz

Py:   s == s[::-1]
来源：http://qjx.sysykeji.top

PHP:  $s === strrev($s);
来源：http://rjn.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://hhh.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://nzd.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lna.fengsongda.top

Go:   // 双指针从两端比较
来源：http://gyd.hesvh.cn

Ruby: s == s.reverse
来源：http://fbn.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://spp.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://uqq.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydu.gotoacloud.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mge.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://dmp.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://jqm.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://naf.cucudq.cn

Go:   // 手写 map[int]int
来源：http://hdd.guannengcc.top

Ruby: // 手写 Hash
来源：http://fev.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://fwf.snrcjt.cn

[N08] 生成全排列
来源：http://kad.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://snt.uphjek.com

PHP:  // 手写递归交换
来源：http://ecw.xziqi.cn

JS:   // 手写回溯递归
来源：http://yhy.chenlongwang.top

TS:   // 手写回溯递归
来源：http://gmq.zhoulong.xyz

Java: // 手写回溯递归
来源：http://ehr.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://dra.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://adg.shzxlz.cn

C#:   // 手写回溯递归
来源：http://zxw.jinqigufen.top

[N09] 栈与队列
来源：http://brr.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydo.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rka.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ztw.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cil.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bfu.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ylr.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dsr.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wcc.hysaishi.cn

[N10] 链表节点定义
来源：http://zek.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ywy.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tqh.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uut.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iux.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://upv.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ojt.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ekk.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://byk.bbcook.cn

[N11] 二叉树中序遍历
来源：http://vri.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ull.316326.xyz

PHP:  // 手写递归函数
来源：http://xin.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgk.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yrg.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://juc.ybcxt.top

Go:   // 手写递归
来源：http://ghm.gotoacloud.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gkq.jinqigufen.top

C#:   // 手写递归
来源：http://mgk.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rdk.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wde.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aus.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zhw.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gyz.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pah.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://meu.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pcz.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kxi.quarkkingdee.top

================================================================================
来源：http://dwx.sxryk.cn

O. 并发与异步
来源：http://ryl.xylfe.cn

================================================================================
来源：http://sqv.zhixingplan.top

[O01] 启动一个线程
来源：http://wnw.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bil.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rwh.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yjp.gzhubu.top

TS:   // 同 JS
来源：http://juf.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://qmr.zdbjq.cn

Go:   go f()
来源：http://onp.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://kmg.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://clv.guannengcc.top

[O02] 使用线程池
来源：http://dvh.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ips.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zif.52xcode.cn

JS:   // worker_threads 线程池
来源：http://vuh.vehdjk.com

TS:   // worker_threads 线程池
来源：http://crq.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ayv.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bnc.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bnl.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oxz.cheryme.top

[O03] 加锁保护共享数据
来源：http://jvk.zdqjudy.top

Py:   with lock: shared += 1
来源：http://coi.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://ces.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://obo.cqqwz.cn

TS:   // 同 JS
来源：http://muk.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://xsf.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oik.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hvh.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://ggl.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://dwf.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://ovy.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lbg.uphjek.com

JS:   async function f() { await g(); }
来源：http://tyz.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://afm.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uzi.hongshengwenyu.top


<!-- 参考信息 -->