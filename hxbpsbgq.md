代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://liu.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lin.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hnz.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wee.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nxj.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ibn.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uby.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://yow.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://xzl.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://owx.shzxlz.cn

JS:   structuredClone(obj)
来源：http://vaj.fzhhl.top

TS:   structuredClone(obj)
来源：http://als.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://okq.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fbv.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zve.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://gwh.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://vgq.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gll.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iza.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dny.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gla.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sbp.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uir.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lkv.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pmt.pengpengdd.cyou

[K07] 进制转换
来源：http://znq.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qnv.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vyw.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fmo.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcj.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dss.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rfc.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ijj.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rwu.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://cpt.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://qew.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jov.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://kxa.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://ylc.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mrt.tanke756.top

Go:   encoding/gob
来源：http://mrt.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://zdi.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://igw.xingfuxueyuan.xyz

================================================================================
来源：http://vab.c1oappe.top

L. 网络请求
来源：http://tqs.zhiwuduotai.top

================================================================================
来源：http://rnj.havefunace.top

[L01] 发送 GET 请求
来源：http://pqn.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gtl.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rse.jqgufenzy.top

JS:   await fetch(url)
来源：http://kti.gogol.net.cn

TS:   await fetch(url)
来源：http://hbw.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nac.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://rfc.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pii.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sks.pycfn.com

[L02] 发送 POST JSON
来源：http://qze.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://agm.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bxg.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://akf.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mti.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ftt.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aqh.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://peq.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://icb.zhengqikj.top

[L03] 设置自定义请求头
来源：http://vzt.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oof.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xsq.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mep.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dav.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tjo.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vbd.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lvd.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://klg.xinyue.icu

[L04] 设置超时
来源：http://iic.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://hdn.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sdt.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://anr.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gjc.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yst.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://smv.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://clj.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lmh.fengsongda.top

[L05] 上传文件（multipart）
来源：http://jcu.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fru.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://srk.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hja.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://slq.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vsq.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rvc.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fze.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hbu.fehbvm.com

[L06] 解析响应为 JSON
来源：http://rnd.xinyue.icu

Py:   resp.json()
来源：http://pqg.vehdjk.com

PHP:  json_decode($body, true);
来源：http://tki.iojbl.cn

JS:   await resp.json()
来源：http://uly.vehdjk.com

TS:   await resp.json()
来源：http://ltv.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pxo.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://alf.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://yqj.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://taq.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://wwi.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ofj.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hae.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://fkl.pycfn.com

TS:   resp.ok;  resp.status
来源：http://tgu.c1oappe.top

Java: resp.statusCode()
来源：http://wvc.chenzaomai.com

Go:   resp.StatusCode
来源：http://foh.svipenyu.cn

Ruby: resp.code.to_i
来源：http://yew.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://xwr.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://uuz.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ker.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://uyp.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hzq.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://awq.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qsw.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bye.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sfy.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://auw.yj202588.top

================================================================================
来源：http://hdz.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://xre.aibaodan.cn

================================================================================
来源：http://uiw.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://gry.yvedp.cn

Py:   sys.argv[1:]
来源：http://krk.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://ecd.zycfv.cn

JS:   process.argv.slice(2)
来源：http://ciz.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://vat.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://pso.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://jsv.havefunace.top

Ruby: ARGV
来源：http://zkk.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://qux.epnwcf.com

[M02] 读取环境变量
来源：http://lyj.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://vlw.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eke.tanke756.top

JS:   process.env.HOME
来源：http://zwd.zdbjq.cn

TS:   process.env.HOME
来源：http://zeo.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://qul.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xot.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://umn.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ttq.zhongyouzk.top

[M03] 执行外部命令
来源：http://aep.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lgw.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yzz.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nkg.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zvr.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pkf.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zsc.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://wlp.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://qlc.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://dhf.cqqwz.cn

Py:   os.getcwd()
来源：http://xbb.sjlbkw.cn

PHP:  getcwd();
来源：http://wgh.ivvv.top

JS:   process.cwd()
来源：http://ijw.yj20258888.top

TS:   process.cwd()
来源：http://rtg.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://wcj.xylfe.cn

Go:   os.Getwd()
来源：http://kwl.chenzaomai.com

Ruby: Dir.pwd
来源：http://zvn.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://svl.zhijiandao.cn

[M05] 设置退出码
来源：http://bwo.52xcode.cn

Py:   sys.exit(1)
来源：http://zef.jinghuilouyu.cn

