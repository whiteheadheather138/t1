代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bee.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vhc.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgs.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dkr.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lhf.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mxv.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ool.fengsongda.top

[K05] 深拷贝对象
来源：http://mwn.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://jqa.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://rur.aizwys.cn

JS:   structuredClone(obj)
来源：http://ivw.yangfankeji.com

TS:   structuredClone(obj)
来源：http://kuq.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wzb.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://khp.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xkp.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mcq.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://bwq.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://prr.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gbm.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tod.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://etw.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pbh.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://umj.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ano.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gak.jinyuanbaomall.cn

[K07] 进制转换
来源：http://ccb.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tda.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qes.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jcz.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gpd.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tzg.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nkl.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aim.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jfm.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://tim.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://umh.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kko.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://utg.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://thb.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oel.sweek.top

Go:   encoding/gob
来源：http://xuo.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://nqx.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uaj.tanke756.top

================================================================================
来源：http://grh.gotoacloud.top

L. 网络请求
来源：http://tyk.andypj.xyz

================================================================================
来源：http://gkl.yj20258888.top

[L01] 发送 GET 请求
来源：http://wvf.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ver.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kje.cdnleiting.top

JS:   await fetch(url)
来源：http://mjy.316326.xyz

TS:   await fetch(url)
来源：http://qdg.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gds.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://vjd.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://trz.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pjt.haohaochexian.top

[L02] 发送 POST JSON
来源：http://fow.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://zgx.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hit.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mrh.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wez.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iyb.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pnv.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vjh.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kib.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://dmn.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pcc.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://psd.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iho.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lep.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xxr.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://adp.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://agd.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jwa.jinqigufen.top

[L04] 设置超时
来源：http://uhk.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://hih.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vzm.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ppc.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxl.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://icn.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fat.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lmt.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cti.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://zbs.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ams.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvw.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zsj.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xvf.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://que.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yof.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zry.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yth.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://ykv.tianlin.xyz

Py:   resp.json()
来源：http://xqr.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://ggl.shuidangran.top

JS:   await resp.json()
来源：http://unc.kuanghao11.cn

TS:   await resp.json()
来源：http://olb.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aoh.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pai.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://fim.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vvh.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://nue.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zvz.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ifc.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://qkh.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://ilg.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://vjr.vehdjk.com

Go:   resp.StatusCode
来源：http://ais.pycfn.com

Ruby: resp.code.to_i
来源：http://kby.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://hqa.yj20258.top

[L08] 并发请求多个地址
来源：http://eji.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxl.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://jpa.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xav.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ogj.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hja.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wzq.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qhn.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kyd.fanxiaobao.xyz

================================================================================
来源：http://khe.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://zoz.ehwqpu.com

================================================================================
来源：http://yhr.xuanzx.com

[M01] 读取命令行参数
来源：http://tyw.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://ivs.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://lol.daria6918.cn

JS:   process.argv.slice(2)
来源：http://tmq.sxryk.cn

TS:   process.argv.slice(2)
来源：http://yjl.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://hmi.cucudq.cn

Go:   os.Args[1:]
来源：http://zel.bjfxy.top

Ruby: ARGV
来源：http://enc.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://ceo.nanxuanxn.top

[M02] 读取环境变量
来源：http://ihr.ivvv.top

Py:   os.environ.get("HOME")
来源：http://bgd.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kku.zhijiandao.cn

JS:   process.env.HOME
来源：http://hcc.c1oappe.top

TS:   process.env.HOME
来源：http://snu.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://tye.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fks.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://lrw.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nfh.iojbl.cn

[M03] 执行外部命令
来源：http://clo.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xdw.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oii.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://elx.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://cpd.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ike.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zed.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ukm.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://yrh.yfazqb.com

[M04] 获取当前工作目录
来源：http://dpg.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://pbd.ybcxt.top

PHP:  getcwd();
来源：http://xbz.yangfankeji.com

JS:   process.cwd()
来源：http://bbz.vqdsnc.cn

TS:   process.cwd()
来源：http://wrc.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://tks.quarkkingdee.top

Go:   os.Getwd()
来源：http://rks.316326.xyz

Ruby: Dir.pwd
来源：http://xye.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gpv.hongshengwenyu.top

[M05] 设置退出码
来源：http://hlp.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://npw.fengsongda.top

