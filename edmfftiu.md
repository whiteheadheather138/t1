代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dgn.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://aaw.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://qzx.zdbjq.cn

[J06] 计算两时间之差
来源：http://qlh.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://zvf.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://iof.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bnp.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jpy.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://wmj.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://xrf.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://bib.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://lqu.jlsjyb.cn

[J07] 比较两个日期
来源：http://knk.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://wpf.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hrj.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zts.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dkc.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vuf.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ybu.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://nzz.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://noc.yuanzhike.top

[J08] 提取年月日与星期
来源：http://urj.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zwh.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qtf.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tjd.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qgy.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fsr.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zsm.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://drq.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iht.zhixingplan.top

[J09] 时区处理
来源：http://nvy.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zqw.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jzp.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yam.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvi.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oar.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xjl.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dih.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://slr.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://was.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://prl.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rdb.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nyw.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vin.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://esp.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wnh.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rkw.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pfv.shanyushiyangkeji.top

================================================================================
来源：http://aed.daria6918.cn

K. JSON 与序列化
来源：http://dyy.jinqigufen.top

================================================================================
来源：http://xtr.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://rop.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qhv.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aep.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://uao.316326.xyz

TS:   JSON.stringify(obj)
来源：http://jwe.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qgq.yongpay.top

Go:   json.Marshal(obj)
来源：http://ufi.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://crb.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://imq.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://ydy.snrcjt.cn

Py:   json.loads(s)
来源：http://tmj.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aeg.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://odi.cdnleiting.top

TS:   JSON.parse(s)
来源：http://nff.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zkr.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://cuf.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://zbk.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://csz.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://hby.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ovl.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://flq.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ile.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ymf.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hlk.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ebq.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://foi.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xrz.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://nda.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tou.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nee.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ktr.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jsc.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kdz.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fra.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kuo.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wpb.fengsongda.top

[K05] 深拷贝对象
来源：http://zkl.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://brv.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://zqd.tian-w.cn

JS:   structuredClone(obj)
来源：http://dcg.zycfv.cn

TS:   structuredClone(obj)
来源：http://uhp.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mvf.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gof.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dqf.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://awk.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://vqm.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lig.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ptz.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fiw.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mcb.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yws.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fbu.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hmv.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mql.mhx1999.top

[K07] 进制转换
来源：http://mlh.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ghg.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bsl.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kal.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dqi.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jfi.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tqq.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jxw.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qda.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://mke.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://anf.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uub.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://vjt.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://iob.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dtp.ydjk.org.cn

Go:   encoding/gob
来源：http://jfr.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://sdk.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ulg.nanxinkj.top

================================================================================
来源：http://mqh.dianchejie.cn

L. 网络请求
来源：http://bnf.ydzc1.top

================================================================================
来源：http://eih.fehbvm.com

[L01] 发送 GET 请求
来源：http://han.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uif.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cux.yonumen.top

JS:   await fetch(url)
来源：http://owp.aibaodan.cn

TS:   await fetch(url)
来源：http://bmj.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yne.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://nhx.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://azq.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sfa.nwbrower.top

[L02] 发送 POST JSON
来源：http://yqx.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://vpz.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mpq.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xcx.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wry.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cmx.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yzn.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://edt.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vck.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://vki.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fgc.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zzt.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpo.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://itz.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zob.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qhn.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://new.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bea.feifeiyinyue.top

[L04] 设置超时
来源：http://yil.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://jyk.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pbp.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmy.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyo.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://trz.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cwn.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mkh.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tsc.mhx1999.top

[L05] 上传文件（multipart）
来源：http://fqt.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://awn.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hbp.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ntg.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yir.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://amg.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eac.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kdm.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqu.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://wrp.wangdashe.top

Py:   resp.json()
来源：http://xdk.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://ncz.xinyue.icu

JS:   await resp.json()
来源：http://jwa.xuanzx.com

TS:   await resp.json()
来源：http://yhn.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ttq.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zwk.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://wvg.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://keg.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://cdf.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bpb.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qwk.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://pwm.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://qrc.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://acc.jqgfzy.top

Go:   resp.StatusCode
来源：http://jlm.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://whr.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://grv.uphjek.com

