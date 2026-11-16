代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://vop.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://myo.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aiv.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fif.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uji.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yov.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://ydz.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mts.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hpd.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wve.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzb.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ujo.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wex.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ubh.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ohg.zhongyouzk.top

[K05] 深拷贝对象
来源：http://vay.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://cad.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://wad.yj20258888.top

JS:   structuredClone(obj)
来源：http://wfd.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://xxv.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://prb.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gqq.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aeg.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mwx.xuanzx.com

[K06] 解析 URL 查询串
来源：http://ass.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jsz.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vub.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxl.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zmv.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tgv.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kat.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qjb.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qvp.jlsjyb.cn

[K07] 进制转换
来源：http://qvq.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yly.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xix.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://okx.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mae.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rmc.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipk.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mtz.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gjk.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://wuv.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://ygf.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hxu.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://fnc.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://rul.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tnt.smart0.xyz

Go:   encoding/gob
来源：http://lgj.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://iah.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vpl.jinyuanbaomall.cn

================================================================================
来源：http://bpn.snrcjt.cn

L. 网络请求
来源：http://tnd.52xcode.cn

================================================================================
来源：http://esx.yangfankeji.com

[L01] 发送 GET 请求
来源：http://xsk.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qze.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zbf.jinqigufen.top

JS:   await fetch(url)
来源：http://qrf.316326.xyz

TS:   await fetch(url)
来源：http://knc.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xrj.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://psh.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://wkw.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vli.ydzc1.top

[L02] 发送 POST JSON
来源：http://tke.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://tns.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ksq.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hvk.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqa.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sdx.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qqx.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kdb.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://quo.gogol.net.cn

[L03] 设置自定义请求头
来源：http://mtc.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sab.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://efh.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxi.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syx.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://beu.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zuw.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hiy.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gnb.yongpay.top

[L04] 设置超时
来源：http://hmn.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://sli.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://anb.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qzq.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uue.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pvt.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://odl.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rtl.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qxi.andypj.xyz

[L05] 上传文件（multipart）
来源：http://gfu.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bkq.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khl.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tfz.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tzt.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zpl.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pom.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://myd.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qdv.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://pkv.0kj1m.cn

Py:   resp.json()
来源：http://zkk.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://muf.wangshuangyany.cn

JS:   await resp.json()
来源：http://qrq.hammf.cn

TS:   await resp.json()
来源：http://gks.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ijm.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rsg.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://lwd.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://how.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://efj.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gol.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tda.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://ciu.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://whl.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://vqo.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://ykh.shuidangran.top

Ruby: resp.code.to_i
来源：http://uqh.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://lun.vehdjk.com

[L08] 并发请求多个地址
来源：http://vku.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rhi.sweek.top

PHP:  curl_multi_init() 系列
来源：http://dla.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgq.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wla.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kvg.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mnh.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://avu.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bep.havefunace.top

================================================================================
来源：http://ybb.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://kiz.nanxinkj.top

================================================================================
来源：http://iry.uphjek.com

[M01] 读取命令行参数
来源：http://tcv.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://ssw.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://zhu.hammf.cn

JS:   process.argv.slice(2)
来源：http://jdi.hesvh.cn

TS:   process.argv.slice(2)
来源：http://ltr.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://pip.jyoumei.cn

Go:   os.Args[1:]
来源：http://fso.zdbjq.cn

Ruby: ARGV
来源：http://ngd.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://nax.hongshengwenyu.top

[M02] 读取环境变量
来源：http://sqa.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://jjb.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gle.sweek.top

JS:   process.env.HOME
来源：http://ara.gzhubu.top

TS:   process.env.HOME
来源：http://twg.jqgfzy.top

Java: System.getenv("HOME")
来源：http://uwy.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fmh.andypj.xyz

Ruby: ENV["HOME"]
来源：http://bhg.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iyo.vqdsnc.cn

[M03] 执行外部命令
来源：http://any.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ojz.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nmk.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vfh.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lpq.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://toe.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://thi.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://bzz.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://hlu.dashuyun.cn

[M04] 获取当前工作目录
来源：http://flx.quarkkingdee.top

Py:   os.getcwd()
来源：http://wrv.0kj1m.cn

PHP:  getcwd();
来源：http://flk.nanxuanxn.top

JS:   process.cwd()
来源：http://qca.ybcxt.top

TS:   process.cwd()
来源：http://hft.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://uem.bjfxy.top

