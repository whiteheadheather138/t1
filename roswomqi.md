代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://idg.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qlr.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rbp.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wxv.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wad.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sha.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssq.zycfv.cn

================================================================================
来源：http://lxo.fengsongda.top

J. 日期与时间
来源：http://yst.jinqigfzy.top

================================================================================
来源：http://uku.dashuyun.cn

[J01] 获取当前时间
来源：http://tte.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://nvj.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jrk.cashguo.top

JS:   new Date();  Date.now()
来源：http://slo.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://ojy.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mkd.ybcxt.top

Go:   time.Now()
来源：http://etu.jyoumei.cn

Ruby: Time.now
来源：http://fdq.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qsy.fehbvm.com

[J02] 格式化输出
来源：http://xvw.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kbh.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://quh.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://elz.fengsongda.top

TS:   d.toISOString()
来源：http://bqb.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fea.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgl.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xsu.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tbe.zhixingplan.top

[J03] 字符串解析为日期
来源：http://xrc.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vvs.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tug.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://yxh.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://qcz.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zvw.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://txh.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://eci.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rab.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://qck.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rvm.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hze.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vsq.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pju.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vqw.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gbo.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://owd.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://acb.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://yju.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://etc.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jpx.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://noo.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://htj.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://lpl.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vmo.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://cpa.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qfi.snrcjt.cn

[J06] 计算两时间之差
来源：http://xbe.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://tbc.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://ypd.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://udy.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qgn.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://onh.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://tjx.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://fmf.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://wtl.feifeiyinyue.top

[J07] 比较两个日期
来源：http://qtu.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://dxu.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jsf.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://xxl.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lvx.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ivo.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tqu.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://apc.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://pcu.hfpthk.cn

[J08] 提取年月日与星期
来源：http://vqp.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://clq.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://thb.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yes.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wbq.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ggy.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ezr.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gbk.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hyy.zdbjq.cn

[J09] 时区处理
来源：http://ifo.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qxq.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bmd.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xdm.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zvt.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wbq.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xbo.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jqx.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ibn.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://dnv.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://okd.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jdf.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvn.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oqi.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fms.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://efl.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qiw.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kop.vqdsnc.cn

================================================================================
来源：http://cso.zhoulong.xyz

K. JSON 与序列化
来源：http://rwy.zdbjq.cn

================================================================================
来源：http://fpg.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://tii.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://giq.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iid.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://elv.uphjek.com

TS:   JSON.stringify(obj)
来源：http://ila.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eml.shuidangran.top

Go:   json.Marshal(obj)
来源：http://ctk.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://lqm.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yap.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://dih.redwolf501.top

Py:   json.loads(s)
来源：http://wxs.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xjm.316326.xyz

JS:   JSON.parse(s)
来源：http://kti.fzhhl.top

TS:   JSON.parse(s)
来源：http://uis.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://giu.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://xnb.pycfn.com

Ruby: JSON.parse(s)
来源：http://kbx.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tib.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://hio.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://clj.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iiy.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://llk.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pki.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gog.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uvr.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://xmd.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jnf.yongpay.top

[K04] 读取 JSON 文件
来源：http://evd.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ird.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pvx.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jas.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gcq.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nwo.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uhl.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dqm.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dkn.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://tpy.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://wty.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://gly.sysykeji.top

JS:   structuredClone(obj)
来源：http://xwf.52xcode.cn

TS:   structuredClone(obj)
来源：http://gsk.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://upb.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eqh.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hmu.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ejr.hnqzz.top

[K06] 解析 URL 查询串
来源：http://dqs.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pyy.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xjj.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jdp.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qfw.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://scu.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bqu.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ggw.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sgv.zhixingplan.top

[K07] 进制转换
来源：http://ddo.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rce.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wng.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gno.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zbs.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yxb.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xvb.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bfm.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hzc.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://qbi.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://gvu.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://dky.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://tfp.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://leq.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ahq.yj20258.top

Go:   encoding/gob
来源：http://srd.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://dgh.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yxa.hongshengwenyu.top

================================================================================
来源：http://zjo.ctjpmb.com

L. 网络请求
来源：http://wri.cdnleiting.top

