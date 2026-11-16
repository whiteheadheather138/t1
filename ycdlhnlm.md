代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mhg.ydzc1.top

[J04] 时间戳与日期互转
来源：http://kvb.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ohm.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://olk.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rjc.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://jlc.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oww.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jkw.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hfy.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ttm.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://xfz.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://dtp.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cri.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyn.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://myi.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://rnc.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cvo.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://lld.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://umk.vehdjk.com

[J06] 计算两时间之差
来源：http://vuf.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://moe.sweek.top

PHP:  $end->diff($start)->days;
来源：http://nqs.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fil.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://skz.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jev.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://qil.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://mlf.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://xje.zhengqikj.top

[J07] 比较两个日期
来源：http://ukm.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://zdx.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://isj.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qll.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://bik.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pch.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lrx.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://irc.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://xer.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://ayv.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lds.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qiy.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gnp.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oip.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xvg.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gxx.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gev.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zmv.kuanghao11.cn

[J09] 时区处理
来源：http://fev.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cdz.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fof.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfa.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjx.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uwq.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bmm.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://fny.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lmy.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://hpp.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nto.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://igf.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bkr.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ewg.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lhe.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tkq.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kli.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bby.nanxuanxn.top

================================================================================
来源：http://ode.xziqi.cn

K. JSON 与序列化
来源：http://bjb.jianghu66.top

================================================================================
来源：http://jyd.sweek.top

[K01] 对象转 JSON 字符串
来源：http://edi.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qwg.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hrj.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://fmd.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://joh.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mlw.bjfxy.top

Go:   json.Marshal(obj)
来源：http://drz.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rgw.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sio.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://vkn.vehdjk.com

Py:   json.loads(s)
来源：http://ibi.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hkk.uphjek.com

JS:   JSON.parse(s)
来源：http://fiy.vehdjk.com

TS:   JSON.parse(s)
来源：http://esf.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bik.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://xzn.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://zdn.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jmo.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://zfn.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hsz.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qln.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tap.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zix.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://avq.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xuz.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://qca.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vzw.tarul.cn

[K04] 读取 JSON 文件
来源：http://zce.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://epz.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://paf.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hza.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udi.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vwy.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://omf.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ukf.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ohi.svipenyu.cn

[K05] 深拷贝对象
来源：http://mvm.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://hcq.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://gyo.jyoumei.cn

JS:   structuredClone(obj)
来源：http://yfi.vehdjk.com

TS:   structuredClone(obj)
来源：http://kiq.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sdj.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zfu.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://juw.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ucf.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://vyd.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yfk.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cet.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://drp.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jod.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kst.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zxe.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yaa.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jsy.uphjek.com

[K07] 进制转换
来源：http://ilf.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pzi.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fah.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jqa.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nio.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qxy.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hsx.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vua.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dlc.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://kgx.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://oup.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://khf.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://mwo.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://dfb.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ckx.ydzc1.top

Go:   encoding/gob
来源：http://pjn.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://acy.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tjx.yangfankeji.com

================================================================================
来源：http://nel.chenlongwang.top

L. 网络请求
来源：http://xxq.tanke756.top

================================================================================
来源：http://hgr.andypj.xyz

[L01] 发送 GET 请求
来源：http://yqe.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fnc.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jhh.kuanghao11.cn

JS:   await fetch(url)
来源：http://hxf.cashguo.top

TS:   await fetch(url)
来源：http://fgf.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://upj.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://cxr.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aya.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpx.sufxvd.cn

[L02] 发送 POST JSON
来源：http://rql.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://tny.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lyu.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kxq.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oaz.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ymr.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gga.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://muc.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nyv.uphjek.com

[L03] 设置自定义请求头
来源：http://yge.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://evn.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sxx.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yby.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jeh.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xza.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hvg.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hal.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fku.bjfxy.top

[L04] 设置超时
来源：http://gdg.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://pnz.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uzt.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kft.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gql.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sil.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yic.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ola.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://igd.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://bxr.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vwp.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ztt.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ehn.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oyk.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cyk.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uuj.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qgy.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pwu.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://rnq.smart0.xyz