[L08] 并发请求多个地址
来源：http://teo.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xdg.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://vsq.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fyy.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmz.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tfs.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ckt.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pdn.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ena.yangfankeji.com

================================================================================
来源：http://pse.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://ucn.sufxvd.cn

================================================================================
来源：http://rzj.bjfxy.top

[M01] 读取命令行参数
来源：http://vak.yonumen.top

Py:   sys.argv[1:]
来源：http://xxa.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://yse.nwbrower.top

JS:   process.argv.slice(2)
来源：http://xtj.xylfe.cn

TS:   process.argv.slice(2)
来源：http://ele.yj202588.top

Java: args 数组（main 方法参数）
来源：http://iai.vqdsnc.cn

Go:   os.Args[1:]
来源：http://zsn.daxiang520.top

Ruby: ARGV
来源：http://phn.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://yof.ehwqpu.com

[M02] 读取环境变量
来源：http://frr.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://qeh.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pjf.yj20258888.top

JS:   process.env.HOME
来源：http://abs.fehbvm.com

TS:   process.env.HOME
来源：http://bzr.chenlongwang.top

Java: System.getenv("HOME")
来源：http://cxe.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tzz.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://dzg.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ocr.cqqwz.cn

[M03] 执行外部命令
来源：http://goy.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lqk.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lnn.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://acq.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://usa.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kzr.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yci.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://tde.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://qzc.hcnkem.com

[M04] 获取当前工作目录
来源：http://rso.shzxlz.cn

Py:   os.getcwd()
来源：http://afp.meibo888.top

PHP:  getcwd();
来源：http://htw.sysykeji.top

JS:   process.cwd()
来源：http://sdp.feifeiyinyue.top

TS:   process.cwd()
来源：http://lds.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://xwh.shangyingyoupin.top

Go:   os.Getwd()
来源：http://tsy.uphjek.com

Ruby: Dir.pwd
来源：http://qiq.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://kwz.zhijiandao.cn

[M05] 设置退出码
来源：http://eva.guannengcc.top

Py:   sys.exit(1)
来源：http://mtc.fehbvm.com

PHP:  exit(1);
来源：http://uxp.gotoacloud.top

JS:   process.exit(1)
来源：http://axt.guannengcc.top

TS:   process.exit(1)
来源：http://xxv.sxryk.cn

Java: System.exit(1)
来源：http://rby.tian-w.cn

Go:   os.Exit(1)
来源：http://zwn.cdnleiting.top

Ruby: exit 1
来源：http://jpj.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kko.zhoulong.xyz

[M06] 向标准错误输出
来源：http://pon.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://lbt.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wyr.chenzaomai.com

JS:   console.error("err")
来源：http://cxp.chenzaomai.com

TS:   console.error("err")
来源：http://gty.cucudq.cn

Java: System.err.println("err")
来源：http://vgv.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pgj.fehbvm.com

Ruby: warn "err"
来源：http://zbd.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://oyb.yonumen.top

[M07] 判断是否为主入口
来源：http://tof.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://uzx.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ara.zhengqikj.top

JS:   require.main === module
来源：http://wpa.kuanghao11.cn

TS:   require.main === module
来源：http://rzr.tianlin.xyz

Java: public static void main(String[] args)
来源：http://rzp.sufxvd.cn

Go:   func main()
来源：http://tav.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ouk.cheryme.top

C#:   static void Main(string[] args)
来源：http://hmm.tanke756.top

[M08] 获取系统与运行时信息
来源：http://nyr.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://zec.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://pil.ctjpmb.com

JS:   process.platform;  process.version
来源：http://eyk.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://yvl.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sok.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uwt.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pva.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xop.hesvh.cn

================================================================================
来源：http://pxf.xuanzx.com

N. 数据结构与算法
来源：http://unx.jinqigfzy.top

================================================================================
来源：http://whb.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://ili.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://jut.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fwu.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://whj.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ijq.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://htg.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://sqs.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ziy.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rvo.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://oje.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://zrf.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ymh.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rpy.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sve.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pdi.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://gya.havefunace.top

Ruby: arr.sort
来源：http://voj.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lrv.pycfn.com

[N03] 快速排序（分治示例）
来源：http://rmj.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wki.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://xak.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cun.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lcv.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://btd.vqdsnc.cn


<!-- 参考信息 -->