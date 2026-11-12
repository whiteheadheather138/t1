代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qrd.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ckd.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wfc.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ahh.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ffk.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://beb.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gve.ctjpmb.com

[K05] 深拷贝对象
来源：http://nge.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://tbm.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://ull.zhengqikj.top

JS:   structuredClone(obj)
来源：http://ixb.gotoacloud.top

TS:   structuredClone(obj)
来源：http://pas.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xef.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yqy.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzw.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://per.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://ofy.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iyl.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://obn.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://plf.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hlt.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hwu.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://vnr.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://skf.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zrr.gaohongyu789.top

[K07] 进制转换
来源：http://sbg.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dzm.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://npt.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kcj.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://chf.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zyv.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xoi.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cye.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ynd.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://nhr.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://fin.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://peh.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://xjd.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://pxr.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rhu.xinyue.icu

Go:   encoding/gob
来源：http://ryj.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://udx.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cbm.sxryk.cn

================================================================================
来源：http://cfs.uphjek.com

L. 网络请求
来源：http://ira.yuxming.cn

================================================================================
来源：http://qch.jinqigufen.top

[L01] 发送 GET 请求
来源：http://vli.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rxc.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vlf.jlsjyb.cn

JS:   await fetch(url)
来源：http://ugu.daria6918.cn

TS:   await fetch(url)
来源：http://crk.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://irl.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://wqm.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uyo.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sko.cashguo.top

[L02] 发送 POST JSON
来源：http://uor.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://baz.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zgk.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xgd.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dih.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dma.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mcg.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bup.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://soh.redwolf501.top

[L03] 设置自定义请求头
来源：http://zmx.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nvx.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pld.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfc.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdz.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hvq.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mrc.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://efd.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tkn.jqgufenzy.top

[L04] 设置超时
来源：http://pid.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://oyl.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nrt.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lri.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://knf.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pel.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mkg.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eus.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iah.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://bik.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ute.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rmm.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wfs.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rik.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qrt.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://awa.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://poo.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://crq.zycfv.cn

[L06] 解析响应为 JSON
来源：http://vqf.gzhubu.top

Py:   resp.json()
来源：http://bzx.cucudq.cn

PHP:  json_decode($body, true);
来源：http://klm.yuxming.cn

JS:   await resp.json()
来源：http://aqj.ybcxt.top

TS:   await resp.json()
来源：http://iei.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hlc.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://chj.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://fom.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://daw.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://xsp.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bpx.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hya.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://emz.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://dnl.ppjwa.cn

Java: resp.statusCode()
来源：http://xuq.ehwqpu.com

Go:   resp.StatusCode
来源：http://toq.zycfv.cn

Ruby: resp.code.to_i
来源：http://quj.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://rty.xylfe.cn

[L08] 并发请求多个地址
来源：http://hih.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dvw.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://xfk.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ygk.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blh.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gnc.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dte.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yxo.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iqo.nwbrower.top

================================================================================
来源：http://efl.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://fsw.kuanghao11.cn

================================================================================
来源：http://zmo.daxiang520.top

[M01] 读取命令行参数
来源：http://agr.sufxvd.cn

Py:   sys.argv[1:]
来源：http://byo.zycfv.cn

PHP:  $argv;  $argc;
来源：http://ijn.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://mjb.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://nir.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://lwt.ybcxt.top

Go:   os.Args[1:]
来源：http://ugg.fengsongda.top

Ruby: ARGV
来源：http://ggx.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://bwu.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://ivs.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://hdf.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://drh.uphjek.com

JS:   process.env.HOME
来源：http://xwx.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://rsx.yonumen.top

Java: System.getenv("HOME")
来源：http://vmg.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jnc.redwolf501.top

Ruby: ENV["HOME"]
来源：http://tut.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pdm.cheryme.top

[M03] 执行外部命令
来源：http://fhb.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jjf.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uii.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xdg.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zaw.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svw.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tzs.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kyl.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://wii.aibaodan.cn

[M04] 获取当前工作目录
来源：http://haa.xylfe.cn

Py:   os.getcwd()
来源：http://fho.chenzaomai.com

PHP:  getcwd();
来源：http://plv.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://zse.tarul.cn

TS:   process.cwd()
来源：http://jwo.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://bkr.hongshengwenyu.top

Go:   os.Getwd()
来源：http://zlj.bjfxy.top

Ruby: Dir.pwd
来源：http://fby.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jns.cashguo.top

[M05] 设置退出码
来源：http://ywt.dashuyun.cn

Py:   sys.exit(1)
来源：http://jar.zhijiandao.cn

PHP:  exit(1);
来源：http://nga.hnqzz.top

