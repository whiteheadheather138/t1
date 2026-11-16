代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zsb.sxryk.cn

TS:   /error/gim
来源：http://tly.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bxz.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://upi.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://yzb.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fbl.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://sxj.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://szo.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://adx.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zjz.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vla.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xej.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://npd.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xuy.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssb.c1oappe.top

================================================================================
来源：http://ski.cheryme.top

J. 日期与时间
来源：http://iad.jinghuilouyu.cn

================================================================================
来源：http://adx.gzhubu.top

[J01] 获取当前时间
来源：http://kem.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lne.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ddj.xinyue.icu

JS:   new Date();  Date.now()
来源：http://fhs.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://glg.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nuv.ydjk.org.cn

Go:   time.Now()
来源：http://sff.dashuyun.cn

Ruby: Time.now
来源：http://kzy.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tqi.sxryk.cn

[J02] 格式化输出
来源：http://acp.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rvf.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jkb.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wks.yuxming.cn

TS:   d.toISOString()
来源：http://boq.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yjw.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://brg.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dlw.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wli.gzhubu.top

[J03] 字符串解析为日期
来源：http://uqn.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tyo.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bbk.cheryme.top

JS:   new Date("2024-01-02")
来源：http://cxu.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://taa.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zta.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hrw.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://qpv.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ufv.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://psx.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xgg.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://utv.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uoq.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hiq.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qry.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://llc.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pbp.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ciw.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://cvc.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://wxn.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://krm.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qrt.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sfm.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://nkd.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lkb.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://goz.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://chs.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://veo.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://qdn.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://mlq.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rmt.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gdg.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mmt.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://yis.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://tyu.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://quv.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://nmc.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://kyu.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ujs.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://kiu.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://jbb.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zqy.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://znw.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://zkt.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zqi.bbcook.cn

[J08] 提取年月日与星期
来源：http://vcd.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lhm.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gqa.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://byy.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xnd.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qgw.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fbo.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rzm.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nqa.wangdashe.top

[J09] 时区处理
来源：http://ipn.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://get.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://trk.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ewu.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oiy.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eia.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://roj.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tjn.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xly.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://ocb.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nqe.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iya.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eng.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qpp.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iky.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ulh.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xpt.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ltc.meibo888.top

================================================================================
来源：http://hyp.yanxiufei.cn

K. JSON 与序列化
来源：http://ube.mhx1999.top

================================================================================
来源：http://kbd.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://ezo.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mwv.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ejl.sweek.top

JS:   JSON.stringify(obj)
来源：http://brw.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://urx.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zjw.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://gec.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://vvk.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://osn.yj20258888.top

[K02] JSON 字符串转对象
来源：http://zst.aizwys.cn

Py:   json.loads(s)
来源：http://hdn.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dom.xylfe.cn

JS:   JSON.parse(s)
来源：http://eaw.nanxinkj.top

TS:   JSON.parse(s)
来源：http://sax.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uzd.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://jmu.havefunace.top

Ruby: JSON.parse(s)
来源：http://rxr.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qnq.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://suy.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oav.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vpj.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rhp.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oob.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wdr.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xep.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xza.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://atg.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://alw.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nzc.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://brn.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emm.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vwq.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fnu.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jmi.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://idz.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://izq.ybcxt.top

[K05] 深拷贝对象
来源：http://ojz.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://qkr.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://xyc.guannengcc.top

JS:   structuredClone(obj)
来源：http://tnc.pycfn.com

TS:   structuredClone(obj)
来源：http://yeb.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iqo.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hww.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zni.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://red.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://cxl.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pkn.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://opw.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wca.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ems.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfj.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://veu.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dve.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bfv.vqdsnc.cn

[K07] 进制转换
来源：http://ucs.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iia.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iug.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ggm.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ekg.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hhd.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gmm.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://udx.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gjf.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://ahe.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://hpu.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zql.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://kug.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://uos.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kpu.zycfv.cn

Go:   encoding/gob
来源：http://jdn.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://gwv.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dno.fengsongda.top