================================================================================
来源：http://gii.andypj.xyz

[L01] 发送 GET 请求
来源：http://wdg.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qff.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nji.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://vwu.zhiwuduotai.top

TS:   await fetch(url)
来源：http://aca.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://swx.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://iec.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ysf.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kfp.fzhhl.top

[L02] 发送 POST JSON
来源：http://nvc.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://psn.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gry.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hvl.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlu.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ucq.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rnp.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wpy.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eey.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://nlw.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bbs.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bzj.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uwj.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lep.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mkr.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eng.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://add.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://osi.yj20258888.top

[L04] 设置超时
来源：http://xcl.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://tzu.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zog.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyh.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://erm.kuanghao11.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ozt.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jok.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwg.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zva.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://lsq.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cxm.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mme.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lts.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mob.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rfc.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://akt.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vjf.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qut.cheryme.top

[L06] 解析响应为 JSON
来源：http://fnl.feifeiyinyue.top

Py:   resp.json()
来源：http://esn.shuidangran.top

PHP:  json_decode($body, true);
来源：http://krq.gaohongyu789.top

JS:   await resp.json()
来源：http://cxo.shanyushiyangtech.top

TS:   await resp.json()
来源：http://xio.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tld.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hfy.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://mcx.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fkp.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://dlu.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bwc.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wxz.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://hje.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://yms.snrcjt.cn

Java: resp.statusCode()
来源：http://fpd.fktsv.cn

Go:   resp.StatusCode
来源：http://qej.yangfankeji.com

Ruby: resp.code.to_i
来源：http://evk.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://tkz.daria6918.cn

[L08] 并发请求多个地址
来源：http://dwq.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zyp.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://ofu.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smg.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dby.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://psr.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wks.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fvn.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yrl.ydjk.org.cn

================================================================================
来源：http://jpe.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://rhw.yj202588.top

================================================================================
来源：http://did.jianghu66.top

[M01] 读取命令行参数
来源：http://gxp.316326.xyz

Py:   sys.argv[1:]
来源：http://llz.ydzc1.top

PHP:  $argv;  $argc;
来源：http://rfe.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://tlc.yj20258888.top

TS:   process.argv.slice(2)
来源：http://twg.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://kmo.9152youxi.cn

Go:   os.Args[1:]
来源：http://wct.xuetiantiany.cn

Ruby: ARGV
来源：http://jff.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://yyx.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://frp.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://lnm.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ewk.xziqi.cn

JS:   process.env.HOME
来源：http://zpj.zhijiandao.cn

TS:   process.env.HOME
来源：http://mwj.yj20258888.top

Java: System.getenv("HOME")
来源：http://yfe.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ypj.xuanzx.com

Ruby: ENV["HOME"]
来源：http://znj.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tbb.jinqigufen.top

[M03] 执行外部命令
来源：http://iyq.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cmh.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tuf.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mqm.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ddf.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tjo.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bvv.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fsz.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://oqs.jianghu66.top

[M04] 获取当前工作目录
来源：http://xpk.ppjwa.cn

Py:   os.getcwd()
来源：http://khb.cheryme.top

PHP:  getcwd();
来源：http://enu.zhixingplan.top

JS:   process.cwd()
来源：http://hcx.mhx1999.top

TS:   process.cwd()
来源：http://rkj.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://gef.dashuyun.cn

Go:   os.Getwd()
来源：http://nsn.yuxming.cn

Ruby: Dir.pwd
来源：http://byz.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hzk.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://nmg.jianghu66.top

Py:   sys.exit(1)
来源：http://xed.tianlin.xyz

PHP:  exit(1);
来源：http://ypo.zhengqikj.top

JS:   process.exit(1)
来源：http://krs.cqqwz.cn

TS:   process.exit(1)
来源：http://gtk.sxryk.cn

Java: System.exit(1)
来源：http://zbk.zhixingplan.top

Go:   os.Exit(1)
来源：http://iqm.jianghu66.top

Ruby: exit 1
来源：http://snd.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://umy.guowangkeji.top

[M06] 向标准错误输出
来源：http://hmp.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://lyk.daria6918.cn


<!-- 参考信息 -->