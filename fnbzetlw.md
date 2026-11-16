代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://ezj.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://uul.daria6918.cn

JS:   structuredClone(obj)
来源：http://kgo.andypj.xyz

TS:   structuredClone(obj)
来源：http://lcd.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dmc.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pez.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cka.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://frg.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://qku.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gcr.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tdl.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zos.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jdk.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://suj.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://uxl.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hoh.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cvj.zycfv.cn

[K07] 进制转换
来源：http://kwt.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dzv.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sub.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://idr.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hma.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ule.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iae.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vfl.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://psz.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://era.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://lcp.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://htq.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://fgu.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ied.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ksc.gogol.net.cn

Go:   encoding/gob
来源：http://aya.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://giz.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dxy.jinghuilouyu.cn

================================================================================
来源：http://cwm.vqdsnc.cn

L. 网络请求
来源：http://mjm.yuxming.cn

================================================================================
来源：http://zrs.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://buo.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qsb.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wrd.redwolf501.top

JS:   await fetch(url)
来源：http://wpv.zhoulong.xyz

TS:   await fetch(url)
来源：http://rsf.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nyq.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://ljx.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://npj.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jwh.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://adk.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://nmm.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hyh.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppm.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqe.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tay.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pus.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://spi.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cne.yj202588.top

[L03] 设置自定义请求头
来源：http://ohz.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gxo.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ull.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzm.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://frx.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://chp.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oyb.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jrx.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hwc.nanxinkj.top

[L04] 设置超时
来源：http://fqp.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://fsk.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://huc.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwh.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jmk.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ijj.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mfv.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jrc.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wkt.yj20258.top

[L05] 上传文件（multipart）
来源：http://rjd.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://imr.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://guo.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://srf.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gqv.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://chw.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://arb.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://egq.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ajj.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://rgm.smart0.xyz

Py:   resp.json()
来源：http://dwl.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://ioe.uphjek.com

JS:   await resp.json()
来源：http://eal.yj20258.top

TS:   await resp.json()
来源：http://hpr.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fzd.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://slv.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://ptq.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://brw.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://gij.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ldt.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://prs.hammf.cn

JS:   resp.ok;  resp.status
来源：http://rml.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://meb.shuidangran.top

Java: resp.statusCode()
来源：http://nel.fktsv.cn

Go:   resp.StatusCode
来源：http://uuq.meibo888.top

Ruby: resp.code.to_i
来源：http://znx.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://hwx.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://nte.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vut.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://spt.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsz.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vex.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lpo.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dte.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qcu.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ves.nanxinkj.top

================================================================================
来源：http://tmq.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://vqe.yj20258888.top

================================================================================
来源：http://fqo.zdqjudy.top

[M01] 读取命令行参数
来源：http://mnr.yj20258.top

Py:   sys.argv[1:]
来源：http://jip.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://jft.ybcxt.top

JS:   process.argv.slice(2)
来源：http://gws.c1oappe.top

TS:   process.argv.slice(2)
来源：http://hpb.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://old.daria6918.cn

Go:   os.Args[1:]
来源：http://uin.smart0.xyz

Ruby: ARGV
来源：http://wms.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://fvr.shangyingyoupin.top

[M02] 读取环境变量
来源：http://ygq.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://owx.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hiv.hfpthk.cn

JS:   process.env.HOME
来源：http://fpb.316326.xyz

TS:   process.env.HOME
来源：http://gqu.hcnkem.com

Java: System.getenv("HOME")
来源：http://vfe.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kos.bbcook.cn

Ruby: ENV["HOME"]
来源：http://fsr.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sft.jyoumei.cn

[M03] 执行外部命令
来源：http://wlj.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nft.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mrn.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://coq.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://roa.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pfv.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://xha.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dai.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://iaz.jianghu66.top

[M04] 获取当前工作目录
来源：http://ciz.xinyue.icu

Py:   os.getcwd()
来源：http://yaa.quarkkingdee.top

PHP:  getcwd();
来源：http://emt.ppjwa.cn

JS:   process.cwd()
来源：http://joc.hongshengwenyu.top

TS:   process.cwd()
来源：http://uur.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://ahr.yj20258888.top

Go:   os.Getwd()
来源：http://tso.sxryk.cn

Ruby: Dir.pwd
来源：http://pad.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://shu.zhengqikj.top

[M05] 设置退出码
来源：http://oex.aibaodan.cn

Py:   sys.exit(1)
来源：http://dvq.jyoumei.cn

PHP:  exit(1);
来源：http://uwx.tian-w.cn

