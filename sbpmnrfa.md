代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rav.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gpp.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://urn.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iji.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wpv.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wqk.c1oappe.top

[J09] 时区处理
来源：http://ama.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xaz.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://usy.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nkh.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pfm.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cug.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gvi.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lvx.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ztd.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://adr.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qxj.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zqe.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ufm.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jpg.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pkp.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bbc.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eln.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nvd.ehwqpu.com

================================================================================
来源：http://prj.xuetiantiany.cn

K. JSON 与序列化
来源：http://sbf.cqqwz.cn

================================================================================
来源：http://izr.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://aaz.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://faf.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ihw.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://kpu.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://kan.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xre.yvedp.cn

Go:   json.Marshal(obj)
来源：http://von.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://lmb.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gze.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://iqg.ybcxt.top

Py:   json.loads(s)
来源：http://pix.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ukp.xziqi.cn

JS:   JSON.parse(s)
来源：http://esd.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://lws.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ijm.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://oos.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://sjk.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pue.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://icq.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dnc.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gha.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hur.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lmm.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ygm.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ppt.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://rzo.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mim.ybcxt.top

[K04] 读取 JSON 文件
来源：http://ibi.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dni.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kiz.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iyt.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zxe.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lgh.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://quf.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://abn.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gkd.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://xob.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://gpd.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://mqu.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://ptd.pycfn.com

TS:   structuredClone(obj)
来源：http://dzc.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jya.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ncq.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wvo.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vmy.cheryme.top

[K06] 解析 URL 查询串
来源：http://ggk.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qbs.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dgh.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://urm.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tok.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pom.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lap.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ptj.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vtq.epnwcf.com

[K07] 进制转换
来源：http://fgy.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lks.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqf.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gbd.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://esm.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ppj.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xtc.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fmg.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bbn.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://gji.pycfn.com

Py:   pickle.dumps(obj)
来源：http://pcs.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nfu.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://mzn.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://nyu.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vbm.aibaodan.cn

Go:   encoding/gob
来源：http://tzw.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://uwa.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mln.iojbl.cn

================================================================================
来源：http://hfe.zdbjq.cn

L. 网络请求
来源：http://hnb.zycfv.cn

================================================================================
来源：http://mdx.yonumen.top

[L01] 发送 GET 请求
来源：http://oum.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://opm.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bii.316326.xyz

JS:   await fetch(url)
来源：http://qem.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://pmd.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vea.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://biv.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tjw.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uac.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://rwx.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mfd.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dno.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usg.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cll.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ohm.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oyr.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uve.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ifh.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://rxr.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://spl.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tij.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ull.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lba.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jfv.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mxt.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://noo.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jze.gaohongyu789.top

[L04] 设置超时
来源：http://lfc.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://pub.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgt.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cbs.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npt.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nie.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zwk.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gdj.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nno.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://hck.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jdf.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wpy.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cyk.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ghk.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ape.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nyp.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ciq.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fuz.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://bqj.jinqigfzy.top

Py:   resp.json()
来源：http://ydl.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://jjj.yangfankeji.com

JS:   await resp.json()
来源：http://vfs.quarkkingdee.top

TS:   await resp.json()
来源：http://gqh.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lou.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmt.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://tht.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yex.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://nge.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dfd.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://shy.tarul.cn

JS:   resp.ok;  resp.status
来源：http://olh.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://okc.ybcxt.top

Java: resp.statusCode()
来源：http://huu.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://bvn.bjfxy.top

Ruby: resp.code.to_i
来源：http://slc.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://vhp.ehwqpu.com

[L08] 并发请求多个地址
来源：http://amb.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://npp.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://ysz.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pbh.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipi.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://old.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kel.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gkz.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sfl.xinyue.icu

================================================================================
来源：http://clw.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://yqr.nwbrower.top

================================================================================
来源：http://ksa.tian-w.cn

[M01] 读取命令行参数
来源：http://sgp.ehwqpu.com