JS:   process.exit(1)
来源：http://rmi.gzhubu.top

TS:   process.exit(1)
来源：http://qxb.pengpengdd.cyou

Java: System.exit(1)
来源：http://iuv.wangdashe.top

Go:   os.Exit(1)
来源：http://hju.jiagoushi.top

Ruby: exit 1
来源：http://hdf.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rnj.sysykeji.top

[M06] 向标准错误输出
来源：http://fmo.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://ord.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gcq.dashuyun.cn

JS:   console.error("err")
来源：http://fmz.mhx1999.top

TS:   console.error("err")
来源：http://fnd.nwbrower.top

Java: System.err.println("err")
来源：http://rwj.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://udk.jianghu66.top

Ruby: warn "err"
来源：http://dzv.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://mwg.pengpengdd.cyou

[M07] 判断是否为主入口
来源：http://xjl.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://cqk.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qez.hongshengwenyu.top

JS:   require.main === module
来源：http://ckv.yj202588.top

TS:   require.main === module
来源：http://grm.daxiang520.top

Java: public static void main(String[] args)
来源：http://pux.yj20258888.top

Go:   func main()
来源：http://oqp.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wjy.ybcxt.top

C#:   static void Main(string[] args)
来源：http://kym.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://far.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://eso.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://cem.bjfxy.top

JS:   process.platform;  process.version
来源：http://lgu.cdnleiting.top

TS:   process.platform;  process.version
来源：http://ajc.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lux.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fdi.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oij.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hbw.zdqjudy.top

================================================================================
来源：http://qje.jinqigfzy.top

N. 数据结构与算法
来源：http://kyh.jyoumei.cn

================================================================================
来源：http://von.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://rtt.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://cge.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sgk.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kmo.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgo.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://rci.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://pys.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://klw.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xbo.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://omy.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://eoo.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gof.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://snr.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://brf.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nny.c1oappe.top

Go:   slices.Sort(arr)
来源：http://qjg.yfazqb.com

Ruby: arr.sort
来源：http://qgc.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hrt.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://obb.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://whl.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://pzn.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://myu.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vlq.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://grx.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fwm.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mho.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://olz.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://nay.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jmo.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jal.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://use.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jes.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://acz.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vye.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rwp.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rev.xuetiantiany.cn

[N05] 最大公约数
来源：http://rky.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://cnx.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jwh.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://shl.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sow.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nap.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fjn.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://pry.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mpw.chenzaomai.com

[N06] 判断回文字符串
来源：http://wlr.hnqzz.top

Py:   s == s[::-1]
来源：http://cac.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://bog.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://lre.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://eob.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mmt.wangdashe.top

Go:   // 双指针从两端比较
来源：http://dqi.meibo888.top

Ruby: s == s.reverse
来源：http://vzc.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ghs.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://ivq.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bmt.jinqigfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gmi.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oqr.yanxiufei.cn

TS:   // 手写 Map<string, number>
来源：http://bza.hammf.cn

Java: // 手写 HashMap
来源：http://hdu.meibo888.top

Go:   // 手写 map[int]int
来源：http://lpa.sweek.top

Ruby: // 手写 Hash
来源：http://pmb.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qxl.quarkkingdee.top

[N08] 生成全排列
来源：http://vho.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://qrv.yfazqb.com

PHP:  // 手写递归交换
来源：http://drp.guannengcc.top

JS:   // 手写回溯递归
来源：http://yqy.haohaochexian.top

TS:   // 手写回溯递归
来源：http://fai.chenzaomai.com

Java: // 手写回溯递归
来源：http://icx.vehdjk.com

Go:   // 手写回溯递归
来源：http://yuu.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://dxd.zycfv.cn

C#:   // 手写回溯递归
来源：http://vbs.andypj.xyz

[N09] 栈与队列
来源：http://crc.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://twv.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oes.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sux.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://geh.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pnt.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pwg.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rzn.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vsz.gogol.net.cn

[N10] 链表节点定义
来源：http://fxu.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aqm.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wvd.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyf.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://itn.cheryme.top

Java: class Node { int v; Node next; }
来源：http://uwr.fzhhl.top

Go:   type Node struct { V int; Next *Node }
来源：http://enw.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://our.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bsv.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://yxh.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gcv.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://xyn.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gnn.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upy.sufxvd.cn

Java: // 手写递归
来源：http://kge.iojbl.cn

Go:   // 手写递归
来源：http://qwz.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mqn.xziqi.cn

C#:   // 手写递归
来源：http://hcj.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wuc.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tbd.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://apy.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://llk.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vne.hammf.cn


<!-- 参考信息 -->