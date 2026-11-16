代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tla.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ecv.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jli.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ezr.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://deu.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uxq.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ikn.jlsjyb.cn

================================================================================
来源：http://iuf.jiagoushi.top

J. 日期与时间
来源：http://wvm.jyoumei.cn

================================================================================
来源：http://kse.hnxiangtu.top

[J01] 获取当前时间
来源：http://gdt.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qdf.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ltv.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://mbp.gzhubu.top

TS:   new Date();  Date.now()
来源：http://lqs.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yhr.xuanzx.com

Go:   time.Now()
来源：http://mzx.xinyue.icu

Ruby: Time.now
来源：http://cgr.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://shl.ctjpmb.com

[J02] 格式化输出
来源：http://zkk.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://esp.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://igo.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgc.jinqigfzy.top

TS:   d.toISOString()
来源：http://ecp.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nry.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xsf.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://goq.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bid.aibaodan.cn

[J03] 字符串解析为日期
来源：http://lxh.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://npp.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lay.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://pzx.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://qcv.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vom.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xog.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://cii.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fgw.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://blt.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vyk.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yrk.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ctp.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://xfh.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vau.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xse.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bkq.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://saf.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://ftw.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://wuw.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ldh.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rxv.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://irf.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://pxw.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrq.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://txv.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rjn.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://ocv.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://vcq.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://fkb.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lpr.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ham.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://rcb.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://ovz.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://sqt.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://cyc.xylfe.cn

[J07] 比较两个日期
来源：http://apt.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://kci.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aat.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://vca.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://aus.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cyj.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ghd.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sei.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://cwj.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://vfg.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nzh.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baf.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vrp.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rxr.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://epe.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vxr.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gup.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fdo.tianlin.xyz

[J09] 时区处理
来源：http://nhq.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://obx.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ygl.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zfp.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://umb.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mnk.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://orb.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uqk.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ita.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://sjq.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://llp.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qnk.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hyw.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://azj.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vwv.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bqf.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gnn.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rsf.sxryk.cn

================================================================================
来源：http://xbm.hnqzz.top

K. JSON 与序列化
来源：http://xqq.tanke756.top

================================================================================
来源：http://tic.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://qqt.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yrc.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tlw.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://dcf.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://jvv.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://opo.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://hfv.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://wbu.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oaj.tian-w.cn

[K02] JSON 字符串转对象
来源：http://kfa.sufxvd.cn

Py:   json.loads(s)
来源：http://usy.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fwd.yvedp.cn

JS:   JSON.parse(s)
来源：http://zeb.aibaodan.cn

TS:   JSON.parse(s)
来源：http://sgl.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://edc.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://emy.tanke756.top

Ruby: JSON.parse(s)
来源：http://fin.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xwq.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://yze.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ucz.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dwf.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://rzp.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://usc.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://flk.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dez.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://txy.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://glf.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://clu.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fnm.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fag.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bqh.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ega.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wcm.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vtz.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wpi.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xse.zhixingplan.top

[K05] 深拷贝对象
来源：http://eyz.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://afr.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://puk.tarul.cn

JS:   structuredClone(obj)
来源：http://xkx.cheryme.top

TS:   structuredClone(obj)
来源：http://upb.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hmr.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ycd.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kcx.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://qdl.vehdjk.com

[K06] 解析 URL 查询串
来源：http://bjs.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xyk.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jvo.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ila.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fmd.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xeb.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://lfa.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wqj.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://akh.fengsongda.top

[K07] 进制转换
来源：http://zgv.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dnj.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jpv.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mgq.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nad.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rrl.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zfg.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pfu.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wkt.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://zeb.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://okh.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://gmc.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://yym.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://qgl.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nmp.zdqjudy.top

Go:   encoding/gob
来源：http://zqe.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://qks.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oen.guowangkeji.top

================================================================================
来源：http://rcm.fktsv.cn

L. 网络请求
来源：http://oms.fzhhl.top

