代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtp.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://lam.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ube.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://wqw.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xrb.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tyc.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kfz.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lfs.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ugu.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://srz.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qqs.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mql.bbcook.cn

================================================================================
来源：http://yvf.cdnleiting.top

K. JSON 与序列化
来源：http://lkp.cashguo.top

================================================================================
来源：http://pxs.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://kft.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iqn.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gba.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://qoq.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://rme.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wib.daria6918.cn

Go:   json.Marshal(obj)
来源：http://qkq.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://bsh.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kbp.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://zhb.zhengqikj.top

Py:   json.loads(s)
来源：http://ukd.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fdt.meibo888.top

JS:   JSON.parse(s)
来源：http://tyr.xziqi.cn

TS:   JSON.parse(s)
来源：http://exu.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://asl.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://dle.bbcook.cn

Ruby: JSON.parse(s)
来源：http://kee.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dsl.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://vrx.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fyc.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jyi.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kft.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nux.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ebx.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sax.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://zmr.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pvj.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://grp.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pxa.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eea.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://far.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qct.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ifo.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dkc.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jni.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://psr.meibo888.top

[K05] 深拷贝对象
来源：http://xwt.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://wnk.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://cao.tianlin.xyz

JS:   structuredClone(obj)
来源：http://suu.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://xto.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bpt.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wjh.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kmr.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://hrn.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://nal.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ycs.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bod.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://szz.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pos.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hpx.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://yvu.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bab.gaohongyu789.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hqf.zhengqikj.top

[K07] 进制转换
来源：http://mwc.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vux.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tcf.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uud.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xax.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dfc.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yuu.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yrb.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ncv.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://bpk.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://wwa.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xmg.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://kno.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://bfc.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yea.fengsongda.top

Go:   encoding/gob
来源：http://vzf.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://ifn.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cfc.yj202588.top

================================================================================
来源：http://sie.nanxuanxn.top

L. 网络请求
来源：http://cox.hcnkem.com

================================================================================
来源：http://mfi.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://zof.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ysa.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gmr.yvedp.cn

JS:   await fetch(url)
来源：http://dwx.smart0.xyz

TS:   await fetch(url)
来源：http://rlk.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fso.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://usw.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dnl.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgq.cqqwz.cn

[L02] 发送 POST JSON
来源：http://hnh.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://geo.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://seb.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vch.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dxt.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ewi.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dca.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fhu.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ecx.c1oappe.top

[L03] 设置自定义请求头
来源：http://awi.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://npi.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mqh.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yag.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bqh.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lss.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pzb.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://slb.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lhy.nanxinkj.top

[L04] 设置超时
来源：http://gxc.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://rbb.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kjf.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irs.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jnf.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kcd.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wky.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://okv.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://osq.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://fbm.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vij.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vaq.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rgl.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nmj.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://beg.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lnw.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jna.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pgl.andypj.xyz

[L06] 解析响应为 JSON
来源：http://sdi.yj202588.top

Py:   resp.json()
来源：http://tai.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://hgh.aibaodan.cn

JS:   await resp.json()
来源：http://unu.mhx1999.top

TS:   await resp.json()
来源：http://wga.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ind.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nzf.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://mpj.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qlj.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://ufr.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cmu.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fqr.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://yqh.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://ace.bjfxy.top

Java: resp.statusCode()
来源：http://yhf.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://egc.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://nrl.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://wue.yfazqb.com

[L08] 并发请求多个地址
来源：http://jvg.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ada.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://rho.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ndc.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wef.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://orx.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bax.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nth.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rln.yuanzhike.top

================================================================================
来源：http://sqz.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://jih.hesvh.cn

================================================================================
来源：http://wib.jianghu66.top

[M01] 读取命令行参数
来源：http://hyr.fehbvm.com

Py:   sys.argv[1:]
来源：http://ezu.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://rce.cucudq.cn

JS:   process.argv.slice(2)
来源：http://kec.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://vpu.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://zgo.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://geo.yonumen.top

Ruby: ARGV
来源：http://kpj.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://mdz.jqgufenzy.top

[M02] 读取环境变量
来源：http://woy.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://rnf.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zxx.zhoulong.xyz

