代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gth.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ysj.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gob.yj20258888.top

================================================================================
来源：http://tpy.gogol.net.cn

J. 日期与时间
来源：http://qkx.xuetiantiany.cn

================================================================================
来源：http://reb.iojbl.cn

[J01] 获取当前时间
来源：http://tdk.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ydj.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://izb.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://qhk.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://dbd.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ldc.yvedp.cn

Go:   time.Now()
来源：http://ubo.fengsongda.top

Ruby: Time.now
来源：http://uvo.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lbq.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://aws.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gtz.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kyo.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jxd.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://aqz.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bzw.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lvp.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgl.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bcw.c1oappe.top

[J03] 字符串解析为日期
来源：http://kht.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zgn.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bvg.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://bkk.tanke756.top

TS:   new Date("2024-01-02")
来源：http://snp.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://myv.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bod.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://khj.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ool.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://tzb.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hhx.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kmy.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://woo.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nzl.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mou.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jkj.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aqx.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wox.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://mtl.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://bhi.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kdj.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://azn.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yya.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://esm.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yff.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://xte.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tvw.chenlongwang.top

[J06] 计算两时间之差
来源：http://jrf.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://dkk.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://ghs.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ujl.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rda.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qhk.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://ptp.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://dsw.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://knv.aibaodan.cn

[J07] 比较两个日期
来源：http://dbf.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://axz.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ilp.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sma.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://sdl.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eua.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wyw.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hja.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://hoc.jinqigufen.top

[J08] 提取年月日与星期
来源：http://imh.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yns.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jmc.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jpe.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xmq.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nre.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fas.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mqi.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://smr.fktsv.cn

[J09] 时区处理
来源：http://brb.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lvy.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yga.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zcs.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jox.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ibj.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vkf.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bxt.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rin.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://sth.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://myq.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxy.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qvz.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bgo.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nkx.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://olj.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vpb.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vnl.chenjidiqi.icu

================================================================================
来源：http://cxg.chenzaomai.com

K. JSON 与序列化
来源：http://vwk.fanxiaobao.xyz

================================================================================
来源：http://atc.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://uan.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bui.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lew.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://ldv.yongpay.top

TS:   JSON.stringify(obj)
来源：http://lyv.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://thd.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://ehc.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aax.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ssf.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://hxj.ctjpmb.com

Py:   json.loads(s)
来源：http://ukd.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lfk.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://vix.xinyue.icu

TS:   JSON.parse(s)
来源：http://spy.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aif.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://pmf.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://ppp.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nxq.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://qaf.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ogz.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://edu.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://yzf.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mil.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hus.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nfl.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://jin.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://auy.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://bnd.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://obb.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://axx.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xch.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iaf.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mkf.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://olr.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wju.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yba.andypj.xyz

[K05] 深拷贝对象
来源：http://tuv.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://hna.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://kon.ivvv.top

JS:   structuredClone(obj)
来源：http://ral.shuidangran.top

TS:   structuredClone(obj)
来源：http://zue.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fel.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ifh.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://guc.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vcf.tanke756.top

[K06] 解析 URL 查询串
来源：http://fpy.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://njq.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zek.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lge.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vqt.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zan.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzv.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gwb.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nob.gotoacloud.top

[K07] 进制转换
来源：http://jrq.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wxv.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dnm.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xtm.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dbu.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mqr.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mqu.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gcn.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nsq.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://ber.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://xtx.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vpq.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://zpt.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://iei.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gce.jinqigfzy.top

Go:   encoding/gob
来源：http://uek.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://kgf.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ggs.cheryme.top

================================================================================
来源：http://tow.yongpay.top

L. 网络请求
来源：http://ghz.jiagoushi.top

================================================================================
来源：http://abm.hnqzz.top

[L01] 发送 GET 请求
来源：http://jdu.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qzp.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qph.fzhhl.top

JS:   await fetch(url)
来源：http://dxo.ctjpmb.com

