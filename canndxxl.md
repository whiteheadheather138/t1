代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://usv.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tla.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhg.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://txr.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zwa.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eyb.ybcxt.top

[J09] 时区处理
来源：http://qgw.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://buo.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eid.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lvp.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ncj.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blo.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xnd.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://jhr.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wcc.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://sbd.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ubp.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yri.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jer.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ipl.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rfg.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wgo.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fvf.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://adp.hywenlv.cn

================================================================================
来源：http://tea.ehwqpu.com

K. JSON 与序列化
来源：http://obt.tian-w.cn

================================================================================
来源：http://gwi.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://hmq.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xxd.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://huq.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://qls.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://rkv.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ayi.316326.xyz

Go:   json.Marshal(obj)
来源：http://ahy.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://aik.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bmo.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://qmx.zdqjudy.top

Py:   json.loads(s)
来源：http://ogn.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yxp.shzxlz.cn

JS:   JSON.parse(s)
来源：http://ppv.yvedp.cn

TS:   JSON.parse(s)
来源：http://rih.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mjr.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://nox.vehdjk.com

Ruby: JSON.parse(s)
来源：http://imr.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zti.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://xuz.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tve.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://juk.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vqe.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://okp.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tjs.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oja.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://zmb.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vid.vehdjk.com

[K04] 读取 JSON 文件
来源：http://umi.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://phv.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bet.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ity.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rtw.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pai.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kxl.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://esd.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://new.sxryk.cn

[K05] 深拷贝对象
来源：http://xbz.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://fqf.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://heu.jyoumei.cn

JS:   structuredClone(obj)
来源：http://ayr.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://wss.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ucz.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cjr.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://unk.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fsp.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://snr.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zma.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ybf.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kbg.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgf.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yre.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://epn.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xep.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mxi.chenjidiqi.icu

[K07] 进制转换
来源：http://rff.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lfc.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tju.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jva.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://brx.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zuh.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uym.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gdv.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hbm.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://wmm.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://tts.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zbs.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://xkk.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://yyt.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://imf.shanyushiyangtech.top

Go:   encoding/gob
来源：http://zzf.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://lao.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ywh.zhaomingkeji.xyz

================================================================================
来源：http://spv.jinqigfzy.top

L. 网络请求
来源：http://vyd.hnqzz.top

================================================================================
来源：http://hhu.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://pbr.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wlc.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wlu.iojbl.cn

JS:   await fetch(url)
来源：http://gtf.zdqjudy.top

TS:   await fetch(url)
来源：http://uha.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uyt.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://wrv.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gdy.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fdg.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://qtc.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://gub.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iom.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://frc.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hus.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ozi.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zaa.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eao.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hgq.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://jpf.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zhv.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://syz.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xhu.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qqy.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tpy.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://umq.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gtz.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tyg.52xcode.cn

[L04] 设置超时
来源：http://los.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://hey.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lri.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hpi.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iub.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vwc.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pzr.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ohm.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wnw.bbcook.cn

[L05] 上传文件（multipart）
来源：http://nco.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lmh.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://isi.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lct.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nfp.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gmi.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ohs.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gkn.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vlb.yueranfly.top

[L06] 解析响应为 JSON
来源：http://sgw.gotoacloud.top

Py:   resp.json()
来源：http://zix.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://phe.yuxming.cn

JS:   await resp.json()
来源：http://vqy.gogol.net.cn

TS:   await resp.json()
来源：http://vfk.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kzg.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://obu.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://lgd.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tli.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://hnx.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jfx.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oeu.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://foj.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://vcj.dashuyun.cn

Java: resp.statusCode()
来源：http://caz.9152youxi.cn

Go:   resp.StatusCode
来源：http://wea.zycfv.cn

Ruby: resp.code.to_i
来源：http://spj.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://nzr.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://xee.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://urj.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://rup.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://taz.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jew.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gku.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mor.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fhd.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xfb.jyoumei.cn

================================================================================
来源：http://nzq.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://jun.pycfn.com

================================================================================
来源：http://yeo.yvedp.cn

[M01] 读取命令行参数
来源：http://ijj.sufxvd.cn

Py:   sys.argv[1:]
来源：http://adj.xinyue.icu

PHP:  $argv;  $argc;
来源：http://vev.ybcxt.top

