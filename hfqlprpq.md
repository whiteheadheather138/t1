代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ydm.yuanzhike.top

TS:   /error/gim
来源：http://kfw.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gnk.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hbu.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://dkb.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cfs.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://ped.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fjr.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://adz.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mva.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eue.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qlc.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tmz.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyd.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://byg.zhijiandao.cn

================================================================================
来源：http://iuw.hnqzz.top

J. 日期与时间
来源：http://jvs.zdbjq.cn

================================================================================
来源：http://wgd.fktsv.cn

[J01] 获取当前时间
来源：http://ovm.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://dcz.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pum.yj20258.top

JS:   new Date();  Date.now()
来源：http://obv.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://kkg.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bwf.gotoacloud.top

Go:   time.Now()
来源：http://ttf.quarkkingdee.top

Ruby: Time.now
来源：http://ntr.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lbe.uphjek.com

[J02] 格式化输出
来源：http://fky.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://for.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ghu.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://skr.cheryme.top

TS:   d.toISOString()
来源：http://cxb.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kat.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tzr.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tso.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jif.jiagoushi.top

[J03] 字符串解析为日期
来源：http://vnq.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aag.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mxz.hammf.cn

JS:   new Date("2024-01-02")
来源：http://eos.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://gfr.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ykt.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ebp.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://nvl.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qlh.hammf.cn

[J04] 时间戳与日期互转
来源：http://syc.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://klw.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kok.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://alv.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oyl.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sgq.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mpo.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ovo.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dic.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://ffe.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://oax.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ncm.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://odl.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqi.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://qey.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://spo.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://hff.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://gtt.yueranfly.top

[J06] 计算两时间之差
来源：http://ggt.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://ten.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://cwl.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vkn.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gdv.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://xfx.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://cgg.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://yua.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://uzf.nwbrower.top

[J07] 比较两个日期
来源：http://dek.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://nbc.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hbn.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ius.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://wfy.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izq.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ynq.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://vgn.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://dsz.tian-w.cn

[J08] 提取年月日与星期
来源：http://imk.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dvb.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qaj.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://doa.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rhy.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ans.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pzg.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fzd.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nvx.gotoacloud.top

[J09] 时区处理
来源：http://znz.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://haz.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://poc.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pyw.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://shj.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hvc.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rql.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://act.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oma.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://ycu.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://qqb.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://get.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vct.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://prz.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vpk.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kkh.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xdd.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uep.zhaomingkeji.xyz

================================================================================
来源：http://cwb.zhengqikj.top

K. JSON 与序列化
来源：http://rjg.yfazqb.com

================================================================================
来源：http://uwh.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://scl.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zby.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fsb.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://ldr.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://ckx.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oae.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://xxa.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://frs.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jwm.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://lai.feifeiyinyue.top

Py:   json.loads(s)
来源：http://ghb.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vkh.cucudq.cn

JS:   JSON.parse(s)
来源：http://lzm.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://gco.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jbr.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://rzj.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://mfu.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rjz.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://yot.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ffp.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pcj.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://als.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wjt.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lff.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zsl.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dij.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qki.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://nns.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qyl.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qka.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhl.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ywm.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ejs.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uop.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://blw.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://opq.aibaodan.cn

[K05] 深拷贝对象
来源：http://jrd.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://sgn.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://xgv.yj20258888.top

JS:   structuredClone(obj)
来源：http://rmt.xinyue.icu

TS:   structuredClone(obj)
来源：http://qek.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tfo.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ddm.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dpj.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gto.yvedp.cn

[K06] 解析 URL 查询串
来源：http://fdv.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hqi.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://frv.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oml.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://djt.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://who.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ejj.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ria.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://udo.hywenlv.cn

[K07] 进制转换
来源：http://ueb.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bus.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vnk.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ccf.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://efd.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nun.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tow.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lko.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uzk.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://nfl.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://lgi.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hwk.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://zxn.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://xbl.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tlf.316326.xyz

