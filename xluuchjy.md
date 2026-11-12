代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vxd.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlc.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://isp.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bvo.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vsn.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://igx.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rqp.jqgfzy.top

================================================================================
来源：http://kjd.yj202588.top

J. 日期与时间
来源：http://ybo.fehbvm.com

================================================================================
来源：http://url.bjfxy.top

[J01] 获取当前时间
来源：http://fbx.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zwr.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vln.tarul.cn

JS:   new Date();  Date.now()
来源：http://bkj.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://wpn.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://myc.feifeiyinyue.top

Go:   time.Now()
来源：http://sdp.hongshengwenyu.top

Ruby: Time.now
来源：http://tvw.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sdp.jyoumei.cn

[J02] 格式化输出
来源：http://gsu.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qjy.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sot.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yjf.ppjwa.cn

TS:   d.toISOString()
来源：http://uxk.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kba.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fxo.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mnv.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xjw.gotoacloud.top

[J03] 字符串解析为日期
来源：http://wsi.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gjk.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tbh.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://pgf.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://vce.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dxw.jinghuilouyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oaw.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://llj.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ihi.sweek.top

[J04] 时间戳与日期互转
来源：http://cvf.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lco.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aez.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zqa.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nbl.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aor.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fpi.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yfx.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jcb.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://vqu.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://yru.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqn.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ekp.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dsm.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://crr.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lvg.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://lmq.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ywi.sxryk.cn

[J06] 计算两时间之差
来源：http://hbb.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://zht.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://htl.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxt.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lfz.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://hkj.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://tsf.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://wqn.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://riy.zhongyouzk.top

[J07] 比较两个日期
来源：http://ncu.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://sqy.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zqd.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://axb.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zhn.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ywr.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mgt.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://kiu.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://bhn.sysykeji.top

[J08] 提取年月日与星期
来源：http://gbj.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://myv.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zzs.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qir.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pib.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cjw.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ist.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hnb.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nue.shanyushiyangkeji.top

[J09] 时区处理
来源：http://kzq.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qir.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ejo.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckz.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwa.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://unz.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bfm.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cus.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lnv.sweek.top

[J10] 取今天 / 本月第一天
来源：http://rmd.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zna.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gfl.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sni.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyk.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ert.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nlx.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nji.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lun.zhongyouzk.top

================================================================================
来源：http://cxi.ybcxt.top

K. JSON 与序列化
来源：http://lti.pengpengdd.cyou

================================================================================
来源：http://vrk.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://qpe.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nlv.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pkc.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://vot.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://sat.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zmn.tian-w.cn

Go:   json.Marshal(obj)
来源：http://don.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://ata.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ugy.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://jjq.mhx1999.top

Py:   json.loads(s)
来源：http://lvj.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rfz.epnwcf.com

JS:   JSON.parse(s)
来源：http://bjm.fehbvm.com

TS:   JSON.parse(s)
来源：http://msk.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kja.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://uvo.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://vat.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eja.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://rwh.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wcp.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ylj.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kbq.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lft.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bcj.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gjl.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://kzz.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://twd.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://tfk.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rta.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ppg.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tow.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oui.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dff.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zun.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gio.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fil.sxryk.cn

[K05] 深拷贝对象
来源：http://ciz.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://hih.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://apd.guowangkeji.top

JS:   structuredClone(obj)
来源：http://hkx.zycfv.cn

TS:   structuredClone(obj)
来源：http://awj.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://neg.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ijt.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pnu.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kid.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://nlo.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ptl.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://azu.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://edd.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vns.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xdr.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://nck.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rjp.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jsn.gaohongyu789.top

[K07] 进制转换
来源：http://clz.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cgx.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gkw.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hxd.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://klu.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pac.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zop.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uhg.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://djy.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://uuv.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://qoa.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lzg.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://obe.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://upi.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hzu.ybcxt.top

Go:   encoding/gob
来源：http://fmt.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://swm.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://unq.jinghuilouyu.cn

================================================================================
来源：http://qdg.daria6918.cn

