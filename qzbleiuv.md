代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://oeq.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zny.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohd.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://jgu.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xqr.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://iyx.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://dvs.pycfn.com

[J06] 计算两时间之差
来源：http://yto.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://csy.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://pvx.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kka.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fkr.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://bxg.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://lqx.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://eyt.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://shj.316326.xyz

[J07] 比较两个日期
来源：http://brt.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://zpd.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kdy.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lte.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://auk.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://odf.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lph.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://fyk.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://iop.fengsongda.top

[J08] 提取年月日与星期
来源：http://jdg.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rqu.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lqp.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jki.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tej.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vym.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://prw.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hnr.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vga.zycfv.cn

[J09] 时区处理
来源：http://ggu.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dit.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nvk.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oha.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://crt.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://boh.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fpa.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yjx.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bda.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://imz.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://hla.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zqr.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://agd.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qzt.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://npq.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qgk.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kkk.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cio.ybcxt.top

================================================================================
来源：http://hae.hesvh.cn

K. JSON 与序列化
来源：http://wcd.shanyushiyangtech.top

================================================================================
来源：http://glo.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://vcr.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ydx.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ndg.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://oko.yj20258.top

TS:   JSON.stringify(obj)
来源：http://vaf.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ouv.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://iko.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://gvi.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pxd.sxryk.cn

[K02] JSON 字符串转对象
来源：http://imb.tianlin.xyz

Py:   json.loads(s)
来源：http://sse.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xdq.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://wan.yj20258888.top

TS:   JSON.parse(s)
来源：http://ids.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uqd.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://jap.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://zar.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://agj.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://dvf.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vqk.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pip.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://saw.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ecg.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yfc.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fhf.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dmi.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bua.hesvh.cn

[K04] 读取 JSON 文件
来源：http://odn.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tuo.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kge.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uoy.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lxo.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zep.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nge.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uhx.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hgd.yueranfly.top

[K05] 深拷贝对象
来源：http://wvc.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://qwm.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://rqy.svipenyu.cn

JS:   structuredClone(obj)
来源：http://yro.guannengcc.top

TS:   structuredClone(obj)
来源：http://vwd.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gjg.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xnn.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jnl.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ubs.c1oappe.top

[K06] 解析 URL 查询串
来源：http://muh.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bjx.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ptu.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iiu.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rvl.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://doe.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cus.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://atf.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://srf.wangdashe.top

[K07] 进制转换
来源：http://lxq.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pqx.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://heu.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cpd.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zgh.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vby.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xtj.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://otv.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tot.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://nai.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://lpb.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ada.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://gdz.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://lqh.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ehb.xylfe.cn

Go:   encoding/gob
来源：http://bek.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://oic.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ggb.vqdsnc.cn

================================================================================
来源：http://src.jqgufenzy.top

L. 网络请求
来源：http://ahr.vehdjk.com

================================================================================
来源：http://taa.cqqwz.cn

[L01] 发送 GET 请求
来源：http://oxv.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ude.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://div.yj20258888.top

JS:   await fetch(url)
来源：http://tgz.jqgfzy.top

TS:   await fetch(url)
来源：http://zcs.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://npo.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://kgv.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://soy.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hcq.daxiang520.top

[L02] 发送 POST JSON
来源：http://kuk.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://pvx.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nrh.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yex.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rja.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nur.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jay.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nip.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cbr.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://qyh.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qog.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qsx.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zqb.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://idq.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fzb.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lun.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lbg.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dwn.shanyushiyangtech.top

[L04] 设置超时
来源：http://zoj.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://sqa.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://huc.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgb.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://plp.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fca.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rfd.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cic.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jhn.yj20258.top

[L05] 上传文件（multipart）
来源：http://rtr.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qes.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tjj.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ruw.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://itj.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hxl.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bkw.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zqa.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://smd.vehdjk.com

[L06] 解析响应为 JSON
来源：http://vby.xylfe.cn

Py:   resp.json()
来源：http://xpt.havefunace.top

PHP:  json_decode($body, true);
来源：http://fio.guannengcc.top

JS:   await resp.json()
来源：http://lmb.wangdashe.top

TS:   await resp.json()
来源：http://osj.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ocd.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wbi.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://msw.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bnu.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://ueb.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://evu.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txz.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://rpf.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://xrh.meibo888.top