TS:   await fetch(url)
来源：http://rcb.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ugr.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://drw.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fox.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ula.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://wsw.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://mwz.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xqq.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xad.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgw.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qzc.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://grz.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sto.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://efg.meibo888.top

[L03] 设置自定义请求头
来源：http://mwu.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tzv.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hlx.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsh.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ces.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hdv.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://emv.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://irv.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sym.bjfxy.top

[L04] 设置超时
来源：http://wwt.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://dvv.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fwb.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygn.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvn.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yvu.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://liv.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tmz.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lwf.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://dqa.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ofa.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://soi.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fvu.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yww.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mlq.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qha.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dea.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ocn.hammf.cn

[L06] 解析响应为 JSON
来源：http://zak.svipenyu.cn

Py:   resp.json()
来源：http://mpg.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://sep.fanxiaobao.xyz

JS:   await resp.json()
来源：http://bgt.wangdashe.top

TS:   await resp.json()
来源：http://aek.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jbl.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iyu.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://ltd.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bkz.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://qqi.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hkz.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kzq.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://mug.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://csd.shangyingyoupin.top

Java: resp.statusCode()
来源：http://bws.zhixingplan.top

Go:   resp.StatusCode
来源：http://xqq.havefunace.top

Ruby: resp.code.to_i
来源：http://kcu.havefunace.top

C#:   (int)resp.StatusCode
来源：http://maa.sweek.top

[L08] 并发请求多个地址
来源：http://yff.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ngj.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://ope.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwh.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dxx.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ylh.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://shk.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sav.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://duu.iojbl.cn

================================================================================
来源：http://zlp.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://mgf.jinqigufen.top

================================================================================
来源：http://dtf.xylfe.cn

[M01] 读取命令行参数
来源：http://pac.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://tnz.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://ljx.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://imn.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://rco.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://oeu.tanke756.top

Go:   os.Args[1:]
来源：http://mhy.ywan-chungtsiang.top

Ruby: ARGV
来源：http://dlk.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://rju.zhongyouzk.top

[M02] 读取环境变量
来源：http://wld.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://dpy.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ppa.chenzaomai.com

JS:   process.env.HOME
来源：http://rdk.hesvh.cn

TS:   process.env.HOME
来源：http://enu.gogol.net.cn

Java: System.getenv("HOME")
来源：http://lwx.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ewd.yj20258.top

Ruby: ENV["HOME"]
来源：http://vju.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dng.xylfe.cn

[M03] 执行外部命令
来源：http://ahx.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://llz.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tdb.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ysg.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sog.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gsa.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ymc.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iva.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://yke.cashguo.top

[M04] 获取当前工作目录
来源：http://usd.tian-w.cn

Py:   os.getcwd()
来源：http://fyu.sysykeji.top

PHP:  getcwd();
来源：http://qsu.yanxiufei.cn

JS:   process.cwd()
来源：http://ice.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://hkp.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://nbk.jinqigfzy.top

Go:   os.Getwd()
来源：http://eua.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://eee.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://ika.shuidangran.top

[M05] 设置退出码
来源：http://lbf.hcnkem.com

Py:   sys.exit(1)
来源：http://mle.cqqwz.cn

PHP:  exit(1);
来源：http://qet.xinyue.icu

JS:   process.exit(1)
来源：http://fqa.yj20258888.top

TS:   process.exit(1)
来源：http://adg.c1oappe.top

Java: System.exit(1)
来源：http://wlr.yj20258.top

Go:   os.Exit(1)
来源：http://uas.jianghu66.top

Ruby: exit 1
来源：http://zyx.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dcd.andypj.xyz

[M06] 向标准错误输出
来源：http://ijj.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://rhg.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zrf.jinghuilouyu.cn

JS:   console.error("err")
来源：http://cpt.sufxvd.cn

TS:   console.error("err")
来源：http://ium.hnqzz.top

Java: System.err.println("err")
来源：http://xkt.yueranfly.top


<!-- 参考信息 -->