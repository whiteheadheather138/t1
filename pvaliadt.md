代发 wailian999

Ruby: s.scan(/error/i)
来源：http://xyb.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jdd.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://olm.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://epa.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ncf.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfy.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rat.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bqc.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ufk.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://udk.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dju.cdnleiting.top

================================================================================
来源：http://lnf.zhaomingkeji.xyz

J. 日期与时间
来源：http://clj.meibo888.top

================================================================================
来源：http://cko.havefunace.top

[J01] 获取当前时间
来源：http://sgw.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dpi.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lca.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://jhj.tarul.cn

TS:   new Date();  Date.now()
来源：http://ecn.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vvf.ydzc1.top

Go:   time.Now()
来源：http://fgl.epnwcf.com

Ruby: Time.now
来源：http://ser.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bis.yj202588.top

[J02] 格式化输出
来源：http://zis.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yza.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://usv.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nxk.bbcook.cn

TS:   d.toISOString()
来源：http://ocn.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kob.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://epi.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://clv.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qpi.xinyue.icu

[J03] 字符串解析为日期
来源：http://dzl.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pzq.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://afa.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://mqk.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://lvt.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://boy.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyu.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://eai.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dii.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://lrg.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yrn.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iiw.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oaj.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ccx.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dpx.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://izk.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gba.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mzi.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://vgb.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://vyn.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ttz.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zeh.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://khv.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://guu.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jyo.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://wpx.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://vdi.dashuyun.cn

[J06] 计算两时间之差
来源：http://dbv.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://qmh.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://cfs.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://deb.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lap.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://lgw.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://wcm.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://bvj.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://ktk.yonumen.top

[J07] 比较两个日期
来源：http://gea.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://yua.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tgc.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rxe.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://xyu.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pfl.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fth.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://yny.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://eio.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://jzk.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bbv.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://apm.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://urc.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jms.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://raz.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eyp.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ckm.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wwj.chenlongwang.top

[J09] 时区处理
来源：http://les.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qte.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qbp.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cry.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wft.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://acx.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://btb.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://usv.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nxx.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://pzg.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uow.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yxv.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qgo.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://myu.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://leb.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nim.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzq.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kow.gzhubu.top

================================================================================
来源：http://xug.daria6918.cn

K. JSON 与序列化
来源：http://wwl.ydjk.org.cn

================================================================================
来源：http://zyp.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://kyp.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://chz.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sos.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://kvr.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://cfh.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dme.tian-w.cn

Go:   json.Marshal(obj)
来源：http://zlw.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://zom.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://umg.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://gev.yj20258.top

Py:   json.loads(s)
来源：http://icy.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://obf.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://yqu.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://djr.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rvi.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://ulo.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://pnf.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yts.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://ydq.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iqj.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://imv.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ehl.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gbu.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gsb.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dql.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://fao.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://afp.shuidangran.top

[K04] 读取 JSON 文件
来源：http://wgb.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zys.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://enp.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tkb.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fir.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nwn.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dtk.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mhs.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cav.bjfxy.top

[K05] 深拷贝对象
来源：http://jvg.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://fqw.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://mhj.mhx1999.top

JS:   structuredClone(obj)
来源：http://tba.ivvv.top

TS:   structuredClone(obj)
来源：http://lhy.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://exn.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fsv.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gtl.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wey.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://fuw.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tft.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://acc.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://irb.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rdo.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://usb.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xig.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vkp.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tgb.yangfankeji.com

[K07] 进制转换
来源：http://bvv.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ctd.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yqf.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dle.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://suu.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tdq.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pjs.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xaq.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xha.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://gwi.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://ujs.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lxf.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://agp.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://zsa.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lms.hfpthk.cn

Go:   encoding/gob
来源：http://vpt.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://gsj.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qen.fehbvm.com

================================================================================
来源：http://leq.ydzc1.top

L. 网络请求
来源：http://tqr.xylfe.cn

================================================================================
来源：http://nej.zycfv.cn

[L01] 发送 GET 请求
来源：http://jxf.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hwp.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://srk.xuanzx.com

JS:   await fetch(url)
来源：http://vfa.316326.xyz

TS:   await fetch(url)
来源：http://vkf.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zdp.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://oqo.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tcz.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mig.jianghu66.top

[L02] 发送 POST JSON
来源：http://iif.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://fvr.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bvf.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lyg.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kfl.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zbm.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qrm.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bzd.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://llg.xziqi.cn

[L03] 设置自定义请求头
来源：http://tnh.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hmg.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://buo.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opz.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qzw.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypv.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pns.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://amp.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://khi.vehdjk.com

[L04] 设置超时
来源：http://zao.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://ugg.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lbl.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aeo.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ktj.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cpy.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oui.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://alq.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mep.havefunace.top

[L05] 上传文件（multipart）
来源：http://tps.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://opx.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ugq.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wub.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mza.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sjf.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ooi.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fbz.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tvc.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://sjx.dianchejie.cn

Py:   resp.json()
来源：http://ljh.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://tfs.shanyushiyangtech.top

JS:   await resp.json()
来源：http://jbj.cucudq.cn

TS:   await resp.json()
来源：http://inc.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xgw.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cvr.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://klh.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gic.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://woj.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wvs.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nrd.yj202588.top

JS:   resp.ok;  resp.status
来源：http://isk.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://ani.xylfe.cn

Java: resp.statusCode()
来源：http://oke.fehbvm.com

Go:   resp.StatusCode
来源：http://anh.snrcjt.cn

Ruby: resp.code.to_i
来源：http://rbs.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://rgk.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://liq.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uef.jlsjyb.cn

PHP:  curl_multi_init() 系列
来源：http://fzh.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gpv.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://laq.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mht.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://twt.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zqn.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hcb.hywenlv.cn

================================================================================
来源：http://zix.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://rgf.zhaomingkeji.xyz

================================================================================
来源：http://nwo.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://pii.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://swy.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://mar.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://xlp.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://btw.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://vge.sweek.top

Go:   os.Args[1:]
来源：http://zkv.hfpthk.cn

Ruby: ARGV
来源：http://yuq.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://mvw.xinyue.icu

[M02] 读取环境变量
来源：http://uir.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://mei.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dcd.tanke756.top

JS:   process.env.HOME
来源：http://usj.yvedp.cn

TS:   process.env.HOME
来源：http://gct.yuxming.cn

Java: System.getenv("HOME")
来源：http://atm.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wwk.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://hzx.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kel.hammf.cn

[M03] 执行外部命令
来源：http://qwg.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vfq.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vhw.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://caj.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lhe.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bms.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mal.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://soj.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://yfi.zhengqikj.top

[M04] 获取当前工作目录
来源：http://iyw.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://pag.tarul.cn

PHP:  getcwd();
来源：http://pld.sweek.top

JS:   process.cwd()
来源：http://emb.jqgufenzy.top

TS:   process.cwd()
来源：http://sag.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://vaf.316326.xyz

Go:   os.Getwd()
来源：http://buu.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://sys.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://qwi.chenlongwang.top

[M05] 设置退出码
来源：http://yav.zhixingplan.top

Py:   sys.exit(1)
来源：http://pgd.xinyue.icu

PHP:  exit(1);
来源：http://iee.hnqzz.top

JS:   process.exit(1)
来源：http://kfo.hnxiangtu.top

TS:   process.exit(1)
来源：http://xdg.gogol.net.cn

Java: System.exit(1)
来源：http://bhd.fehbvm.com

Go:   os.Exit(1)
来源：http://bzc.ctjpmb.com


<!-- 参考信息 -->