Go:   encoding/gob
来源：http://gcr.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://iug.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ide.yj20258.top

================================================================================
来源：http://utm.vqdsnc.cn

L. 网络请求
来源：http://tne.hnxiangtu.top

================================================================================
来源：http://byj.cucudq.cn

[L01] 发送 GET 请求
来源：http://vvx.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uhh.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eia.sysykeji.top

JS:   await fetch(url)
来源：http://lfv.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://cvv.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://irl.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://gzb.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://adx.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gtg.fzhhl.top

[L02] 发送 POST JSON
来源：http://grw.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bmy.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gon.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnq.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lkn.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cse.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pmx.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://orh.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://olg.nwbrower.top

[L03] 设置自定义请求头
来源：http://std.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cef.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nve.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ekd.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gir.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://umt.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kpo.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lxy.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bah.9152youxi.cn

[L04] 设置超时
来源：http://htc.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://zoa.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://anh.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qlc.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://big.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vhh.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yzr.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://agu.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qpm.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://lhr.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://egf.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bhe.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://chz.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ewe.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ope.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kze.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://axd.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ycc.sweek.top

[L06] 解析响应为 JSON
来源：http://zoq.dianchejie.cn

Py:   resp.json()
来源：http://joy.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://bhz.ctjpmb.com

JS:   await resp.json()
来源：http://tbw.zhongyouzk.top

TS:   await resp.json()
来源：http://fdd.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bsw.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://noo.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://eba.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jfy.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://gnm.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hzv.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uga.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://zxj.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://myh.uphjek.com

Java: resp.statusCode()
来源：http://kyl.uphjek.com

Go:   resp.StatusCode
来源：http://fwb.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://rdb.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://rmx.0kj1m.cn

[L08] 并发请求多个地址
来源：http://esh.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rhg.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://rhh.daria6918.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cdc.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://efx.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vns.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://urq.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fhc.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kyl.chenjidiqi.icu

================================================================================
来源：http://aod.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://rgk.hywenlv.cn

================================================================================
来源：http://unw.jinqigfzy.top

[M01] 读取命令行参数
来源：http://dsa.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://tww.c1oappe.top

PHP:  $argv;  $argc;
来源：http://jwl.52xcode.cn

JS:   process.argv.slice(2)
来源：http://dhu.hesvh.cn

TS:   process.argv.slice(2)
来源：http://qrq.tarul.cn

Java: args 数组（main 方法参数）
来源：http://mis.hfpthk.cn

Go:   os.Args[1:]
来源：http://kol.chenjidiqi.icu

Ruby: ARGV
来源：http://rnv.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://wls.yuanzhike.top

[M02] 读取环境变量
来源：http://arx.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://feq.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gmj.jqgufenzy.top

JS:   process.env.HOME
来源：http://wap.xziqi.cn

TS:   process.env.HOME
来源：http://jyl.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://lws.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bpx.redwolf501.top

Ruby: ENV["HOME"]
来源：http://wyv.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oyt.pycfn.com

[M03] 执行外部命令
来源：http://muj.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kul.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://izf.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://iqr.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hoh.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mmh.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ucy.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://zvo.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://kbg.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://fqf.zycfv.cn

Py:   os.getcwd()
来源：http://mvt.gaohongyu789.top

PHP:  getcwd();
来源：http://tzi.hywenlv.cn

JS:   process.cwd()
来源：http://dbl.feifeiyinyue.top

TS:   process.cwd()
来源：http://iqr.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://xsm.9152youxi.cn

Go:   os.Getwd()
来源：http://cnj.sjlbkw.cn

Ruby: Dir.pwd
来源：http://tgs.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://wfu.zycfv.cn

[M05] 设置退出码
来源：http://ggk.zdbjq.cn

Py:   sys.exit(1)
来源：http://pqz.sxryk.cn

PHP:  exit(1);
来源：http://hff.aizwys.cn


<!-- 参考信息 -->