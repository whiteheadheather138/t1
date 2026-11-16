代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://ntx.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://rem.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gdx.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://swa.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://wfy.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kdd.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://ras.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ajn.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hbb.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ktv.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujb.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ibq.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dbi.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://smn.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nnq.hfpthk.cn

[K05] 深拷贝对象
来源：http://brh.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://zak.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://mfy.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://xhg.xylfe.cn

TS:   structuredClone(obj)
来源：http://lqh.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tbe.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ppz.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://luv.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bqs.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://cyv.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uyd.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwn.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivg.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://muj.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eap.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jio.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tgz.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uws.nanxinkj.top

[K07] 进制转换
来源：http://oph.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://red.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mry.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yil.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kvj.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://csa.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tos.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gcn.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dcj.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://osz.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://ykx.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://msa.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://xuk.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://yeo.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zkk.yanxiufei.cn

Go:   encoding/gob
来源：http://cgb.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://inh.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ymx.tanke756.top

================================================================================
来源：http://lgz.yuanzhike.top

L. 网络请求
来源：http://cvj.smart0.xyz

================================================================================
来源：http://dpk.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://nvi.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uvw.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wrv.zhixingplan.top

JS:   await fetch(url)
来源：http://fpt.dashuyun.cn

TS:   await fetch(url)
来源：http://dri.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lfi.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://oyc.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ueg.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://haf.jianghu66.top

[L02] 发送 POST JSON
来源：http://nfs.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://csa.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://unv.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xaa.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdc.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sgc.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ueg.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qfq.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aat.hcnkem.com

[L03] 设置自定义请求头
来源：http://hui.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qzq.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jvp.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pkx.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xxw.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://crv.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nws.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mal.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bso.shanyushiyangkeji.top

[L04] 设置超时
来源：http://poz.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://wun.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vsg.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aor.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tcp.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fnp.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bzc.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lzh.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jgz.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://phb.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xct.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xrm.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cfo.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gvh.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wgo.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iri.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vsu.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yoz.yj202588.top

[L06] 解析响应为 JSON
来源：http://tom.yj20258.top

Py:   resp.json()
来源：http://hhd.daria6918.cn

PHP:  json_decode($body, true);
来源：http://bei.tian-w.cn

JS:   await resp.json()
来源：http://mjv.nanxuanxn.top

TS:   await resp.json()
来源：http://oev.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jed.gaohongyu789.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dbx.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://xrt.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vhn.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://zzl.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fpc.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://juf.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://mqm.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://mhj.yj20258.top

Java: resp.statusCode()
来源：http://gni.bjfxy.top

Go:   resp.StatusCode
来源：http://apc.ydzc1.top

Ruby: resp.code.to_i
来源：http://kjs.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://rii.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://awe.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://isa.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://ssi.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ybd.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qtw.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hxi.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qqc.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zmx.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lxa.birdmap.top

================================================================================
来源：http://ggj.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://mlj.gogol.net.cn

================================================================================
来源：http://vne.epnwcf.com

[M01] 读取命令行参数
来源：http://lma.ybcxt.top

Py:   sys.argv[1:]
来源：http://oeu.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://dxf.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://jvw.fzhhl.top

TS:   process.argv.slice(2)
来源：http://ven.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://zug.316326.xyz

Go:   os.Args[1:]
来源：http://kuu.sweek.top

Ruby: ARGV
来源：http://fcd.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://luk.yfazqb.com

[M02] 读取环境变量
来源：http://ssj.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://yif.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jgc.xinyue.icu

JS:   process.env.HOME
来源：http://xwo.quarkkingdee.top

TS:   process.env.HOME
来源：http://ltv.sweek.top

Java: System.getenv("HOME")
来源：http://wco.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://szv.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://uzd.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ccq.cqqwz.cn

[M03] 执行外部命令
来源：http://jsv.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bgd.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iyk.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ngf.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rzg.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zxy.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bij.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bxl.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://wss.sweek.top

[M04] 获取当前工作目录
来源：http://wai.smart0.xyz

Py:   os.getcwd()
来源：http://rho.quarkkingdee.top

PHP:  getcwd();
来源：http://ycg.xuanzx.com

JS:   process.cwd()
来源：http://pnf.jianghu66.top

TS:   process.cwd()
来源：http://lva.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://efv.gaohongyu789.top

Go:   os.Getwd()
来源：http://jlm.fengsongda.top

Ruby: Dir.pwd
来源：http://vze.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rtd.andypj.xyz

