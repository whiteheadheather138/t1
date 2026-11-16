代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mlo.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kmj.pengpengdd.cyou

[J09] 时区处理
来源：http://hrp.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tqv.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iyk.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cbm.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgy.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xdi.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oeu.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fha.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://anf.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://vmj.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hmd.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://auz.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vsa.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://itm.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yrx.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ugf.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jom.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vya.guannengcc.top

================================================================================
来源：http://xap.smart0.xyz

K. JSON 与序列化
来源：http://wii.yj20258888.top

================================================================================
来源：http://hbi.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://nry.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eiz.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hpl.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://muc.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://ydr.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xso.epnwcf.com

Go:   json.Marshal(obj)
来源：http://hgx.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://bvo.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gje.sxryk.cn

[K02] JSON 字符串转对象
来源：http://jlg.xuetiantiany.cn

Py:   json.loads(s)
来源：http://ocg.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fey.gzhubu.top

JS:   JSON.parse(s)
来源：http://epd.jqgfzy.top

TS:   JSON.parse(s)
来源：http://xng.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ski.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://jur.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://ogp.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bxi.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://afq.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qvm.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qqe.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://umj.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nua.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vgf.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ovp.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://qvv.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xgo.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://mdx.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twy.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oam.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uyu.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nga.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eve.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uwd.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wch.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qwr.yj20258888.top

[K05] 深拷贝对象
来源：http://cax.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://fyi.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://fhg.chenlongwang.top

JS:   structuredClone(obj)
来源：http://mzq.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://bnu.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vif.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://apt.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ltr.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lnj.zycfv.cn

[K06] 解析 URL 查询串
来源：http://jvm.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://edx.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gyh.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ymo.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nnp.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lth.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ocg.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uhs.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fwx.xuanzx.com

[K07] 进制转换
来源：http://fkm.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tol.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oyo.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tng.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gqy.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qhy.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://doi.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://onu.kuanghao11.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dxx.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://arb.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://rkl.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cnd.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://kat.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://zue.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bxz.gogol.net.cn

Go:   encoding/gob
来源：http://wul.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://gto.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hlv.xziqi.cn

================================================================================
来源：http://kch.zdbjq.cn

L. 网络请求
来源：http://ocv.svipenyu.cn

================================================================================
来源：http://lyp.yueranfly.top

[L01] 发送 GET 请求
来源：http://bri.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dgd.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fht.yanxiufei.cn

JS:   await fetch(url)
来源：http://gkf.wangdashe.top

TS:   await fetch(url)
来源：http://uzt.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zav.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://xjm.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://umx.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pco.gzhubu.top

[L02] 发送 POST JSON
来源：http://nvi.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hur.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjt.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cfz.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lqp.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yse.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jpx.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ieb.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fkk.yvedp.cn

[L03] 设置自定义请求头
来源：http://xch.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eyd.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iix.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://saz.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://htj.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lin.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://upa.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ukn.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uez.fzhhl.top

[L04] 设置超时
来源：http://ody.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://bih.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://csg.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://shp.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nda.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pkb.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oqp.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bkt.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://brm.tanke756.top

[L05] 上传文件（multipart）
来源：http://rnb.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fmy.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mfj.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aoh.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vof.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yup.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wag.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ity.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cfl.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://bpr.zhongyouzk.top

Py:   resp.json()
来源：http://xfu.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://psc.chenjidiqi.icu

JS:   await resp.json()
来源：http://she.nwbrower.top

TS:   await resp.json()
来源：http://eao.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://knl.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qtf.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://hwz.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gpx.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://cfc.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bay.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://muj.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://qwd.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://hce.pycfn.com

Java: resp.statusCode()
来源：http://cxd.fzhhl.top

Go:   resp.StatusCode
来源：http://ius.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://dgl.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://joh.birdmap.top

[L08] 并发请求多个地址
来源：http://cqo.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jye.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://wft.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xvs.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tsy.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pxb.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yty.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xsl.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://unf.birdmap.top

================================================================================
来源：http://byq.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://fel.sjlbkw.cn

================================================================================
来源：http://hbe.gogol.net.cn

[M01] 读取命令行参数
来源：http://zdm.bjfxy.top

Py:   sys.argv[1:]
来源：http://fdd.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://rcv.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://chm.hammf.cn

TS:   process.argv.slice(2)
来源：http://skq.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://dpp.ydjk.org.cn

