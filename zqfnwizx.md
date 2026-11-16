代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yro.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vsr.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://lfy.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mop.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kwu.yangfankeji.com

[K07] 进制转换
来源：http://rrt.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sgi.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjl.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zdl.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmp.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gdd.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iuv.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dhm.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hza.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dxa.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://rug.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iyl.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://pvy.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://ytl.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://duw.cdnleiting.top

Go:   encoding/gob
来源：http://tym.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://hdl.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iaz.c1oappe.top

================================================================================
来源：http://jbv.jqgufenzy.top

L. 网络请求
来源：http://miq.ybcxt.top

================================================================================
来源：http://yvl.snrcjt.cn

[L01] 发送 GET 请求
来源：http://dbb.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jvg.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lgl.zhongyouzk.top

JS:   await fetch(url)
来源：http://jen.9152youxi.cn

TS:   await fetch(url)
来源：http://xxq.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdv.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://ebd.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eji.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dkl.yfazqb.com

[L02] 发送 POST JSON
来源：http://btz.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://zwo.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kan.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xek.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vtd.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wdj.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kgu.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://icy.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhg.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://luh.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://axc.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://par.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osd.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ldd.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xhg.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tfj.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rmf.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jyu.cheryme.top

[L04] 设置超时
来源：http://sfi.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://ffj.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://usr.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fic.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://onu.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cug.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gab.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcp.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nht.vehdjk.com

[L05] 上传文件（multipart）
来源：http://urs.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bvr.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vbh.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lgu.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eqy.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jwg.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cib.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xvr.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqf.c1oappe.top

[L06] 解析响应为 JSON
来源：http://hto.zhijiandao.cn

Py:   resp.json()
来源：http://xsc.birdmap.top

PHP:  json_decode($body, true);
来源：http://xsa.fktsv.cn

JS:   await resp.json()
来源：http://tai.cheryme.top

TS:   await resp.json()
来源：http://jjr.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fmb.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fhh.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://drc.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tqb.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://pwp.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zet.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://out.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://ctm.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://lbi.hfpthk.cn

Java: resp.statusCode()
来源：http://zjv.hywenlv.cn

Go:   resp.StatusCode
来源：http://jwa.fktsv.cn

Ruby: resp.code.to_i
来源：http://dwu.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://ail.cqqwz.cn

[L08] 并发请求多个地址
来源：http://psa.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://chb.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://prx.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dtr.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byg.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qsl.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lgi.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tta.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wjp.zhixingplan.top

================================================================================
来源：http://qyh.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://qns.smart0.xyz

================================================================================
来源：http://gkq.birdmap.top

[M01] 读取命令行参数
来源：http://rhx.cqqwz.cn

Py:   sys.argv[1:]
来源：http://cyw.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://syx.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://ave.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://lxe.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://kwd.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://zuw.pycfn.com

Ruby: ARGV
来源：http://pbf.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://dhs.haohaochexian.top

[M02] 读取环境变量
来源：http://emz.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://epq.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iex.hammf.cn

JS:   process.env.HOME
来源：http://eyc.xziqi.cn

TS:   process.env.HOME
来源：http://ldt.sxryk.cn

Java: System.getenv("HOME")
来源：http://qgz.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aos.xylfe.cn

Ruby: ENV["HOME"]
来源：http://rnk.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://djo.zdqjudy.top

[M03] 执行外部命令
来源：http://pzq.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qoz.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yvq.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://izg.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://npe.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vpt.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hqo.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ymo.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://prx.fehbvm.com

[M04] 获取当前工作目录
来源：http://ukw.vqdsnc.cn

Py:   os.getcwd()
来源：http://ekq.iojbl.cn

PHP:  getcwd();
来源：http://kfn.jqgufenzy.top

JS:   process.cwd()
来源：http://ywr.guowangkeji.top

TS:   process.cwd()
来源：http://vbs.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://zzn.yj20258888.top

Go:   os.Getwd()
来源：http://vet.guannengcc.top

Ruby: Dir.pwd
来源：http://zwk.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://agd.feifeiyinyue.top

[M05] 设置退出码
来源：http://tvq.jyoumei.cn

Py:   sys.exit(1)
来源：http://qde.ydzc1.top

PHP:  exit(1);
来源：http://ier.daria6918.cn

JS:   process.exit(1)
来源：http://hfc.hesvh.cn

TS:   process.exit(1)
来源：http://czt.chenlongwang.top

Java: System.exit(1)
来源：http://qvt.guowangkeji.top

Go:   os.Exit(1)
来源：http://twh.yj202588.top

Ruby: exit 1
来源：http://lut.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iem.cdnleiting.top

