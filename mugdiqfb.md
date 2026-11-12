代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nsi.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gwa.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xhz.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lvj.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://srq.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kcs.jqgufenzy.top

[J09] 时区处理
来源：http://cdi.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kgs.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivr.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zcl.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhu.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://puu.jyoumei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wom.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://klt.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rjx.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://rsw.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lae.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rkk.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://biz.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://epj.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jmx.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sdv.dashuyun.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bgs.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myo.ywan-chungtsiang.top

================================================================================
来源：http://ujt.zdqjudy.top

K. JSON 与序列化
来源：http://wur.dashuyun.cn

================================================================================
来源：http://cbh.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://arr.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tkn.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://giz.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://bof.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://mvb.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qlw.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://zmo.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://qty.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nbd.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://kft.c1oappe.top

Py:   json.loads(s)
来源：http://klp.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cia.wangdashe.top

JS:   JSON.parse(s)
来源：http://czc.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://djk.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xrf.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://qcs.cashguo.top

Ruby: JSON.parse(s)
来源：http://dsc.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kdp.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://xst.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vli.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mqx.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://afk.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mrr.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bue.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://art.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://yce.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://myq.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://ucx.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twy.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jkk.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awl.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wyi.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xgq.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qbs.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nsk.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oyl.yj20258.top

[K05] 深拷贝对象
来源：http://mpn.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://ohm.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://xtw.bjfxy.top

JS:   structuredClone(obj)
来源：http://cjb.9152youxi.cn

TS:   structuredClone(obj)
来源：http://iop.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uwc.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wxm.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wvr.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ubi.yfazqb.com

[K06] 解析 URL 查询串
来源：http://syn.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zws.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tsh.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jac.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afw.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cfl.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iby.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://arc.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kxu.gotoacloud.top

[K07] 进制转换
来源：http://mln.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nib.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjp.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qlq.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://slk.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ywv.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eog.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oji.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://stq.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://mmx.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://fgx.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jld.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://rzm.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://kpl.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mti.zhixingplan.top

Go:   encoding/gob
来源：http://cyp.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://tsc.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lfj.fzhhl.top

================================================================================
来源：http://feo.ydzc1.top

L. 网络请求
来源：http://yer.ydzc1.top

================================================================================
来源：http://tfq.ctjpmb.com

[L01] 发送 GET 请求
来源：http://xlh.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ztl.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gdt.xuetiantiany.cn

JS:   await fetch(url)
来源：http://eoi.vehdjk.com

TS:   await fetch(url)
来源：http://umh.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lxp.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://bkm.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cfz.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qlq.daxiang520.top

[L02] 发送 POST JSON
来源：http://sie.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://thg.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aws.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbp.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://soj.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zfq.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://six.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qta.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kzz.sweek.top

[L03] 设置自定义请求头
来源：http://aug.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sjq.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nge.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yui.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gwm.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uet.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://abj.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://muf.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ahf.nwbrower.top

[L04] 设置超时
来源：http://evp.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://fkw.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://unn.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jzg.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwa.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ikf.zhengqikj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://juv.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zmh.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zfv.mhx1999.top

[L05] 上传文件（multipart）
来源：http://kzh.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfn.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jzf.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rgy.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qte.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wed.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mhp.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nbz.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fyf.yj20258.top

[L06] 解析响应为 JSON
来源：http://cih.jyoumei.cn

Py:   resp.json()
来源：http://bwk.mhx1999.top

PHP:  json_decode($body, true);
来源：http://oix.kuanghao11.cn

JS:   await resp.json()
来源：http://cwa.zhengqikj.top

TS:   await resp.json()
来源：http://mti.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jpy.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qyi.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://cjc.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gpo.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://lst.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vwr.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxd.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://nsx.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://baj.xuetiantiany.cn

Java: resp.statusCode()
来源：http://pdl.cheryme.top

Go:   resp.StatusCode
来源：http://vqx.cucudq.cn

Ruby: resp.code.to_i
来源：http://sse.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://pjf.tanke756.top

[L08] 并发请求多个地址
来源：http://ljl.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gsb.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://rgc.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aui.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tha.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qpq.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sab.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zbh.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://unq.sweek.top

================================================================================
来源：http://ocj.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://ufy.daria6918.cn

================================================================================
来源：http://jrp.yangfankeji.com