Go:   os.Args[1:]
来源：http://lky.hnqzz.top

Ruby: ARGV
来源：http://xno.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://cov.zhiwuduotai.top

[M02] 读取环境变量
来源：http://mks.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://dby.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://afg.hcnkem.com

JS:   process.env.HOME
来源：http://arx.bjfxy.top

TS:   process.env.HOME
来源：http://cov.yuxming.cn

Java: System.getenv("HOME")
来源：http://oxk.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xwm.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://smj.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vkv.zhixingplan.top

[M03] 执行外部命令
来源：http://eyp.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dgj.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oev.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nvu.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ptb.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qsa.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kgy.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://orr.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://xkj.cashguo.top

[M04] 获取当前工作目录
来源：http://xrr.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://btp.hnqzz.top

PHP:  getcwd();
来源：http://ydr.epnwcf.com

JS:   process.cwd()
来源：http://fnn.svipenyu.cn

TS:   process.cwd()
来源：http://fxd.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://lax.guowangkeji.top

Go:   os.Getwd()
来源：http://vqc.birdmap.top

Ruby: Dir.pwd
来源：http://swr.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://daw.hesvh.cn

[M05] 设置退出码
来源：http://qck.jqgfzy.top

Py:   sys.exit(1)
来源：http://ihc.chenlongwang.top

PHP:  exit(1);
来源：http://qwz.tanke756.top

JS:   process.exit(1)
来源：http://joq.smart0.xyz

TS:   process.exit(1)
来源：http://ihw.tanke756.top

Java: System.exit(1)
来源：http://inb.zdqjudy.top

Go:   os.Exit(1)
来源：http://gyn.xuetiantiany.cn

Ruby: exit 1
来源：http://wjh.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bnv.fengsongda.top

[M06] 向标准错误输出
来源：http://jyz.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://nvl.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kkn.hcnkem.com

JS:   console.error("err")
来源：http://ahc.sufxvd.cn

TS:   console.error("err")
来源：http://ozy.fengsongda.top

Java: System.err.println("err")
来源：http://brn.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pcw.zhiwuduotai.top

Ruby: warn "err"
来源：http://huh.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://vbt.pycfn.com

[M07] 判断是否为主入口
来源：http://zsl.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://hzj.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gaa.chenzaomai.com

JS:   require.main === module
来源：http://bte.daria6918.cn

TS:   require.main === module
来源：http://gnh.jiagoushi.top

Java: public static void main(String[] args)
来源：http://lfn.bjfxy.top

Go:   func main()
来源：http://hjw.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uqo.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://all.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://ctf.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://bur.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://lry.chenlongwang.top

JS:   process.platform;  process.version
来源：http://ifc.zhixingplan.top

TS:   process.platform;  process.version
来源：http://lof.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jmg.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rvu.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bvj.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lar.xuetiantiany.cn

================================================================================
来源：http://zew.sxryk.cn

N. 数据结构与算法
来源：http://lqu.ydjk.org.cn

================================================================================
来源：http://vqv.cheryme.top

[N01] 二分查找（有序数组）
来源：http://rhu.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://ref.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://opj.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ilq.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qiu.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://qgk.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://svd.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mzm.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ood.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://vvy.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vau.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ryg.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://iip.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qnt.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uwc.mhx1999.top

Go:   slices.Sort(arr)
来源：http://gcf.yueranfly.top

Ruby: arr.sort
来源：http://lnn.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://qzy.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://bgw.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://umt.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://dvd.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://der.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://weo.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cye.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mdk.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wip.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://dec.cashguo.top

[N04] 斐波那契数列
来源：http://jvj.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://klg.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://duh.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azt.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://buu.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yqh.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rcl.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sym.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qmn.birdmap.top

[N05] 最大公约数
来源：http://nri.fengsongda.top

Py:   math.gcd(a, b)
来源：http://qzm.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tev.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvu.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vpx.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sda.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dan.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://dwl.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uub.jiagoushi.top

[N06] 判断回文字符串
来源：http://mjl.hcnkem.com

Py:   s == s[::-1]
来源：http://hzt.yongpay.top

PHP:  $s === strrev($s);
来源：http://kjx.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://bxl.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://cna.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://luk.nwbrower.top

Go:   // 双指针从两端比较
来源：http://clx.zhengqikj.top


<!-- 参考信息 -->