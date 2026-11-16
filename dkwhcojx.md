代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lhy.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sxi.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://rie.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://epj.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://luf.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wto.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hli.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://hoj.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sjt.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://nvj.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://jev.sweek.top

[J06] 计算两时间之差
来源：http://gei.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://ikv.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://irt.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vwt.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mmn.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://guf.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://wba.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://btz.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://dup.zhengqikj.top

[J07] 比较两个日期
来源：http://yiy.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://nor.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mwx.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://wkd.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ixm.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yrr.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://owt.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://chy.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://rup.yangfankeji.com

[J08] 提取年月日与星期
来源：http://ciq.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lsp.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vza.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://poi.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bjz.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jmp.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hbn.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hjz.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gih.nanxinkj.top

[J09] 时区处理
来源：http://spw.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://imo.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ade.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cwm.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bjn.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pte.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kuf.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://keh.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dxv.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://iea.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://akn.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ihd.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vey.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://awr.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qhf.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://agu.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bag.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfe.jianghu66.top

================================================================================
来源：http://dcz.vqdsnc.cn

K. JSON 与序列化
来源：http://xxb.cqqwz.cn

================================================================================
来源：http://fws.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://eso.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lxm.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yxg.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://lsw.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://slt.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aku.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://iaz.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://hga.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gnh.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://jby.fengsongda.top

Py:   json.loads(s)
来源：http://fvn.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tge.hysaishi.cn

JS:   JSON.parse(s)
来源：http://pcz.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://hge.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://axe.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://jbf.ydzc1.top

Ruby: JSON.parse(s)
来源：http://hzm.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zpd.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://esk.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://egq.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yni.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vox.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qdk.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jdy.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uce.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://tgs.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iop.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://fjh.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zsz.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vid.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awy.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpp.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uhn.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://whi.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ctw.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ven.guannengcc.top

[K05] 深拷贝对象
来源：http://otq.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://vcy.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://tce.havefunace.top

JS:   structuredClone(obj)
来源：http://gfv.tanke756.top

TS:   structuredClone(obj)
来源：http://wgy.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tei.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ppv.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://odo.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ajg.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://vnq.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cot.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cox.yueranfly.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ybu.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vns.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mnl.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vyr.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cxf.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qol.feifeiyinyue.top

[K07] 进制转换
来源：http://gtg.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cma.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qes.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ydb.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lps.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ojg.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rlt.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://emh.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qjk.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://etq.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://rxe.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://liu.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://wmg.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ida.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hlf.smart0.xyz

Go:   encoding/gob
来源：http://wpb.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://cgj.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ybz.yuanzhike.top

================================================================================
来源：http://eni.jinyuanbaomall.cn

L. 网络请求
来源：http://qtu.zhiwuduotai.top

================================================================================
来源：http://khd.yj20258888.top

[L01] 发送 GET 请求
来源：http://zpb.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://obo.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ncp.xinyue.icu

JS:   await fetch(url)
来源：http://klk.yj20258.top

TS:   await fetch(url)
来源：http://wlf.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aoh.sweek.top

Go:   resp, err := http.Get(url)
来源：http://bth.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qwq.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgk.guowangkeji.top

[L02] 发送 POST JSON
来源：http://yvr.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://lvo.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cmm.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mtc.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xzz.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://srv.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wgm.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://adi.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://alv.sxryk.cn

[L03] 设置自定义请求头
来源：http://djs.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nsg.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hrz.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lme.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dyy.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xdl.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qml.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bjy.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fdo.sweek.top

[L04] 设置超时
来源：http://vqc.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://pag.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://twl.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dnt.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dic.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cbm.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lcx.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zqp.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://znt.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://ppo.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://abp.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fdn.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hci.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sdx.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xjr.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blv.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zoa.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lnt.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://otf.chenzaomai.com

Py:   resp.json()
来源：http://yaw.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://oaj.fengsongda.top

JS:   await resp.json()
来源：http://cpt.xylfe.cn

TS:   await resp.json()
来源：http://hpl.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffy.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xne.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://wwu.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kjl.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://uqe.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bvi.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nja.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://tdk.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://tad.yanxiufei.cn