================================================================================
来源：http://grk.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://xwi.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rza.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yts.fktsv.cn

JS:   await fetch(url)
来源：http://ufj.hnxiangtu.top

TS:   await fetch(url)
来源：http://jsv.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hcs.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://zqp.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wzs.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pap.tarul.cn

[L02] 发送 POST JSON
来源：http://bnb.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://cgd.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ibq.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ots.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cgs.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ark.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hqc.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mcy.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://arq.zycfv.cn

[L03] 设置自定义请求头
来源：http://gjh.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ymy.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mlc.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zmg.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nvs.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rmu.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cqu.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://crz.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://coj.epnwcf.com

[L04] 设置超时
来源：http://ckw.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://liy.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oci.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyl.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jsr.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fvm.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mme.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wuu.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cdp.bbcook.cn

[L05] 上传文件（multipart）
来源：http://jan.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uxj.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yeu.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://biz.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fhn.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nqx.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pdn.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bfr.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bpp.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://roy.zhengqikj.top

Py:   resp.json()
来源：http://lby.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://qwv.vehdjk.com

JS:   await resp.json()
来源：http://ltn.mhx1999.top

TS:   await resp.json()
来源：http://rtu.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wbq.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dva.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://qdd.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uhn.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://waa.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fdg.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bim.tarul.cn

JS:   resp.ok;  resp.status
来源：http://mpt.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://gqc.zhengqikj.top

Java: resp.statusCode()
来源：http://lng.jqgufenzy.top

Go:   resp.StatusCode
来源：http://svx.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://mbo.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://axi.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://epf.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://swb.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://hnt.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svh.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xeb.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xvo.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zfr.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oar.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jup.shuidangran.top

================================================================================
来源：http://sli.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://fbn.xylfe.cn

================================================================================
来源：http://tpy.vqdsnc.cn

[M01] 读取命令行参数
来源：http://jsz.ppjwa.cn

Py:   sys.argv[1:]
来源：http://mqr.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://zhs.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://yqi.fehbvm.com

TS:   process.argv.slice(2)
来源：http://wrg.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://zhz.jyoumei.cn

Go:   os.Args[1:]
来源：http://waj.hongshengwenyu.top

Ruby: ARGV
来源：http://mnp.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://llc.shzxlz.cn

[M02] 读取环境变量
来源：http://ptv.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://bld.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cds.ivvv.top

JS:   process.env.HOME
来源：http://tvz.yongpay.top

TS:   process.env.HOME
来源：http://aek.tanke756.top

Java: System.getenv("HOME")
来源：http://xmu.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://til.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://agg.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ogl.ydjk.org.cn

[M03] 执行外部命令
来源：http://gdn.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://asy.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ifv.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lcg.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cyl.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ngv.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xba.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://hdu.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://gku.vehdjk.com

[M04] 获取当前工作目录
来源：http://bcu.ctjpmb.com

Py:   os.getcwd()
来源：http://kwm.ppjwa.cn

PHP:  getcwd();
来源：http://xxb.smart0.xyz

JS:   process.cwd()
来源：http://lwd.jiagoushi.top

TS:   process.cwd()
来源：http://sno.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://vpd.0kj1m.cn

Go:   os.Getwd()
来源：http://utv.0kj1m.cn

Ruby: Dir.pwd
来源：http://lxh.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fri.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://ray.dashuyun.cn

Py:   sys.exit(1)
来源：http://jkf.wangdashe.top

PHP:  exit(1);
来源：http://uju.yfazqb.com

JS:   process.exit(1)
来源：http://npx.gzhubu.top

TS:   process.exit(1)
来源：http://mld.fanxiaobao.xyz

Java: System.exit(1)
来源：http://uxv.zycfv.cn

Go:   os.Exit(1)
来源：http://oam.ppjwa.cn

Ruby: exit 1
来源：http://xov.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gqi.nanxinkj.top

[M06] 向标准错误输出
来源：http://gvc.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://vub.zhoulong.xyz


<!-- 参考信息 -->