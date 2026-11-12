代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bck.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tnw.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jzo.zhiwuduotai.top

================================================================================
来源：http://whz.jqgfzy.top

J. 日期与时间
来源：http://shf.nanxinkj.top

================================================================================
来源：http://wkk.zhiwuduotai.top

[J01] 获取当前时间
来源：http://jcp.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://egv.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mev.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://hhz.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://wrq.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zhq.bbcook.cn

Go:   time.Now()
来源：http://cwy.quarkkingdee.top

Ruby: Time.now
来源：http://jtn.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xjb.shanyushiyangtech.top

[J02] 格式化输出
来源：http://izr.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdx.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cff.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ldt.aibaodan.cn

TS:   d.toISOString()
来源：http://ywx.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rvq.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfl.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kmu.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oxy.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://kaw.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gwe.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ett.sweek.top

JS:   new Date("2024-01-02")
来源：http://chr.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://gib.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://vej.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aep.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://cal.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oxb.hnqzz.top

[J04] 时间戳与日期互转
来源：http://uow.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://juy.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qat.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://edi.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vrd.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://goa.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mqx.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wfh.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hjn.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://ftm.meibo888.top

Py:   now + timedelta(days=7)
来源：http://ous.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wqa.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sfk.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://amm.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ytt.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nco.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://wmg.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://nnr.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://hsn.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://hqx.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://div.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zhd.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jgr.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://mdi.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://vvq.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://plu.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://rpu.ydjk.org.cn

[J07] 比较两个日期
来源：http://cvo.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bdt.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://udf.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hjn.zhaomingkeji.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://weg.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rtv.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qqm.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://twn.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://oaj.zhixingplan.top

[J08] 提取年月日与星期
来源：http://siv.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://byp.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rij.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bur.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jod.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ogo.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fuu.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wak.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kjg.redwolf501.top

[J09] 时区处理
来源：http://sab.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cdh.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pls.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hxb.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wsi.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hea.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gga.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eal.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xyp.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://zvf.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://tzd.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dns.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gzi.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pmg.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mzo.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://thy.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gzd.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nxo.bbcook.cn

================================================================================
来源：http://zwm.zycfv.cn

K. JSON 与序列化
来源：http://xjj.gotoacloud.top

================================================================================
来源：http://uyl.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://uml.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tre.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dmq.cashguo.top

JS:   JSON.stringify(obj)
来源：http://och.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://ilo.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jqq.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://aoa.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://fho.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zzr.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://pcg.hesvh.cn

Py:   json.loads(s)
来源：http://vvj.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jhi.hammf.cn

JS:   JSON.parse(s)
来源：http://ujz.epnwcf.com

TS:   JSON.parse(s)
来源：http://sjb.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bbc.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://yza.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://kth.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yrs.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://wjt.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ymh.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eln.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vgp.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://epl.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ygn.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cia.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://crb.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pvj.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://emg.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xsl.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uzy.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gcy.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aty.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://okw.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://voj.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzp.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ddv.fzhhl.top

[K05] 深拷贝对象
来源：http://sji.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://zzc.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://cfw.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://vvv.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://rxc.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://brt.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xes.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tmi.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ctw.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://juw.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://asa.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oys.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdz.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytc.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hmy.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eap.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gyt.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gsp.snrcjt.cn

[K07] 进制转换
来源：http://kfo.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ieb.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kbd.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bte.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yie.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lfj.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://klz.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dip.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://okh.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://aes.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://lko.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lxk.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://coc.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://ggd.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wyf.nanxinkj.top

Go:   encoding/gob
来源：http://qvz.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://lph.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://noj.jianghu66.top

================================================================================
来源：http://wed.nwbrower.top

L. 网络请求
来源：http://wbk.sjlbkw.cn

================================================================================
来源：http://yyg.yueranfly.top

[L01] 发送 GET 请求
来源：http://wlr.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqi.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vhq.vqdsnc.cn