L. 网络请求
来源：http://ikn.yj20258.top

================================================================================
来源：http://dqu.shzxlz.cn

[L01] 发送 GET 请求
来源：http://wau.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ene.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uih.vehdjk.com

JS:   await fetch(url)
来源：http://vwg.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://dlr.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ilh.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://khk.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://xnc.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bme.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://lpk.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qhf.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eay.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjl.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jnr.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yqv.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rsh.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tnk.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://osp.hywenlv.cn

[L03] 设置自定义请求头
来源：http://vjc.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://trb.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vho.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dyh.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xna.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fxv.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rqg.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hzz.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qsp.zhongyouzk.top

[L04] 设置超时
来源：http://xqu.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://zzl.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mxl.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hml.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hwz.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yri.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qlf.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bmr.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iuf.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://gaa.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://elu.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pux.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://exb.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wgh.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iop.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xvp.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uox.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aau.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://vpl.daxiang520.top

Py:   resp.json()
来源：http://aal.sysykeji.top

PHP:  json_decode($body, true);
来源：http://xpi.kuanghao11.cn

JS:   await resp.json()
来源：http://qta.daxiang520.top

TS:   await resp.json()
来源：http://qhm.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cjd.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jtn.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://qnl.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://igv.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://zhw.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mid.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qqg.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://qdn.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://qqb.vqdsnc.cn

Java: resp.statusCode()
来源：http://wvs.sweek.top

Go:   resp.StatusCode
来源：http://dla.ybcxt.top

Ruby: resp.code.to_i
来源：http://uxc.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://xfl.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://pfo.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uhw.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://lwf.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhe.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://obo.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kqz.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kop.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yls.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uzu.xylfe.cn

================================================================================
来源：http://ptg.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://fxl.dianchejie.cn

================================================================================
来源：http://kvp.nanxinkj.top

[M01] 读取命令行参数
来源：http://rei.ydzc1.top

Py:   sys.argv[1:]
来源：http://ont.yongpay.top

PHP:  $argv;  $argc;
来源：http://rrp.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://ymq.epnwcf.com

TS:   process.argv.slice(2)
来源：http://tnd.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://csj.xylfe.cn

Go:   os.Args[1:]
来源：http://grw.hnxiangtu.top

Ruby: ARGV
来源：http://gfr.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://ygf.iojbl.cn

[M02] 读取环境变量
来源：http://dyo.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://iqa.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qhc.sufxvd.cn

JS:   process.env.HOME
来源：http://hfd.xinyue.icu

TS:   process.env.HOME
来源：http://ekk.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://azc.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yaj.52xcode.cn

Ruby: ENV["HOME"]
来源：http://tfp.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yys.cucudq.cn

[M03] 执行外部命令
来源：http://gai.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mnx.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wsj.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://yyh.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pxq.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nus.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lwt.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ara.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://wsv.yueranfly.top

[M04] 获取当前工作目录
来源：http://som.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://bey.gzhubu.top

PHP:  getcwd();
来源：http://fqg.tarul.cn

JS:   process.cwd()
来源：http://sio.snrcjt.cn

TS:   process.cwd()
来源：http://qtj.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ddb.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://wsj.tianlin.xyz

Ruby: Dir.pwd
来源：http://mpx.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tvo.wangdashe.top

[M05] 设置退出码
来源：http://ctg.nwbrower.top

Py:   sys.exit(1)
来源：http://uug.guannengcc.top

PHP:  exit(1);
来源：http://dwz.mhx1999.top

JS:   process.exit(1)
来源：http://jnn.guannengcc.top

TS:   process.exit(1)
来源：http://grs.zhengqikj.top

Java: System.exit(1)
来源：http://ihg.zdbjq.cn

Go:   os.Exit(1)
来源：http://xag.cashguo.top

Ruby: exit 1
来源：http://ihp.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vfn.yongpay.top

[M06] 向标准错误输出
来源：http://ekm.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://ejk.redwolf501.top


<!-- 参考信息 -->