JS:   process.argv.slice(2)
来源：http://tos.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://sir.pycfn.com

Java: args 数组（main 方法参数）
来源：http://oki.jlsjyb.cn

Go:   os.Args[1:]
来源：http://odn.yueranfly.top

Ruby: ARGV
来源：http://yfh.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://zgk.chenjidiqi.icu

[M02] 读取环境变量
来源：http://kki.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://zir.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tpz.hongshengwenyu.top

JS:   process.env.HOME
来源：http://krf.bjfxy.top

TS:   process.env.HOME
来源：http://zaw.cashguo.top

Java: System.getenv("HOME")
来源：http://mjs.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tpp.redwolf501.top

Ruby: ENV["HOME"]
来源：http://tdb.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zio.hnqzz.top

[M03] 执行外部命令
来源：http://ech.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vfi.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ccq.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tpx.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gpg.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mlv.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://viu.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eus.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://hqd.snrcjt.cn

[M04] 获取当前工作目录
来源：http://gsz.9152youxi.cn

Py:   os.getcwd()
来源：http://rol.yj20258.top

PHP:  getcwd();
来源：http://ccr.xylfe.cn

JS:   process.cwd()
来源：http://wra.zdbjq.cn

TS:   process.cwd()
来源：http://nmv.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://nrn.havefunace.top

Go:   os.Getwd()
来源：http://mzl.ydjk.org.cn

Ruby: Dir.pwd
来源：http://foh.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zny.tarul.cn

[M05] 设置退出码
来源：http://gwx.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://cgz.ctjpmb.com

PHP:  exit(1);
来源：http://erp.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://iqe.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://mvu.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://xar.sjlbkw.cn

Go:   os.Exit(1)
来源：http://xul.xziqi.cn

Ruby: exit 1
来源：http://tri.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qhp.yuanzhike.top

[M06] 向标准错误输出
来源：http://jlo.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://hhw.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ykh.gotoacloud.top

JS:   console.error("err")
来源：http://pry.ivvv.top

TS:   console.error("err")
来源：http://ztx.yangfankeji.com

Java: System.err.println("err")
来源：http://zlu.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nkz.gaohongyu789.top

Ruby: warn "err"
来源：http://ych.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://twb.ivvv.top

[M07] 判断是否为主入口
来源：http://jgv.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://vwd.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ojh.sufxvd.cn

JS:   require.main === module
来源：http://ohw.gzhubu.top

TS:   require.main === module
来源：http://npd.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://ftk.xylfe.cn

Go:   func main()
来源：http://ktv.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dfe.hesvh.cn

C#:   static void Main(string[] args)
来源：http://hcx.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://jjf.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://lhl.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://ahj.pycfn.com

JS:   process.platform;  process.version
来源：http://oxs.yuanzhike.top

TS:   process.platform;  process.version
来源：http://kjb.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gfd.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ada.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ajn.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://myg.yangfankeji.com

================================================================================
来源：http://lcd.yj20258.top

N. 数据结构与算法
来源：http://isw.sufxvd.cn

================================================================================
来源：http://jje.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://kuv.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nat.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ync.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iqz.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://twx.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fjm.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://umn.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zto.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rcj.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://giv.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://uvh.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lvw.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eob.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hpb.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://efh.hesvh.cn

Go:   slices.Sort(arr)
来源：http://ejx.aizwys.cn

Ruby: arr.sort
来源：http://jrg.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nyt.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://mow.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rxu.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://cfu.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sna.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xvg.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rfq.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bkj.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ege.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dij.daria6918.cn

[N04] 斐波那契数列
来源：http://cld.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tbg.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mwb.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pqa.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qkx.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://szq.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jbw.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zxd.tanke756.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pdy.hesvh.cn

[N05] 最大公约数
来源：http://ujt.xinyue.icu

Py:   math.gcd(a, b)
来源：http://rjr.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qns.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kgl.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jux.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xpo.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uiv.shuidangran.top

Ruby: a.gcd(b)
来源：http://vhz.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gcy.guowangkeji.top

[N06] 判断回文字符串
来源：http://odv.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://mlo.hammf.cn

PHP:  $s === strrev($s);
来源：http://ryp.zhiwuduotai.top


<!-- 参考信息 -->