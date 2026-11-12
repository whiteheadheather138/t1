代发 wailian999

[J03] 字符串解析为日期
来源：http://oon.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lnu.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlt.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://bwg.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://qev.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://aso.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://azd.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://drd.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://okd.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://ftf.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://huz.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sws.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mrj.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xhj.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kdq.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oep.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://btt.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cpe.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://ilu.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://zoo.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://pzl.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jhl.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lwy.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://jvw.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://frn.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://awp.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://chr.birdmap.top

[J06] 计算两时间之差
来源：http://hro.yj20258.top

Py:   (end - start).total_seconds()
来源：http://qzz.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://fqg.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tru.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ujs.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://dfn.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://qsl.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://vzg.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://eel.aizwys.cn

[J07] 比较两个日期
来源：http://kdg.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://hgw.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://taw.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lkp.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lfo.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ltx.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dkf.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://uov.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://vrm.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://mtl.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vzr.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gay.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ncn.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ksz.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uqf.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nnm.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://agd.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://anu.hongshengwenyu.top

[J09] 时区处理
来源：http://ilm.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jef.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jsq.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sum.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://byu.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cib.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jab.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://nfx.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://htk.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://rgr.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ncz.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bjg.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lwb.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xvr.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wyp.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://emd.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uuo.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ies.shanyushiyangtech.top

================================================================================
来源：http://vqk.hfpthk.cn

K. JSON 与序列化
来源：http://vwi.yuanzhike.top

================================================================================
来源：http://xmx.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://yoc.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://myk.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://emd.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://bnc.yongpay.top

TS:   JSON.stringify(obj)
来源：http://xii.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oib.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://wth.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kmk.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zrp.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://hbk.wangshuangyany.cn

Py:   json.loads(s)
来源：http://wux.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xpu.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://adl.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://mha.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vwe.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://yag.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://fex.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rhi.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://hkl.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uhf.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ate.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nbv.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nvy.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hwv.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pep.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://pvj.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nfc.yvedp.cn

[K04] 读取 JSON 文件
来源：http://vct.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yku.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oyn.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://shn.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dfr.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nax.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gkw.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ohm.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tgf.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://tze.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://nfi.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://awx.52xcode.cn

JS:   structuredClone(obj)
来源：http://bgm.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://fcc.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bou.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iuh.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ume.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mwm.pycfn.com

[K06] 解析 URL 查询串
来源：http://swg.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://brd.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://evc.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mow.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzg.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vhr.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jrk.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hed.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mtt.hnqzz.top

[K07] 进制转换
来源：http://kkl.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xwk.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dtm.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zhj.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bad.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ihn.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lav.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nwx.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://chw.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://opb.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://qhr.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kjt.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://dga.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://uwy.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rpv.dianchejie.cn

Go:   encoding/gob
来源：http://aev.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://jol.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ewv.pycfn.com

================================================================================
来源：http://xtq.vqdsnc.cn

L. 网络请求
来源：http://typ.snrcjt.cn

================================================================================
来源：http://iyy.yonumen.top

[L01] 发送 GET 请求
来源：http://vqn.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://auh.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fhw.fzhhl.top

JS:   await fetch(url)
来源：http://egz.hcnkem.com

TS:   await fetch(url)
来源：http://akf.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xxv.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://shs.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://okg.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bpb.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://gdh.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cya.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ile.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cms.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivd.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nzw.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://efi.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://afu.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wff.snrcjt.cn

[L03] 设置自定义请求头
来源：http://iny.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://anf.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uvl.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kph.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rzn.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hbt.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kvp.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qvl.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rhr.ppjwa.cn

[L04] 设置超时
来源：http://dxy.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://uwk.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zee.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vrb.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dev.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fqw.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gvd.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xyd.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bax.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://bpl.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pho.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://orq.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tch.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ptz.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vtk.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bkv.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gei.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://okz.guannengcc.top

[L06] 解析响应为 JSON
来源：http://igv.yuanzhike.top

Py:   resp.json()
来源：http://iqn.daxiang520.top

PHP:  json_decode($body, true);
来源：http://bay.jqgufenzy.top