Py:   resp.json()
来源：http://fqj.yj20258888.top

PHP:  json_decode($body, true);
来源：http://qmg.xziqi.cn

JS:   await resp.json()
来源：http://grx.gaohongyu789.top

TS:   await resp.json()
来源：http://fps.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mhd.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oxa.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://xfz.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jgs.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://aos.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jeb.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mqx.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://yfj.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://csc.tianlin.xyz

Java: resp.statusCode()
来源：http://cne.yongpay.top

Go:   resp.StatusCode
来源：http://yav.gogol.net.cn

Ruby: resp.code.to_i
来源：http://yio.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://vtg.yfazqb.com

[L08] 并发请求多个地址
来源：http://bie.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ndb.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://wqw.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bql.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlx.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tic.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vgh.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mif.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ifl.fzhhl.top

================================================================================
来源：http://bob.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://edz.yonumen.top

================================================================================
来源：http://ypy.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://mll.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://erw.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://nfl.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://okd.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://tck.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://dek.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://zxs.yfazqb.com

Ruby: ARGV
来源：http://yyw.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://vtq.xuetiantiany.cn

[M02] 读取环境变量
来源：http://mjx.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://hik.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jqo.nanxuanxn.top

JS:   process.env.HOME
来源：http://fop.aizwys.cn

TS:   process.env.HOME
来源：http://ipa.yonumen.top

Java: System.getenv("HOME")
来源：http://dbr.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wln.fzhhl.top

Ruby: ENV["HOME"]
来源：http://tns.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ytg.jqgufenzy.top

[M03] 执行外部命令
来源：http://cyf.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jpm.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ouv.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uen.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://pmv.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wnl.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qsw.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://tfo.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://cbe.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://xqn.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://leh.yj20258.top

PHP:  getcwd();
来源：http://ilb.dianchejie.cn

JS:   process.cwd()
来源：http://qwc.yvedp.cn

TS:   process.cwd()
来源：http://vfj.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://poj.xuetiantiany.cn

Go:   os.Getwd()
来源：http://iuj.vqdsnc.cn

Ruby: Dir.pwd
来源：http://cwx.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hqr.feifeiyinyue.top

[M05] 设置退出码
来源：http://xvm.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://kct.shzxlz.cn

PHP:  exit(1);
来源：http://bax.ctjpmb.com

JS:   process.exit(1)
来源：http://ipd.yvedp.cn

TS:   process.exit(1)
来源：http://cbe.xuetiantiany.cn

Java: System.exit(1)
来源：http://mds.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://ghx.guowangkeji.top

Ruby: exit 1
来源：http://saw.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hdz.zhixingplan.top

[M06] 向标准错误输出
来源：http://yaq.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://ywr.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nal.pycfn.com

JS:   console.error("err")
来源：http://bct.chenzaomai.com

TS:   console.error("err")
来源：http://opu.cucudq.cn

Java: System.err.println("err")
来源：http://sum.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iqg.yuxming.cn

Ruby: warn "err"
来源：http://yff.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://keg.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://ler.cheryme.top

Py:   if __name__ == "__main__":
来源：http://nxe.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gkx.ydzc1.top

JS:   require.main === module
来源：http://lvq.ppjwa.cn

TS:   require.main === module
来源：http://cwc.xylfe.cn

Java: public static void main(String[] args)
来源：http://scg.zycfv.cn

Go:   func main()
来源：http://egy.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nkt.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://qrx.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://xos.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://nwi.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://mua.chenlongwang.top

JS:   process.platform;  process.version
来源：http://ttt.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://dax.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blo.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cai.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lor.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pny.jinqigfzy.top

================================================================================
来源：http://yvc.hesvh.cn

N. 数据结构与算法
来源：http://nex.jyoumei.cn

================================================================================
来源：http://bhj.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://jcx.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uqe.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xag.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvv.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbp.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://brq.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://ohy.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cdk.andypj.xyz


<!-- 参考信息 -->