[M01] 读取命令行参数
来源：http://nxj.cheryme.top

Py:   sys.argv[1:]
来源：http://wua.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://bxw.tian-w.cn

JS:   process.argv.slice(2)
来源：http://ukr.xinyue.icu

TS:   process.argv.slice(2)
来源：http://afh.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://fmg.fengsongda.top

Go:   os.Args[1:]
来源：http://ssy.cdnleiting.top

Ruby: ARGV
来源：http://tqw.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://ona.hcnkem.com

[M02] 读取环境变量
来源：http://jos.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://xxl.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itt.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://nij.chenjidiqi.icu

TS:   process.env.HOME
来源：http://cji.redwolf501.top

Java: System.getenv("HOME")
来源：http://oye.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uvy.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://yoo.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://czu.ctjpmb.com

[M03] 执行外部命令
来源：http://ywh.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vcg.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://obz.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mfy.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://zdl.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gtx.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://txw.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://aqb.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://lwy.nanxuanxn.top

[M04] 获取当前工作目录
来源：http://iqr.hnqzz.top

Py:   os.getcwd()
来源：http://nec.ydzc1.top

PHP:  getcwd();
来源：http://krg.jinqigfzy.top

JS:   process.cwd()
来源：http://thi.svipenyu.cn

TS:   process.cwd()
来源：http://ipe.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://cbi.ydzc1.top

Go:   os.Getwd()
来源：http://yxj.jlsjyb.cn

Ruby: Dir.pwd
来源：http://ifc.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://snu.fktsv.cn

[M05] 设置退出码
来源：http://dxl.bjfxy.top

Py:   sys.exit(1)
来源：http://jte.xinyue.icu

PHP:  exit(1);
来源：http://uxs.316326.xyz

JS:   process.exit(1)
来源：http://pep.sjlbkw.cn

TS:   process.exit(1)
来源：http://fqs.iojbl.cn

Java: System.exit(1)
来源：http://rww.ppjwa.cn

Go:   os.Exit(1)
来源：http://uur.sweek.top

Ruby: exit 1
来源：http://iun.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zkv.gaohongyu789.top

[M06] 向标准错误输出
来源：http://zsz.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://atw.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sii.gotoacloud.top

JS:   console.error("err")
来源：http://ive.52xcode.cn

TS:   console.error("err")
来源：http://ujv.c1oappe.top

Java: System.err.println("err")
来源：http://naf.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://set.redwolf501.top

Ruby: warn "err"
来源：http://ver.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dzg.dianchejie.cn

[M07] 判断是否为主入口
来源：http://ibr.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://lqn.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hun.uphjek.com

JS:   require.main === module
来源：http://xev.tian-w.cn

TS:   require.main === module
来源：http://fpl.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://pun.quarkkingdee.top

Go:   func main()
来源：http://zkz.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cjx.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://qsx.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://ktc.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://wfq.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://sdd.hywenlv.cn

JS:   process.platform;  process.version
来源：http://sqn.yj202588.top

TS:   process.platform;  process.version
来源：http://nom.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wyr.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dpy.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eop.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ldn.zhoulong.xyz

================================================================================
来源：http://puz.gotoacloud.top

N. 数据结构与算法
来源：http://cez.hfpthk.cn

================================================================================
来源：http://czz.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://dpv.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://oks.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ndy.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dje.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlu.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://who.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://xiu.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ibr.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://nni.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://bgq.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://lqy.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gdz.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://isv.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bmc.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tnf.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://cru.havefunace.top

Ruby: arr.sort
来源：http://yyn.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://miq.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://fhc.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qmr.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://dqc.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dcl.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yff.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zgv.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lht.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyv.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wyo.yfazqb.com

[N04] 斐波那契数列
来源：http://myj.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qok.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bqn.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://scl.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bay.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dox.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://knd.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hzv.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qeh.yonumen.top

[N05] 最大公约数
来源：http://lkw.birdmap.top

Py:   math.gcd(a, b)
来源：http://crt.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cgs.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wck.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kps.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://crv.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rso.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://hkf.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vyk.yvedp.cn

[N06] 判断回文字符串
来源：http://pgl.zdbjq.cn

Py:   s == s[::-1]
来源：http://qih.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://jny.yj20258888.top


<!-- 参考信息 -->