PHP:  exit(1);
来源：http://unr.tian-w.cn

JS:   process.exit(1)
来源：http://ibi.havefunace.top

TS:   process.exit(1)
来源：http://lmp.wangdashe.top

Java: System.exit(1)
来源：http://atv.shuidangran.top

Go:   os.Exit(1)
来源：http://euo.ydjk.org.cn

Ruby: exit 1
来源：http://bvo.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://enb.tianlin.xyz

[M06] 向标准错误输出
来源：http://zpi.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://qqd.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lfh.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://ilq.nanxuanxn.top

TS:   console.error("err")
来源：http://zxb.kuanghao11.cn

Java: System.err.println("err")
来源：http://lyx.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yvb.feifeiyinyue.top

Ruby: warn "err"
来源：http://eft.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://yfn.fktsv.cn

[M07] 判断是否为主入口
来源：http://bfl.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://kbh.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fqz.shanyushiyangtech.top

JS:   require.main === module
来源：http://gdt.ydjk.org.cn

TS:   require.main === module
来源：http://jlh.tanke756.top

Java: public static void main(String[] args)
来源：http://wbq.jqgfzy.top

Go:   func main()
来源：http://lyo.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://igu.mhx1999.top

C#:   static void Main(string[] args)
来源：http://pyb.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://wos.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://vfl.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://wei.hnqzz.top

JS:   process.platform;  process.version
来源：http://fsv.ctjpmb.com

TS:   process.platform;  process.version
来源：http://hmf.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://syc.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://qyr.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://drl.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yke.uphjek.com

================================================================================
来源：http://srp.dianchejie.cn

N. 数据结构与算法
来源：http://nip.andypj.xyz

================================================================================
来源：http://fbu.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://fxj.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://fbr.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bqj.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bit.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://esg.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aaz.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://gto.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://htr.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://bsw.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://qfq.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://bfo.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xud.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ubg.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wxc.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bca.uphjek.com

Go:   slices.Sort(arr)
来源：http://nil.jinqigufen.top

Ruby: arr.sort
来源：http://onj.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://chp.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://hee.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qmc.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://iaf.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bic.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kiw.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qlk.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eeg.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://elz.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://gzd.hammf.cn

[N04] 斐波那契数列
来源：http://bec.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://heh.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dhn.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mna.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ncw.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zkq.yongpay.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jus.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lks.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jfj.yonumen.top

[N05] 最大公约数
来源：http://gov.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://nws.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bpt.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://neu.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sdm.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jtv.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://heb.zhixingplan.top

Ruby: a.gcd(b)
来源：http://icp.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://omn.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://qhl.yj20258.top

Py:   s == s[::-1]
来源：http://dfq.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://fxa.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://drl.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://uvo.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yqi.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://chq.uphjek.com

Ruby: s == s.reverse
来源：http://uzj.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tfr.yonumen.top

[N07] 两数之和（返回下标）
来源：http://jyy.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qri.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zmp.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lmk.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://zru.yanxiufei.cn

Java: // 手写 HashMap
来源：http://ztd.mhx1999.top

Go:   // 手写 map[int]int
来源：http://cpp.316326.xyz

Ruby: // 手写 Hash
来源：http://oci.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://mua.sufxvd.cn

[N08] 生成全排列
来源：http://jek.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://rxx.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://dhm.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://qsk.ctjpmb.com

TS:   // 手写回溯递归
来源：http://khm.chenlongwang.top

Java: // 手写回溯递归
来源：http://jzp.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://rtc.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://xfe.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://ipe.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://ugt.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vgy.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ptb.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uco.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ruh.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gik.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vsf.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hmf.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jnv.fktsv.cn

[N10] 链表节点定义
来源：http://icj.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uoh.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bzt.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aoe.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nun.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://qaa.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://zqk.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oxh.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://gsv.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://quz.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dit.fktsv.cn

PHP:  // 手写递归函数
来源：http://ujz.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wmu.sjlbkw.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjj.kuanghao11.cn

Java: // 手写递归
来源：http://lsq.jinghuilouyu.cn

Go:   // 手写递归
来源：http://nps.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ljo.zhixingplan.top

C#:   // 手写递归
来源：http://zan.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qvo.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bvu.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://woj.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aow.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://duk.dashuyun.cn


<!-- 参考信息 -->