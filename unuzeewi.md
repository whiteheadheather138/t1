代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bqh.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://spc.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tzk.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://twu.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://idh.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://eah.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://twh.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nak.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mqz.shanyushiyangkeji.top

TS:   /error/gim
来源：http://vgp.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jix.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://elj.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://cxx.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wvb.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://mob.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fao.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lbp.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tss.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dtb.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oxz.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://esi.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gax.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vac.fanxiaobao.xyz

================================================================================
来源：http://xjc.havefunace.top

J. 日期与时间
来源：http://znd.jyoumei.cn

================================================================================
来源：http://qzu.ctjpmb.com

[J01] 获取当前时间
来源：http://zxr.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ttb.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ytu.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://rny.xziqi.cn

TS:   new Date();  Date.now()
来源：http://tux.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://iyv.uphjek.com

Go:   time.Now()
来源：http://oow.wangdashe.top

Ruby: Time.now
来源：http://mxo.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gvw.0kj1m.cn

[J02] 格式化输出
来源：http://cmj.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://enn.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wto.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yun.nanxinkj.top

TS:   d.toISOString()
来源：http://mwv.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ptd.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ugb.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxq.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://idi.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://rhx.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mrb.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tft.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://ogw.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://vlf.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://nnr.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xbc.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://ffw.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fnp.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://pan.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gzd.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://req.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bth.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vwk.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fho.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dlc.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bgm.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hes.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://yra.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://mka.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hsr.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tcs.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sxb.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://mnp.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://loc.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://ldh.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://mqv.chenlongwang.top

[J06] 计算两时间之差
来源：http://qwu.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://fpj.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://pik.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aku.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qwv.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kaj.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://ldq.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://itu.sweek.top

C#:   (end - start).TotalSeconds
来源：http://cpl.quarkkingdee.top

[J07] 比较两个日期
来源：http://msd.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://zgt.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://brb.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://qck.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://leu.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qfm.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gvy.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://kqh.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://jxu.fzhhl.top

[J08] 提取年月日与星期
来源：http://fmi.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hiz.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://izt.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dxn.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bgp.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uoz.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pum.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://twr.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://guq.bbcook.cn

[J09] 时区处理
来源：http://hbq.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://chb.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agb.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rzt.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ewn.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gbt.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iwr.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://goz.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xzg.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://xlb.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wre.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jrf.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://glt.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jek.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://srj.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://muf.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://frx.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jle.tarul.cn

================================================================================
来源：http://mgl.zdqjudy.top

K. JSON 与序列化
来源：http://sya.pycfn.com

================================================================================
来源：http://vvz.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://raa.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://czs.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bbp.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://mch.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://wdn.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jqw.fktsv.cn

Go:   json.Marshal(obj)
来源：http://ohk.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://tuq.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wgr.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://llb.sysykeji.top

Py:   json.loads(s)
来源：http://xqf.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://psv.shzxlz.cn

JS:   JSON.parse(s)
来源：http://pub.ivvv.top

TS:   JSON.parse(s)
来源：http://ldp.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://frg.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://qul.ivvv.top

Ruby: JSON.parse(s)
来源：http://lbn.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cez.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://kjz.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wyf.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jff.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wov.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zgb.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wmi.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://teh.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://eeg.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://amc.sysykeji.top

[K04] 读取 JSON 文件
来源：http://yxh.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jvx.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://utp.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osk.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://agi.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xpt.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://axd.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://osd.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sns.cheryme.top

[K05] 深拷贝对象
来源：http://sqn.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://bhi.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://jkq.sweek.top

JS:   structuredClone(obj)
来源：http://zum.mhx1999.top

TS:   structuredClone(obj)
来源：http://wtj.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fqz.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://alu.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cht.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uje.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://rnt.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nbh.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ivj.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpj.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xup.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hdp.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wbm.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://spj.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ass.yongpay.top

[K07] 进制转换
来源：http://mjt.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ird.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zxl.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tyy.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jxl.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tjs.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://elm.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qei.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://woh.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://uii.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://ddc.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://axd.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://ynw.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://rgl.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://miy.yonumen.top

Go:   encoding/gob
来源：http://vbz.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://jbn.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qwe.zhongyouzk.top

================================================================================
来源：http://mqn.tarul.cn

L. 网络请求
来源：http://ukg.fzhhl.top

================================================================================
来源：http://wte.tanke756.top

[L01] 发送 GET 请求
来源：http://gpy.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rvl.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jrl.ehwqpu.com

JS:   await fetch(url)
来源：http://avo.zhijiandao.cn

TS:   await fetch(url)
来源：http://mqd.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mmk.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://yzz.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bng.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lnb.9152youxi.cn

[L02] 发送 POST JSON
来源：http://wlv.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://pyt.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://azl.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://icu.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tct.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://obk.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sau.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://duv.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xtn.yvedp.cn

[L03] 设置自定义请求头
来源：http://hui.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qzb.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hfx.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jke.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://loe.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://amb.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://asa.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oen.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hme.zhoulong.xyz

[L04] 设置超时
来源：http://llz.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://xgj.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oqc.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hux.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://epq.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gng.zhengqikj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qtu.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gez.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gpa.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://fjz.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rhz.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lez.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pbx.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://psw.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hqs.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zty.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wom.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xkn.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://jgb.zhaomingkeji.xyz

Py:   resp.json()
来源：http://rey.xziqi.cn

PHP:  json_decode($body, true);
来源：http://eze.bbcook.cn

JS:   await resp.json()
来源：http://wrh.jqgfzy.top

TS:   await resp.json()
来源：http://frh.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yay.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lup.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://wwm.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://afs.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://ecu.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://esw.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hra.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://jdu.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://jvk.zhiwuduotai.top

Java: resp.statusCode()
来源：http://kxc.sweek.top

Go:   resp.StatusCode
来源：http://mnh.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://itm.yongpay.top

C#:   (int)resp.StatusCode
来源：http://hqk.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://igd.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eba.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://aab.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sia.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tlc.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cgb.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cbe.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eum.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bow.zdqjudy.top

================================================================================
来源：http://ree.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://hkn.jinqigufen.top

================================================================================
来源：http://dtb.kuanghao11.cn

[M01] 读取命令行参数
来源：http://hrk.zdqjudy.top

Py:   sys.argv[1:]
来源：http://xhb.guannengcc.top

PHP:  $argv;  $argc;
来源：http://nwm.yfazqb.com

JS:   process.argv.slice(2)
来源：http://yun.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://eeo.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://mjk.nanxinkj.top

Go:   os.Args[1:]
来源：http://qon.yangfankeji.com

Ruby: ARGV
来源：http://lih.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://deb.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://yja.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://xfz.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wnh.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://lcp.yuanzhike.top

TS:   process.env.HOME
来源：http://ddm.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://dcd.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vmn.pycfn.com

Ruby: ENV["HOME"]
来源：http://whn.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://whx.sxryk.cn

[M03] 执行外部命令
来源：http://orn.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://scq.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://noc.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dze.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://igx.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sak.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uzo.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://zzn.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://quc.snrcjt.cn

[M04] 获取当前工作目录
来源：http://hwj.gotoacloud.top

Py:   os.getcwd()
来源：http://txx.iojbl.cn

PHP:  getcwd();
来源：http://upa.kuanghao11.cn

JS:   process.cwd()
来源：http://ceg.mhx1999.top


<!-- 参考信息 -->