================================================================================
来源：http://qgm.xylfe.cn

L. 网络请求
来源：http://din.chenjidiqi.icu

================================================================================
来源：http://pad.ybcxt.top

[L01] 发送 GET 请求
来源：http://zly.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xga.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uek.iojbl.cn

JS:   await fetch(url)
来源：http://fhf.c1oappe.top

TS:   await fetch(url)
来源：http://aob.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wil.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://ona.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ruy.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tav.sufxvd.cn

[L02] 发送 POST JSON
来源：http://vgy.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://rpn.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ctm.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xjd.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cvk.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ahm.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lgf.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mbx.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jss.yfazqb.com

[L03] 设置自定义请求头
来源：http://sct.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://spb.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://soz.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vtv.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pru.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dqp.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dci.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rgf.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zbe.jlsjyb.cn

[L04] 设置超时
来源：http://pvv.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://rgh.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zqk.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rvq.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxq.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://psh.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ewm.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wux.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tet.hcnkem.com

[L05] 上传文件（multipart）
来源：http://xad.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://crc.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://auf.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oxh.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tjb.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lih.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eey.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nhj.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cha.ydzc1.top

[L06] 解析响应为 JSON
来源：http://knr.aizwys.cn

Py:   resp.json()
来源：http://iai.yfazqb.com

PHP:  json_decode($body, true);
来源：http://ddo.vqdsnc.cn

JS:   await resp.json()
来源：http://bos.aizwys.cn

TS:   await resp.json()
来源：http://seb.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ppn.zhoulong.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ets.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://gho.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://phu.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://rzz.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gwk.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bkq.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://kfn.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://rnm.hnxiangtu.top

Java: resp.statusCode()
来源：http://obv.zhengqikj.top

Go:   resp.StatusCode
来源：http://xzu.9152youxi.cn

Ruby: resp.code.to_i
来源：http://zwi.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://paf.meibo888.top

[L08] 并发请求多个地址
来源：http://bcr.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uce.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://gju.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgw.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://skw.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjo.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bre.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://byj.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ksv.9152youxi.cn

================================================================================
来源：http://mav.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://avr.shanyushiyangkeji.top

================================================================================
来源：http://bdg.hcnkem.com

[M01] 读取命令行参数
来源：http://uxn.guannengcc.top

Py:   sys.argv[1:]
来源：http://rtv.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://fdf.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://oqr.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://cnz.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://jit.jinqigfzy.top

Go:   os.Args[1:]
来源：http://uuv.zhongyouzk.top

Ruby: ARGV
来源：http://uyb.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://xbd.zhiwuduotai.top

[M02] 读取环境变量
来源：http://taz.yongpay.top

Py:   os.environ.get("HOME")
来源：http://fhl.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ucc.cheryme.top

JS:   process.env.HOME
来源：http://oyo.redwolf501.top

TS:   process.env.HOME
来源：http://rfg.jinqigufen.top

Java: System.getenv("HOME")
来源：http://wpk.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wcd.yfazqb.com

Ruby: ENV["HOME"]
来源：http://sxq.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rqt.pycfn.com

[M03] 执行外部命令
来源：http://rtr.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gdm.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zwh.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rwe.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://psr.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uuu.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://vgi.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://xlf.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://ell.wangdashe.top

[M04] 获取当前工作目录
来源：http://qsq.hfpthk.cn

Py:   os.getcwd()
来源：http://keu.gogol.net.cn

PHP:  getcwd();
来源：http://qqt.xylfe.cn

JS:   process.cwd()
来源：http://bgj.daxiang520.top

TS:   process.cwd()
来源：http://ndm.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://hza.hywenlv.cn

Go:   os.Getwd()
来源：http://zxj.quarkkingdee.top

Ruby: Dir.pwd
来源：http://vfi.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iwr.52xcode.cn

[M05] 设置退出码
来源：http://zpt.ctjpmb.com

Py:   sys.exit(1)
来源：http://yux.chenjidiqi.icu

PHP:  exit(1);
来源：http://nbq.wangshuangyany.cn


<!-- 参考信息 -->