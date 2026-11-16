代发 wailian999

Ruby: s.scan(/error/i)
来源：http://rft.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qiw.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://wil.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ajc.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zjr.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jmk.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://puz.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://urw.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uez.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bxn.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rrb.iojbl.cn

================================================================================
来源：http://ibb.ydjk.org.cn

J. 日期与时间
来源：http://oct.wangshuangyany.cn

================================================================================
来源：http://siw.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://pvr.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://bzi.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zjg.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://agy.hammf.cn

TS:   new Date();  Date.now()
来源：http://lgk.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rov.shuidangran.top

Go:   time.Now()
来源：http://vhe.zdqjudy.top

Ruby: Time.now
来源：http://fqz.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xig.ehwqpu.com

[J02] 格式化输出
来源：http://kud.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cuf.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cro.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xkt.52xcode.cn

TS:   d.toISOString()
来源：http://fli.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vou.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uao.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrs.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yxf.yfazqb.com

[J03] 字符串解析为日期
来源：http://koy.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tkf.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xsy.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://dmt.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://rra.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://rxg.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ywf.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://nkh.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ebl.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://lwm.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nwx.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zvs.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dwz.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bhr.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nid.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://avg.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pze.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vtz.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://reu.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://gcn.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yoe.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbl.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eec.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://chv.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ogr.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://pld.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://nck.sysykeji.top

[J06] 计算两时间之差
来源：http://apx.havefunace.top

Py:   (end - start).total_seconds()
来源：http://hon.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://kme.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://okk.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ycj.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://poq.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://ogx.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://cso.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://vtq.cdnleiting.top

[J07] 比较两个日期
来源：http://miq.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://wrh.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wos.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://nep.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://udu.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dpr.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://btx.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://vnm.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://prs.cashguo.top

[J08] 提取年月日与星期
来源：http://cep.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gek.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dqs.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bhz.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ifb.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bsk.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oup.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tjf.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gbt.hnqzz.top

[J09] 时区处理
来源：http://xdr.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mvo.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://esn.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://das.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlr.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jss.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://azs.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eyq.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qrl.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://ruv.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ctz.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kuv.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wig.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jkv.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bnm.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tfm.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://udt.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rdw.tian-w.cn

================================================================================
来源：http://sjf.jqgfzy.top

K. JSON 与序列化
来源：http://vjd.bbcook.cn

================================================================================
来源：http://utg.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://llu.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xon.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gkw.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://uva.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://cqq.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cys.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://knd.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://zkx.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bgm.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://aaq.jqgufenzy.top

Py:   json.loads(s)
来源：http://ewi.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sro.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://heb.nwbrower.top

TS:   JSON.parse(s)
来源：http://wmt.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqb.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://cbq.cheryme.top

Ruby: JSON.parse(s)
来源：http://gpg.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lpp.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://fcx.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xhx.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fyz.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xfc.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ivh.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://frh.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ini.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://kzd.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tjz.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://fyf.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tgm.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pua.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://thb.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wwn.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://exw.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lxo.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://brt.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lug.sweek.top

[K05] 深拷贝对象
来源：http://vza.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://ctf.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://ndn.andypj.xyz

JS:   structuredClone(obj)
来源：http://eir.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://bax.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nkd.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jty.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bla.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cok.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://imj.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qjx.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kbt.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkh.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gpl.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hjt.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nlb.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rbq.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pyo.yfazqb.com

[K07] 进制转换
来源：http://wwp.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://diu.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jlg.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ifs.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fdc.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wqw.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bmn.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wgz.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nyp.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://xmq.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://soc.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tri.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://ysj.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://kzh.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mqz.zhoulong.xyz

Go:   encoding/gob
来源：http://fgm.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://yrq.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://koi.zhaomingkeji.xyz

================================================================================
来源：http://gme.jinqigufen.top

L. 网络请求
来源：http://lkd.316326.xyz

================================================================================
来源：http://qoy.316326.xyz

[L01] 发送 GET 请求
来源：http://blz.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sxv.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ehm.sjlbkw.cn

