代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dma.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bht.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://orp.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vrx.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hwo.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://acn.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://abf.bjfxy.top

[K05] 深拷贝对象
来源：http://ora.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://zcn.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://jol.svipenyu.cn

JS:   structuredClone(obj)
来源：http://phf.xinyue.icu

TS:   structuredClone(obj)
来源：http://bbo.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tev.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wtp.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ozx.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qws.gzhubu.top

[K06] 解析 URL 查询串
来源：http://iac.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jvb.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qag.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qwt.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kmw.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cld.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bbw.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ats.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://muh.xuetiantiany.cn

[K07] 进制转换
来源：http://gbe.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vtv.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gsi.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lxn.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bjv.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://srr.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dmo.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vis.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gnz.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://hli.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://bct.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vpb.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://wcn.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://jnw.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qzd.yangfankeji.com

Go:   encoding/gob
来源：http://jax.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://xaw.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pso.ywan-chungtsiang.top

================================================================================
来源：http://voc.quarkkingdee.top

L. 网络请求
来源：http://fyy.9152youxi.cn

================================================================================
来源：http://von.nwbrower.top

[L01] 发送 GET 请求
来源：http://iym.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zej.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vle.ivvv.top

JS:   await fetch(url)
来源：http://yuj.haohaochexian.top

TS:   await fetch(url)
来源：http://ozi.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nxr.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://xtz.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bon.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rol.cqqwz.cn

[L02] 发送 POST JSON
来源：http://uuz.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://msl.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdh.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qkf.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zja.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugf.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://byr.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tvu.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fpj.zhengqikj.top

[L03] 设置自定义请求头
来源：http://nvs.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yln.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xze.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ted.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ups.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pmd.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ucr.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wyp.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://naq.jinqigfzy.top

[L04] 设置超时
来源：http://ugt.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://yan.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yaq.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iqv.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bps.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qyl.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nnt.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rmn.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sky.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://nke.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hkm.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hgs.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pht.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tem.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sig.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ivf.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vqn.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nmv.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://tzw.cheryme.top

Py:   resp.json()
来源：http://xto.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://jel.uphjek.com

JS:   await resp.json()
来源：http://ibb.jqgfzy.top

TS:   await resp.json()
来源：http://ysb.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dpz.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://evh.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://gmb.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vjk.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://dgc.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aqs.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://niq.meibo888.top

JS:   resp.ok;  resp.status
来源：http://nse.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://mmz.guannengcc.top

Java: resp.statusCode()
来源：http://kxt.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://iya.dianchejie.cn

Ruby: resp.code.to_i
来源：http://mdo.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://gwd.52xcode.cn

[L08] 并发请求多个地址
来源：http://cqx.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pus.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://qwt.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vds.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rkl.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uhw.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mlw.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vjj.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zml.jlsjyb.cn

================================================================================
来源：http://bgj.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://gdw.yonumen.top

================================================================================
来源：http://vsg.bjfxy.top

[M01] 读取命令行参数
来源：http://gfp.zdqjudy.top

Py:   sys.argv[1:]
来源：http://gga.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://lvu.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://ulc.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://ygx.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://usd.zdbjq.cn

Go:   os.Args[1:]
来源：http://vjv.zhijiandao.cn

Ruby: ARGV
来源：http://uyu.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://hfm.aizwys.cn

[M02] 读取环境变量
来源：http://ewg.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://cvt.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fgk.jqgufenzy.top

JS:   process.env.HOME
来源：http://lbj.yangfankeji.com

TS:   process.env.HOME
来源：http://qjy.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://ozw.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ocz.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://rfs.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fna.ppjwa.cn

[M03] 执行外部命令
来源：http://iln.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://heg.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qvn.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ahy.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zgd.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gag.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fvl.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kph.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://raf.tanke756.top

[M04] 获取当前工作目录
来源：http://nvn.yuxming.cn

Py:   os.getcwd()
来源：http://pta.bjfxy.top

PHP:  getcwd();
来源：http://npb.yonumen.top

JS:   process.cwd()
来源：http://ipr.gotoacloud.top

TS:   process.cwd()
来源：http://hop.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ovq.shzxlz.cn

Go:   os.Getwd()
来源：http://snm.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://muw.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://prc.tianlin.xyz

[M05] 设置退出码
来源：http://oyj.jinqigufen.top

Py:   sys.exit(1)
来源：http://gkn.chenlongwang.top

PHP:  exit(1);
来源：http://vmn.fzhhl.top