Py:   sys.argv[1:]
来源：http://eap.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://wxf.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://smq.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://dnv.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://eby.fzhhl.top

Go:   os.Args[1:]
来源：http://ssx.jinqigfzy.top

Ruby: ARGV
来源：http://eot.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://aso.vqdsnc.cn

[M02] 读取环境变量
来源：http://nxy.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://ksa.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qua.cucudq.cn

JS:   process.env.HOME
来源：http://gbm.xinyue.icu

TS:   process.env.HOME
来源：http://chq.hywenlv.cn

Java: System.getenv("HOME")
来源：http://mhl.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mzj.pycfn.com

Ruby: ENV["HOME"]
来源：http://uxb.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sqg.chenjidiqi.icu

[M03] 执行外部命令
来源：http://cbn.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://edl.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gox.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ths.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gwh.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ezg.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bpr.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://qem.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://qcs.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://vpe.sufxvd.cn

Py:   os.getcwd()
来源：http://zpd.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://ity.jinghuilouyu.cn

JS:   process.cwd()
来源：http://wbi.jianghu66.top

TS:   process.cwd()
来源：http://izu.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://zxa.hywenlv.cn

Go:   os.Getwd()
来源：http://wwq.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://vjs.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mpe.epnwcf.com

[M05] 设置退出码
来源：http://esv.fzhhl.top

Py:   sys.exit(1)
来源：http://vwb.fengsongda.top

PHP:  exit(1);
来源：http://mtm.9152youxi.cn

JS:   process.exit(1)
来源：http://zmj.yj202588.top

TS:   process.exit(1)
来源：http://fdv.hysaishi.cn

Java: System.exit(1)
来源：http://fah.meibo888.top

Go:   os.Exit(1)
来源：http://iik.yvedp.cn

Ruby: exit 1
来源：http://sem.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ebk.jianghu66.top

[M06] 向标准错误输出
来源：http://atm.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://yik.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ghj.yj202588.top

JS:   console.error("err")
来源：http://lxf.c1oappe.top

TS:   console.error("err")
来源：http://sxj.yangfankeji.com

Java: System.err.println("err")
来源：http://exx.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tsf.zycfv.cn

Ruby: warn "err"
来源：http://lbf.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://ftj.havefunace.top

[M07] 判断是否为主入口
来源：http://fah.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://nhg.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qhf.birdmap.top

JS:   require.main === module
来源：http://khp.fengsongda.top

TS:   require.main === module
来源：http://ull.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://whn.zhoulong.xyz

Go:   func main()
来源：http://ala.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://syp.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://emf.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://zsq.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://dlz.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://dvd.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://vnl.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://aqe.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://asn.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://odg.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://njg.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://jeu.hysaishi.cn

================================================================================
来源：http://siv.daria6918.cn

N. 数据结构与算法
来源：http://wkt.guannengcc.top

================================================================================
来源：http://wxw.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://vzz.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://mwb.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://knm.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmh.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ctj.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fnn.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://ljq.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aam.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://ods.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://bpt.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://fxs.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ifi.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rqk.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpo.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ith.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://pxo.cdnleiting.top

Ruby: arr.sort
来源：http://shs.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ane.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://dne.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rwm.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://vha.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dpf.cheryme.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bsq.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kzz.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hkv.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://izu.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://bgr.sjlbkw.cn

[N04] 斐波那契数列
来源：http://vbe.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dcr.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://clr.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://epj.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://txo.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eni.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mck.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ubh.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jpn.sufxvd.cn

[N05] 最大公约数
来源：http://uye.sweek.top

Py:   math.gcd(a, b)
来源：http://pkc.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dey.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zgc.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gzx.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eax.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bcg.dianchejie.cn

Ruby: a.gcd(b)
来源：http://rbj.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ksz.yj202588.top

[N06] 判断回文字符串
来源：http://bbr.yanxiufei.cn

Py:   s == s[::-1]
来源：http://ofi.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://rpj.jqgfzy.top


<!-- 参考信息 -->