JS:   process.env.HOME
来源：http://ilq.yongpay.top

TS:   process.env.HOME
来源：http://jvp.tarul.cn

Java: System.getenv("HOME")
来源：http://lto.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rtx.pycfn.com

Ruby: ENV["HOME"]
来源：http://nqw.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://crt.316326.xyz

[M03] 执行外部命令
来源：http://teq.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rit.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gka.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rct.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qwn.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jom.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rrt.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tne.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://gwf.bjfxy.top

[M04] 获取当前工作目录
来源：http://gwl.cucudq.cn

Py:   os.getcwd()
来源：http://vsc.uphjek.com

PHP:  getcwd();
来源：http://mpr.bjfxy.top

JS:   process.cwd()
来源：http://xrf.ydzc1.top

TS:   process.cwd()
来源：http://abp.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://bxp.svipenyu.cn

Go:   os.Getwd()
来源：http://elb.jyoumei.cn

Ruby: Dir.pwd
来源：http://cuz.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nbh.chenjidiqi.icu

[M05] 设置退出码
来源：http://fmb.gzhubu.top

Py:   sys.exit(1)
来源：http://xfd.guannengcc.top

PHP:  exit(1);
来源：http://mhy.vqdsnc.cn

JS:   process.exit(1)
来源：http://vrh.snrcjt.cn

TS:   process.exit(1)
来源：http://tqi.andypj.xyz

Java: System.exit(1)
来源：http://pyn.yangfankeji.com

Go:   os.Exit(1)
来源：http://sff.yongpay.top

Ruby: exit 1
来源：http://spk.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://buf.sweek.top

[M06] 向标准错误输出
来源：http://cee.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://yhc.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rlg.cashguo.top

JS:   console.error("err")
来源：http://mtb.cqqwz.cn

TS:   console.error("err")
来源：http://fsy.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://eaq.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cts.chenlongwang.top

Ruby: warn "err"
来源：http://yjs.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://cfb.daria6918.cn

[M07] 判断是否为主入口
来源：http://imw.hammf.cn

Py:   if __name__ == "__main__":
来源：http://vkt.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wci.hysaishi.cn

JS:   require.main === module
来源：http://gas.gotoacloud.top

TS:   require.main === module
来源：http://wnc.cashguo.top

Java: public static void main(String[] args)
来源：http://bbi.ivvv.top

Go:   func main()
来源：http://yfy.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dbj.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://hjt.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://mzz.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://dax.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://afg.guannengcc.top

JS:   process.platform;  process.version
来源：http://ucv.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://ypg.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wvc.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://stb.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ixv.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://awm.yfazqb.com

================================================================================
来源：http://hqf.ybcxt.top

N. 数据结构与算法
来源：http://ovu.c1oappe.top

================================================================================
来源：http://bmt.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://trd.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://fpn.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mfk.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ltp.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mop.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://jri.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://pif.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://pak.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fpm.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://ojf.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://ydd.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hqk.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rip.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ahe.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ylv.tian-w.cn

Go:   slices.Sort(arr)
来源：http://esh.shangyingyoupin.top

Ruby: arr.sort
来源：http://cac.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://ame.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://hia.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bdl.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://koj.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lwr.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kja.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wwc.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vta.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yda.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://frq.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://ymb.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nmz.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uaj.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fbq.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqm.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xoi.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://psq.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zmp.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovz.yj20258888.top

[N05] 最大公约数
来源：http://ons.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://dta.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gbm.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ymf.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gbb.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://udn.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qtu.fzhhl.top

Ruby: a.gcd(b)
来源：http://orb.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wxj.jqgufenzy.top

[N06] 判断回文字符串
来源：http://vgv.sjlbkw.cn

Py:   s == s[::-1]
来源：http://bqt.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://arj.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://ntb.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://thh.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gty.xinyue.icu

Go:   // 双指针从两端比较
来源：http://aol.cdnleiting.top

Ruby: s == s.reverse
来源：http://lla.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xwu.birdmap.top

[N07] 两数之和（返回下标）
来源：http://mdu.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wwp.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tbc.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pzs.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://wsd.wangdashe.top

Java: // 手写 HashMap
来源：http://mow.ywan-chungtsiang.top


<!-- 参考信息 -->