JS:   process.exit(1)
来源：http://cnc.yangfankeji.com

TS:   process.exit(1)
来源：http://iqp.cheryme.top

Java: System.exit(1)
来源：http://byr.zycfv.cn

Go:   os.Exit(1)
来源：http://wby.tian-w.cn

Ruby: exit 1
来源：http://plf.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lbe.svipenyu.cn

[M06] 向标准错误输出
来源：http://ikn.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://mjb.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eqf.vqdsnc.cn

JS:   console.error("err")
来源：http://wto.yvedp.cn

TS:   console.error("err")
来源：http://tmq.andypj.xyz

Java: System.err.println("err")
来源：http://ypr.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwa.jyoumei.cn

Ruby: warn "err"
来源：http://nuo.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://nib.dashuyun.cn

[M07] 判断是否为主入口
来源：http://rbt.havefunace.top

Py:   if __name__ == "__main__":
来源：http://bmb.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://afd.dianchejie.cn

JS:   require.main === module
来源：http://cao.gotoacloud.top

TS:   require.main === module
来源：http://zzq.xziqi.cn

Java: public static void main(String[] args)
来源：http://hap.nwbrower.top

Go:   func main()
来源：http://qrz.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wgg.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://jnk.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://ojs.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://slj.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://iaw.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://bns.dianchejie.cn

TS:   process.platform;  process.version
来源：http://tcr.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zbz.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wdb.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://noo.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tug.jqgufenzy.top

================================================================================
来源：http://epp.jinqigfzy.top

N. 数据结构与算法
来源：http://mcf.bjfxy.top

================================================================================
来源：http://xgx.cheryme.top

[N01] 二分查找（有序数组）
来源：http://hzv.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://pjh.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iec.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vez.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://scp.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://bzh.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://ayf.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lwq.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://llq.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://zxu.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ojc.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bbh.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://osc.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://obs.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://flx.tanke756.top

Go:   slices.Sort(arr)
来源：http://jza.jqgufenzy.top

Ruby: arr.sort
来源：http://zvq.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://yjz.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://orm.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://esd.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://xje.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffl.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ugc.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hqv.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ktc.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xjm.nanxuanxn.top

C#:   // 手写递归，或 Array.Sort
来源：http://zrt.316326.xyz

[N04] 斐波那契数列
来源：http://atb.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jxd.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kwt.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hje.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydj.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jlw.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dmf.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ujt.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ain.vqdsnc.cn

[N05] 最大公约数
来源：http://wck.hesvh.cn

Py:   math.gcd(a, b)
来源：http://ucl.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bky.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qit.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ukj.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cyc.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zin.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://upz.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qks.zycfv.cn

[N06] 判断回文字符串
来源：http://dma.daria6918.cn

Py:   s == s[::-1]
来源：http://dap.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://zej.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://ltl.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://oup.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fjt.fktsv.cn

Go:   // 双指针从两端比较
来源：http://yfi.yongpay.top

Ruby: s == s.reverse
来源：http://fjm.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yjp.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://agh.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tol.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dlz.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://whz.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://qym.hcnkem.com

Java: // 手写 HashMap
来源：http://xzn.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://itk.snrcjt.cn

Ruby: // 手写 Hash
来源：http://pph.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zgr.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://swt.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://hqy.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://nkz.iojbl.cn

JS:   // 手写回溯递归
来源：http://ywr.jinqigufen.top

TS:   // 手写回溯递归
来源：http://llv.jyoumei.cn

Java: // 手写回溯递归
来源：http://ezj.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://acn.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://tda.cucudq.cn

C#:   // 手写回溯递归
来源：http://fhw.jinghuilouyu.cn

[N09] 栈与队列
来源：http://yqt.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vfl.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cpn.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fjv.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lsk.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vda.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mff.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kfq.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kmn.zhijiandao.cn

[N10] 链表节点定义
来源：http://pww.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ayp.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sqf.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nso.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yhi.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://uuf.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://yuo.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gur.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uki.yvedp.cn

[N11] 二叉树中序遍历
来源：http://jpd.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lru.epnwcf.com

PHP:  // 手写递归函数
来源：http://vdn.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fmi.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://anq.havefunace.top

Java: // 手写递归
来源：http://dol.jqgfzy.top

Go:   // 手写递归
来源：http://pbj.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pri.xuanzx.com

C#:   // 手写递归
来源：http://yip.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bxi.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uek.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oas.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zaw.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://idt.ctjpmb.com


<!-- 参考信息 -->