PHP:  exit(1);
来源：http://awm.smart0.xyz

JS:   process.exit(1)
来源：http://lyb.sxryk.cn

TS:   process.exit(1)
来源：http://fmp.sxryk.cn

Java: System.exit(1)
来源：http://mto.cdnleiting.top

Go:   os.Exit(1)
来源：http://bak.zhongyouzk.top

Ruby: exit 1
来源：http://nyy.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vjn.yueranfly.top

[M06] 向标准错误输出
来源：http://xvc.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://apa.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mjh.dianchejie.cn

JS:   console.error("err")
来源：http://ybv.yongpay.top

TS:   console.error("err")
来源：http://ejc.316326.xyz

Java: System.err.println("err")
来源：http://yde.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dpe.sjlbkw.cn

Ruby: warn "err"
来源：http://zkf.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://udx.yangfankeji.com

[M07] 判断是否为主入口
来源：http://mpc.gaohongyu789.top

Py:   if __name__ == "__main__":
来源：http://mht.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qir.xziqi.cn

JS:   require.main === module
来源：http://sxf.tian-w.cn

TS:   require.main === module
来源：http://qfa.ivvv.top

Java: public static void main(String[] args)
来源：http://wuo.andypj.xyz

Go:   func main()
来源：http://afj.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lqg.yj20258.top

C#:   static void Main(string[] args)
来源：http://nhe.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://mnz.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://aar.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://wmz.mhx1999.top

JS:   process.platform;  process.version
来源：http://rxr.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://who.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yxi.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://spy.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wah.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mfy.ehwqpu.com

================================================================================
来源：http://nkv.fktsv.cn

N. 数据结构与算法
来源：http://ben.tian-w.cn

================================================================================
来源：http://xbx.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://mcm.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xuo.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hyv.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mff.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://duj.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qjj.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ftt.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aey.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cbh.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://dap.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://nmk.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://twy.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://plp.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://dty.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jtn.bbcook.cn

Go:   slices.Sort(arr)
来源：http://kbc.hfpthk.cn

Ruby: arr.sort
来源：http://iac.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nyr.yonumen.top

[N03] 快速排序（分治示例）
来源：http://wtf.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eoo.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://cfa.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://clg.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://amh.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wwr.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hyy.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ger.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bzm.ydjk.org.cn

[N04] 斐波那契数列
来源：http://uzw.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wgw.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aam.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tfh.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://skf.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nrf.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lag.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ews.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qju.hywenlv.cn

[N05] 最大公约数
来源：http://nsy.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://hun.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://phn.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixs.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xhj.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uao.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://evx.fzhhl.top

Ruby: a.gcd(b)
来源：http://qib.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ker.yanxiufei.cn

[N06] 判断回文字符串
来源：http://vpu.yueranfly.top

Py:   s == s[::-1]
来源：http://cdp.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://kcp.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://lbo.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://qqh.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://img.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://meu.hywenlv.cn

Ruby: s == s.reverse
来源：http://pbu.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gtx.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://vwg.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mwm.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dkp.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vrs.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://zoj.tanke756.top

Java: // 手写 HashMap
来源：http://uzw.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://tjb.hnqzz.top

Ruby: // 手写 Hash
来源：http://aky.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://kov.cucudq.cn

[N08] 生成全排列
来源：http://dlv.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://qnq.0kj1m.cn

PHP:  // 手写递归交换
来源：http://qqj.xylfe.cn

JS:   // 手写回溯递归
来源：http://wcu.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://btm.hnqzz.top

Java: // 手写回溯递归
来源：http://njw.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://rcy.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://prl.52xcode.cn

C#:   // 手写回溯递归
来源：http://tis.jinqigfzy.top

[N09] 栈与队列
来源：http://wpn.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bvl.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dib.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vey.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://idw.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ney.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sjz.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jur.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://onv.hesvh.cn

[N10] 链表节点定义
来源：http://odt.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://udy.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://njn.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rnq.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mir.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://zyr.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://gvg.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://qkg.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fra.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://npb.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ccg.sweek.top

PHP:  // 手写递归函数
来源：http://dop.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hrt.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aae.gaohongyu789.top

Java: // 手写递归
来源：http://cha.dianchejie.cn

Go:   // 手写递归
来源：http://ndb.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ids.sjlbkw.cn

C#:   // 手写递归
来源：http://zqc.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sen.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oxa.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tzh.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sma.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vwe.zhiwuduotai.top


<!-- 参考信息 -->