JS:   await fetch(url)
来源：http://jjq.zhijiandao.cn

TS:   await fetch(url)
来源：http://mbd.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wnu.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://xsz.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://avq.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://txt.zhixingplan.top

[L02] 发送 POST JSON
来源：http://vqi.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://fdy.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kge.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sxu.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ehp.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://arn.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bzy.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qxo.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://che.cashguo.top

[L03] 设置自定义请求头
来源：http://nne.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://out.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://snb.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://snr.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qhc.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djd.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zgh.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gjd.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gvs.yuanzhike.top

[L04] 设置超时
来源：http://pwj.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://bbw.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ejt.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://loj.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://got.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pzz.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wre.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zwg.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kqf.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://jpy.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://egm.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ilk.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ihq.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wbz.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zwt.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zul.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wac.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uqa.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://slk.gotoacloud.top

Py:   resp.json()
来源：http://dsn.yj20258.top

PHP:  json_decode($body, true);
来源：http://vfr.zdbjq.cn

JS:   await resp.json()
来源：http://ame.hammf.cn

TS:   await resp.json()
来源：http://owq.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bbc.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zec.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://fyp.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jae.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://edx.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://csy.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iho.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://oau.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://qog.feifeiyinyue.top

Java: resp.statusCode()
来源：http://wqi.jinqigufen.top

Go:   resp.StatusCode
来源：http://gqt.yonumen.top

Ruby: resp.code.to_i
来源：http://bkn.havefunace.top

C#:   (int)resp.StatusCode
来源：http://myd.aizwys.cn

[L08] 并发请求多个地址
来源：http://rbn.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pus.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://jnr.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ted.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://taj.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yjp.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vxh.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vkw.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nem.ctjpmb.com

================================================================================
来源：http://ith.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://tve.jqgfzy.top

================================================================================
来源：http://xhe.dashuyun.cn

[M01] 读取命令行参数
来源：http://arl.jyoumei.cn

Py:   sys.argv[1:]
来源：http://tui.yj20258.top

PHP:  $argv;  $argc;
来源：http://zzg.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://lue.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://qpk.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://hvf.zhongyouzk.top

Go:   os.Args[1:]
来源：http://yyg.kuanghao11.cn

Ruby: ARGV
来源：http://ibg.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://vgu.dianchejie.cn

[M02] 读取环境变量
来源：http://vcn.cashguo.top

Py:   os.environ.get("HOME")
来源：http://xto.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jgt.cqqwz.cn

JS:   process.env.HOME
来源：http://etz.jqgufenzy.top

TS:   process.env.HOME
来源：http://psd.sweek.top

Java: System.getenv("HOME")
来源：http://osn.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://omf.yj20258888.top

Ruby: ENV["HOME"]
来源：http://zlb.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lhp.zhixingplan.top

[M03] 执行外部命令
来源：http://rwm.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxe.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://khg.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bqh.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hyv.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xjs.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nsm.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://iiu.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://unw.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://azm.ehwqpu.com

Py:   os.getcwd()
来源：http://loc.jianghu66.top

PHP:  getcwd();
来源：http://lav.yanxiufei.cn

JS:   process.cwd()
来源：http://fgj.aibaodan.cn

TS:   process.cwd()
来源：http://pvm.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://xjb.sjlbkw.cn

Go:   os.Getwd()
来源：http://tuu.yj20258888.top

Ruby: Dir.pwd
来源：http://kfs.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://gah.zhongyouzk.top

[M05] 设置退出码
来源：http://ytm.cucudq.cn

Py:   sys.exit(1)
来源：http://xlx.guowangkeji.top

PHP:  exit(1);
来源：http://dot.xylfe.cn

JS:   process.exit(1)
来源：http://cay.kuanghao11.cn

TS:   process.exit(1)
来源：http://smy.smart0.xyz

Java: System.exit(1)
来源：http://syd.zhengqikj.top

Go:   os.Exit(1)
来源：http://xss.ehwqpu.com


<!-- 参考信息 -->