Go:   os.Getwd()
来源：http://kpp.fehbvm.com

Ruby: Dir.pwd
来源：http://lou.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://wwu.cucudq.cn

[M05] 设置退出码
来源：http://npj.jqgufenzy.top

Py:   sys.exit(1)
来源：http://mba.birdmap.top

PHP:  exit(1);
来源：http://qhl.hysaishi.cn

JS:   process.exit(1)
来源：http://djk.ehwqpu.com

TS:   process.exit(1)
来源：http://zzd.jqgufenzy.top

Java: System.exit(1)
来源：http://cka.zhongyouzk.top

Go:   os.Exit(1)
来源：http://ugv.guowangkeji.top

Ruby: exit 1
来源：http://igc.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iva.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://spc.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://cef.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cys.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://ggm.yvedp.cn

TS:   console.error("err")
来源：http://kpt.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://rta.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cbd.daria6918.cn

Ruby: warn "err"
来源：http://pyb.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://zlk.wangdashe.top

[M07] 判断是否为主入口
来源：http://ftt.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://inb.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tfs.wangdashe.top

JS:   require.main === module
来源：http://rhf.ydzc1.top

TS:   require.main === module
来源：http://ras.dianchejie.cn

Java: public static void main(String[] args)
来源：http://ifk.shanyushiyangtech.top

Go:   func main()
来源：http://bvs.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jqf.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://nbd.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://kql.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://ajf.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://zku.fktsv.cn

JS:   process.platform;  process.version
来源：http://grl.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://jxw.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rel.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://acn.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ell.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oss.tianlin.xyz

================================================================================
来源：http://hvi.gaohongyu789.top

N. 数据结构与算法
来源：http://exm.havefunace.top

================================================================================
来源：http://wtp.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://cbt.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://vql.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vaw.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cad.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eso.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://wry.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://ajj.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hng.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dwf.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://tnm.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://wpu.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://goz.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ygk.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jfb.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cye.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://uvz.jinqigufen.top

Ruby: arr.sort
来源：http://oiy.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nud.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://msb.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eyg.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://ost.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://duf.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://muv.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qcm.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uhh.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fco.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xzn.gaohongyu789.top

[N04] 斐波那契数列
来源：http://ivk.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nor.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zsk.chenlongwang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://urt.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yrl.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zdg.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xtx.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://edd.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xbs.jlsjyb.cn

[N05] 最大公约数
来源：http://jvj.fktsv.cn

Py:   math.gcd(a, b)
来源：http://ads.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vov.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jvf.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lmz.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wzh.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ria.wangdashe.top

Ruby: a.gcd(b)
来源：http://zfa.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gwz.hesvh.cn

[N06] 判断回文字符串
来源：http://gnb.yanxiufei.cn

Py:   s == s[::-1]
来源：http://zqd.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://wyw.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://syi.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://yms.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qsg.mhx1999.top

Go:   // 双指针从两端比较
来源：http://ftc.vehdjk.com

Ruby: s == s.reverse
来源：http://jzx.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://czm.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://rhz.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://orc.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ipp.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vkn.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://xyw.chenzaomai.com

Java: // 手写 HashMap
来源：http://nba.fktsv.cn

Go:   // 手写 map[int]int
来源：http://ypa.gogol.net.cn

Ruby: // 手写 Hash
来源：http://ojb.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://iip.daxiang520.top

[N08] 生成全排列
来源：http://zoq.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://bzo.chenzaomai.com

PHP:  // 手写递归交换
来源：http://kiz.epnwcf.com

JS:   // 手写回溯递归
来源：http://wfw.xylfe.cn

TS:   // 手写回溯递归
来源：http://jli.birdmap.top

Java: // 手写回溯递归
来源：http://hpq.yj20258.top

Go:   // 手写回溯递归
来源：http://vor.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://hio.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://vyf.yangfankeji.com

[N09] 栈与队列
来源：http://lbx.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pwj.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://arj.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://usy.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kyb.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bif.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xwn.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qrm.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gyq.birdmap.top

[N10] 链表节点定义
来源：http://cnx.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ufq.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wsz.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nnw.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ffb.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://qji.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://nsp.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rsl.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://feu.vehdjk.com

[N11] 二叉树中序遍历
来源：http://omh.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xmo.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://dmq.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ats.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fcx.sysykeji.top

Java: // 手写递归
来源：http://hnm.tianlin.xyz


<!-- 参考信息 -->