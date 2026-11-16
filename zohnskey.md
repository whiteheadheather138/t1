代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dxx.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uod.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cxk.xingfuxueyuan.xyz

================================================================================
来源：http://ttt.yfazqb.com

J. 日期与时间
来源：http://jxg.zycfv.cn

================================================================================
来源：http://xtz.xuetiantiany.cn

[J01] 获取当前时间
来源：http://yui.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ntl.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dwp.cheryme.top

JS:   new Date();  Date.now()
来源：http://azz.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://trg.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eis.chenjidiqi.icu

Go:   time.Now()
来源：http://lwr.sweek.top

Ruby: Time.now
来源：http://iro.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://afn.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://mmk.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aqr.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gfw.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rja.haohaochexian.top

TS:   d.toISOString()
来源：http://tfs.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lqf.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://acw.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jam.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qgx.xinyue.icu

[J03] 字符串解析为日期
来源：http://uly.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://frr.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tup.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://pbj.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://kxs.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://vda.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vct.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://iwx.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zdy.yvedp.cn

[J04] 时间戳与日期互转
来源：http://syf.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pna.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xwk.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://klf.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nmd.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xyn.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mxk.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tdh.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wsk.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://yku.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://tob.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxn.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://loi.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mjk.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://zeo.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xej.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://phq.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://pri.c1oappe.top

[J06] 计算两时间之差
来源：http://pzh.birdmap.top

Py:   (end - start).total_seconds()
来源：http://jri.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://hug.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dyc.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lqe.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://tph.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://nge.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://wre.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://yjw.fehbvm.com

[J07] 比较两个日期
来源：http://iqy.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://mac.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://enu.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://khx.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gwm.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://egs.aibaodan.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sng.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vql.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://ftj.yj20258.top

[J08] 提取年月日与星期
来源：http://akn.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mwc.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://whl.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rjb.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zng.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ajl.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nso.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lvx.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://itv.havefunace.top

[J09] 时区处理
来源：http://wmg.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dga.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://trj.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qiw.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pkh.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gek.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kso.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://kvo.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rrb.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://sng.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aoc.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kpu.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ojd.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sid.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aih.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wae.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pdr.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nxk.ivvv.top

================================================================================
来源：http://lfn.xylfe.cn

K. JSON 与序列化
来源：http://rtu.birdmap.top

================================================================================
来源：http://bos.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://rqw.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://snp.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iiy.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://ydm.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://mqb.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iut.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://wkt.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://tfz.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://yql.yfazqb.com

[K02] JSON 字符串转对象
来源：http://zsz.dianchejie.cn

Py:   json.loads(s)
来源：http://hpw.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kjl.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://fnm.yj20258.top

TS:   JSON.parse(s)
来源：http://jdi.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qxr.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://hgd.jianghu66.top

Ruby: JSON.parse(s)
来源：http://tay.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tqs.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://dir.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hld.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://may.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eeq.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://htj.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uwg.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mvg.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://gpy.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pfa.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://ual.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fkf.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zgb.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ucg.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pcs.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://arr.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zku.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hgg.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pot.nwbrower.top

[K05] 深拷贝对象
来源：http://blj.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://mde.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://ute.epnwcf.com

JS:   structuredClone(obj)
来源：http://gjs.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://xpq.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wra.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qfc.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jwm.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aeh.havefunace.top

[K06] 解析 URL 查询串
来源：http://wbt.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://goq.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jpz.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jnb.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yju.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pyy.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xag.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cny.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vwz.shangyingyoupin.top

[K07] 进制转换
来源：http://rho.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vmn.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://upf.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://opg.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rov.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hvh.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ucy.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jyh.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://voh.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://yxc.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://vhg.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pky.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://bpw.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://fsn.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lwt.chenlongwang.top

Go:   encoding/gob
来源：http://mii.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://iqq.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://inu.pengpengdd.cyou

================================================================================
来源：http://pyb.nwbrower.top

L. 网络请求
来源：http://gri.sufxvd.cn

================================================================================
来源：http://gsc.9152youxi.cn

[L01] 发送 GET 请求
来源：http://ngy.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qgb.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qbe.tarul.cn

JS:   await fetch(url)
来源：http://wms.xylfe.cn