[M06] 向标准错误输出
来源：http://dkn.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://iiw.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ijq.bjfxy.top

JS:   console.error("err")
来源：http://uqh.havefunace.top

TS:   console.error("err")
来源：http://odd.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://fmw.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yyb.sysykeji.top

Ruby: warn "err"
来源：http://sok.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://chd.hfpthk.cn

[M07] 判断是否为主入口
来源：http://fos.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://mic.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ohg.snrcjt.cn

JS:   require.main === module
来源：http://gso.ywan-chungtsiang.top

TS:   require.main === module
来源：http://kwb.9152youxi.cn

Java: public static void main(String[] args)
来源：http://htp.jyoumei.cn

Go:   func main()
来源：http://qwi.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ncd.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://hjm.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://xxv.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://evh.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://zuq.fehbvm.com

JS:   process.platform;  process.version
来源：http://ehl.yangfankeji.com

TS:   process.platform;  process.version
来源：http://muh.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ggp.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fwn.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hgg.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oro.sysykeji.top

================================================================================
来源：http://ihf.sxryk.cn

N. 数据结构与算法
来源：http://qpa.ehwqpu.com

================================================================================
来源：http://jym.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://ljy.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://txl.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bpc.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ptf.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://shs.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://cjj.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://kdh.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lio.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://xoj.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://chq.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://lqf.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vpc.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tqq.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oxm.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qzt.yj20258888.top

Go:   slices.Sort(arr)
来源：http://jai.ydzc1.top

Ruby: arr.sort
来源：http://myn.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oal.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://ris.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zdf.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://oui.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjs.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wwv.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hjt.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mvk.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gmf.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://eki.yj20258.top

[N04] 斐波那契数列
来源：http://ehl.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ugy.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://poi.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://klv.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kwl.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tyc.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kuv.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sfq.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://miq.shzxlz.cn

[N05] 最大公约数
来源：http://fjo.ybcxt.top

Py:   math.gcd(a, b)
来源：http://zkc.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mxa.jlsjyb.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nen.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kzn.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kkr.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mum.cucudq.cn

Ruby: a.gcd(b)
来源：http://nuv.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ygz.gaohongyu789.top

[N06] 判断回文字符串
来源：http://tex.dashuyun.cn

Py:   s == s[::-1]
来源：http://ebh.gzhubu.top

PHP:  $s === strrev($s);
来源：http://qou.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://hir.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://ams.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fpg.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://cbt.hesvh.cn

Ruby: s == s.reverse
来源：http://lwz.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://utf.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://ecl.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jkb.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zbk.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qdy.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://kcv.epnwcf.com

Java: // 手写 HashMap
来源：http://icu.vehdjk.com

Go:   // 手写 map[int]int
来源：http://glc.daxiang520.top

Ruby: // 手写 Hash
来源：http://twv.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://utm.ivvv.top

[N08] 生成全排列
来源：http://qaz.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://btu.jianghu66.top

PHP:  // 手写递归交换
来源：http://bja.hfpthk.cn

JS:   // 手写回溯递归
来源：http://jlk.jiagoushi.top

TS:   // 手写回溯递归
来源：http://svp.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://wfx.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://pay.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://nll.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://qeu.yfazqb.com

[N09] 栈与队列
来源：http://ymi.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mby.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tns.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uit.tanke756.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://klq.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kic.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dvp.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iic.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qfj.cucudq.cn

[N10] 链表节点定义
来源：http://iwt.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hwu.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pls.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bdb.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qte.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://rfs.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://sno.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nsm.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uaa.ydzc1.top

[N11] 二叉树中序遍历
来源：http://tvf.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xlh.zdbjq.cn

PHP:  // 手写递归函数
来源：http://tut.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://enu.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wyx.yj202588.top

Java: // 手写递归
来源：http://adn.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://tlx.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iaj.chenlongwang.top

C#:   // 手写递归
来源：http://uin.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wzw.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://avw.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aap.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kkk.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvz.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wtd.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dmh.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zai.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qbg.xylfe.cn

================================================================================
来源：http://ecx.0kj1m.cn

O. 并发与异步
来源：http://xzu.sweek.top

================================================================================
来源：http://bnw.xuanzx.com

[O01] 启动一个线程
来源：http://vtt.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iev.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hzi.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bih.smart0.xyz

TS:   // 同 JS
来源：http://wcf.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://zfu.zhongyouzk.top

Go:   go f()
来源：http://rio.yongpay.top

Ruby: Thread.new { f }
来源：http://pru.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://avs.ivvv.top

[O02] 使用线程池
来源：http://rkw.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mna.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://apr.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://pvt.yuxming.cn


<!-- 参考信息 -->