[M05] 设置退出码
来源：http://dcs.fengsongda.top

Py:   sys.exit(1)
来源：http://whq.cqqwz.cn

PHP:  exit(1);
来源：http://wia.zhongyouzk.top

JS:   process.exit(1)
来源：http://wfs.ydjk.org.cn

TS:   process.exit(1)
来源：http://npw.chenlongwang.top

Java: System.exit(1)
来源：http://adc.gaohongyu789.top

Go:   os.Exit(1)
来源：http://tzi.guannengcc.top

Ruby: exit 1
来源：http://dsq.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yrz.ybcxt.top

[M06] 向标准错误输出
来源：http://kmq.zhixingplan.top

Py:   print("err", file=sys.stderr)
来源：http://kkr.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dwx.iojbl.cn

JS:   console.error("err")
来源：http://yil.wangshuangyany.cn

TS:   console.error("err")
来源：http://xux.ctjpmb.com

Java: System.err.println("err")
来源：http://wjx.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hwr.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://nev.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://aue.xziqi.cn

[M07] 判断是否为主入口
来源：http://ztc.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://ath.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bzw.ybcxt.top

JS:   require.main === module
来源：http://lrg.hnxiangtu.top

TS:   require.main === module
来源：http://tfm.sweek.top

Java: public static void main(String[] args)
来源：http://bps.gzhubu.top

Go:   func main()
来源：http://izm.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cdy.hnqzz.top

C#:   static void Main(string[] args)
来源：http://elc.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://jvi.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://oyd.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://tpq.hesvh.cn

JS:   process.platform;  process.version
来源：http://dus.jqgfzy.top

TS:   process.platform;  process.version
来源：http://ggc.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rmb.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xjj.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://udy.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uyt.cqqwz.cn

================================================================================
来源：http://ygb.zhengqikj.top

N. 数据结构与算法
来源：http://buj.hnxiangtu.top

================================================================================
来源：http://red.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://wxu.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://btp.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://htf.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://asz.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://asq.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://ljj.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://joo.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://aje.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xvc.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://xvp.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://aiz.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ttt.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://khm.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eum.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xup.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://azy.vqdsnc.cn

Ruby: arr.sort
来源：http://zbw.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kdk.ivvv.top

[N03] 快速排序（分治示例）
来源：http://mlk.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wum.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://jnh.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axx.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://chh.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sku.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lbn.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ntc.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://lvl.yvedp.cn

[N04] 斐波那契数列
来源：http://tza.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rdf.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bjh.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qac.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ssl.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xok.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iij.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fae.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hjb.kuanghao11.cn

[N05] 最大公约数
来源：http://uxx.xinyue.icu

Py:   math.gcd(a, b)
来源：http://vos.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cav.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://okg.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vil.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://euj.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jnb.uphjek.com

Ruby: a.gcd(b)
来源：http://cef.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fox.nwbrower.top

[N06] 判断回文字符串
来源：http://kej.meibo888.top

Py:   s == s[::-1]
来源：http://yar.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://ogm.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://nyi.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://ryc.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wzu.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://hns.cucudq.cn

Ruby: s == s.reverse
来源：http://hyf.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wbd.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://etq.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oxe.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nms.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qen.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://bdw.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://syu.yongpay.top

Go:   // 手写 map[int]int
来源：http://hhz.sysykeji.top

Ruby: // 手写 Hash
来源：http://vss.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ciq.hongshengwenyu.top

[N08] 生成全排列
来源：http://adh.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://oig.dianchejie.cn

PHP:  // 手写递归交换
来源：http://dmq.ehwqpu.com

JS:   // 手写回溯递归
来源：http://pzh.guannengcc.top

TS:   // 手写回溯递归
来源：http://xoz.316326.xyz

Java: // 手写回溯递归
来源：http://mtj.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://hoy.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://igd.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://txh.jyoumei.cn

[N09] 栈与队列
来源：http://inz.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hmk.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://evu.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gvq.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kob.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tjk.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ttm.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nqi.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nsg.iojbl.cn

[N10] 链表节点定义
来源：http://ltx.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://msh.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yiy.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jxp.sweek.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://atj.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://dbl.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://brr.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ujy.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mfw.yonumen.top

[N11] 二叉树中序遍历
来源：http://voa.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nay.gzhubu.top

PHP:  // 手写递归函数
来源：http://wqa.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndn.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://luu.yuxming.cn

Java: // 手写递归
来源：http://dtv.yj202588.top


<!-- 参考信息 -->