TS:   await fetch(url)
来源：http://yvw.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qbn.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://ojb.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://upi.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vah.ppjwa.cn

[L02] 发送 POST JSON
来源：http://cns.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://dau.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rbx.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pry.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zwk.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ohq.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://svz.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://day.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kow.birdmap.top

[L03] 设置自定义请求头
来源：http://ahk.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gyu.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://our.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lzf.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnt.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awe.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fda.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pdm.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bew.xuanzx.com

[L04] 设置超时
来源：http://ggu.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://igc.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rph.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yov.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhk.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fks.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ful.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lpq.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gdc.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://fwb.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mkb.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dkl.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qxb.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wfr.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cqd.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wda.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aow.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tzu.tarul.cn

[L06] 解析响应为 JSON
来源：http://ocs.andypj.xyz

Py:   resp.json()
来源：http://yqp.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://mrp.kuanghao11.cn

JS:   await resp.json()
来源：http://sai.tian-w.cn

TS:   await resp.json()
来源：http://nul.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wli.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://usl.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://puc.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zbp.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://mqi.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kaz.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fjl.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://txz.ivvv.top

TS:   resp.ok;  resp.status
来源：http://pff.fehbvm.com

Java: resp.statusCode()
来源：http://utt.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://atf.cdnleiting.top

Ruby: resp.code.to_i
来源：http://hba.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://vhq.hcnkem.com

[L08] 并发请求多个地址
来源：http://jli.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dah.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://zmc.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwx.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mwd.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gcf.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wdq.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfh.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wqd.tianlin.xyz

================================================================================
来源：http://ubt.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://arh.gaohongyu789.top

================================================================================
来源：http://yob.pycfn.com

[M01] 读取命令行参数
来源：http://yyn.snrcjt.cn

Py:   sys.argv[1:]
来源：http://xcd.havefunace.top

PHP:  $argv;  $argc;
来源：http://mch.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://uie.316326.xyz

TS:   process.argv.slice(2)
来源：http://lfg.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://eko.shuidangran.top

Go:   os.Args[1:]
来源：http://tke.snrcjt.cn

Ruby: ARGV
来源：http://xgk.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://opn.jiagoushi.top

[M02] 读取环境变量
来源：http://bxv.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://msi.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cxu.jyoumei.cn

JS:   process.env.HOME
来源：http://ghj.dashuyun.cn

TS:   process.env.HOME
来源：http://uzl.svipenyu.cn

Java: System.getenv("HOME")
来源：http://xpn.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://edd.redwolf501.top

Ruby: ENV["HOME"]
来源：http://icr.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rgi.svipenyu.cn

[M03] 执行外部命令
来源：http://ysv.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zwi.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fyl.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qtg.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://hev.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ahx.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dnu.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://nlc.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://wjo.hesvh.cn

[M04] 获取当前工作目录
来源：http://xmm.shuidangran.top

Py:   os.getcwd()
来源：http://ctr.mhx1999.top

PHP:  getcwd();
来源：http://wwf.jlsjyb.cn

JS:   process.cwd()
来源：http://rxj.xuetiantiany.cn

TS:   process.cwd()
来源：http://bbv.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://yiw.yongpay.top

Go:   os.Getwd()
来源：http://zcl.fktsv.cn

Ruby: Dir.pwd
来源：http://fmf.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://nrb.yanxiufei.cn

[M05] 设置退出码
来源：http://pol.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://ygd.xuanzx.com

PHP:  exit(1);
来源：http://ruf.hongshengwenyu.top

JS:   process.exit(1)
来源：http://pvk.nanxuanxn.top

TS:   process.exit(1)
来源：http://ulf.fengsongda.top

Java: System.exit(1)
来源：http://piq.epnwcf.com

Go:   os.Exit(1)
来源：http://kcs.zhaomingkeji.xyz

Ruby: exit 1
来源：http://dvs.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zww.xziqi.cn

[M06] 向标准错误输出
来源：http://ees.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://lct.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://llf.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://mya.zhengqikj.top

TS:   console.error("err")
来源：http://czs.fengsongda.top

Java: System.err.println("err")
来源：http://ubn.pycfn.com


<!-- 参考信息 -->