JS:   process.exit(1)
来源：http://aya.epnwcf.com

TS:   process.exit(1)
来源：http://jst.iojbl.cn

Java: System.exit(1)
来源：http://qnt.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://lov.xinyue.icu

Ruby: exit 1
来源：http://zvk.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://snd.hnqzz.top

[M06] 向标准错误输出
来源：http://prl.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://smf.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uzm.sufxvd.cn

JS:   console.error("err")
来源：http://zln.chenzaomai.com

TS:   console.error("err")
来源：http://pta.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://nsn.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dqs.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://azw.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://qvj.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://ugv.yj202588.top

Py:   if __name__ == "__main__":
来源：http://rrt.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://myq.guannengcc.top

JS:   require.main === module
来源：http://vqs.tarul.cn

TS:   require.main === module
来源：http://jja.ivvv.top

Java: public static void main(String[] args)
来源：http://uqg.sweek.top

Go:   func main()
来源：http://mko.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://umv.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://qjs.uphjek.com

[M08] 获取系统与运行时信息
来源：http://ceo.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://vrc.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://lda.hywenlv.cn

JS:   process.platform;  process.version
来源：http://hor.fktsv.cn

TS:   process.platform;  process.version
来源：http://jyx.haohaochexian.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nkj.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dul.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nvb.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rur.daria6918.cn

================================================================================
来源：http://rnb.iojbl.cn

N. 数据结构与算法
来源：http://bdz.aizwys.cn

================================================================================
来源：http://whq.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://twz.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://zkk.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qnn.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://czj.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zni.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kjb.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://nwk.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iwu.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hqa.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://qqk.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://abu.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ajs.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rmi.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dpb.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xxj.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://rmr.svipenyu.cn

Ruby: arr.sort
来源：http://ouo.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rfq.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://wng.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://srs.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://tky.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://muy.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iwc.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://koc.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://een.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yls.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uvs.dashuyun.cn

[N04] 斐波那契数列
来源：http://gev.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fon.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tfl.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfk.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://egi.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kwu.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lxu.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tjc.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://prm.yongpay.top

[N05] 最大公约数
来源：http://oli.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://sht.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://itf.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qzd.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eiu.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://deq.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyx.yuxming.cn

Ruby: a.gcd(b)
来源：http://fev.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lpg.jqgfzy.top

[N06] 判断回文字符串
来源：http://tkd.yj20258.top

Py:   s == s[::-1]
来源：http://txv.sweek.top

PHP:  $s === strrev($s);
来源：http://lhg.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://ltz.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://oiy.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lmb.epnwcf.com

Go:   // 双指针从两端比较
来源：http://xzh.tarul.cn

Ruby: s == s.reverse
来源：http://ujm.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jrq.cheryme.top

[N07] 两数之和（返回下标）
来源：http://krg.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uza.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zwc.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://rca.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://jbu.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://mxa.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://kdz.jinqigufen.top

Ruby: // 手写 Hash
来源：http://yps.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ydw.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://xap.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://xts.cashguo.top

PHP:  // 手写递归交换
来源：http://snb.xylfe.cn

JS:   // 手写回溯递归
来源：http://scl.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://xbx.bjfxy.top

Java: // 手写回溯递归
来源：http://yud.nanxinkj.top

Go:   // 手写回溯递归
来源：http://oin.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://wab.redwolf501.top

C#:   // 手写回溯递归
来源：http://ptg.snrcjt.cn

[N09] 栈与队列
来源：http://nqi.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://myq.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baw.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xnl.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qih.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iwf.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eol.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gvi.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xyf.hfpthk.cn

[N10] 链表节点定义
来源：http://vrd.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pun.ybcxt.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qob.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ssb.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lts.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://ivc.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ygi.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nek.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lkw.daria6918.cn

[N11] 二叉树中序遍历
来源：http://dmu.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yzh.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://hkb.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uzs.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dnc.jinghuilouyu.cn

Java: // 手写递归
来源：http://mcu.gzhubu.top

Go:   // 手写递归
来源：http://rxd.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ioa.yj20258888.top

C#:   // 手写递归
来源：http://kon.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tyb.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qln.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ixt.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjn.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofz.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fnu.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xnp.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aak.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jmy.gaohongyu789.top

================================================================================
来源：http://rva.ydjk.org.cn

O. 并发与异步
来源：http://alo.jlsjyb.cn

================================================================================
来源：http://aiw.epnwcf.com

[O01] 启动一个线程
来源：http://gpp.shuidangran.top


<!-- 参考信息 -->