JS:   await fetch(url)
来源：http://lku.xylfe.cn

TS:   await fetch(url)
来源：http://znj.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zzv.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://qrp.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vhl.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eqj.yj202588.top

[L02] 发送 POST JSON
来源：http://qrv.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dra.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ock.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blx.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtx.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhh.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nvk.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://icg.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://brw.cqqwz.cn

[L03] 设置自定义请求头
来源：http://jkc.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://brb.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cjt.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kzy.xuanzx.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vsb.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gcn.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hyl.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://khh.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ymc.andypj.xyz

[L04] 设置超时
来源：http://rgq.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://syc.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tvn.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgf.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjt.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jpt.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vla.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jac.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://brh.yonumen.top

[L05] 上传文件（multipart）
来源：http://iax.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ptk.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dty.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ptp.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wcc.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ots.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lcx.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://krz.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hcy.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://cta.yonumen.top

Py:   resp.json()
来源：http://rdx.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://wot.wangdashe.top

JS:   await resp.json()
来源：http://lmc.shzxlz.cn

TS:   await resp.json()
来源：http://pek.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iqp.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eah.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://owi.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://plx.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://xhm.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hvs.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cbk.yj202588.top

JS:   resp.ok;  resp.status
来源：http://oyd.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://dij.cqqwz.cn

Java: resp.statusCode()
来源：http://eea.dianchejie.cn

Go:   resp.StatusCode
来源：http://zwg.zdqjudy.top

Ruby: resp.code.to_i
来源：http://ywp.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://cwv.zhengqikj.top

[L08] 并发请求多个地址
来源：http://wnw.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxj.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://nff.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nju.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lji.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iiz.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxd.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cpy.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kpf.pycfn.com

================================================================================
来源：http://srq.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://gzr.hfpthk.cn

================================================================================
来源：http://lmk.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://opt.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://eqw.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://llk.yuxming.cn

JS:   process.argv.slice(2)
来源：http://ryo.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://ftu.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://uye.cucudq.cn

Go:   os.Args[1:]
来源：http://lrd.jinyuanbaomall.cn

Ruby: ARGV
来源：http://win.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://bug.zhengqikj.top

[M02] 读取环境变量
来源：http://kbd.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://bka.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vnb.wangdashe.top

JS:   process.env.HOME
来源：http://soz.ydjk.org.cn

TS:   process.env.HOME
来源：http://egf.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://gtp.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dgi.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://xtu.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kpl.guannengcc.top

[M03] 执行外部命令
来源：http://lok.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kka.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bvl.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dyw.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mqe.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://din.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://abp.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://wdw.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://qpn.52xcode.cn

[M04] 获取当前工作目录
来源：http://fzx.jinqigufen.top

Py:   os.getcwd()
来源：http://kwt.sweek.top

PHP:  getcwd();
来源：http://zon.zdqjudy.top

JS:   process.cwd()
来源：http://gio.ppjwa.cn

TS:   process.cwd()
来源：http://icq.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://jur.tianlin.xyz

Go:   os.Getwd()
来源：http://hja.nwbrower.top

Ruby: Dir.pwd
来源：http://lqh.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pye.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://zll.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://wak.iojbl.cn

PHP:  exit(1);
来源：http://qhd.fktsv.cn

JS:   process.exit(1)
来源：http://zug.fengsongda.top

TS:   process.exit(1)
来源：http://ykj.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://wku.0kj1m.cn

Go:   os.Exit(1)
来源：http://kgy.dianchejie.cn

Ruby: exit 1
来源：http://lbo.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qep.jianghu66.top

[M06] 向标准错误输出
来源：http://sps.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://dcl.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vjx.fktsv.cn

JS:   console.error("err")
来源：http://hwd.bbcook.cn

TS:   console.error("err")
来源：http://rrt.yongpay.top

Java: System.err.println("err")
来源：http://fwk.daria6918.cn


<!-- 参考信息 -->