Java: resp.statusCode()
来源：http://lgn.nanxuanxn.top

Go:   resp.StatusCode
来源：http://uhs.zhixingplan.top

Ruby: resp.code.to_i
来源：http://uqs.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://zxc.cheryme.top

[L08] 并发请求多个地址
来源：http://vkd.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ghz.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://sro.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kob.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://joe.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gzt.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yem.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wax.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yta.xuetiantiany.cn

================================================================================
来源：http://shi.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://rzn.xingfuxueyuan.xyz

================================================================================
来源：http://som.chenlongwang.top

[M01] 读取命令行参数
来源：http://tpe.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://hfn.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://eyp.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://ytv.bjfxy.top

TS:   process.argv.slice(2)
来源：http://rgi.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://xbe.ybcxt.top

Go:   os.Args[1:]
来源：http://qtv.fanxiaobao.xyz

Ruby: ARGV
来源：http://liz.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://lbw.xuetiantiany.cn

[M02] 读取环境变量
来源：http://ivk.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://ari.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ccp.yvedp.cn

JS:   process.env.HOME
来源：http://xok.cucudq.cn

TS:   process.env.HOME
来源：http://lze.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://ysa.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cdj.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://bue.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xvq.chenlongwang.top

[M03] 执行外部命令
来源：http://zcx.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xpc.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://chl.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uix.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jwz.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nzd.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ihp.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://jpu.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://tgj.cheryme.top

[M04] 获取当前工作目录
来源：http://sfv.shangyingyoupin.top

Py:   os.getcwd()
来源：http://otq.gogol.net.cn

PHP:  getcwd();
来源：http://mbq.sjlbkw.cn

JS:   process.cwd()
来源：http://eig.sxryk.cn

TS:   process.cwd()
来源：http://shh.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://ejq.vqdsnc.cn

Go:   os.Getwd()
来源：http://gvd.xziqi.cn

Ruby: Dir.pwd
来源：http://zyi.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vns.cheryme.top

[M05] 设置退出码
来源：http://wnt.ydjk.org.cn

Py:   sys.exit(1)
来源：http://coy.shangyingyoupin.top

PHP:  exit(1);
来源：http://qui.zhijiandao.cn

JS:   process.exit(1)
来源：http://vde.dashuyun.cn

TS:   process.exit(1)
来源：http://aev.zhijiandao.cn

Java: System.exit(1)
来源：http://rge.yj20258.top

Go:   os.Exit(1)
来源：http://zwv.snrcjt.cn

Ruby: exit 1
来源：http://bgs.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://miu.zdqjudy.top

[M06] 向标准错误输出
来源：http://rpg.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://zsg.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xzp.xinyue.icu

JS:   console.error("err")
来源：http://zyk.bbcook.cn

TS:   console.error("err")
来源：http://uco.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://grd.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gnd.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://alw.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://xfo.sufxvd.cn

[M07] 判断是否为主入口
来源：http://nvy.cheryme.top

Py:   if __name__ == "__main__":
来源：http://ekd.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rie.ctjpmb.com

JS:   require.main === module
来源：http://jlf.jianghu66.top

TS:   require.main === module
来源：http://sjs.jianghu66.top

Java: public static void main(String[] args)
来源：http://gzq.zhiwuduotai.top

Go:   func main()
来源：http://frg.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yfu.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://vns.pycfn.com

[M08] 获取系统与运行时信息
来源：http://tvf.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://izn.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://olc.ivvv.top

JS:   process.platform;  process.version
来源：http://xwd.tian-w.cn

TS:   process.platform;  process.version
来源：http://pxr.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wfq.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aak.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ceh.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yej.pengpengdd.cyou

================================================================================
来源：http://wve.bbcook.cn

N. 数据结构与算法
来源：http://qnk.ydzc1.top

================================================================================
来源：http://kra.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://ock.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://nav.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gcn.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpz.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yzk.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://ouz.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://prt.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gdg.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ugi.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://rlu.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://lot.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ddx.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jga.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hhs.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yyi.yongpay.top

Go:   slices.Sort(arr)
来源：http://lss.jiagoushi.top

Ruby: arr.sort
来源：http://hyq.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://aiv.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://ohx.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://muk.jinqigfzy.top


<!-- 参考信息 -->