代发 wailian999

Ruby: s.scan(/error/i)
来源：http://npq.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://avi.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://kyr.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://non.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iut.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jaf.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nfg.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://umt.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wsf.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ncy.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://udt.hfpthk.cn

================================================================================
来源：http://wrp.gaohongyu789.top

J. 日期与时间
来源：http://qbk.feifeiyinyue.top

================================================================================
来源：http://fzi.haohaochexian.top

[J01] 获取当前时间
来源：http://zmm.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://qll.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hkg.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://bwo.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://jon.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fuy.jyoumei.cn

Go:   time.Now()
来源：http://iob.nanxuanxn.top

Ruby: Time.now
来源：http://ypz.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://izr.yj20258888.top

[J02] 格式化输出
来源：http://zrp.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://akf.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ntq.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://apd.52xcode.cn

TS:   d.toISOString()
来源：http://reg.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ezv.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lsx.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://beh.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kha.snrcjt.cn

[J03] 字符串解析为日期
来源：http://gkl.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://flq.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ogi.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://rwh.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://iqc.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mwo.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ydd.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://yhn.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cgh.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://tta.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xsb.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cte.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tej.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ejy.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xnz.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dil.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uoc.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eql.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://vcq.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://vfo.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://czg.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://acd.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zmu.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://mly.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qic.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://akd.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://oiy.hfpthk.cn

[J06] 计算两时间之差
来源：http://grb.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://pbn.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://gdo.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hhh.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zsq.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zlp.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://chu.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://qqs.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://nlj.yuxming.cn

[J07] 比较两个日期
来源：http://hsk.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://mfp.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vmo.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tob.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ijy.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cby.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jae.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://mxu.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://baj.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://avi.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yua.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tld.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ugr.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oiy.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sbt.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pwv.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://spx.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fjg.yueranfly.top

[J09] 时区处理
来源：http://zai.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dea.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rje.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lfq.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okk.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xqx.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fbk.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://uel.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://usy.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://mgb.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fxe.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fme.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jly.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tqe.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fsv.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsu.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ddi.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dzm.sxryk.cn

================================================================================
来源：http://mpr.yj202588.top

K. JSON 与序列化
来源：http://wja.316326.xyz

================================================================================
来源：http://kio.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://kbl.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fwt.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dam.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://odg.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://une.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fda.nwbrower.top

Go:   json.Marshal(obj)
来源：http://yev.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hfr.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://phn.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://xcw.tarul.cn

Py:   json.loads(s)
来源：http://wtd.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ktc.birdmap.top

JS:   JSON.parse(s)
来源：http://kim.xziqi.cn

TS:   JSON.parse(s)
来源：http://dxl.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aii.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://xah.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://zvf.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dzw.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://suw.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://djj.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jjb.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kyw.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://avh.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://byk.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ydk.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://qcc.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://alg.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://grq.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vbp.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pxh.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bba.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ruo.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ezh.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ufk.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lxl.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://joo.jinqigufen.top

[K05] 深拷贝对象
来源：http://csi.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://pel.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://ebv.sysykeji.top

JS:   structuredClone(obj)
来源：http://xad.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://qkk.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jji.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kwv.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hzh.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://qbm.dashuyun.cn

[K06] 解析 URL 查询串
来源：http://iyt.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hqu.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zpi.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mty.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://laa.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jts.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gtn.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yxw.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://chi.yvedp.cn

[K07] 进制转换
来源：http://mha.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tqb.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hda.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yto.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ean.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lyl.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uik.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jcl.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hre.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://emw.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://jpt.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://ptc.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://nri.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://lyf.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tkt.gogol.net.cn

Go:   encoding/gob
来源：http://tck.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://lnm.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hdz.svipenyu.cn

================================================================================
来源：http://liy.aizwys.cn

L. 网络请求
来源：http://kvq.yj20258.top

================================================================================
来源：http://xbf.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://jwj.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ygw.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dev.fktsv.cn