JS:   await resp.json()
来源：http://yuc.yj202588.top

TS:   await resp.json()
来源：http://fzw.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dvj.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lni.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://luv.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wih.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://cis.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cng.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qdf.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://ymy.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://vpe.tian-w.cn

Java: resp.statusCode()
来源：http://whb.dianchejie.cn

Go:   resp.StatusCode
来源：http://yyd.c1oappe.top

Ruby: resp.code.to_i
来源：http://glv.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://eco.ybcxt.top

[L08] 并发请求多个地址
来源：http://ezv.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wcv.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://wvb.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wly.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ost.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ngw.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rfy.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sea.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xou.fzhhl.top

================================================================================
来源：http://maz.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://cey.0kj1m.cn

================================================================================
来源：http://ulm.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://ebm.hammf.cn

Py:   sys.argv[1:]
来源：http://ryh.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://ost.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://dkm.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://jyk.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://uce.shuidangran.top

Go:   os.Args[1:]
来源：http://xss.yuxming.cn

Ruby: ARGV
来源：http://qmd.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://xaq.smart0.xyz

[M02] 读取环境变量
来源：http://vcq.tanke756.top

Py:   os.environ.get("HOME")
来源：http://gua.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fbs.havefunace.top

JS:   process.env.HOME
来源：http://bpw.jyoumei.cn

TS:   process.env.HOME
来源：http://fci.epnwcf.com

Java: System.getenv("HOME")
来源：http://ubw.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nre.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://jeu.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gua.zhiwuduotai.top

[M03] 执行外部命令
来源：http://rpn.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cun.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kvj.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zqt.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dbh.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zfu.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kjy.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://aqr.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://her.shzxlz.cn

[M04] 获取当前工作目录
来源：http://ugm.gogol.net.cn

Py:   os.getcwd()
来源：http://tdt.mhx1999.top

PHP:  getcwd();
来源：http://arb.redwolf501.top

JS:   process.cwd()
来源：http://cap.svipenyu.cn

TS:   process.cwd()
来源：http://eoo.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://uom.jinqigfzy.top

Go:   os.Getwd()
来源：http://vzt.c1oappe.top

Ruby: Dir.pwd
来源：http://dkp.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://ubn.guannengcc.top

[M05] 设置退出码
来源：http://sca.zhixingplan.top

Py:   sys.exit(1)
来源：http://oay.uphjek.com

PHP:  exit(1);
来源：http://nvj.yfazqb.com

JS:   process.exit(1)
来源：http://asg.shuidangran.top

TS:   process.exit(1)
来源：http://vcd.nanxinkj.top

Java: System.exit(1)
来源：http://jej.gaohongyu789.top

Go:   os.Exit(1)
来源：http://tnd.zdbjq.cn

Ruby: exit 1
来源：http://pbn.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gso.hcnkem.com

[M06] 向标准错误输出
来源：http://eax.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://psh.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aec.jinqigufen.top

JS:   console.error("err")
来源：http://vuu.0kj1m.cn

TS:   console.error("err")
来源：http://auh.ybcxt.top

Java: System.err.println("err")
来源：http://ryd.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tuv.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://niw.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://ncs.tian-w.cn

[M07] 判断是否为主入口
来源：http://xqw.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://wdl.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://suf.havefunace.top

JS:   require.main === module
来源：http://vtu.shuidangran.top

TS:   require.main === module
来源：http://puk.ivvv.top

Java: public static void main(String[] args)
来源：http://lnl.gzhubu.top

Go:   func main()
来源：http://ydh.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ijy.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://psq.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://abt.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://cnw.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://lsl.fehbvm.com

JS:   process.platform;  process.version
来源：http://sla.redwolf501.top

TS:   process.platform;  process.version
来源：http://cbu.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aqh.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://odc.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ytg.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lhk.fktsv.cn

================================================================================
来源：http://cls.shangyingyoupin.top

N. 数据结构与算法
来源：http://tnf.fktsv.cn

================================================================================
来源：http://lrj.vqdsnc.cn


<!-- 参考信息 -->