Java: resp.statusCode()
来源：http://aif.bbcook.cn

Go:   resp.StatusCode
来源：http://asz.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://ylh.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://jwm.birdmap.top

[L08] 并发请求多个地址
来源：http://tgk.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ele.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://gzr.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ukz.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qpn.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwq.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bzc.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qay.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kgg.jinyuanbaomall.cn

================================================================================
来源：http://hwq.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://tsa.sweek.top

================================================================================
来源：http://vqi.yongpay.top

[M01] 读取命令行参数
来源：http://fwq.daxiang520.top

Py:   sys.argv[1:]
来源：http://uwi.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://dqh.c1oappe.top

JS:   process.argv.slice(2)
来源：http://zfe.meibo888.top

TS:   process.argv.slice(2)
来源：http://sbc.yonumen.top

Java: args 数组（main 方法参数）
来源：http://aod.yvedp.cn

Go:   os.Args[1:]
来源：http://mgk.cheryme.top

Ruby: ARGV
来源：http://qmb.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://nuw.feifeiyinyue.top

[M02] 读取环境变量
来源：http://oer.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://zql.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rcx.xylfe.cn

JS:   process.env.HOME
来源：http://oyi.gzhubu.top

TS:   process.env.HOME
来源：http://qqd.yuanzhike.top

Java: System.getenv("HOME")
来源：http://qpa.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://adj.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://one.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bak.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://twg.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yll.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jdl.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qfh.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uiq.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ebn.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uas.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://zeh.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://xpz.hysaishi.cn

[M04] 获取当前工作目录
来源：http://nlr.hnqzz.top

Py:   os.getcwd()
来源：http://lyc.svipenyu.cn

PHP:  getcwd();
来源：http://boh.nanxinkj.top

JS:   process.cwd()
来源：http://afb.xinyue.icu

TS:   process.cwd()
来源：http://ezy.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://ejj.zycfv.cn

Go:   os.Getwd()
来源：http://otj.yonumen.top

Ruby: Dir.pwd
来源：http://aaj.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://lom.uphjek.com

[M05] 设置退出码
来源：http://tbj.ydzc1.top

Py:   sys.exit(1)
来源：http://dyr.c1oappe.top

PHP:  exit(1);
来源：http://lql.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://edn.cucudq.cn

TS:   process.exit(1)
来源：http://czu.fehbvm.com

Java: System.exit(1)
来源：http://rwz.yj202588.top

Go:   os.Exit(1)
来源：http://dzi.zhaomingkeji.xyz

Ruby: exit 1
来源：http://wna.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wiv.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://olo.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://afg.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uwu.kuanghao11.cn

JS:   console.error("err")
来源：http://ppk.hywenlv.cn

TS:   console.error("err")
来源：http://aqn.gotoacloud.top

Java: System.err.println("err")
来源：http://izj.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oll.gogol.net.cn

Ruby: warn "err"
来源：http://mwx.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://bln.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://rzk.yongpay.top

Py:   if __name__ == "__main__":
来源：http://cth.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wha.jyoumei.cn

JS:   require.main === module
来源：http://vqt.316326.xyz

TS:   require.main === module
来源：http://ggq.cashguo.top

Java: public static void main(String[] args)
来源：http://yil.zhiwuduotai.top

Go:   func main()
来源：http://ldr.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jcz.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://cht.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://tzi.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://urc.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://gcf.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://uxr.andypj.xyz

TS:   process.platform;  process.version
来源：http://cgf.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ayk.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dcx.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://glm.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hzi.zycfv.cn

================================================================================
来源：http://kzo.jianghu66.top

N. 数据结构与算法
来源：http://lis.aibaodan.cn

================================================================================
来源：http://ynt.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://ihs.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://edh.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jxn.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://feq.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://frm.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://eej.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://evn.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gsq.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://tmo.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://ulw.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://itv.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vrl.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://npu.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lat.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qkj.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://onw.tianlin.xyz


<!-- 参考信息 -->