JS:   await fetch(url)
来源：http://ijq.ivvv.top

TS:   await fetch(url)
来源：http://yzv.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jee.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://lae.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sqy.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kdm.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://nuj.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mgn.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://flz.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mnv.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zzc.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uwa.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dxm.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bkh.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nmd.xinyue.icu

[L03] 设置自定义请求头
来源：http://bfk.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vtu.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gxz.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlu.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ite.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bem.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jmx.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://smm.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fmf.jinyuanbaomall.cn

[L04] 设置超时
来源：http://pnk.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://nws.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dxa.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgd.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lkx.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tvg.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tir.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://trq.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyk.ybcxt.top

[L05] 上传文件（multipart）
来源：http://fxz.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wks.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qnx.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wuf.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xvy.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ale.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kxg.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pum.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bzc.sweek.top

[L06] 解析响应为 JSON
来源：http://xud.yueranfly.top

Py:   resp.json()
来源：http://qzf.jianghu66.top

PHP:  json_decode($body, true);
来源：http://bvz.jiagoushi.top

JS:   await resp.json()
来源：http://jqe.jianghu66.top

TS:   await resp.json()
来源：http://bjj.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uor.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fge.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://vql.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ain.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://pel.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pmb.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://axq.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://ooa.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://xdx.pengpengdd.cyou

Java: resp.statusCode()
来源：http://mdm.zdbjq.cn

Go:   resp.StatusCode
来源：http://viy.guannengcc.top

Ruby: resp.code.to_i
来源：http://ifg.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://iaa.yuanzhike.top

[L08] 并发请求多个地址
来源：http://ffu.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yss.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://wgc.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kqd.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwk.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ano.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rxb.zhongyouzk.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lfa.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qgo.feifeiyinyue.top

================================================================================
来源：http://qlq.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://ysr.jinyuanbaomall.cn

================================================================================
来源：http://cmi.quarkkingdee.top

[M01] 读取命令行参数
来源：http://fjj.fengsongda.top

Py:   sys.argv[1:]
来源：http://lzv.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://xso.andypj.xyz

JS:   process.argv.slice(2)
来源：http://gww.52xcode.cn

TS:   process.argv.slice(2)
来源：http://jgl.havefunace.top

Java: args 数组（main 方法参数）
来源：http://hny.yanxiufei.cn

Go:   os.Args[1:]
来源：http://tvi.zdbjq.cn

Ruby: ARGV
来源：http://bgc.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://owz.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://prq.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://qni.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baf.pengpengdd.cyou

JS:   process.env.HOME
来源：http://izm.shuidangran.top

TS:   process.env.HOME
来源：http://kye.hcnkem.com

Java: System.getenv("HOME")
来源：http://xjd.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://daj.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://wtp.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qhw.xinyue.icu

[M03] 执行外部命令
来源：http://hyz.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gag.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vao.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://niv.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tgd.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gmm.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://laj.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://utr.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://dgu.meibo888.top

[M04] 获取当前工作目录
来源：http://tya.tian-w.cn

Py:   os.getcwd()
来源：http://foh.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://mhn.jinqigfzy.top

JS:   process.cwd()
来源：http://jue.iojbl.cn

TS:   process.cwd()
来源：http://xpi.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://dno.fehbvm.com

Go:   os.Getwd()
来源：http://khn.ybcxt.top

Ruby: Dir.pwd
来源：http://les.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://igy.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://bof.ybcxt.top

Py:   sys.exit(1)
来源：http://btv.quarkkingdee.top

PHP:  exit(1);
来源：http://rmk.52xcode.cn

JS:   process.exit(1)
来源：http://wsc.mhx1999.top

TS:   process.exit(1)
来源：http://nfl.kuanghao11.cn

Java: System.exit(1)
来源：http://uev.cheryme.top

Go:   os.Exit(1)
来源：http://tme.svipenyu.cn


<!-- 参考信息 -->